# Comparing `tmp/up42_py-1.0.1.tar.gz` & `tmp/up42_py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up42_py-1.0.1.tar", max compression
+gzip compressed data, was "up42_py-1.0.2.tar", max compression
```

## Comparing `up42_py-1.0.1.tar` & `up42_py-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1061 2024-05-13 13:28:15.224450 up42_py-1.0.1/LICENSE
--rw-r--r--   0        0        0     2927 2024-05-13 13:28:15.224450 up42_py-1.0.1/README.md
--rw-r--r--   0        0        0     1785 2024-05-13 13:28:15.244451 up42_py-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1731 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/__init__.py
--rw-r--r--   0        0        0     7963 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/asset.py
--rw-r--r--   0        0        0     3754 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/asset_searcher.py
--rw-r--r--   0        0        0     5068 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/auth.py
--rw-r--r--   0        0        0    20308 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/catalog.py
--rw-r--r--   0        0        0      706 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/data/aoi_berlin.geojson
--rw-r--r--   0        0        0      703 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/data/aoi_washington.geojson
--rw-r--r--   0        0        0      135 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/host.py
--rw-r--r--   0        0        0        0 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/http/__init__.py
--rw-r--r--   0        0        0     1782 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/http/client.py
--rw-r--r--   0        0        0      482 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/http/config.py
--rw-r--r--   0        0        0      673 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/http/http_adapter.py
--rw-r--r--   0        0        0     3290 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/http/oauth.py
--rw-r--r--   0        0        0     1113 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/http/session.py
--rw-r--r--   0        0        0     1885 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/initialization.py
--rw-r--r--   0        0        0     3424 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/main.py
--rw-r--r--   0        0        0     8372 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/order.py
--rw-r--r--   0        0        0      910 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/stac_client.py
--rw-r--r--   0        0        0     8485 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/storage.py
--rw-r--r--   0        0        0    10622 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/tasking.py
--rw-r--r--   0        0        0     3287 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/tools.py
--rw-r--r--   0        0        0    15164 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/utils.py
--rw-r--r--   0        0        0     6749 2024-05-13 13:28:15.252451 up42_py-1.0.1/up42/webhooks.py
--rw-r--r--   0        0        0     3964 1970-01-01 00:00:00.000000 up42_py-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-15 11:22:44.134850 up42_py-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2927 2024-05-15 11:22:44.134850 up42_py-1.0.2/README.md
+-rw-r--r--   0        0        0     1785 2024-05-15 11:22:44.154850 up42_py-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1731 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/__init__.py
+-rw-r--r--   0        0        0     7963 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/asset.py
+-rw-r--r--   0        0        0     3754 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/asset_searcher.py
+-rw-r--r--   0        0        0     5068 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/auth.py
+-rw-r--r--   0        0        0    20308 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/catalog.py
+-rw-r--r--   0        0        0      706 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/data/aoi_berlin.geojson
+-rw-r--r--   0        0        0      703 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/data/aoi_washington.geojson
+-rw-r--r--   0        0        0      135 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/host.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/http/__init__.py
+-rw-r--r--   0        0        0     1782 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/http/client.py
+-rw-r--r--   0        0        0      482 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/http/config.py
+-rw-r--r--   0        0        0      673 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/http/http_adapter.py
+-rw-r--r--   0        0        0     3378 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/http/oauth.py
+-rw-r--r--   0        0        0     1113 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/http/session.py
+-rw-r--r--   0        0        0     1885 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/initialization.py
+-rw-r--r--   0        0        0     3424 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/main.py
+-rw-r--r--   0        0        0     8372 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/order.py
+-rw-r--r--   0        0        0      910 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/stac_client.py
+-rw-r--r--   0        0        0     8485 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/storage.py
+-rw-r--r--   0        0        0    10622 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/tasking.py
+-rw-r--r--   0        0        0     3287 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/tools.py
+-rw-r--r--   0        0        0    15164 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/utils.py
+-rw-r--r--   0        0        0     6749 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/webhooks.py
+-rw-r--r--   0        0        0     3964 1970-01-01 00:00:00.000000 up42_py-1.0.2/PKG-INFO
```

### Comparing `up42_py-1.0.1/LICENSE` & `up42_py-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/README.md` & `up42_py-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/pyproject.toml` & `up42_py-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "up42-py"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python SDK for UP42, the geospatial marketplace and developer platform."
 authors = ["UP42 GmbH <support@up42.com>"]
 license = "https://github.com/up42/up42-py/blob/master/LICENSE"
 readme = "README.md"
 packages = [
     { include = "up42", from = "." },
 ]
