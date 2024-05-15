# Comparing `tmp/fluxional-0.1.6.tar.gz` & `tmp/fluxional-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxional-0.1.6.tar", max compression
+gzip compressed data, was "fluxional-0.1.7.tar", max compression
```

## Comparing `fluxional-0.1.6.tar` & `fluxional-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2024-04-28 17:10:39.085356 fluxional-0.1.6/LICENSE
--rw-r--r--   0        0        0     3908 2024-04-29 21:12:21.619975 fluxional-0.1.6/README.md
--rw-r--r--   0        0        0      421 2024-05-09 01:45:41.373948 fluxional-0.1.6/fluxional/__init__.py
--rw-r--r--   0        0        0       85 2024-04-28 18:14:21.913877 fluxional-0.1.6/fluxional/__main__.py
--rw-r--r--   0        0        0     1429 2024-04-28 18:14:21.923877 fluxional-0.1.6/fluxional/cli/__init__.py
--rw-r--r--   0        0        0      397 2024-04-28 18:14:21.923877 fluxional-0.1.6/fluxional/core/__init__.py
--rw-r--r--   0        0        0    21405 2024-05-09 01:45:17.632254 fluxional-0.1.6/fluxional/core/app.py
--rw-r--r--   0        0        0     6976 2024-04-28 18:14:21.933877 fluxional-0.1.6/fluxional/core/core.py
--rw-r--r--   0        0        0     2927 2024-04-28 18:14:21.933877 fluxional-0.1.6/fluxional/core/events.py
--rw-r--r--   0        0        0    11708 2024-04-28 18:14:21.943877 fluxional-0.1.6/fluxional/core/handlers.py
--rw-r--r--   0        0        0        1 2024-04-28 18:14:21.943877 fluxional-0.1.6/fluxional/core/infrastructure/__init__.py
--rw-r--r--   0        0        0    19676 2024-04-28 18:14:21.953877 fluxional-0.1.6/fluxional/core/infrastructure/base.py
--rw-r--r--   0        0        0     7699 2024-04-28 18:14:21.953877 fluxional-0.1.6/fluxional/core/infrastructure/cdk.py
--rw-r--r--   0        0        0     9554 2024-04-28 18:14:21.953877 fluxional-0.1.6/fluxional/core/infrastructure/resources.py
--rw-r--r--   0        0        0      816 2024-04-28 18:14:21.953877 fluxional-0.1.6/fluxional/core/infrastructure/types.py
--rw-r--r--   0        0        0     5818 2024-04-28 18:14:21.953877 fluxional-0.1.6/fluxional/core/logic.py
--rw-r--r--   0        0        0     8343 2024-04-28 18:14:21.953877 fluxional-0.1.6/fluxional/core/settings.py
--rw-r--r--   0        0        0     4045 2024-04-28 18:14:21.953877 fluxional-0.1.6/fluxional/core/tools.py
--rw-r--r--   0        0        0     5158 2024-04-28 18:14:21.953877 fluxional-0.1.6/fluxional/core/types.py
--rw-r--r--   0        0        0       74 2024-04-28 18:14:21.953877 fluxional-0.1.6/fluxional/deployment/__init__.py
--rw-r--r--   0        0        0     1164 2024-04-28 18:14:21.953877 fluxional-0.1.6/fluxional/deployment/constants.py
--rw-r--r--   0        0        0    15517 2024-04-30 22:02:31.375706 fluxional-0.1.6/fluxional/deployment/engine.py
--rw-r--r--   0        0        0      345 2024-04-28 18:14:21.953877 fluxional-0.1.6/fluxional/deployment/exceptions.py
--rw-r--r--   0        0        0        1 2024-04-30 22:01:04.012000 fluxional-0.1.6/fluxional/deployment/utils.py
--rw-r--r--   0        0        0     3652 2024-04-28 18:14:21.963877 fluxional-0.1.6/fluxional/dev/__init__.py
--rw-r--r--   0        0        0     3003 2024-04-28 18:14:21.963877 fluxional-0.1.6/fluxional/dev/client.py
--rw-r--r--   0        0        0     3350 2024-04-28 18:14:21.963877 fluxional-0.1.6/fluxional/dev/runner.py
--rw-r--r--   0        0        0      326 2024-04-28 18:14:21.963877 fluxional-0.1.6/fluxional/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-28 18:14:21.963877 fluxional-0.1.6/fluxional/py.typed
--rw-r--r--   0        0        0      461 2024-04-28 18:14:21.963877 fluxional-0.1.6/fluxional/types.py
--rw-r--r--   0        0        0      935 2024-04-28 18:14:21.963877 fluxional-0.1.6/fluxional/utils.py
--rw-r--r--   0        0        0     1151 2024-05-09 01:45:36.713938 fluxional-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 fluxional-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-28 17:10:39.085356 fluxional-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3908 2024-04-29 21:12:21.619975 fluxional-0.1.7/README.md
+-rw-r--r--   0        0        0      421 2024-05-15 20:00:12.862573 fluxional-0.1.7/fluxional/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-28 18:14:21.913877 fluxional-0.1.7/fluxional/__main__.py
+-rw-r--r--   0        0        0     1429 2024-04-28 18:14:21.923877 fluxional-0.1.7/fluxional/cli/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-28 18:14:21.923877 fluxional-0.1.7/fluxional/core/__init__.py
+-rw-r--r--   0        0        0    21405 2024-05-09 01:45:17.632254 fluxional-0.1.7/fluxional/core/app.py
+-rw-r--r--   0        0        0     6976 2024-04-28 18:14:21.933877 fluxional-0.1.7/fluxional/core/core.py
+-rw-r--r--   0        0        0     2927 2024-04-28 18:14:21.933877 fluxional-0.1.7/fluxional/core/events.py
+-rw-r--r--   0        0        0    11708 2024-04-28 18:14:21.943877 fluxional-0.1.7/fluxional/core/handlers.py
+-rw-r--r--   0        0        0        1 2024-04-28 18:14:21.943877 fluxional-0.1.7/fluxional/core/infrastructure/__init__.py
+-rw-r--r--   0        0        0    20142 2024-05-15 19:51:13.339223 fluxional-0.1.7/fluxional/core/infrastructure/base.py
+-rw-r--r--   0        0        0     7699 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/infrastructure/cdk.py
+-rw-r--r--   0        0        0     9554 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/infrastructure/resources.py
+-rw-r--r--   0        0        0      816 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/infrastructure/types.py
+-rw-r--r--   0        0        0     5818 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/logic.py
+-rw-r--r--   0        0        0     8343 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/settings.py
+-rw-r--r--   0        0        0     4045 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/tools.py
+-rw-r--r--   0        0        0     5158 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/core/types.py
+-rw-r--r--   0        0        0       74 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/deployment/__init__.py
+-rw-r--r--   0        0        0     1164 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/deployment/constants.py
+-rw-r--r--   0        0        0    15517 2024-04-30 22:02:31.375706 fluxional-0.1.7/fluxional/deployment/engine.py
+-rw-r--r--   0        0        0      345 2024-04-28 18:14:21.953877 fluxional-0.1.7/fluxional/deployment/exceptions.py
+-rw-r--r--   0        0        0        1 2024-04-30 22:01:04.012000 fluxional-0.1.7/fluxional/deployment/utils.py
+-rw-r--r--   0        0        0     3652 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/dev/__init__.py
+-rw-r--r--   0        0        0     3003 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/dev/client.py
+-rw-r--r--   0        0        0     3350 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/dev/runner.py
+-rw-r--r--   0        0        0      326 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/py.typed
+-rw-r--r--   0        0        0      461 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/types.py
+-rw-r--r--   0        0        0      935 2024-04-28 18:14:21.963877 fluxional-0.1.7/fluxional/utils.py
+-rw-r--r--   0        0        0     1151 2024-05-15 20:00:26.002692 fluxional-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 fluxional-0.1.7/PKG-INFO
```

### Comparing `fluxional-0.1.6/LICENSE` & `fluxional-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/README.md` & `fluxional-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/cli/__init__.py` & `fluxional-0.1.7/fluxional/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/core/app.py` & `fluxional-0.1.7/fluxional/core/app.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/core/core.py` & `fluxional-0.1.7/fluxional/core/core.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/core/events.py` & `fluxional-0.1.7/fluxional/core/events.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/core/handlers.py` & `fluxional-0.1.7/fluxional/core/handlers.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/core/infrastructure/base.py` & `fluxional-0.1.7/fluxional/core/infrastructure/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,14 +414,19 @@
                         aws_s3_notifications.LambdaDestination(func)
                     )
 
                     bucket.add_object_removed_notification(
                         aws_s3_notifications.LambdaDestination(func)
                     )
 
