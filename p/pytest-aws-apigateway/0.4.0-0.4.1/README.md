# Comparing `tmp/pytest_aws_apigateway-0.4.0.tar.gz` & `tmp/pytest_aws_apigateway-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_aws_apigateway-0.4.0.tar", last modified: Tue May 14 20:14:15 2024, max compression
+gzip compressed data, was "pytest_aws_apigateway-0.4.1.tar", last modified: Tue May 14 20:26:02 2024, max compression
```

## Comparing `pytest_aws_apigateway-0.4.0.tar` & `pytest_aws_apigateway-0.4.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.244119 pytest_aws_apigateway-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.240119 pytest_aws_apigateway-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.240119 pytest_aws_apigateway-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 20:14:15.244119 pytest_aws_apigateway-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.240119 pytest_aws_apigateway-0.4.0/changes/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/changes/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:14:15.244119 pytest_aws_apigateway-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.240119 pytest_aws_apigateway-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.240119 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.244119 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 20:14:15.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-14 20:14:15.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:14:15.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-14 20:14:15.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 20:14:15.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 20:14:15.000000 pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.244119 pytest_aws_apigateway-0.4.0/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tasks/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:15.244119 pytest_aws_apigateway-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tests/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-14 20:14:08.000000 pytest_aws_apigateway-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.982100 pytest_aws_apigateway-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.974100 pytest_aws_apigateway-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/changes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:26:02.982100 pytest_aws_apigateway-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.974100 pytest_aws_apigateway-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 20:26:02.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-14 20:26:02.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:26:02.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-14 20:26:02.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 20:26:02.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 20:26:02.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tasks/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tests/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tox.ini
```

### Comparing `pytest_aws_apigateway-0.4.0/.github/workflows/main.yml` & `pytest_aws_apigateway-0.4.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.0/LICENSE` & `pytest_aws_apigateway-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.0/PKG-INFO` & `pytest_aws_apigateway-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.4.0
+Version: 0.4.1
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytest_aws_apigateway-0.4.0/README.md` & `pytest_aws_apigateway-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.0/pyproject.toml` & `pytest_aws_apigateway-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/apigateway.py` & `pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/apigateway.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 import json
 import re
-from typing import Any, Callable
+from typing import Any
+from typing import Callable
 from typing import Union
 
 import httpx
 import pytest_httpx
 
-from pytest_aws_apigateway.context import LambdaContext, create_context
-from pytest_aws_apigateway.integration import ResponseFormatError
+from pytest_aws_apigateway.context import LambdaContext
+from pytest_aws_apigateway.context import create_context
 from pytest_aws_apigateway.integration import IntegrationResponse
+from pytest_aws_apigateway.integration import ResponseFormatError
 from pytest_aws_apigateway.integration import build_integration_request
 from pytest_aws_apigateway.integration import transform_integration_response
 
 __all__ = ["ApiGatewayMock"]
 
 
 class ApiGatewayMock:
+    """Mock acting as an AWS ApiGateway for AWS Lambda prox integrations."""
+
     def __init__(self, httpx_mock: pytest_httpx.HTTPXMock):
         self.httpx_mock = httpx_mock
         ...
 
     def add_integration(
         self,
         resource: str,
         method: str,
         endpoint: str,
         handler: Callable[[dict[str, Any], LambdaContext], IntegrationResponse],
     ):
+        """
+        Register an AWS Lambda function handler that will be called if a request matches.
+
+        Args:
+            resource: Resource path where to mount the integration. Will be combined with endpoint to match request URLs
+            method: HTTP method for which the integration should be called
+            endpoint: API endpoint for the API gateway. Example: 'http://localhost'
+            handler: AWS Lambda handler function that will be called when a request matches
+        """
         resource = self._normalize_resource(resource)
         endpoint = self._normalize_endpoint(endpoint)
 
         url = self._url_expression(endpoint, resource)
 
         def integration(request: httpx.Request) -> httpx.Response:
             event = build_integration_request(request, resource)
```

### Comparing `pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/context.py` & `pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/context.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway/integration.py` & `pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/PKG-INFO` & `pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.4.0
+Version: 0.4.1
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytest_aws_apigateway-0.4.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt` & `pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.0/tasks/release.py` & `pytest_aws_apigateway-0.4.1/tasks/release.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.0/tests/test_apigateway.py` & `pytest_aws_apigateway-0.4.1/tests/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.0/tests/test_integration.py` & `pytest_aws_apigateway-0.4.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.0/tests/test_plugin.py` & `pytest_aws_apigateway-0.4.1/tests/test_plugin.py`

 * *Files identical despite different names*

