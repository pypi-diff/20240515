# Comparing `tmp/polars_expr_transformer-0.1.2.tar.gz` & `tmp/polars_expr_transformer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polars_expr_transformer-0.1.2.tar", last modified: Tue May 14 20:13:05 2024, max compression
+gzip compressed data, was "polars_expr_transformer-0.1.3.tar", last modified: Tue May 14 20:14:11 2024, max compression
```

## Comparing `polars_expr_transformer-0.1.2.tar` & `polars_expr_transformer-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:13:05.108264 polars_expr_transformer-0.1.2/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    11357 2024-05-14 19:35:59.000000 polars_expr_transformer-0.1.2/LICENSE
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     2286 2024-05-14 20:13:05.108042 polars_expr_transformer-0.1.2/PKG-INFO
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1485 2024-05-14 20:00:49.000000 polars_expr_transformer-0.1.2/README.md
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:13:05.103898 polars_expr_transformer-0.1.2/polars_expr_transformer/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       84 2024-05-14 19:28:50.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/__init__.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:13:05.104703 polars_expr_transformer-0.1.2/polars_expr_transformer/configs/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:27.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/configs/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1290 2024-05-14 18:00:12.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/configs/settings.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:13:05.105660 polars_expr_transformer-0.1.2/polars_expr_transformer/funcs/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      386 2024-05-14 18:00:27.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/funcs/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     8014 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/funcs/date_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4155 2024-05-14 18:00:47.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/funcs/logic_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1165 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/funcs/math_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      131 2024-05-13 15:12:03.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/funcs/special_funcs.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     6622 2024-05-14 18:01:02.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/funcs/string_functions.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      276 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/funcs/utils.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1980 2024-05-14 17:53:37.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/function_overview.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      104 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/main_module.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:13:05.106674 polars_expr_transformer-0.1.2/polars_expr_transformer/process/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:30:35.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/process/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     5237 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/process/models.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1512 2024-05-14 17:59:40.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/process/polars_expr_transformer.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4060 2024-05-14 15:26:05.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/process/preprocess.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4511 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/process/process_inline.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1618 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/process/standardize.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3148 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/process/tokenize.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     5038 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/process/tree.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      238 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/schemas.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:13:05.107028 polars_expr_transformer-0.1.2/polars_expr_transformer/utils/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/utils/__init__.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:59.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/utils/settings.py
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    13506 2024-05-13 15:00:14.000000 polars_expr_transformer-0.1.2/polars_expr_transformer/utils/utils.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:13:05.107619 polars_expr_transformer-0.1.2/polars_expr_transformer.egg-info/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     2286 2024-05-14 20:13:05.000000 polars_expr_transformer-0.1.2/polars_expr_transformer.egg-info/PKG-INFO
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1335 2024-05-14 20:13:05.000000 polars_expr_transformer-0.1.2/polars_expr_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-14 20:13:05.000000 polars_expr_transformer-0.1.2/polars_expr_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       99 2024-05-14 20:13:05.000000 polars_expr_transformer-0.1.2/polars_expr_transformer.egg-info/requires.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       24 2024-05-14 20:13:05.000000 polars_expr_transformer-0.1.2/polars_expr_transformer.egg-info/top_level.txt
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       38 2024-05-14 20:13:05.108312 polars_expr_transformer-0.1.2/setup.cfg
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1829 2024-05-14 20:11:59.000000 polars_expr_transformer-0.1.2/setup.py
-drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:13:05.107331 polars_expr_transformer-0.1.2/tests/
--rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1518 2024-05-14 19:53:33.000000 polars_expr_transformer-0.1.2/tests/test.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.089948 polars_expr_transformer-0.1.3/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    11357 2024-05-14 19:35:59.000000 polars_expr_transformer-0.1.3/LICENSE
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     2291 2024-05-14 20:14:11.089780 polars_expr_transformer-0.1.3/PKG-INFO
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1485 2024-05-14 20:00:49.000000 polars_expr_transformer-0.1.3/README.md
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.086177 polars_expr_transformer-0.1.3/polars_expr_transformer/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       84 2024-05-14 19:28:50.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/__init__.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.087029 polars_expr_transformer-0.1.3/polars_expr_transformer/configs/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:27.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/configs/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1290 2024-05-14 18:00:12.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/configs/settings.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.087896 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      386 2024-05-14 18:00:27.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     8014 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/date_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4155 2024-05-14 18:00:47.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/logic_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1165 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/math_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      131 2024-05-13 15:12:03.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/special_funcs.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     6622 2024-05-14 18:01:02.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/string_functions.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      276 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/utils.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1980 2024-05-14 17:53:37.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/function_overview.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      104 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/main_module.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.088813 polars_expr_transformer-0.1.3/polars_expr_transformer/process/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:30:35.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     5237 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/models.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1512 2024-05-14 17:59:40.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/polars_expr_transformer.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4060 2024-05-14 15:26:05.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/preprocess.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     4511 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/process_inline.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1618 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/standardize.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     3148 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/tokenize.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     5038 2024-05-14 17:57:19.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/process/tree.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)      238 2024-05-14 19:26:46.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/schemas.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.089106 polars_expr_transformer-0.1.3/polars_expr_transformer/utils/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-08 21:05:26.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/utils/__init__.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-13 14:35:59.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/utils/settings.py
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)    13506 2024-05-13 15:00:14.000000 polars_expr_transformer-0.1.3/polars_expr_transformer/utils/utils.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.089384 polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     2291 2024-05-14 20:14:11.000000 polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1335 2024-05-14 20:14:11.000000 polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)        1 2024-05-14 20:14:11.000000 polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       99 2024-05-14 20:14:11.000000 polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/requires.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       24 2024-05-14 20:14:11.000000 polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/top_level.txt
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)       38 2024-05-14 20:14:11.089987 polars_expr_transformer-0.1.3/setup.cfg
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1834 2024-05-14 20:14:05.000000 polars_expr_transformer-0.1.3/setup.py
+drwxr-xr-x   0 edwardvaneechoud   (501) staff       (20)        0 2024-05-14 20:14:11.089214 polars_expr_transformer-0.1.3/tests/
+-rw-r--r--   0 edwardvaneechoud   (501) staff       (20)     1518 2024-05-14 19:53:33.000000 polars_expr_transformer-0.1.3/tests/test.py
```

### Comparing `polars_expr_transformer-0.1.2/LICENSE` & `polars_expr_transformer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/PKG-INFO` & `polars_expr_transformer-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: polars_expr_transformer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Transform string-based expressions into Polars DataFrame operations
-Home-page: https://github.com/evaneechoud/polars_expr_transformer
+Home-page: https://github.com/edwardvaneechoud/polars_expr_transformer
 Author: Edward van Eehoud
 Author-email: evaneechoudl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `polars_expr_transformer-0.1.2/README.md` & `polars_expr_transformer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/configs/settings.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/configs/settings.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/funcs/date_functions.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/date_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/funcs/logic_functions.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/logic_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/funcs/math_functions.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/math_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/funcs/string_functions.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/funcs/string_functions.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/function_overview.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/function_overview.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/process/models.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/process/models.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/process/polars_expr_transformer.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/process/polars_expr_transformer.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/process/preprocess.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/process/preprocess.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/process/process_inline.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/process/process_inline.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/process/standardize.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/process/standardize.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/process/tokenize.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/process/tokenize.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/process/tree.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/process/tree.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer/utils/utils.py` & `polars_expr_transformer-0.1.3/polars_expr_transformer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer.egg-info/PKG-INFO` & `polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: polars_expr_transformer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Transform string-based expressions into Polars DataFrame operations
-Home-page: https://github.com/evaneechoud/polars_expr_transformer
+Home-page: https://github.com/edwardvaneechoud/polars_expr_transformer
 Author: Edward van Eehoud
 Author-email: evaneechoudl@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `polars_expr_transformer-0.1.2/polars_expr_transformer.egg-info/SOURCES.txt` & `polars_expr_transformer-0.1.3/polars_expr_transformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polars_expr_transformer-0.1.2/setup.py` & `polars_expr_transformer-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
     """Load requirements from a pip requirements file."""
     with open(filename, 'r') as file:
         lines = file.readlines()
     return [line.strip() for line in lines if line and not line.startswith("#")]
 
 setup(
     name='polars_expr_transformer',  # Package name
-    version='0.1.2',  # Package version
+    version='0.1.3',  # Package version
     description='Transform string-based expressions into Polars DataFrame operations',  # Short description
     long_description=long_description,
     long_description_content_type='text/markdown',  # Use markdown format for long description
     author='Edward van Eehoud',  # Replace with your name
     author_email='evaneechoudl@gmail.com',  # Replace with your email
-    url='https://github.com/evaneechoud/polars_expr_transformer',  # Replace with the URL to your package repository
+    url='https://github.com/edwardvaneechoud/polars_expr_transformer',  # Replace with the URL to your package repository
     packages=find_packages(include=['polars_expr_transformer', 'polars_expr_transformer.*']),  # Automatically find package directories
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',  # Specify the minimum Python version required
```

### Comparing `polars_expr_transformer-0.1.2/tests/test.py` & `polars_expr_transformer-0.1.3/tests/test.py`

 * *Files identical despite different names*

