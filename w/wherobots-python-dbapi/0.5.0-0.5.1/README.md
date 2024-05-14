# Comparing `tmp/wherobots_python_dbapi-0.5.0.tar.gz` & `tmp/wherobots_python_dbapi-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wherobots_python_dbapi-0.5.0.tar", max compression
+gzip compressed data, was "wherobots_python_dbapi-0.5.1.tar", max compression
```

## Comparing `wherobots_python_dbapi-0.5.0.tar` & `wherobots_python_dbapi-0.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/LICENSE
--rw-r--r--   0        0        0     2651 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/README.md
--rw-r--r--   0        0        0      944 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/__init__.py
--rw-r--r--   0        0        0      184 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/__init__.py
--rw-r--r--   0        0        0     8317 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/connection.py
--rw-r--r--   0        0        0     1767 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/constants.py
--rw-r--r--   0        0        0     2774 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/cursor.py
--rw-r--r--   0        0        0     5718 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/driver.py
--rw-r--r--   0        0        0      310 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/errors.py
--rw-r--r--   0        0        0       80 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/region.py
--rw-r--r--   0        0        0      491 2024-05-13 03:05:01.527868 wherobots_python_dbapi-0.5.0/wherobots/db/runtime.py
--rw-r--r--   0        0        0     3495 1970-01-01 00:00:00.000000 wherobots_python_dbapi-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 22:50:19.264396 wherobots_python_dbapi-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2651 2024-05-13 22:50:19.264396 wherobots_python_dbapi-0.5.1/README.md
+-rw-r--r--   0        0        0      944 2024-05-13 22:50:19.264396 wherobots_python_dbapi-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 22:50:19.264396 wherobots_python_dbapi-0.5.1/wherobots/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-13 22:50:19.264396 wherobots_python_dbapi-0.5.1/wherobots/db/__init__.py
+-rw-r--r--   0        0        0     8317 2024-05-13 22:50:19.264396 wherobots_python_dbapi-0.5.1/wherobots/db/connection.py
+-rw-r--r--   0        0        0     1767 2024-05-13 22:50:19.264396 wherobots_python_dbapi-0.5.1/wherobots/db/constants.py
+-rw-r--r--   0        0        0     2774 2024-05-13 22:50:19.264396 wherobots_python_dbapi-0.5.1/wherobots/db/cursor.py
+-rw-r--r--   0        0        0     5754 2024-05-13 22:50:19.264396 wherobots_python_dbapi-0.5.1/wherobots/db/driver.py
+-rw-r--r--   0        0        0      310 2024-05-13 22:50:19.264396 wherobots_python_dbapi-0.5.1/wherobots/db/errors.py
+-rw-r--r--   0        0        0       80 2024-05-13 22:50:19.264396 wherobots_python_dbapi-0.5.1/wherobots/db/region.py
+-rw-r--r--   0        0        0      491 2024-05-13 22:50:19.264396 wherobots_python_dbapi-0.5.1/wherobots/db/runtime.py
+-rw-r--r--   0        0        0     3495 1970-01-01 00:00:00.000000 wherobots_python_dbapi-0.5.1/PKG-INFO
```

### Comparing `wherobots_python_dbapi-0.5.0/LICENSE` & `wherobots_python_dbapi-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wherobots_python_dbapi-0.5.0/README.md` & `wherobots_python_dbapi-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `wherobots_python_dbapi-0.5.0/pyproject.toml` & `wherobots_python_dbapi-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wherobots-python-dbapi"
-version = "0.5.0"
+version = "0.5.1"
 description = "Python DB-API driver for Wherobots DB"
 authors = ["Maxime Petazzoni <max@wherobots.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "wherobots" }]
 
 [project.urls]
```

### Comparing `wherobots_python_dbapi-0.5.0/wherobots/db/connection.py` & `wherobots_python_dbapi-0.5.1/wherobots/db/connection.py`

 * *Files identical despite different names*

### Comparing `wherobots_python_dbapi-0.5.0/wherobots/db/constants.py` & `wherobots_python_dbapi-0.5.1/wherobots/db/constants.py`

 * *Files identical despite different names*

### Comparing `wherobots_python_dbapi-0.5.0/wherobots/db/cursor.py` & `wherobots_python_dbapi-0.5.1/wherobots/db/cursor.py`

 * *Files identical despite different names*

### Comparing `wherobots_python_dbapi-0.5.0/wherobots/db/driver.py` & `wherobots_python_dbapi-0.5.1/wherobots/db/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     headers = {}
     if token:
         headers["Authorization"] = f"Bearer {token}"
     elif api_key:
         headers["X-API-Key"] = api_key
 
+    host = host or DEFAULT_ENDPOINT
     runtime = runtime or DEFAULT_RUNTIME
     region = region or DEFAULT_REGION
 
     logging.info(
         "Requesting %s/%s runtime in %s from %s ...",
         runtime.name,
         runtime.value,
```

### Comparing `wherobots_python_dbapi-0.5.0/PKG-INFO` & `wherobots_python_dbapi-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wherobots-python-dbapi
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python DB-API driver for Wherobots DB
 License: Apache 2.0
 Author: Maxime Petazzoni
 Author-email: max@wherobots.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

