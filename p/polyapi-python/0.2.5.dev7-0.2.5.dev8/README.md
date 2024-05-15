# Comparing `tmp/polyapi_python-0.2.5.dev7.tar.gz` & `tmp/polyapi_python-0.2.5.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi_python-0.2.5.dev7.tar", last modified: Tue May 14 20:02:59 2024, max compression
+gzip compressed data, was "polyapi_python-0.2.5.dev8.tar", last modified: Tue May 14 20:34:28 2024, max compression
```

## Comparing `polyapi_python-0.2.5.dev7.tar` & `polyapi_python-0.2.5.dev8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:02:59.276771 polyapi_python-0.2.5.dev7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-14 20:02:59.276771 polyapi_python-0.2.5.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:02:59.272771 polyapi_python-0.2.5.dev7/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/rendered_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:02:59.276771 polyapi_python-0.2.5.dev7/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-14 20:02:59.000000 polyapi_python-0.2.5.dev7/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-14 20:02:59.000000 polyapi_python-0.2.5.dev7/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:02:59.000000 polyapi_python-0.2.5.dev7/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 20:02:59.000000 polyapi_python-0.2.5.dev7/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 20:02:59.000000 polyapi_python-0.2.5.dev7/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:02:59.276771 polyapi_python-0.2.5.dev7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:02:59.276771 polyapi_python-0.2.5.dev7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/tests/test_rendered_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-14 20:02:55.000000 polyapi_python-0.2.5.dev7/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:34:28.182940 polyapi_python-0.2.5.dev8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-14 20:34:28.182940 polyapi_python-0.2.5.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:34:28.182940 polyapi_python-0.2.5.dev8/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/rendered_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:34:28.182940 polyapi_python-0.2.5.dev8/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-14 20:34:28.000000 polyapi_python-0.2.5.dev8/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-14 20:34:28.000000 polyapi_python-0.2.5.dev8/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:34:28.000000 polyapi_python-0.2.5.dev8/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 20:34:28.000000 polyapi_python-0.2.5.dev8/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 20:34:28.000000 polyapi_python-0.2.5.dev8/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:34:28.186940 polyapi_python-0.2.5.dev8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:34:28.182940 polyapi_python-0.2.5.dev8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_rendered_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_variables.py
```

### Comparing `polyapi_python-0.2.5.dev7/LICENSE` & `polyapi_python-0.2.5.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/PKG-INFO` & `polyapi_python-0.2.5.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.5.dev7
+Version: 0.2.5.dev8
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.5.dev7/README.md` & `polyapi_python-0.2.5.dev8/README.md`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/__init__.py` & `polyapi_python-0.2.5.dev8/polyapi/__init__.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/api.py` & `polyapi_python-0.2.5.dev8/polyapi/api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/auth.py` & `polyapi_python-0.2.5.dev8/polyapi/auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/cli.py` & `polyapi_python-0.2.5.dev8/polyapi/cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/client.py` & `polyapi_python-0.2.5.dev8/polyapi/client.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/config.py` & `polyapi_python-0.2.5.dev8/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/constants.py` & `polyapi_python-0.2.5.dev8/polyapi/constants.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/error_handler.py` & `polyapi_python-0.2.5.dev8/polyapi/error_handler.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/execute.py` & `polyapi_python-0.2.5.dev8/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/function_cli.py` & `polyapi_python-0.2.5.dev8/polyapi/function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/generate.py` & `polyapi_python-0.2.5.dev8/polyapi/generate.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/rendered_spec.py` & `polyapi_python-0.2.5.dev8/polyapi/rendered_spec.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Dict, Optional
+import os
+from typing import Optional
 
 import requests
 from polyapi.config import get_api_key_and_url
 from polyapi.generate import read_cached_specs, render_spec
 from polyapi.typedefs import SpecificationDto
 
 
@@ -20,29 +21,27 @@
         data["customFunctionId"] = spec["id"]
     else:
         raise NotImplementedError("todo")
 
     # use super key on develop-k8s here!
     _, base_url = get_api_key_and_url()
     if not base_url:
-        # local node server runs on port 8000
-        base_url = "http://localhost:8000"
+        base_url = os.environ.get("HOST_URL")
 
     url = f"{base_url}/functions/rendered-specs"
     headers = {"Authorization": f"Bearer {api_key}"}
     resp = requests.post(url, json=data, headers=headers)
     assert resp.status_code == 201, (resp.text, resp.status_code)
     # this needs to run with something like `kn func run...`
 
 
 def _get_spec(api_key: str, spec_id: str) -> Optional[SpecificationDto]:
     _, base_url = get_api_key_and_url()
     if not base_url:
-        # local node server runs on port 8000
-        base_url = "http://localhost:8000"
+        base_url = os.environ.get("HOST_URL")
 
     url = f"{base_url}/specs"
     headers = {"Authorization": f"Bearer {api_key}"}
     resp = requests.get(url, headers=headers)
     if resp.status_code == 200:
         specs = resp.json()
         for spec in specs:
```

### Comparing `polyapi_python-0.2.5.dev7/polyapi/schema.py` & `polyapi_python-0.2.5.dev8/polyapi/schema.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/server.py` & `polyapi_python-0.2.5.dev8/polyapi/server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/typedefs.py` & `polyapi_python-0.2.5.dev8/polyapi/typedefs.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/utils.py` & `polyapi_python-0.2.5.dev8/polyapi/utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/variables.py` & `polyapi_python-0.2.5.dev8/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi/webhook.py` & `polyapi_python-0.2.5.dev8/polyapi/webhook.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/polyapi_python.egg-info/PKG-INFO` & `polyapi_python-0.2.5.dev8/polyapi_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.5.dev7
+Version: 0.2.5.dev8
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.5.dev7/polyapi_python.egg-info/SOURCES.txt` & `polyapi_python-0.2.5.dev8/polyapi_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/pyproject.toml` & `polyapi_python-0.2.5.dev8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.5.dev7"
+version = "0.2.5.dev8"
 description = "The Python Client for PolyAPI, the IPaaS by Developers for Developers"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
     "pydantic==2.6.4",
```

### Comparing `polyapi_python-0.2.5.dev7/tests/test_api.py` & `polyapi_python-0.2.5.dev8/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/tests/test_auth.py` & `polyapi_python-0.2.5.dev8/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/tests/test_function_cli.py` & `polyapi_python-0.2.5.dev8/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/tests/test_rendered_spec.py` & `polyapi_python-0.2.5.dev8/tests/test_rendered_spec.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/tests/test_server.py` & `polyapi_python-0.2.5.dev8/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/tests/test_utils.py` & `polyapi_python-0.2.5.dev8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev7/tests/test_variables.py` & `polyapi_python-0.2.5.dev8/tests/test_variables.py`

 * *Files identical despite different names*

