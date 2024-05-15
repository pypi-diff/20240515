# Comparing `tmp/flask_jwt_oidc-0.6.0.tar.gz` & `tmp/flask_jwt_oidc-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_jwt_oidc-0.6.0.tar", max compression
+gzip compressed data, was "flask_jwt_oidc-0.7.0.tar", max compression
```

## Comparing `flask_jwt_oidc-0.6.0.tar` & `flask_jwt_oidc-0.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1695 2024-04-25 06:27:35.896596 flask_jwt_oidc-0.6.0/LICENSE
--rw-r--r--   0        0        0     3734 2024-04-25 06:27:35.896651 flask_jwt_oidc-0.6.0/README.md
--rw-r--r--   0        0        0      736 2024-04-25 06:27:35.897757 flask_jwt_oidc-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1739 2024-04-25 06:27:35.897953 flask_jwt_oidc-0.6.0/src/flask_jwt_oidc/__init__.py
--rw-r--r--   0        0        0      939 2024-04-25 06:27:35.898063 flask_jwt_oidc-0.6.0/src/flask_jwt_oidc/exceptions.py
--rw-r--r--   0        0        0    15530 2024-04-25 06:27:35.898201 flask_jwt_oidc-0.6.0/src/flask_jwt_oidc/jwt_manager.py
--rw-r--r--   0        0        0     4428 1970-01-01 00:00:00.000000 flask_jwt_oidc-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1695 2024-04-25 06:27:35.896596 flask_jwt_oidc-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3734 2024-04-25 06:27:35.896651 flask_jwt_oidc-0.7.0/README.md
+-rw-r--r--   0        0        0      737 2024-05-15 17:37:03.045772 flask_jwt_oidc-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1739 2024-04-25 06:27:35.897953 flask_jwt_oidc-0.7.0/src/flask_jwt_oidc/__init__.py
+-rw-r--r--   0        0        0      939 2024-04-25 06:27:35.898063 flask_jwt_oidc-0.7.0/src/flask_jwt_oidc/exceptions.py
+-rw-r--r--   0        0        0    15530 2024-04-25 06:27:35.898201 flask_jwt_oidc-0.7.0/src/flask_jwt_oidc/jwt_manager.py
+-rw-r--r--   0        0        0     4425 1970-01-01 00:00:00.000000 flask_jwt_oidc-0.7.0/PKG-INFO
```

### Comparing `flask_jwt_oidc-0.6.0/LICENSE` & `flask_jwt_oidc-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_jwt_oidc-0.6.0/README.md` & `flask_jwt_oidc-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `flask_jwt_oidc-0.6.0/pyproject.toml` & `flask_jwt_oidc-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "flask-jwt-oidc"
-version = "0.6.0"
+version = "0.7.0"
 description = "Opinionated flask oidc client"
 authors = [
    "thor wolpert <thor@wolpert.ca>"
 ]
 license = "BSD 3-Clause"
 readme = "README.md"
 packages = [{include = "flask_jwt_oidc", from = "src"}]
 
 [project.urls]
 Homepage = "https://github.com/thorwolpert/flask-jwt-oidc"
 Issues = "https://github.com/thorwolpert/flask-jwt-oidc/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-Flask = "^2"
+Flask = ">=2"
 cachelib = "^0.13.0"
 python-jose = "^3.3.0"
 six = "^1.16.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 python-dotenv = "^1.0.1"
```

### Comparing `flask_jwt_oidc-0.6.0/src/flask_jwt_oidc/__init__.py` & `flask_jwt_oidc-0.7.0/src/flask_jwt_oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_jwt_oidc-0.6.0/src/flask_jwt_oidc/exceptions.py` & `flask_jwt_oidc-0.7.0/src/flask_jwt_oidc/exceptions.py`

 * *Files identical despite different names*

### Comparing `flask_jwt_oidc-0.6.0/src/flask_jwt_oidc/jwt_manager.py` & `flask_jwt_oidc-0.7.0/src/flask_jwt_oidc/jwt_manager.py`

 * *Files identical despite different names*

### Comparing `flask_jwt_oidc-0.6.0/PKG-INFO` & `flask_jwt_oidc-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: flask-jwt-oidc
-Version: 0.6.0
+Version: 0.7.0
 Summary: Opinionated flask oidc client
 License: BSD 3-Clause
 Author: thor wolpert
 Author-email: thor@wolpert.ca
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: Flask (>=2,<3)
+Requires-Dist: Flask (>=2)
 Requires-Dist: cachelib (>=0.13.0,<0.14.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Flask JWT OIDC
```

