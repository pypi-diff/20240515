# Comparing `tmp/sindri-0.1.0a23.tar.gz` & `tmp/sindri-0.1.0a24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sindri-0.1.0a23.tar", max compression
+gzip compressed data, was "sindri-0.1.0a24.tar", max compression
```

## Comparing `sindri-0.1.0a23.tar` & `sindri-0.1.0a24.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2024-03-28 21:46:12.836558 sindri-0.1.0a23/LICENSE
--rw-r--r--   0        0        0     1251 2024-03-28 21:46:12.836558 sindri-0.1.0a23/README.md
--rw-r--r--   0        0        0     1030 2024-03-28 21:46:27.532597 sindri-0.1.0a23/pyproject.toml
--rw-r--r--   0        0        0      201 2024-03-28 21:46:12.836558 sindri-0.1.0a23/src/sindri/__init__.py
--rw-r--r--   0        0        0    31954 2024-03-28 21:46:13.148558 sindri-0.1.0a23/src/sindri/sindri.py
--rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 sindri-0.1.0a23/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-15 02:28:28.905309 sindri-0.1.0a24/LICENSE
+-rw-r--r--   0        0        0     1251 2024-05-15 02:28:28.909309 sindri-0.1.0a24/README.md
+-rw-r--r--   0        0        0     1030 2024-05-15 02:28:40.985316 sindri-0.1.0a24/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-15 02:28:28.909309 sindri-0.1.0a24/src/sindri/__init__.py
+-rw-r--r--   0        0        0    32690 2024-05-15 02:28:29.209309 sindri-0.1.0a24/src/sindri/sindri.py
+-rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 sindri-0.1.0a24/PKG-INFO
```

### Comparing `sindri-0.1.0a23/LICENSE` & `sindri-0.1.0a24/LICENSE`

 * *Files identical despite different names*

### Comparing `sindri-0.1.0a23/README.md` & `sindri-0.1.0a24/README.md`

 * *Files identical despite different names*

### Comparing `sindri-0.1.0a23/pyproject.toml` & `sindri-0.1.0a24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ]
 description = "Sindri Python SDK"
 homepage = "https://sindri.app"
 license = "MIT"
 name = "sindri"
 readme = "README.md"
 repository = "https://github.com/Sindri-Labs/sindri-python"
-version = "0.1.0a23"
+version = "0.1.0a24"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.13.0"
 
 [tool.poetry.group.dev.dependencies]
 lazydocs = "^0.4.8"
```

### Comparing `sindri-0.1.0a23/src/sindri/sindri.py` & `sindri-0.1.0a24/src/sindri/sindri.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 import platform
 import tarfile
 import time
 from pprint import pformat
 from urllib.parse import urlparse
 
 import requests  # type: ignore
+from requests.adapters import HTTPAdapter, Retry
 
-__version__ = "v0.1.0a23"
+__version__ = "v0.1.0a24"
 
 
 class Sindri:
     """A utility class for interacting with the [Sindri API](https://www.sindri.app)."""
 
     class APIError(Exception):
         """Custom Exception for Sindri API Errors"""
@@ -230,23 +231,36 @@
 
         # Initialize data if not provided
         if data is None:
             data = {}
 
         # Construct the full path to the API endpoint.
         full_path = os.path.join(self._api_url, path)
+
+        # Create a custom request session that will make all HTTP requests from the same session
+        # retry for a total of 5 times, sleeping between retries with an increasing backoff of
+        # 0s, 2s, 4s, 8s, 16s (the first retry is done immediately). It will retry on basic
+        # connectivity issues (including DNS lookup failures), and HTTP status codes of 502, 503
+        # and 504.
+        session = requests.Session()
+        max_retries = Retry(total=5, backoff_factor=1, status_forcelist=[502, 503, 504])
+        adapter = HTTPAdapter(max_retries=max_retries)
+        session.mount("http://", adapter)
+        session.mount("https://", adapter)
+
+        # Hit the API
         try:
             if method == "POST":
-                response = requests.post(
+                response = session.post(
                     full_path, headers=self.headers_json, data=data, files=files
                 )
             elif method == "GET":
-                response = requests.get(full_path, headers=self.headers_json, params=data)
+                response = session.get(full_path, headers=self.headers_json, params=data)
             elif method == "DELETE":
-                response = requests.delete(full_path, headers=self.headers_json, data=data)
+                response = session.delete(full_path, headers=self.headers_json, data=data)
             else:
                 raise Sindri.APIError("Invalid request method")
         except requests.exceptions.ConnectionError:
             # Raise a clean exception and suppress the original exception's traceback.
             raise Sindri.APIError(
                 f"Unable to connect to the Sindri API. path={full_path}"
             ) from None
```

### Comparing `sindri-0.1.0a23/PKG-INFO` & `sindri-0.1.0a24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sindri
-Version: 0.1.0a23
+Version: 0.1.0a24
 Summary: Sindri Python SDK
 Home-page: https://sindri.app
 License: MIT
 Author: Sindri Labs
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