+                    # This will cause a dependency error and makes no sense if on file upload
+                    # The lambda can't even read the file
+                    # We will refrain from writing though as that could create infinite loop for now
+                    bucket.grant_read(func)
+
     def add_resource_to_stack(self, resource: AllResources):
         if isinstance(resource, LambdaFunction):
             self.add_lambda_function(resource)
         elif isinstance(resource, ApiGateway):
             self.add_rest_api_gateway(resource)
         elif isinstance(resource, WsGateway):
             self.add_websocket_gateway(resource)
@@ -472,18 +477,21 @@
             environment_vars=self.settings.environment,
         )
 
     def stack(self) -> Stack:
         stack_builder = self.get_stack()
         ready: list[str] = []
         resources = self._infrastructure.resources
+        counter = 0
+        limit = 500
 
         # Build each resources based on dependencies resolution
         # Iterate until all resources are built
         while True:
+            counter += 1
             left = [
                 resources[stack_resource].id
                 for stack_resource in resources
                 if resources[stack_resource].id not in ready
             ]
 
             for k in resources:
@@ -508,11 +516,14 @@
                     if not all([i.resource_id in ready for i in permissions]):
                         continue
 
                 # Add the resource to the base infrastructure
                 stack_builder.add_resource_to_stack(resource)
                 ready.append(resource.id)
 
