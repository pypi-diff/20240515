# Comparing `tmp/gsloc-0.1.1.tar.gz` & `tmp/gsloc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsloc-0.1.1.tar", max compression
+gzip compressed data, was "gsloc-0.1.2.tar", max compression
```

## Comparing `gsloc-0.1.1.tar` & `gsloc-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1826 2024-05-15 05:36:10.000004 gsloc-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-15 05:36:10.000004 gsloc-0.1.1/gsloc/__init__.py
--rw-r--r--   0        0        0     2703 2024-05-15 05:36:10.000004 gsloc-0.1.1/gsloc/cli.py
--rw-r--r--   0        0        0     4361 2024-05-15 05:36:10.000004 gsloc-0.1.1/gsloc/core.py
--rw-r--r--   0        0        0        0 2024-05-15 05:36:10.000004 gsloc-0.1.1/gsloc/protobuf/__init__.py
--rw-r--r--   0        0        0     2407 2024-05-15 05:36:10.000004 gsloc-0.1.1/gsloc/protobuf/location_pb2.py
--rw-r--r--   0        0        0     3545 2024-05-15 05:36:10.000004 gsloc-0.1.1/gsloc/protobuf/location_pb2.pyi
--rw-r--r--   0        0        0      555 2024-05-15 05:36:10.004004 gsloc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2644 1970-01-01 00:00:00.000000 gsloc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4150 2024-05-15 21:24:27.006667 gsloc-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 21:24:27.006667 gsloc-0.1.2/gsloc/__init__.py
+-rw-r--r--   0        0        0     2703 2024-05-15 21:24:27.006667 gsloc-0.1.2/gsloc/cli.py
+-rw-r--r--   0        0        0     4916 2024-05-15 21:24:27.006667 gsloc-0.1.2/gsloc/core.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:24:27.006667 gsloc-0.1.2/gsloc/protobuf/__init__.py
+-rw-r--r--   0        0        0     2407 2024-05-15 21:24:27.006667 gsloc-0.1.2/gsloc/protobuf/location_pb2.py
+-rw-r--r--   0        0        0     3545 2024-05-15 21:24:27.006667 gsloc-0.1.2/gsloc/protobuf/location_pb2.pyi
+-rw-r--r--   0        0        0      535 2024-05-15 21:24:27.010667 gsloc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5027 1970-01-01 00:00:00.000000 gsloc-0.1.2/PKG-INFO
```

### Comparing `gsloc-0.1.1/gsloc/cli.py` & `gsloc-0.1.2/gsloc/cli.py`

 * *Files identical despite different names*

### Comparing `gsloc-0.1.1/gsloc/core.py` & `gsloc-0.1.2/gsloc/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,75 @@
 """Core functionality for querying the Apple location service."""
 
 import logging
 import struct
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
+from typing import List
 
 import requests
-from pydantic import BaseModel, Field, ValidationError
 
 from gsloc.protobuf.location_pb2 import Request, Response  # pylint: disable=no-name-in-module
 
 logger = logging.getLogger(__name__)
 
 
 class NoResultsError(Exception):
     """Raised when no results are returned from the Apple location service."""
 
     def __init__(self, mac: str):
         super().__init__(f"No results found for MAC address: {mac}")
 
 
-class WifiInfo(BaseModel):
+@dataclass
+class WifiInfo:
     """Information about a WiFi network."""
 
     mac: str
-    channel: int = Field(gt=0, lt=256)
-    latitude: float = Field(ge=-90, le=90)
-    longitude: float = Field(ge=-180, le=180)
-    accuracy: int = Field(ge=0)
+    channel: int
+    latitude: float
+    longitude: float
+    accuracy: int
     altitude: int
     altitude_accuracy: int
 
+    def validate(self) -> None:
+        """Validates the WifiInfo object."""
+        assert 0 <= self.channel <= 255, "Channel must be between 0 and 255."
+        assert -90 <= self.latitude <= 90, "Latitude must be between -90 and 90."
+        assert -180 <= self.longitude <= 180, "Longitude must be between -180 and 180."
+        assert self.accuracy >= 0, "Accuracy must be greater than or equal to 0."
+        assert self.altitude >= 0, "Altitude must be greater than or equal to 0."
+        assert self.altitude_accuracy >= 0, "Altitude accuracy must be greater than or equal to 0."
+
     @classmethod
     def from_response_wifi(cls, response_wifi: Response.ResponseWifi) -> "WifiInfo":
         """Creates a WifiInfo object from a ResponseWifi object."""
         try:
             return cls(
                 mac=response_wifi.mac,
                 channel=response_wifi.channel,
                 latitude=response_wifi.location.latitude / 1e8,
                 longitude=response_wifi.location.longitude / 1e8,
                 accuracy=response_wifi.location.accuracy,
                 altitude=response_wifi.location.altitude,
                 altitude_accuracy=response_wifi.location.altitudeAccuracy,
             )
-        except ValidationError as e:
+        except AssertionError as e:
+            # Fields are invalid if Apple doesn't know this wifi access point
             raise NoResultsError(response_wifi.mac) from e
 
     def to_feature(self) -> dict:
         """Converts the WifiInfo object to a GeoJSON feature."""
         return {
             "type": "Feature",
             "geometry": {
                 "type": "Point",
                 "coordinates": [self.longitude, self.latitude],
             },
-            "properties": self.model_dump(),
+            "properties": asdict(self),
         }
 
 
 @dataclass
 class PayloadHeader:
     """Header for the request's payload."""
 
@@ -89,15 +100,15 @@
         )
 
 
 class Payload:
     """Payload for the request."""
 
     def __init__(
-        self, header: PayloadHeader, mac_addresses: list[str], noise: int = 0, signal: int = 100
+        self, header: PayloadHeader, mac_addresses: List[str], noise: int = 0, signal: int = 100
     ):
         self.header = header
         self.request = Request()
         self.request.noise = noise
         self.request.signal = signal
         for mac in mac_addresses:
             self.request.wifis.add(mac=mac)
@@ -105,15 +116,15 @@
     def build(self) -> bytes:
         """Builds the payload for the request."""
         message = self.request.SerializeToString()
         size = struct.pack(">h", len(message))
         return self.header.build() + size + message
 
 
-def query(macs: list[str]) -> list[WifiInfo]:
+def query(macs: List[str]) -> List[WifiInfo]:
     """Queries the Apple location service with the given payload."""
     logger.info("Querying Apple location service with MAC addresses: %s", macs)
     payload = Payload(PayloadHeader(), macs)
     response = requests.post(
         url="https://gs-loc.apple.com/clls/wloc",
         data=payload.build(),
         headers={
```

### Comparing `gsloc-0.1.1/gsloc/protobuf/location_pb2.py` & `gsloc-0.1.2/gsloc/protobuf/location_pb2.py`

 * *Files identical despite different names*

### Comparing `gsloc-0.1.1/gsloc/protobuf/location_pb2.pyi` & `gsloc-0.1.2/gsloc/protobuf/location_pb2.pyi`

 * *Files identical despite different names*

### Comparing `gsloc-0.1.1/pyproject.toml` & `gsloc-0.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "gsloc"
-version = "0.1.1"
+version = "0.1.2"
 description = "A simple API for Apple's gs-loc service"
 authors = ["Yibo Wei <david_wyb2001@outlook.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/Microwave-WYB/gsloc"
 repository = "https://github.com/Microwave-WYB/gsloc"
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.7"
 protobuf = "^5.26.1"
-pydantic = "^2.7.1"
 requests = "^2.31.0"
 rich = "^13.7.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

