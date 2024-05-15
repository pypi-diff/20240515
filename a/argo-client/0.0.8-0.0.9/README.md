# Comparing `tmp/argo-client-0.0.8.tar.gz` & `tmp/argo-client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argo-client-0.0.8.tar", last modified: Fri Sep 10 16:42:10 2021, max compression
+gzip compressed data, was "argo-client-0.0.9.tar", last modified: Mon Sep 13 16:46:44 2021, max compression
```

## Comparing `argo-client-0.0.8.tar` & `argo-client-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2021-09-10 16:42:10.290737 argo-client-0.0.8/
--rw-r--r--   0 andrew     (501) staff       (20)     1457 2021-06-30 16:07:44.000000 argo-client-0.0.8/LICENSE
--rw-r--r--   0 andrew     (501) staff       (20)     1097 2021-09-10 16:42:10.290389 argo-client-0.0.8/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)      222 2021-06-30 16:07:44.000000 argo-client-0.0.8/README.md
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2021-09-10 16:42:10.288014 argo-client-0.0.8/argo_client/
--rw-r--r--   0 andrew     (501) staff       (20)        0 2021-06-30 16:07:44.000000 argo-client-0.0.8/argo_client/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)    17459 2021-08-31 17:48:09.000000 argo-client-0.0.8/argo_client/connection.py
--rw-r--r--   0 andrew     (501) staff       (20)      340 2021-07-19 17:22:10.000000 argo-client-0.0.8/argo_client/exceptions.py
--rw-r--r--   0 andrew     (501) staff       (20)     9149 2021-08-31 21:20:11.000000 argo-client-0.0.8/argo_client/interaction.py
--rw-r--r--   0 andrew     (501) staff       (20)     1189 2021-06-30 16:07:44.000000 argo-client-0.0.8/argo_client/netstring.py
--rw-r--r--   0 andrew     (501) staff       (20)        0 2021-06-30 16:07:44.000000 argo-client-0.0.8/argo_client/py.typed
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2021-09-10 16:42:10.289988 argo-client-0.0.8/argo_client.egg-info/
--rw-r--r--   0 andrew     (501) staff       (20)     1097 2021-09-10 16:42:10.000000 argo-client-0.0.8/argo_client.egg-info/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)      398 2021-09-10 16:42:10.000000 argo-client-0.0.8/argo_client.egg-info/SOURCES.txt
--rw-r--r--   0 andrew     (501) staff       (20)        1 2021-09-10 16:42:10.000000 argo-client-0.0.8/argo_client.egg-info/dependency_links.txt
--rw-r--r--   0 andrew     (501) staff       (20)        1 2021-07-22 21:53:04.000000 argo-client-0.0.8/argo_client.egg-info/not-zip-safe
--rw-r--r--   0 andrew     (501) staff       (20)       14 2021-09-10 16:42:10.000000 argo-client-0.0.8/argo_client.egg-info/requires.txt
--rw-r--r--   0 andrew     (501) staff       (20)       12 2021-09-10 16:42:10.000000 argo-client-0.0.8/argo_client.egg-info/top_level.txt
--rw-r--r--   0 andrew     (501) staff       (20)      104 2021-06-30 16:07:44.000000 argo-client-0.0.8/pyproject.toml
--rw-r--r--   0 andrew     (501) staff       (20)       38 2021-09-10 16:42:10.290831 argo-client-0.0.8/setup.cfg
--rw-r--r--   0 andrew     (501) staff       (20)     1309 2021-09-10 16:19:44.000000 argo-client-0.0.8/setup.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2021-09-13 16:46:44.696109 argo-client-0.0.9/
+-rw-r--r--   0 andrew     (501) staff       (20)     1457 2021-09-10 17:05:05.000000 argo-client-0.0.9/LICENSE
+-rw-r--r--   0 andrew     (501) staff       (20)     1097 2021-09-13 16:46:44.695868 argo-client-0.0.9/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)      222 2021-09-10 17:05:05.000000 argo-client-0.0.9/README.md
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2021-09-13 16:46:44.694018 argo-client-0.0.9/argo_client/
+-rw-r--r--   0 andrew     (501) staff       (20)        0 2021-09-10 17:05:05.000000 argo-client-0.0.9/argo_client/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)    17459 2021-09-10 17:05:28.000000 argo-client-0.0.9/argo_client/connection.py
+-rw-r--r--   0 andrew     (501) staff       (20)     9239 2021-09-10 23:46:26.000000 argo-client-0.0.9/argo_client/interaction.py
+-rw-r--r--   0 andrew     (501) staff       (20)     1189 2021-09-10 17:05:05.000000 argo-client-0.0.9/argo_client/netstring.py
+-rw-r--r--   0 andrew     (501) staff       (20)        0 2021-09-10 17:05:05.000000 argo-client-0.0.9/argo_client/py.typed
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2021-09-13 16:46:44.695523 argo-client-0.0.9/argo_client.egg-info/
+-rw-r--r--   0 andrew     (501) staff       (20)     1097 2021-09-13 16:46:44.000000 argo-client-0.0.9/argo_client.egg-info/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)      372 2021-09-13 16:46:44.000000 argo-client-0.0.9/argo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        1 2021-09-13 16:46:44.000000 argo-client-0.0.9/argo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        1 2021-09-10 22:33:17.000000 argo-client-0.0.9/argo_client.egg-info/not-zip-safe
+-rw-r--r--   0 andrew     (501) staff       (20)       14 2021-09-13 16:46:44.000000 argo-client-0.0.9/argo_client.egg-info/requires.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       12 2021-09-13 16:46:44.000000 argo-client-0.0.9/argo_client.egg-info/top_level.txt
+-rw-r--r--   0 andrew     (501) staff       (20)      104 2021-09-10 17:05:05.000000 argo-client-0.0.9/pyproject.toml
+-rw-r--r--   0 andrew     (501) staff       (20)       38 2021-09-13 16:46:44.696196 argo-client-0.0.9/setup.cfg
+-rw-r--r--   0 andrew     (501) staff       (20)     1309 2021-09-10 22:32:39.000000 argo-client-0.0.9/setup.py
```

### Comparing `argo-client-0.0.8/LICENSE` & `argo-client-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `argo-client-0.0.8/PKG-INFO` & `argo-client-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argo-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: A JSON RPC client library.
 Home-page: https://github.com/GaloisInc/argo
 Author: Galois, Inc.
 Author-email: andrew@galois.com
 License: BSD
 Project-URL: Changelog, https://github.com/GaloisInc/argo/blob/master/python/CHANGELOG.md
 Project-URL: Source, https://github.com/GaloisInc/argo/tree/master/python
```

