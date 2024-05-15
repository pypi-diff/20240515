# Comparing `tmp/arduino_iot_cloud-1.1.0.tar.gz` & `tmp/arduino_iot_cloud-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arduino_iot_cloud-1.1.0.tar", last modified: Tue Mar 19 07:35:00 2024, max compression
+gzip compressed data, was "arduino_iot_cloud-1.2.0.tar", last modified: Wed May 15 14:43:11 2024, max compression
```

## Comparing `arduino_iot_cloud-1.1.0.tar` & `arduino_iot_cloud-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:35:00.258521 arduino_iot_cloud-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-03-19 07:35:00.258521 arduino_iot_cloud-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:35:00.258521 arduino_iot_cloud-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/examples/micropython_async_wifi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/examples/micropython_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 07:35:00.258521 arduino_iot_cloud-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:35:00.254521 arduino_iot_cloud-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:35:00.258521 arduino_iot_cloud-1.1.0/src/arduino_iot_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/src/arduino_iot_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-19 07:35:00.000000 arduino_iot_cloud-1.1.0/src/arduino_iot_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/src/arduino_iot_cloud/ucloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/src/arduino_iot_cloud/umqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/src/arduino_iot_cloud/ussl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:35:00.258521 arduino_iot_cloud-1.1.0/src/arduino_iot_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-03-19 07:35:00.000000 arduino_iot_cloud-1.1.0/src/arduino_iot_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-19 07:35:00.000000 arduino_iot_cloud-1.1.0/src/arduino_iot_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 07:35:00.000000 arduino_iot_cloud-1.1.0/src/arduino_iot_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 07:35:00.000000 arduino_iot_cloud-1.1.0/src/arduino_iot_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-19 07:35:00.000000 arduino_iot_cloud-1.1.0/src/arduino_iot_cloud.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:35:00.258521 arduino_iot_cloud-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/tests/ci.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1938 2024-03-19 07:34:53.000000 arduino_iot_cloud-1.1.0/tests/ci.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:11.567544 arduino_iot_cloud-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-15 14:43:11.567544 arduino_iot_cloud-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:11.563544 arduino_iot_cloud-1.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/examples/micropython_async_wifi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/examples/micropython_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:43:11.567544 arduino_iot_cloud-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:11.563544 arduino_iot_cloud-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:11.567544 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 14:43:11.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/ucloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/umqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/ussl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:11.567544 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-15 14:43:11.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-15 14:43:11.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:43:11.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:43:11.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 14:43:11.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:11.567544 arduino_iot_cloud-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/tests/ci.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1938 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/tests/ci.sh
```

### Comparing `arduino_iot_cloud-1.1.0/LICENSE` & `arduino_iot_cloud-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.1.0/PKG-INFO` & `arduino_iot_cloud-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arduino_iot_cloud
-Version: 1.1.0
+Version: 1.2.0
 Summary: Arduino IoT Cloud Python client
 Author-email: Ibrahim Abdelkader <i.abdelkader@arduino.cc>
 Project-URL: Homepage, https://github.com/arduino/arduino-iot-cloud-py
 Project-URL: Bug Tracker, https://github.com/arduino/arduino-iot-cloud-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
```

### Comparing `arduino_iot_cloud-1.1.0/README.md` & `arduino_iot_cloud-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.1.0/examples/example.py` & `arduino_iot_cloud-1.2.0/examples/example.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from arduino_iot_cloud import ArduinoCloudClient
 from arduino_iot_cloud import Location
 from arduino_iot_cloud import Schedule
 from arduino_iot_cloud import ColoredLight
 from arduino_iot_cloud import Task
 from random import uniform
 import argparse
-import ssl
+import ssl # noqa
 
 from secrets import DEVICE_ID
 from secrets import SECRET_KEY  # noqa
 
 KEY_PATH = "pkcs11:token=arduino"
 CERT_PATH = "pkcs11:token=arduino"
 CA_PATH = "ca-root.pem"
@@ -54,25 +54,30 @@
     logging.basicConfig(
         datefmt="%H:%M:%S",
         format="%(asctime)s.%(msecs)03d %(message)s",
         level=logging.DEBUG if args.debug else logging.INFO,
     )
 
     # Create a client object to connect to the Arduino IoT cloud.
