# Comparing `tmp/kal_middleware-0.0.3.tar.gz` & `tmp/kal_middleware-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kal_middleware-0.0.3.tar", last modified: Thu May  9 12:06:47 2024, max compression
+gzip compressed data, was "kal_middleware-0.0.4.tar", last modified: Wed May 15 09:54:48 2024, max compression
```

## Comparing `kal_middleware-0.0.3.tar` & `kal_middleware-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:06:47.655679 kal_middleware-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:06:47.647679 kal_middleware-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:06:47.647679 kal_middleware-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:06:47.651679 kal_middleware-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-09 12:06:47.655679 kal_middleware-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:06:47.651679 kal_middleware-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:06:47.651679 kal_middleware-0.0.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/docs/jwt.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/docs/kal_middleware.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:06:47.651679 kal_middleware-0.0.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/docs/sts.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:06:47.651679 kal_middleware-0.0.3/kal_middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/kal_middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/kal_middleware/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/kal_middleware/kal_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/kal_middleware/sts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:06:47.655679 kal_middleware-0.0.3/kal_middleware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-09 12:06:47.000000 kal_middleware-0.0.3/kal_middleware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-09 12:06:47.000000 kal_middleware-0.0.3/kal_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:06:47.000000 kal_middleware-0.0.3/kal_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 12:06:47.000000 kal_middleware-0.0.3/kal_middleware.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-09 12:06:47.000000 kal_middleware-0.0.3/kal_middleware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 12:06:47.000000 kal_middleware-0.0.3/kal_middleware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:06:47.655679 kal_middleware-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:06:47.655679 kal_middleware-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-09 12:06:36.000000 kal_middleware-0.0.3/tests/test_kal_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:54:48.861660 kal_middleware-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:54:48.853660 kal_middleware-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:54:48.857660 kal_middleware-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:54:48.857660 kal_middleware-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-15 09:54:48.861660 kal_middleware-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:54:48.861660 kal_middleware-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:54:48.861660 kal_middleware-0.0.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/docs/jwt.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/docs/kal_middleware.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:54:48.861660 kal_middleware-0.0.4/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/docs/sts.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:54:48.861660 kal_middleware-0.0.4/kal_middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/kal_middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/kal_middleware/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/kal_middleware/kal_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/kal_middleware/sts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:54:48.861660 kal_middleware-0.0.4/kal_middleware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-15 09:54:48.000000 kal_middleware-0.0.4/kal_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-15 09:54:48.000000 kal_middleware-0.0.4/kal_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:54:48.000000 kal_middleware-0.0.4/kal_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 09:54:48.000000 kal_middleware-0.0.4/kal_middleware.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 09:54:48.000000 kal_middleware-0.0.4/kal_middleware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 09:54:48.000000 kal_middleware-0.0.4/kal_middleware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 09:54:48.861660 kal_middleware-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:54:48.861660 kal_middleware-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-15 09:54:38.000000 kal_middleware-0.0.4/tests/test_kal_middleware.py
```

### Comparing `kal_middleware-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md` & `kal_middleware-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/.github/ISSUE_TEMPLATE/config.yml` & `kal_middleware-0.0.4/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/.github/workflows/docs-build.yml` & `kal_middleware-0.0.4/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/.github/workflows/docs.yml` & `kal_middleware-0.0.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/.github/workflows/installation.yml` & `kal_middleware-0.0.4/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/.github/workflows/macos.yml` & `kal_middleware-0.0.4/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/.github/workflows/pypi.yml` & `kal_middleware-0.0.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/.github/workflows/ubuntu.yml` & `kal_middleware-0.0.4/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/.github/workflows/windows.yml` & `kal_middleware-0.0.4/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/.gitignore` & `kal_middleware-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/LICENSE` & `kal_middleware-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/README.md` & `kal_middleware-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # kal-middleware
 
 
 [![image](https://img.shields.io/pypi/v/kal-middleware.svg)](https://pypi.python.org/pypi/kal-middleware)
-[![image](https://img.shields.io/conda/vn/conda-forge/kal-middleware.svg)](https://anaconda.org/conda-forge/kal-middleware)
 
 `kal-middleware` is a Python package designed for FastAPI applications to provide robust JWT and Service-to-Service (STS) authentication using Firebase and Google Identity Platform.
 
 ## Features
 
 - **JWT Authentication**: Ensures that the JWTs are valid and checks user roles against provided configurations.
 - **STS Authentication**: Validates tokens for service-to-service communication ensuring that only verified services can communicate.
@@ -24,30 +23,35 @@
 ## JWT Authentication
 
 To add JWT authentication to your FastAPI endpoints, you can use the `jwt_authenticated` decorator provided by `kal-middleware`. This decorator checks if the JWT token in the `Authorization` header is valid and whether the user has the appropriate role based on a configuration map.
 
 Here's an example of how to apply the `jwt_authenticated` decorator:
 
 ```python
-from kal_middleware.jwt import jwt_authenticated
+from kal_middleware.jwt import firebase_jwt_authenticated
 
 # Define a function to retrieve the user's role based on their user ID
-def get_user_role_function(user_id: str):
-    # Implement your logic to retrieve the user's role
+def get_user_capabilities(user_id: str):
+    # Implement your logic to retrieve the user's capabilities
     # If the user not found, return "".
-    return "user_role"
+
+    # Example - the user can access the get action in example service only.
+    example_capabilities = {
+        "service": "example_service",
+        "action": "get"
+    }
+    return example_capabilities
 
 # Define a configuration map specifying services, actions, and required permissions
 config_map = {
-    "service": {
+    "example_service": {
         "url": "service_url",
         "actions": {
-            "example": {
-                "permissions": ["user_role", "admin_role"]
-            }
+            "get",
+            "get_all"
         }
     }
 }
 
 # if there is specific variable in the body that needed checks of who access its data only
 def check_access(firebase_uid, body):
     # check in the db the user and his parameters
@@ -55,22 +59,33 @@
     user = {
         "firebase_uid": "12345",
         "org_id": "12345"
     }
     return body["org_id"] == user["org_id"]
 
 @app.get("/your-route/<service>/<action>")
-@jwt_authenticated(get_user_role_function, config_map, check_access)
+@firebase_jwt_authenticated(get_user_capabilities, config_map, check_access)
 async def your_route_function(
         request: Request = None,
         service: Union[str, None] = None,
         action: Union[str, None] = None
 ):
     # Your route logic
     return {"message": "This is a protected route"}
+
+# Or - if there is no need to check for specific data in the body
+@app.get("/your-route-without-check-access/<service>/<action>")
+@firebase_jwt_authenticated(get_user_capabilities, config_map)
+async def your_route_function_without_check_access(
+        request: Request = None,
+        service: Union[str, None] = None,
+        action: Union[str, None] = None
+):
+    # Your route logic
+    return {"message": "This is a protected route"}
 ```
 
 ## STS Authentication
 For service-to-service (STS) authentication using Google's Identity Platform, you can use the `sts_authenticated` decorator. This ensures that the calling service's token is verified to enable secure interactions between services.
 
 Here's how to use the `sts_authenticated` decorator in your FastAPI app:
 - Make sure first you have env variable named `ALLOWED_SERVICE_ACCOUNTS` with the following structure: `example1@gserviceaccount.com, example2@gserviceaccount.com`
```

### Comparing `kal_middleware-0.0.3/docs/contributing.md` & `kal_middleware-0.0.4/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/docs/installation.md` & `kal_middleware-0.0.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/kal_middleware/jwt.py` & `kal_middleware-0.0.4/kal_middleware/jwt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from functools import wraps
 from fastapi import Request, status
 from starlette.responses import Response
 import firebase_admin
 from firebase_admin import auth
-from typing import Callable, Optional, Dict, Any, List, Union
+from typing import Callable, Optional, Dict, Any, Set, Union
 
 default_app = firebase_admin.initialize_app()
 
-def jwt_authenticated(
-    get_user_role_function: Callable[[str], Any],
-    config_map: Dict[str, Dict[str, Union[str, Dict[str, Dict[str, List[str]]]]]],
+def firebase_jwt_authenticated(
+    get_user_capabilities: Callable[[str], Any],
+    config_map: Dict[str, Dict[str, Union[str, Set[str]]]],
     check_access: Optional[Callable[[str, Any], bool]] = None,
 ):
     def decorator(func: Callable) -> Callable:
         @wraps(func)
         async def decorated_function(request: Request, *args, **kwargs):
             # verify the token exists and validate with firebase
             header = request.headers.get("Authorization", None)
@@ -39,27 +39,23 @@
                 return Response(
                     status_code=status.HTTP_404_NOT_FOUND,
                     content=f"Action {action} not found in service {service}.",
                 )
 
             # verify that the user has the permission to execute the request
             user_uid = decoded_token["uid"]
-            permissions = config_map[service]["actions"][action]["permissions"]
-            user_role = await get_user_role_function(user_uid)
+            user_capabilities = await get_user_capabilities(user_uid)
+            access = any(
+                capability["service"] == service and capability["action"] == action for capability in user_capabilities
+            )
 
-            if not user_role:
-                return Response(
-                    status_code=status.HTTP_404_NOT_FOUND,
-                    content=f"User not exist.",
-                )
-
-            if user_role not in permissions:
+            if not access:
                 return Response(
                     status_code=status.HTTP_403_FORBIDDEN,
-                    content=f"User not permitted to call {service}/{action}.",
+                    content=f"The user cannot access {service}/{action}."
                 )
 
             # if the request has body and there is a need to verify the user access to the elements - verify it
             if request.method in ["POST", "PUT"]:
                 if check_access:
                     body = await request.json()
                     if not check_access(user_uid, body):
@@ -73,7 +69,10 @@
             # Process the request
             response = await func(request, *args, **kwargs)
             return response
 
         return decorated_function
 
     return decorator
+
+
+
```

### Comparing `kal_middleware-0.0.3/kal_middleware/sts.py` & `kal_middleware-0.0.4/kal_middleware/sts.py`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/kal_middleware.egg-info/SOURCES.txt` & `kal_middleware-0.0.4/kal_middleware.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/mkdocs.yml` & `kal_middleware-0.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.3/pyproject.toml` & `kal_middleware-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kal-middleware"
-version = "0.0.3"
+version = "0.0.4"
 dynamic = [
     "dependencies",
 ]
 description = "Kaleidoo middleware package"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.3"
+current_version = "0.0.4"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

