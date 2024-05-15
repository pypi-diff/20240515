# Comparing `tmp/python_trading212_alinalihassan-2.0.4.tar.gz` & `tmp/python_trading212_alinalihassan-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_trading212_alinalihassan-2.0.4.tar", max compression
+gzip compressed data, was "python_trading212_alinalihassan-2.0.5.tar", max compression
```

## Comparing `python_trading212_alinalihassan-2.0.4.tar` & `python_trading212_alinalihassan-2.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-05-14 11:03:58.546257 python_trading212_alinalihassan-2.0.4/LICENSE.md
--rw-r--r--   0        0        0     2153 2024-05-14 11:34:26.590899 python_trading212_alinalihassan-2.0.4/README.md
--rw-r--r--   0        0        0     1141 2024-05-14 11:35:26.478240 python_trading212_alinalihassan-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      354 2024-05-14 11:18:38.788326 python_trading212_alinalihassan-2.0.4/trading212/__init__.py
--rw-r--r--   0        0        0     5705 2024-05-14 11:33:35.552004 python_trading212_alinalihassan-2.0.4/trading212/models.py
--rw-r--r--   0        0        0    12544 2024-05-14 11:22:05.790170 python_trading212_alinalihassan-2.0.4/trading212/trading212.py
--rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 python_trading212_alinalihassan-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-14 11:03:58.546257 python_trading212_alinalihassan-2.0.5/LICENSE.md
+-rw-r--r--   0        0        0     2153 2024-05-14 11:34:26.590899 python_trading212_alinalihassan-2.0.5/README.md
+-rw-r--r--   0        0        0     1140 2024-05-15 07:53:45.402723 python_trading212_alinalihassan-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0      354 2024-05-14 11:18:38.788326 python_trading212_alinalihassan-2.0.5/trading212/__init__.py
+-rw-r--r--   0        0        0     5705 2024-05-14 11:33:35.552004 python_trading212_alinalihassan-2.0.5/trading212/models.py
+-rw-r--r--   0        0        0    12544 2024-05-14 13:26:04.620643 python_trading212_alinalihassan-2.0.5/trading212/trading212.py
+-rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 python_trading212_alinalihassan-2.0.5/PKG-INFO
```

### Comparing `python_trading212_alinalihassan-2.0.4/LICENSE.md` & `python_trading212_alinalihassan-2.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_trading212_alinalihassan-2.0.4/README.md` & `python_trading212_alinalihassan-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `python_trading212_alinalihassan-2.0.4/pyproject.toml` & `python_trading212_alinalihassan-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-trading212-alinalihassan"
-version = "2.0.4"
+version = "2.0.5"
 description = "An unofficial client for the official Trading212 API"
 authors = ["Alin Ali Hassan <alinalihassan@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/alinalihassan/python-trading212"
 repository = "https://github.com/alinalihassan/python-trading212"
 documentation = "https://github.com/alinalihassan/python-trading212"
@@ -23,15 +23,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.12",
     "Topic :: Office/Business :: Financial :: Investment",
 ]
 packages = [{ include = "trading212", from = "." }]
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.9"
 requests = "^2.31.0"
 pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 
 [build-system]
```

### Comparing `python_trading212_alinalihassan-2.0.4/trading212/models.py` & `python_trading212_alinalihassan-2.0.5/trading212/models.py`

 * *Files identical despite different names*

### Comparing `python_trading212_alinalihassan-2.0.4/trading212/trading212.py` & `python_trading212_alinalihassan-2.0.5/trading212/trading212.py`

 * *Files identical despite different names*

### Comparing `python_trading212_alinalihassan-2.0.4/PKG-INFO` & `python_trading212_alinalihassan-2.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: python-trading212-alinalihassan
-Version: 2.0.4
+Version: 2.0.5
 Summary: An unofficial client for the official Trading212 API
 Home-page: https://github.com/alinalihassan/python-trading212
 License: MIT
 Keywords: python,trading212,api,client,unofficial,finance,stocks,trading
 Author: Alin Ali Hassan
 Author-email: alinalihassan@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/alinalihassan/python-trading212/issues
 Project-URL: Documentation, https://github.com/alinalihassan/python-trading212
 Project-URL: Repository, https://github.com/alinalihassan/python-trading212
```