```

### Comparing `up42_py-1.0.1/up42/__init__.py` & `up42_py-1.0.2/up42/__init__.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/asset.py` & `up42_py-1.0.2/up42/asset.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/asset_searcher.py` & `up42_py-1.0.2/up42/asset_searcher.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/auth.py` & `up42_py-1.0.2/up42/auth.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/catalog.py` & `up42_py-1.0.2/up42/catalog.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/data/aoi_berlin.geojson` & `up42_py-1.0.2/up42/data/aoi_berlin.geojson`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/data/aoi_washington.geojson` & `up42_py-1.0.2/up42/data/aoi_washington.geojson`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/http/client.py` & `up42_py-1.0.2/up42/http/client.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/http/http_adapter.py` & `up42_py-1.0.2/up42/http/http_adapter.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/http/oauth.py` & `up42_py-1.0.2/up42/http/oauth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import dataclasses as dc
 import datetime as dt
+import threading
 from typing import Optional, Protocol
 
 import requests
 
 from up42.http import config, http_adapter
 
 
@@ -56,30 +57,32 @@
     ):
         self.token_url = token_settings.token_url
         self.duration = token_settings.duration
         self.timeout = token_settings.timeout
         self.adapter = create_adapter(include_post=True)
         self.retrieve = retrieve
         self._token = self._fetch_token()
+        self._lock = threading.Lock()
 
     def __call__(self, request: requests.PreparedRequest) -> requests.PreparedRequest:
         request.headers["Authorization"] = f"Bearer {self.token.access_token}"
         return request
 
     def _fetch_token(self):
         session = requests.Session()
         session.mount("https://", self.adapter)
         access_token = self.retrieve(session, self.token_url, self.timeout)
         expires_on = dt.datetime.now() + dt.timedelta(seconds=self.duration)
         return Token(access_token=access_token, expires_on=expires_on)
 
     @property
     def token(self) -> Token:
-        if self._token.has_expired:
-            self._token = self._fetch_token()
+        with self._lock:
+            if self._token.has_expired:
+                self._token = self._fetch_token()
         return self._token
 
 
 def detect_settings(
     credentials: Optional[dict],
 ) -> Optional[config.CredentialsSettings]:
     if credentials:
```

### Comparing `up42_py-1.0.1/up42/http/session.py` & `up42_py-1.0.2/up42/http/session.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/initialization.py` & `up42_py-1.0.2/up42/initialization.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/main.py` & `up42_py-1.0.2/up42/main.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/order.py` & `up42_py-1.0.2/up42/order.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/stac_client.py` & `up42_py-1.0.2/up42/stac_client.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/storage.py` & `up42_py-1.0.2/up42/storage.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/tasking.py` & `up42_py-1.0.2/up42/tasking.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/tools.py` & `up42_py-1.0.2/up42/tools.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/utils.py` & `up42_py-1.0.2/up42/utils.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/up42/webhooks.py` & `up42_py-1.0.2/up42/webhooks.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.1/PKG-INFO` & `up42_py-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up42-py
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python SDK for UP42, the geospatial marketplace and developer platform.
 License: https://github.com/up42/up42-py/blob/master/LICENSE
 Author: UP42 GmbH
 Author-email: support@up42.com
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: up42-py Version: 1.0.1 Summary: Python SDK for
+Metadata-Version: 2.1 Name: up42-py Version: 1.0.2 Summary: Python SDK for
 UP42, the geospatial marketplace and developer platform. License: https://
 github.com/up42/up42-py/blob/master/LICENSE Author: UP42 GmbH Author-email:
 support@up42.com Requires-Python: >=3.9,<4 Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

