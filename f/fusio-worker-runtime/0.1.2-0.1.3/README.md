# Comparing `tmp/fusio_worker_runtime-0.1.2.tar.gz` & `tmp/fusio_worker_runtime-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusio_worker_runtime-0.1.2.tar", last modified: Mon May 13 19:00:18 2024, max compression
+gzip compressed data, was "fusio_worker_runtime-0.1.3.tar", last modified: Wed May 15 20:21:58 2024, max compression
```

## Comparing `fusio_worker_runtime-0.1.2.tar` & `fusio_worker_runtime-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:00:18.237080 fusio_worker_runtime-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-13 19:00:18.237080 fusio_worker_runtime-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:00:18.237080 fusio_worker_runtime-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:00:18.233080 fusio_worker_runtime-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:00:18.237080 fusio_worker_runtime-0.1.2/src/fusio_worker_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-13 19:00:18.000000 fusio_worker_runtime-0.1.2/src/fusio_worker_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-13 19:00:18.000000 fusio_worker_runtime-0.1.2/src/fusio_worker_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:00:18.000000 fusio_worker_runtime-0.1.2/src/fusio_worker_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-13 19:00:18.000000 fusio_worker_runtime-0.1.2/src/fusio_worker_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 19:00:18.000000 fusio_worker_runtime-0.1.2/src/fusio_worker_runtime.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:00:18.233080 fusio_worker_runtime-0.1.2/src/runtime/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:00:18.237080 fusio_worker_runtime-0.1.2/src/runtime/generated/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/about.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/execute_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/execute_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/execute_context_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/execute_context_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/execute_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/execute_request_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/response_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/response_http.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/response_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/generated/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-13 19:00:14.000000 fusio_worker_runtime-0.1.2/src/runtime/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:58.264879 fusio_worker_runtime-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-15 20:21:58.264879 fusio_worker_runtime-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:21:58.264879 fusio_worker_runtime-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:58.260879 fusio_worker_runtime-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:58.264879 fusio_worker_runtime-0.1.3/src/fusio_worker_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-15 20:21:58.000000 fusio_worker_runtime-0.1.3/src/fusio_worker_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-15 20:21:58.000000 fusio_worker_runtime-0.1.3/src/fusio_worker_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:21:58.000000 fusio_worker_runtime-0.1.3/src/fusio_worker_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 20:21:58.000000 fusio_worker_runtime-0.1.3/src/fusio_worker_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 20:21:58.000000 fusio_worker_runtime-0.1.3/src/fusio_worker_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:58.264879 fusio_worker_runtime-0.1.3/src/runtime/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:21:58.264879 fusio_worker_runtime-0.1.3/src/runtime/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/execute_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/execute_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/execute_context_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/execute_context_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/execute_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/execute_request_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/response_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/response_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/response_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/generated/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-15 20:21:46.000000 fusio_worker_runtime-0.1.3/src/runtime/runtime.py
```

### Comparing `fusio_worker_runtime-0.1.2/LICENSE` & `fusio_worker_runtime-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fusio_worker_runtime-0.1.2/PKG-INFO` & `fusio_worker_runtime-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusio-worker-runtime
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fusio worker Python runtime
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/fusio-worker-python-runtime
 Project-URL: Issues, https://github.com/apioo/fusio-worker-python-runtime/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusio_worker_runtime-0.1.2/pyproject.toml` & `fusio_worker_runtime-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fusio-worker-runtime"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Fusio worker Python runtime"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `fusio_worker_runtime-0.1.2/src/fusio_worker_runtime.egg-info/PKG-INFO` & `fusio_worker_runtime-0.1.3/src/fusio_worker_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusio-worker-runtime
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fusio worker Python runtime
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/fusio-worker-python-runtime
 Project-URL: Issues, https://github.com/apioo/fusio-worker-python-runtime/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusio_worker_runtime-0.1.2/src/fusio_worker_runtime.egg-info/SOURCES.txt` & `fusio_worker_runtime-0.1.3/src/fusio_worker_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusio_worker_runtime-0.1.2/src/runtime/generated/execute.py` & `fusio_worker_runtime-0.1.3/src/runtime/generated/execute.py`

 * *Files identical despite different names*

### Comparing `fusio_worker_runtime-0.1.2/src/runtime/generated/execute_context.py` & `fusio_worker_runtime-0.1.3/src/runtime/generated/execute_context.py`

 * *Files identical despite different names*

### Comparing `fusio_worker_runtime-0.1.2/src/runtime/generated/execute_context_user.py` & `fusio_worker_runtime-0.1.3/src/runtime/generated/execute_context_user.py`

 * *Files identical despite different names*

### Comparing `fusio_worker_runtime-0.1.2/src/runtime/generated/execute_request.py` & `fusio_worker_runtime-0.1.3/src/runtime/generated/execute_request.py`

 * *Files identical despite different names*

### Comparing `fusio_worker_runtime-0.1.2/src/runtime/generated/execute_request_context.py` & `fusio_worker_runtime-0.1.3/src/runtime/generated/execute_request_context.py`

 * *Files identical despite different names*

### Comparing `fusio_worker_runtime-0.1.2/src/runtime/generated/response.py` & `fusio_worker_runtime-0.1.3/src/runtime/generated/response.py`

 * *Files identical despite different names*

### Comparing `fusio_worker_runtime-0.1.2/src/runtime/runtime.py` & `fusio_worker_runtime-0.1.3/src/runtime/runtime.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 import httpx
 import psycopg2
 import pymysql.cursors
 from elasticsearch import Elasticsearch
 from pymongo import MongoClient
 
-from generated.about import About
-from generated.execute import Execute
-from generated.execute_connection import ExecuteConnection
-from generated.response import Response
-from generated.response_event import ResponseEvent
-from generated.response_http import ResponseHTTP
-from generated.response_log import ResponseLog
+from .generated.about import About
+from .generated.execute import Execute
+from .generated.execute_connection import ExecuteConnection
+from .generated.response import Response
+from .generated.response_event import ResponseEvent
+from .generated.response_http import ResponseHTTP
+from .generated.response_log import ResponseLog
 
 
 class Runtime:
     def get(self):
         about = About()
         about.api_version = "1.0.0"
         about.language = "python"
```