-    # To use a secure element, set the token's "pin" and URI in "keyfile" and "certfile", and
-    # the CA certificate (if any) in "ssl_params". Alternatively, a username and password can
-    # be used to authenticate, for example:
-    #   client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY)
-    client = ArduinoCloudClient(
-        device_id=DEVICE_ID,
-        ssl_params={
-            "pin": "1234",
-            "keyfile": KEY_PATH, "certfile": CERT_PATH, "ca_certs": CA_PATH, "cert_reqs": ssl.CERT_REQUIRED
-        },
-    )
+    # The most basic authentication method uses a username and password. The username is the device
+    # ID, and the password is the secret key obtained from the IoT cloud when provisioning a device.
+    client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY)
+
+    # Alternatively, the client also supports key and certificate-based authentication. To use this
+    # mode, set "keyfile" and "certfile", and the CA certificate (if any) in "ssl_params".
+    # Furthermore, secure elements, which can be used to store the key and cert, are also supported.
+    # To secure elements, set "use_hsm" to True in "ssl_params" and set the token's "pin" if any.
+    # client = ArduinoCloudClient(
+    #     device_id=DEVICE_ID,
+    #     ssl_params={
+    #         "use_hsm": True, "pin": "1234",
+    #         "keyfile": KEY_PATH, "certfile": CERT_PATH, "cafile": CA_PATH,
+    #         "verify_mode": ssl.CERT_REQUIRED, "server_hostname" : "iot.arduino.cc"
+    #     },
+    # )
 
     # Register cloud objects.
     # Note: The following objects must be created first in the dashboard and linked to the device.
     # This cloud object is initialized with its last known value from the cloud. When this object is updated
     # from the dashboard, the on_switch_changed function is called with the client object and the new value.
     client.register("sw1", value=None, on_write=on_switch_changed, interval=0.250)
```

### Comparing `arduino_iot_cloud-1.1.0/examples/micropython_async_wifi.py` & `arduino_iot_cloud-1.2.0/examples/micropython_async_wifi.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     logging.basicConfig(
         datefmt="%H:%M:%S",
         format="%(asctime)s.%(msecs)03d %(message)s",
         level=logging.INFO,
     )
 
     # Create a client object to connect to the Arduino IoT cloud.
-    # For MicroPython, the key and cert files must be stored in DER format on the filesystem.
-    # Alternatively, a username and password can be used to authenticate:
+    # The most basic authentication method uses a username and password. The username is the device
+    # ID, and the password is the secret key obtained from the IoT cloud when provisioning a device.
     client = ArduinoCloudClient(
         device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY
     )
 
     # Register cloud objects.
     # Note: The following objects must be created first in the dashboard and linked to the device.
     # This cloud object is initialized with its last known value from the cloud. When this object is updated
```

### Comparing `arduino_iot_cloud-1.1.0/examples/micropython_basic.py` & `arduino_iot_cloud-1.2.0/examples/micropython_basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,22 +69,27 @@
         level=logging.INFO,
     )
 
     # NOTE: Add networking code here or in boot.py
     wifi_connect()
 
     # Create a client object to connect to the Arduino IoT cloud.
-    # For MicroPython, the key and cert files must be stored in DER format on the filesystem.
-    # Alternatively, a username and password can be used to authenticate:
+    # The most basic authentication method uses a username and password. The username is the device
+    # ID, and the password is the secret key obtained from the IoT cloud when provisioning a device.
     client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY)
+
+    # Alternatively, the client also supports key and certificate-based authentication. To use this
+    # mode, set "keyfile" and "certfile", and the CA certificate (if any) in "ssl_params".
+    # Note that for MicroPython, the key and cert files must be stored in DER format on the filesystem.
     # client = ArduinoCloudClient(
     #     device_id=DEVICE_ID,
     #     ssl_params={
-    #         "keyfile": KEY_PATH, "certfile": CERT_PATH, "cadata": CADATA, "cert_reqs": ssl.CERT_REQUIRED
-    #     }
+    #         "keyfile": KEY_PATH, "certfile": CERT_PATH, "cadata": CADATA,
+    #         "verify_mode": ssl.CERT_REQUIRED, "server_hostname" : "iot.arduino.cc"
+    #     },
     # )
 
     # Register cloud objects.
     # Note: The following objects must be created first in the dashboard and linked to the device.
     # This cloud object is initialized with its last known value from the cloud. When this object is updated
     # from the dashboard, the on_switch_changed function is called with the client object and the new value.
     client.register("sw1", value=None, on_write=on_switch_changed, interval=0.250)
