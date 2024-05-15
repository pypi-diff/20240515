# Comparing `tmp/flask_cognito_lib-1.6.1.tar.gz` & `tmp/flask_cognito_lib-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_cognito_lib-1.6.1.tar", max compression
+gzip compressed data, was "flask_cognito_lib-1.6.2.tar", max compression
```

## Comparing `flask_cognito_lib-1.6.1.tar` & `flask_cognito_lib-1.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-10-30 13:08:11.638661 flask_cognito_lib-1.6.1/LICENSE
--rw-r--r--   0        0        0     8042 2023-10-30 13:08:11.638661 flask_cognito_lib-1.6.1/README.md
--rw-r--r--   0        0        0     2281 2023-10-30 13:08:34.787093 flask_cognito_lib-1.6.1/pyproject.toml
--rw-r--r--   0        0        0       82 2023-10-30 13:08:34.751092 flask_cognito_lib-1.6.1/src/flask_cognito_lib/__init__.py
--rw-r--r--   0        0        0     5702 2023-10-30 13:08:11.642661 flask_cognito_lib-1.6.1/src/flask_cognito_lib/config.py
--rw-r--r--   0        0        0     6428 2023-10-30 13:08:11.642661 flask_cognito_lib-1.6.1/src/flask_cognito_lib/decorators.py
--rw-r--r--   0        0        0      384 2023-10-30 13:08:11.642661 flask_cognito_lib-1.6.1/src/flask_cognito_lib/exceptions.py
--rw-r--r--   0        0        0     5995 2023-10-30 13:08:11.642661 flask_cognito_lib-1.6.1/src/flask_cognito_lib/plugin.py
--rw-r--r--   0        0        0      326 2023-10-30 13:08:11.642661 flask_cognito_lib-1.6.1/src/flask_cognito_lib/services/__init__.py
--rw-r--r--   0        0        0     3820 2023-10-30 13:08:11.642661 flask_cognito_lib-1.6.1/src/flask_cognito_lib/services/cognito_svc.py
--rw-r--r--   0        0        0     5802 2023-10-30 13:08:11.642661 flask_cognito_lib-1.6.1/src/flask_cognito_lib/services/token_svc.py
--rw-r--r--   0        0        0     1124 2023-10-30 13:08:11.642661 flask_cognito_lib-1.6.1/src/flask_cognito_lib/utils.py
--rw-r--r--   0        0        0     9429 1970-01-01 00:00:00.000000 flask_cognito_lib-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-03-26 13:01:31.172978 flask_cognito_lib-1.6.2/LICENSE
+-rw-r--r--   0        0        0     8042 2024-03-26 13:01:31.172978 flask_cognito_lib-1.6.2/README.md
+-rw-r--r--   0        0        0     2280 2024-03-26 13:02:01.164702 flask_cognito_lib-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0       82 2024-03-26 13:02:01.140702 flask_cognito_lib-1.6.2/src/flask_cognito_lib/__init__.py
+-rw-r--r--   0        0        0     5702 2024-03-26 13:01:31.176978 flask_cognito_lib-1.6.2/src/flask_cognito_lib/config.py
+-rw-r--r--   0        0        0     6428 2024-03-26 13:01:31.176978 flask_cognito_lib-1.6.2/src/flask_cognito_lib/decorators.py
+-rw-r--r--   0        0        0      384 2024-03-26 13:01:31.176978 flask_cognito_lib-1.6.2/src/flask_cognito_lib/exceptions.py
+-rw-r--r--   0        0        0     5995 2024-03-26 13:01:31.176978 flask_cognito_lib-1.6.2/src/flask_cognito_lib/plugin.py
+-rw-r--r--   0        0        0      326 2024-03-26 13:01:31.176978 flask_cognito_lib-1.6.2/src/flask_cognito_lib/services/__init__.py
+-rw-r--r--   0        0        0     3820 2024-03-26 13:01:31.176978 flask_cognito_lib-1.6.2/src/flask_cognito_lib/services/cognito_svc.py
+-rw-r--r--   0        0        0     5802 2024-03-26 13:01:31.176978 flask_cognito_lib-1.6.2/src/flask_cognito_lib/services/token_svc.py
+-rw-r--r--   0        0        0     1124 2024-03-26 13:01:31.176978 flask_cognito_lib-1.6.2/src/flask_cognito_lib/utils.py
+-rw-r--r--   0        0        0     9479 1970-01-01 00:00:00.000000 flask_cognito_lib-1.6.2/PKG-INFO
```

### Comparing `flask_cognito_lib-1.6.1/LICENSE` & `flask_cognito_lib-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.6.1/README.md` & `flask_cognito_lib-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.6.1/pyproject.toml` & `flask_cognito_lib-1.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask_cognito_lib"
-version = "1.6.1"
+version = "1.6.2"
 description = "A Flask extension that supports protecting routes with AWS Cognito following OAuth 2.1 best practices"
 license = "MIT"
 authors = ["mblackgeo <18327836+mblackgeo@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/mblackgeo/flask-cognito-lib"
 repository = "https://github.com/mblackgeo/flask-cognito-lib"
 keywords = ["Flask", "Extension", "OAuth", "Cognito"]
@@ -26,15 +26,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Flask = ">=2.0,<4.0"
 requests = "~=2.0"
 PyJWT = { extras = ["crypto"], version = ">=2.4,<3.0" }
-urllib3 = "<=2.0"
+urllib3 = "<3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 mypy = "^1.6"
 black = "^22.1.0"
 flake8 = "^4.0.1"
 typed-ast = "^1.5.2"
```

### Comparing `flask_cognito_lib-1.6.1/src/flask_cognito_lib/config.py` & `flask_cognito_lib-1.6.2/src/flask_cognito_lib/config.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.6.1/src/flask_cognito_lib/decorators.py` & `flask_cognito_lib-1.6.2/src/flask_cognito_lib/decorators.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.6.1/src/flask_cognito_lib/plugin.py` & `flask_cognito_lib-1.6.2/src/flask_cognito_lib/plugin.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.6.1/src/flask_cognito_lib/services/cognito_svc.py` & `flask_cognito_lib-1.6.2/src/flask_cognito_lib/services/cognito_svc.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.6.1/src/flask_cognito_lib/services/token_svc.py` & `flask_cognito_lib-1.6.2/src/flask_cognito_lib/services/token_svc.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.6.1/src/flask_cognito_lib/utils.py` & `flask_cognito_lib-1.6.2/src/flask_cognito_lib/utils.py`

 * *Files identical despite different names*

### Comparing `flask_cognito_lib-1.6.1/PKG-INFO` & `flask_cognito_lib-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_cognito_lib
-Version: 1.6.1
+Version: 1.6.2
 Summary: A Flask extension that supports protecting routes with AWS Cognito following OAuth 2.1 best practices
 Home-page: https://github.com/mblackgeo/flask-cognito-lib
 License: MIT
 Keywords: Flask,Extension,OAuth,Cognito
 Author: mblackgeo
 Author-email: 18327836+mblackgeo@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
@@ -14,23 +14,24 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: Flask (>=2.0,<4.0)
 Requires-Dist: PyJWT[crypto] (>=2.4,<3.0)
 Requires-Dist: requests (>=2.0,<3.0)
-Requires-Dist: urllib3 (<=2.0)
+Requires-Dist: urllib3 (<3.0)
 Project-URL: Repository, https://github.com/mblackgeo/flask-cognito-lib
 Description-Content-Type: text/markdown
 
 # Protect Flask routes with AWS Cognito
 
 [![PyPI](https://img.shields.io/pypi/v/flask_cognito_lib?style=for-the-badge)](https://pypi.org/project/flask-cognito-lib/)
 [![Docs](https://img.shields.io/github/actions/workflow/status/mblackgeo/flask-cognito-lib/docs.yml?label=DOCS&style=for-the-badge)](https://mblackgeo.github.io/flask-cognito-lib)
```

