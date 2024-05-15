# Comparing `tmp/alloniaconfigs-1.1.0.tar.gz` & `tmp/alloniaconfigs-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alloniaconfigs-1.1.0.tar", max compression
+gzip compressed data, was "alloniaconfigs-1.1.1.tar", max compression
```

## Comparing `alloniaconfigs-1.1.0.tar` & `alloniaconfigs-1.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2047 2024-05-06 12:32:20.128071 alloniaconfigs-1.1.0/README.md
--rw-r--r--   0        0        0       52 2024-05-06 12:32:20.128071 alloniaconfigs-1.1.0/alloniaconfigs/__init__.py
--rw-r--r--   0        0        0     3514 2024-05-06 12:32:20.128071 alloniaconfigs-1.1.0/alloniaconfigs/configs.py
--rw-r--r--   0        0        0     3441 2024-05-06 12:33:16.468552 alloniaconfigs-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 alloniaconfigs-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2047 2024-05-15 09:15:54.341106 alloniaconfigs-1.1.1/README.md
+-rw-r--r--   0        0        0       52 2024-05-15 09:15:54.341106 alloniaconfigs-1.1.1/alloniaconfigs/__init__.py
+-rw-r--r--   0        0        0     3514 2024-05-15 09:15:54.341106 alloniaconfigs-1.1.1/alloniaconfigs/configs.py
+-rw-r--r--   0        0        0     3441 2024-05-15 09:16:33.849575 alloniaconfigs-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 alloniaconfigs-1.1.1/PKG-INFO
```

### Comparing `alloniaconfigs-1.1.0/README.md` & `alloniaconfigs-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alloniaconfigs-1.1.0/alloniaconfigs/configs.py` & `alloniaconfigs-1.1.1/alloniaconfigs/configs.py`

 * *Files identical despite different names*

### Comparing `alloniaconfigs-1.1.0/pyproject.toml` & `alloniaconfigs-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alloniaconfigs"
-version = "1.1.0"
+version = "1.1.1"
 description = "Class to handle configurations"
 authors = ["ALEIA"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^2.7.0"
```

### Comparing `alloniaconfigs-1.1.0/PKG-INFO` & `alloniaconfigs-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alloniaconfigs
-Version: 1.1.0
+Version: 1.1.1
 Summary: Class to handle configurations
 Author: ALEIA
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