### Comparing `argo-client-0.0.8/argo_client/connection.py` & `argo-client-0.0.9/argo_client/connection.py`

 * *Files identical despite different names*

### Comparing `argo-client-0.0.8/argo_client/interaction.py` & `argo-client-0.0.9/argo_client/interaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Higher-level tracking of the semantics of specific commands."""
 
 from argo_client.connection import ServerConnection
 
 from abc import abstractmethod
-from typing import Any, Dict, Tuple
+from typing import Any, Dict, Optional, Tuple
 from typing_extensions import Protocol
 
 
 class HasServerConnection(Protocol):
     server_connection: ServerConnection
 
 class HasProtocolState(Protocol):
@@ -49,26 +49,28 @@
     associated with the resquest.
 
     """
     _method: str
     _params: Dict[str, Any]
 
     def __init__(self, method: str, params: Dict[str, Any],
-                 connection: HasProtocolState) -> None:
+                 connection: HasProtocolState,
+                 *,
+                 timeout: Optional[float]) -> None:
 
         self.connection = connection
         self._raw_response = None
         self.init_state = connection.protocol_state()
         self._method = method
         self._params = params
         self.add_param('state', self.init_state)
         self.request_id = \
             connection. \
             server_connection. \
-            send_command(self._method, self._params)
+            send_command(self._method, self._params, timeout=timeout)
 
     def add_param(self, name: str, val: Any) -> None:
         self._params[name] = val
 
     def raw_result(self) -> Any:
         """Get the JSON response associated with the request. Blocks until the
         reply is received.
```

### Comparing `argo-client-0.0.8/argo_client/netstring.py` & `argo-client-0.0.9/argo_client/netstring.py`

 * *Files identical despite different names*

### Comparing `argo-client-0.0.8/argo_client.egg-info/PKG-INFO` & `argo-client-0.0.9/argo_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argo-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: A JSON RPC client library.
 Home-page: https://github.com/GaloisInc/argo
 Author: Galois, Inc.
 Author-email: andrew@galois.com
 License: BSD
 Project-URL: Changelog, https://github.com/GaloisInc/argo/blob/master/python/CHANGELOG.md
 Project-URL: Source, https://github.com/GaloisInc/argo/tree/master/python
```

### Comparing `argo-client-0.0.8/setup.py` & `argo-client-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open("README.md") as f:
         content += f.read()
     return content
 
 setup(
     name="argo-client",
     python_requires=">=3.7",
-    version="0.0.8",
+    version="0.0.9",
     url="https://github.com/GaloisInc/argo",
     project_urls={
         "Changelog": "https://github.com/GaloisInc/argo/blob/master/python/CHANGELOG.md",
         "Source": "https://github.com/GaloisInc/argo/tree/master/python",
         "Bug Tracker": "https://github.com/GaloisInc/argo/issues"
     },
     license="BSD",
```

