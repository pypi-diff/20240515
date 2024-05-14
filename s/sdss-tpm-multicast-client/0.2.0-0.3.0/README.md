# Comparing `tmp/sdss_tpm_multicast_client-0.2.0.tar.gz` & `tmp/sdss_tpm_multicast_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_tpm_multicast_client-0.2.0.tar", max compression
+gzip compressed data, was "sdss_tpm_multicast_client-0.3.0.tar", max compression
```

## Comparing `sdss_tpm_multicast_client-0.2.0.tar` & `sdss_tpm_multicast_client-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1836 2024-05-14 22:22:49.206166 sdss_tpm_multicast_client-0.2.0/README.md
--rw-r--r--   0        0        0     1801 2024-05-14 22:22:49.206166 sdss_tpm_multicast_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      448 2024-05-14 22:22:49.206166 sdss_tpm_multicast_client-0.2.0/src/tpm_multicast_client/__init__.py
--rw-r--r--   0        0        0      899 2024-05-14 22:22:49.206166 sdss_tpm_multicast_client-0.2.0/src/tpm_multicast_client/__main__.py
--rw-r--r--   0        0        0     3031 2024-05-14 22:22:49.206166 sdss_tpm_multicast_client-0.2.0/src/tpm_multicast_client/client.py
--rw-r--r--   0        0        0     6534 2024-05-14 22:22:49.206166 sdss_tpm_multicast_client-0.2.0/src/tpm_multicast_client/unpack.py
--rw-r--r--   0        0        0     2381 1970-01-01 00:00:00.000000 sdss_tpm_multicast_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1836 2024-05-14 23:13:36.573907 sdss_tpm_multicast_client-0.3.0/README.md
+-rw-r--r--   0        0        0     1842 2024-05-14 23:13:36.573907 sdss_tpm_multicast_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      523 2024-05-14 23:13:36.573907 sdss_tpm_multicast_client-0.3.0/src/tpm_multicast_client/__init__.py
+-rw-r--r--   0        0        0     1582 2024-05-14 23:13:36.573907 sdss_tpm_multicast_client-0.3.0/src/tpm_multicast_client/__main__.py
+-rw-r--r--   0        0        0     3877 2024-05-14 23:13:36.573907 sdss_tpm_multicast_client-0.3.0/src/tpm_multicast_client/client.py
+-rw-r--r--   0        0        0     1560 2024-05-14 23:13:36.573907 sdss_tpm_multicast_client-0.3.0/src/tpm_multicast_client/server.py
+-rw-r--r--   0        0        0     6534 2024-05-14 23:13:36.573907 sdss_tpm_multicast_client-0.3.0/src/tpm_multicast_client/unpack.py
+-rw-r--r--   0        0        0     2381 1970-01-01 00:00:00.000000 sdss_tpm_multicast_client-0.3.0/PKG-INFO
```

### Comparing `sdss_tpm_multicast_client-0.2.0/README.md` & `sdss_tpm_multicast_client-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss_tpm_multicast_client-0.2.0/pyproject.toml` & `sdss_tpm_multicast_client-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-tpm-multicast-client"
-version = "0.2.0"
+version = "0.3.0"
 description = "TPM multicast client"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD 3-Clause"
 readme = "README.md"
 packages = [
     { include = "tpm_multicast_client", from = "src" }
 ]
@@ -60,14 +60,15 @@
 [tool.coverage.run]
 branch = true
 include = ["src/tpm_multicast_client/*"]
 omit = [
     "**/__init__.py",
     "**/tpm_multicast_client/__main__.py",
     "**/tpm_multicast_client/client.py",
+    "**/tpm_multicast_client/server.py",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     "if TYPE_CHECKING:",
     "# pragma: no cover"
 ]
```

### Comparing `sdss_tpm_multicast_client-0.2.0/src/tpm_multicast_client/client.py` & `sdss_tpm_multicast_client-0.3.0/src/tpm_multicast_client/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 import asyncio
 import socket
 import struct
 import warnings
 
-from typing import Awaitable, Callable
+from typing import Awaitable, Callable, Self
 
 from tpm_multicast_client.unpack import unpack_tpm_data
 
 
 CallbackType = Callable[[dict], None | Awaitable[None]]
 
 MCAST_GRP = "224.1.1.1"
@@ -98,14 +98,45 @@
 
     return await loop.create_datagram_endpoint(
         lambda: TPMClientProtocol(callback, loop),
         sock=get_socket(),
     )
 
 
+class TPMClient:
+    """A singleton class that listens to the TPM multicast."""
+
+    _instance: Self | None = None
+
+    def __new__(cls):
+        if cls._instance is None:
+            cls._instance = super().__new__(cls)
+
+        return cls._instance
+
+    def __init__(self):
+        # Prevent setting the data attribute to None if this is a reinitialisation
+        # of an instance that already existed.
+        already_initialized = hasattr(self, "data")
+        if already_initialized:
+            return
+
+        self.data: dict[str, int | float | str] | None = None
+
+    async def update_data(self, new_data: dict[str, int | float | str]):
+        """Updates the TPM data."""
+
+        self.data = new_data
+
+    async def listen(self):
+        """Listens to the TPM multicast."""
+
+        await listen_to_multicast(self.update_data)
+
+
 async def test():
     """Simple test function."""
 
     async def printer(dd: dict):
         print(dd)
 
     await listen_to_multicast(printer)
```

### Comparing `sdss_tpm_multicast_client-0.2.0/src/tpm_multicast_client/unpack.py` & `sdss_tpm_multicast_client-0.3.0/src/tpm_multicast_client/unpack.py`

 * *Files identical despite different names*

### Comparing `sdss_tpm_multicast_client-0.2.0/PKG-INFO` & `sdss_tpm_multicast_client-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-tpm-multicast-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: TPM multicast client
 License: BSD 3-Clause
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

