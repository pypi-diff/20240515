# Comparing `tmp/varbert-2.1.0.tar.gz` & `tmp/varbert-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varbert-2.1.0.tar", last modified: Fri Feb 23 21:18:42 2024, max compression
+gzip compressed data, was "varbert-2.2.0.tar", last modified: Wed May 15 19:39:24 2024, max compression
```

## Comparing `varbert-2.1.0.tar` & `varbert-2.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:18:42.539015 varbert-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-23 21:18:35.000000 varbert-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-02-23 21:18:42.539015 varbert-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-02-23 21:18:35.000000 varbert-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-23 21:18:42.539015 varbert-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 21:18:35.000000 varbert-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:18:42.535015 varbert-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-02-23 21:18:35.000000 varbert-2.1.0/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:18:42.539015 varbert-2.1.0/varbert/
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-02-23 21:18:35.000000 varbert-2.1.0/varbert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-02-23 21:18:35.000000 varbert-2.1.0/varbert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-02-23 21:18:35.000000 varbert-2.1.0/varbert/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-02-23 21:18:35.000000 varbert-2.1.0/varbert/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15559 2024-02-23 21:18:35.000000 varbert-2.1.0/varbert/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:18:42.539015 varbert-2.1.0/varbert/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 21:18:35.000000 varbert-2.1.0/varbert/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-02-23 21:18:35.000000 varbert-2.1.0/varbert/text_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:18:42.539015 varbert-2.1.0/varbert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-02-23 21:18:42.000000 varbert-2.1.0/varbert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-23 21:18:42.000000 varbert-2.1.0/varbert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 21:18:42.000000 varbert-2.1.0/varbert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-23 21:18:42.000000 varbert-2.1.0/varbert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-23 21:18:42.000000 varbert-2.1.0/varbert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-23 21:18:42.000000 varbert-2.1.0/varbert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:39:24.625843 varbert-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-15 19:39:19.000000 varbert-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-15 19:39:24.625843 varbert-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-15 19:39:19.000000 varbert-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-15 19:39:24.625843 varbert-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:39:19.000000 varbert-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:39:24.621843 varbert-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-05-15 19:39:19.000000 varbert-2.2.0/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:39:24.621843 varbert-2.2.0/varbert/
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-05-15 19:39:19.000000 varbert-2.2.0/varbert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-15 19:39:19.000000 varbert-2.2.0/varbert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-15 19:39:19.000000 varbert-2.2.0/varbert/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-15 19:39:19.000000 varbert-2.2.0/varbert/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15559 2024-05-15 19:39:19.000000 varbert-2.2.0/varbert/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:39:24.625843 varbert-2.2.0/varbert/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:39:19.000000 varbert-2.2.0/varbert/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-15 19:39:19.000000 varbert-2.2.0/varbert/text_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:39:24.625843 varbert-2.2.0/varbert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-15 19:39:24.000000 varbert-2.2.0/varbert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-15 19:39:24.000000 varbert-2.2.0/varbert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:39:24.000000 varbert-2.2.0/varbert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 19:39:24.000000 varbert-2.2.0/varbert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 19:39:24.000000 varbert-2.2.0/varbert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:39:24.000000 varbert-2.2.0/varbert.egg-info/top_level.txt
```

### Comparing `varbert-2.1.0/LICENSE` & `varbert-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `varbert-2.1.0/PKG-INFO` & `varbert-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varbert
-Version: 2.1.0
+Version: 2.2.0
 Summary: The VarBERT API for renaming variables in decompiled code.
 Home-page: https://github.com/binsync/varbert_api
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.8
```

### Comparing `varbert-2.1.0/README.md` & `varbert-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `varbert-2.1.0/setup.cfg` & `varbert-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `varbert-2.1.0/tests/tests.py` & `varbert-2.2.0/tests/tests.py`

 * *Files identical despite different names*

### Comparing `varbert-2.1.0/varbert/__init__.py` & `varbert-2.2.0/varbert/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 
 import importlib.resources
 import tarfile
 from pathlib import Path
 import urllib.request
 import hashlib
 import math
```

### Comparing `varbert-2.1.0/varbert/__main__.py` & `varbert-2.2.0/varbert/__main__.py`

 * *Files identical despite different names*

### Comparing `varbert-2.1.0/varbert/api.py` & `varbert-2.2.0/varbert/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,17 +89,17 @@
                     new_names.add(popular_name)
 
             # remove decompiler based names
             orig_name_2_popular_name = {
                 k: v for k, v in name_pairs if "/*decompiler*/" not in v
             }
         else:
-            # rewrite decompiled based names
+            # rewrite decompiled based names, remove the comment
             orig_name_2_popular_name = {
-                k: v.replace(" /*decompiler*/", "_dec") for k, v in orig_name_2_popular_name.items()
+                k: v.replace(" /*decompiler*/", "") for k, v in orig_name_2_popular_name.items()
             }
 
         # check after filtering
         self.info(f"Predicted {len(orig_name_2_popular_name)} new names for function {function}")
         return orig_name_2_popular_name, renamed_code
 
     @AIAPI.requires_function
```

### Comparing `varbert-2.1.0/varbert/logger.py` & `varbert-2.2.0/varbert/logger.py`

 * *Files identical despite different names*

### Comparing `varbert-2.1.0/varbert/model.py` & `varbert-2.2.0/varbert/model.py`

 * *Files identical despite different names*

### Comparing `varbert-2.1.0/varbert/text_processor.py` & `varbert-2.2.0/varbert/text_processor.py`

 * *Files identical despite different names*

### Comparing `varbert-2.1.0/varbert.egg-info/PKG-INFO` & `varbert-2.2.0/varbert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varbert
-Version: 2.1.0
+Version: 2.2.0
 Summary: The VarBERT API for renaming variables in decompiled code.
 Home-page: https://github.com/binsync/varbert_api
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.8
```

