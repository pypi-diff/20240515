# Comparing `tmp/silver_octo_potato-0.1.3.tar.gz` & `tmp/silver_octo_potato-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silver_octo_potato-0.1.3.tar", max compression
+gzip compressed data, was "silver_octo_potato-0.1.4.tar", max compression
```

## Comparing `silver_octo_potato-0.1.3.tar` & `silver_octo_potato-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-05-08 07:22:25.493228 silver_octo_potato-0.1.3/LICENSE
--rw-r--r--   0        0        0       21 2024-05-09 06:36:16.049309 silver_octo_potato-0.1.3/README.md
--rw-r--r--   0        0        0     1136 2024-05-13 11:24:21.817309 silver_octo_potato-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-09 07:00:32.786349 silver_octo_potato-0.1.3/src/silver_octo_potato/__init__.py
--rw-r--r--   0        0        0       43 2024-05-09 06:55:08.189192 silver_octo_potato-0.1.3/src/silver_octo_potato/example.py
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 silver_octo_potato-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-08 07:22:25.493228 silver_octo_potato-0.1.4/LICENSE
+-rw-r--r--   0        0        0       21 2024-05-09 06:36:16.049309 silver_octo_potato-0.1.4/README.md
+-rw-r--r--   0        0        0     1140 2024-05-15 01:36:43.988552 silver_octo_potato-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-09 07:00:32.786349 silver_octo_potato-0.1.4/src/silver_octo_potato/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-09 06:55:08.189192 silver_octo_potato-0.1.4/src/silver_octo_potato/example.py
+-rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 silver_octo_potato-0.1.4/PKG-INFO
```

### Comparing `silver_octo_potato-0.1.3/LICENSE` & `silver_octo_potato-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `silver_octo_potato-0.1.3/pyproject.toml` & `silver_octo_potato-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "silver_octo_potato"
-version = "0.1.3"
+version = "0.1.4"
 description = "Test Project"
 authors = ["Shota Muto <129914139+MutoShota@users.noreply.github.com>"]
 readme = "README.md"
 license= "Apache-2.0"
 classifiers = [
     "Framework :: Robot Framework",
     "License :: OSI Approved :: Apache Software License",
@@ -30,15 +30,15 @@
 
 packages = [
     { include = "silver_octo_potato", from = "src" }
 ]
 
 [project]
 name = "silver_octo_potato"
-version = "0.1.2"
+version = "0.1.4"
 description = "Test Project"
 authors = [ { name = "Shota Muto" } ]
 readme = "README.md"
 license= { file = "LICENSE" }
 
-[project.urls]
+[tool.poetry.urls]
 Homepage = "https://github.com/MutoShota/silver-octo-potato"
```

### Comparing `silver_octo_potato-0.1.3/PKG-INFO` & `silver_octo_potato-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silver_octo_potato
-Version: 0.1.3
+Version: 0.1.4
 Summary: Test Project
 License: Apache-2.0
 Author: Shota Muto
 Author-email: 129914139+MutoShota@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: Framework :: Robot Framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,11 +12,12 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: netmiko (>=4.3.0,<5.0.0)
+Project-URL: Homepage, https://github.com/MutoShota/silver-octo-potato
 Description-Content-Type: text/markdown
 
 # Silver Octo Potato
```