```

### Comparing `arduino_iot_cloud-1.1.0/package.json` & `arduino_iot_cloud-1.2.0/package.json`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.1.0/pyproject.toml` & `arduino_iot_cloud-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.1.0/src/arduino_iot_cloud/__init__.py` & `arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 # This file is part of the Arduino IoT Cloud Python client.
 # Copyright (c) 2022 Arduino SA
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
+import asyncio
+import binascii
 from .ucloud import ArduinoCloudClient  # noqa
 from .ucloud import ArduinoCloudObject
 from .ucloud import timestamp
 
-try:
-    import asyncio
-    import binascii
-except ImportError:
-    import uasyncio as asyncio
-    import ubinascii as binascii
-
 
 CADATA = binascii.unhexlify(
     b"308201cf30820174a00302010202141f101deba7e125e727c1a391e3ec0d"
     b"174ded4a59300a06082a8648ce3d0403023045310b300906035504061302"
     b"555331173015060355040a130e41726475696e6f204c4c43205553310b30"
     b"09060355040b130249543110300e0603550403130741726475696e6f301e"
     b"170d3138303732343039343730305a170d3438303731363039343730305a"
@@ -31,27 +26,40 @@
     b"0106300f0603551d130101ff040530030101ff301d0603551d0e04160414"
     b"5b3e2a6b8ec9b01aa854e6369b8c09f9fce1b980300a06082a8648ce3d04"
     b"03020349003046022100bfd3dc236668b50adc3f0d0ec373e20ac7f760aa"
     b"100dd320bfe102969b6b05d8022100ead9d9da5acd12529709a8ed660fe1"
     b"8d6444ffe82217304ff2b89aafca8ecf"
 )
 
+async def coro():  # noqa
+    pass
+
+
+def is_async(obj):
+    if hasattr(asyncio, "iscoroutinefunction"):
+        return asyncio.iscoroutinefunction(obj)
+    else:
+        return isinstance(obj, type(coro))
+
 
 class Task(ArduinoCloudObject):
     def __init__(self, name, **kwargs):
         kwargs.update({("runnable", True)})  # Force task creation.
         self.on_run = kwargs.pop("on_run", None)
         if not callable(self.on_run):
             raise TypeError("Expected a callable object")
         super().__init__(name, **kwargs)
 
     async def run(self, aiot):
-        while True:
-            self.on_run(aiot)
-            await asyncio.sleep(self.interval)
+        if is_async(self.on_run):
+            await self.on_run(aiot)
+        else:
+            while True:
+                self.on_run(aiot)
+                await asyncio.sleep(self.interval)
 
 
 class Location(ArduinoCloudObject):
     def __init__(self, name, **kwargs):
         super().__init__(name, keys={"lat", "lon"}, **kwargs)
```

### Comparing `arduino_iot_cloud-1.1.0/src/arduino_iot_cloud/ucloud.py` & `arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/ucloud.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.1.0/src/arduino_iot_cloud/umqtt.py` & `arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/umqtt.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # Based on: https://github.com/micropython/micropython-lib/tree/master/micropython/umqtt.simple
 
 import socket
 import struct
 import select
 import logging
 import arduino_iot_cloud.ussl as ssl
+import sys
 
 
 class MQTTException(Exception):
     pass
 
 
 class MQTTClient:
@@ -88,25 +89,22 @@
     def connect(self, clean_session=True, timeout=5.0):
         addr = socket.getaddrinfo(self.server, self.port)[0][-1]
 
         if self.sock is not None:
             self.sock.close()
             self.sock = None
 
-        try:
-            self.sock = socket.socket()
-            self.sock.settimeout(timeout)
-            self.sock = ssl.wrap_socket(self.sock, self.ssl_params)
-            self.sock.connect(addr)
-        except Exception:
-            self.sock.close()
-            self.sock = socket.socket()
-            self.sock.settimeout(timeout)
+        self.sock = socket.socket()
+        self.sock.settimeout(timeout)
+        if sys.implementation.name == "micropython":
             self.sock.connect(addr)
             self.sock = ssl.wrap_socket(self.sock, self.ssl_params)
+        else:
+            self.sock = ssl.wrap_socket(self.sock, self.ssl_params)
+            self.sock.connect(addr)
 
         premsg = bytearray(b"\x10\0\0\0\0\0")
         msg = bytearray(b"\x04MQTT\x04\x02\0\0")
 
         sz = 10 + 2 + len(self.client_id)
         msg[6] = clean_session << 1
         if self.user is not None:
```

### Comparing `arduino_iot_cloud-1.1.0/src/arduino_iot_cloud.egg-info/PKG-INFO` & `arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arduino_iot_cloud
-Version: 1.1.0
+Version: 1.2.0
 Summary: Arduino IoT Cloud Python client
 Author-email: Ibrahim Abdelkader <i.abdelkader@arduino.cc>
 Project-URL: Homepage, https://github.com/arduino/arduino-iot-cloud-py
 Project-URL: Bug Tracker, https://github.com/arduino/arduino-iot-cloud-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
```

### Comparing `arduino_iot_cloud-1.1.0/src/arduino_iot_cloud.egg-info/SOURCES.txt` & `arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.1.0/tests/ci.py` & `arduino_iot_cloud-1.2.0/tests/ci.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.1.0/tests/ci.sh` & `arduino_iot_cloud-1.2.0/tests/ci.sh`

 * *Files identical despite different names*

