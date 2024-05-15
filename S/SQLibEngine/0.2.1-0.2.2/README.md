# Comparing `tmp/SQLibEngine-0.2.1.tar.gz` & `tmp/SQLibEngine-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLibEngine-0.2.1.tar", last modified: Tue May 14 13:28:08 2024, max compression
+gzip compressed data, was "SQLibEngine-0.2.2.tar", last modified: Wed May 15 20:28:57 2024, max compression
```

## Comparing `SQLibEngine-0.2.1.tar` & `SQLibEngine-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:08.070773 SQLibEngine-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-14 13:28:08.066773 SQLibEngine-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:08.066773 SQLibEngine-0.2.1/SQLib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:08.066773 SQLibEngine-0.2.1/SQLib/Database/
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/Database/Connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/Database/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/Database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:08.066773 SQLibEngine-0.2.1/SQLib/SQLEngine/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/SQLEngine/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/SQLEngine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/SQLEngine/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/SQLEngine/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/SQLEngine/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/SQLEngine/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/SQLib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:28:08.066773 SQLibEngine-0.2.1/SQLibEngine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-14 13:28:08.000000 SQLibEngine-0.2.1/SQLibEngine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-14 13:28:08.000000 SQLibEngine-0.2.1/SQLibEngine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:28:08.000000 SQLibEngine-0.2.1/SQLibEngine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 13:28:08.000000 SQLibEngine-0.2.1/SQLibEngine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:28:08.070773 SQLibEngine-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-14 13:28:03.000000 SQLibEngine-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:57.330154 SQLibEngine-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-15 20:28:57.330154 SQLibEngine-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:57.326154 SQLibEngine-0.2.2/SQLib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:57.330154 SQLibEngine-0.2.2/SQLib/Database/
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/SQLib/Database/Connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/SQLib/Database/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/SQLib/Database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:57.330154 SQLibEngine-0.2.2/SQLib/SQLEngine/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/SQLib/SQLEngine/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/SQLib/SQLEngine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/SQLib/SQLEngine/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/SQLib/SQLEngine/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/SQLib/SQLEngine/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/SQLib/SQLEngine/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/SQLib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:57.330154 SQLibEngine-0.2.2/SQLibEngine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-15 20:28:57.000000 SQLibEngine-0.2.2/SQLibEngine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-15 20:28:57.000000 SQLibEngine-0.2.2/SQLibEngine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:28:57.000000 SQLibEngine-0.2.2/SQLibEngine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 20:28:57.000000 SQLibEngine-0.2.2/SQLibEngine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:28:57.330154 SQLibEngine-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-15 20:28:49.000000 SQLibEngine-0.2.2/setup.py
```

### Comparing `SQLibEngine-0.2.1/LICENSE` & `SQLibEngine-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.2.1/PKG-INFO` & `SQLibEngine-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLibEngine
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple SQLite3 wrapper for Python
 Home-page: https://github.com/TRC-Loop/SQLib
 Author: AK
 Author-email: ak@stellar-code.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 License-File: LICENSE
 
 # SQLib
 
 SQLib is a python library to use SQL Databases without having to write SQL, based on SQLite.
 
 [![Publish Python distributions to PyPI and TestPyPI](https://github.com/TRC-Loop/SQLib/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/TRC-Loop/SQLib/actions/workflows/pypi-publish.yml)
+[![CodeQL](https://github.com/TRC-Loop/SQLib/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/TRC-Loop/SQLib/actions/workflows/github-code-scanning/codeql)
 ![GitHub Release](https://img.shields.io/github/v/release/TRC-Loop/SQLib)
 ![PyPI - Version](https://img.shields.io/pypi/v/SQLibEngine)
 ![GitHub forks](https://img.shields.io/github/forks/TRC-Loop/SQLib?style=flat)
 ![GitHub Repo stars](https://img.shields.io/github/stars/TRC-Loop/SQLib?style=flat)
 ![GitHub License](https://img.shields.io/github/license/TRC-Loop/SQLib?style=flat)
 
 ## Installation
```

### Comparing `SQLibEngine-0.2.1/README.md` & `SQLibEngine-0.2.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SQLib
 
 SQLib is a python library to use SQL Databases without having to write SQL, based on SQLite.
 
 [![Publish Python distributions to PyPI and TestPyPI](https://github.com/TRC-Loop/SQLib/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/TRC-Loop/SQLib/actions/workflows/pypi-publish.yml)
+[![CodeQL](https://github.com/TRC-Loop/SQLib/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/TRC-Loop/SQLib/actions/workflows/github-code-scanning/codeql)
 ![GitHub Release](https://img.shields.io/github/v/release/TRC-Loop/SQLib)
 ![PyPI - Version](https://img.shields.io/pypi/v/SQLibEngine)
 ![GitHub forks](https://img.shields.io/github/forks/TRC-Loop/SQLib?style=flat)
 ![GitHub Repo stars](https://img.shields.io/github/stars/TRC-Loop/SQLib?style=flat)
 ![GitHub License](https://img.shields.io/github/license/TRC-Loop/SQLib?style=flat)
 
 ## Installation
```

### Comparing `SQLibEngine-0.2.1/SQLib/Database/Connection.py` & `SQLibEngine-0.2.2/SQLib/Database/Connection.py`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.2.1/SQLib/SQLEngine/operations.py` & `SQLibEngine-0.2.2/SQLib/SQLEngine/operations.py`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.2.1/SQLib/SQLEngine/tables.py` & `SQLibEngine-0.2.2/SQLib/SQLEngine/tables.py`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.2.1/SQLib/SQLEngine/util.py` & `SQLibEngine-0.2.2/SQLib/SQLEngine/util.py`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.2.1/SQLibEngine.egg-info/PKG-INFO` & `SQLibEngine-0.2.2/SQLibEngine.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLibEngine
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple SQLite3 wrapper for Python
 Home-page: https://github.com/TRC-Loop/SQLib
 Author: AK
 Author-email: ak@stellar-code.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 License-File: LICENSE
 
 # SQLib
 
 SQLib is a python library to use SQL Databases without having to write SQL, based on SQLite.
 
 [![Publish Python distributions to PyPI and TestPyPI](https://github.com/TRC-Loop/SQLib/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/TRC-Loop/SQLib/actions/workflows/pypi-publish.yml)
+[![CodeQL](https://github.com/TRC-Loop/SQLib/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/TRC-Loop/SQLib/actions/workflows/github-code-scanning/codeql)
 ![GitHub Release](https://img.shields.io/github/v/release/TRC-Loop/SQLib)
 ![PyPI - Version](https://img.shields.io/pypi/v/SQLibEngine)
 ![GitHub forks](https://img.shields.io/github/forks/TRC-Loop/SQLib?style=flat)
 ![GitHub Repo stars](https://img.shields.io/github/stars/TRC-Loop/SQLib?style=flat)
 ![GitHub License](https://img.shields.io/github/license/TRC-Loop/SQLib?style=flat)
 
 ## Installation
```

### Comparing `SQLibEngine-0.2.1/setup.py` & `SQLibEngine-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the README.md file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="SQLibEngine",
-    version="0.2.1",
+    version="0.2.2",
     author="AK",
     author_email="ak@stellar-code.com",
     url="https://github.com/TRC-Loop/SQLib",
     description="A simple SQLite3 wrapper for Python",
     long_description=long_description,  # Set the long description
     long_description_content_type="text/markdown",  # Specify the content type
     packages=find_packages(),
```