+            if counter > limit:
+                raise ValueError("Resource dependency loop detected")
+
             if not left:
                 break
 
         return stack_builder
```

### Comparing `fluxional-0.1.6/fluxional/core/infrastructure/cdk.py` & `fluxional-0.1.7/fluxional/core/infrastructure/cdk.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/core/infrastructure/resources.py` & `fluxional-0.1.7/fluxional/core/infrastructure/resources.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/core/infrastructure/types.py` & `fluxional-0.1.7/fluxional/core/infrastructure/types.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/core/logic.py` & `fluxional-0.1.7/fluxional/core/logic.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/core/settings.py` & `fluxional-0.1.7/fluxional/core/settings.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/core/tools.py` & `fluxional-0.1.7/fluxional/core/tools.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/core/types.py` & `fluxional-0.1.7/fluxional/core/types.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/deployment/constants.py` & `fluxional-0.1.7/fluxional/deployment/constants.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/deployment/engine.py` & `fluxional-0.1.7/fluxional/deployment/engine.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/dev/__init__.py` & `fluxional-0.1.7/fluxional/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/dev/client.py` & `fluxional-0.1.7/fluxional/dev/client.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/dev/runner.py` & `fluxional-0.1.7/fluxional/dev/runner.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/fluxional/utils.py` & `fluxional-0.1.7/fluxional/utils.py`

 * *Files identical despite different names*

### Comparing `fluxional-0.1.6/pyproject.toml` & `fluxional-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fluxional"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["fluxional"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">= 3.10 < 4.0"
```

### Comparing `fluxional-0.1.6/PKG-INFO` & `fluxional-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxional
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: MIT
 Author: fluxional
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

