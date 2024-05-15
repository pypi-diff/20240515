# Comparing `tmp/abstract_pandas-0.0.0.94.tar.gz` & `tmp/abstract_pandas-0.0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_pandas-0.0.0.94.tar", last modified: Wed May 15 10:37:58 2024, max compression
+gzip compressed data, was "abstract_pandas-0.0.0.95.tar", last modified: Wed May 15 10:44:06 2024, max compression
```

## Comparing `abstract_pandas-0.0.0.94.tar` & `abstract_pandas-0.0.0.95.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:37:58.582519 abstract_pandas-0.0.0.94/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-15 10:37:58.582519 abstract_pandas-0.0.0.94/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.94/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-15 10:37:58.582519 abstract_pandas-0.0.0.94/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1036 2024-05-15 10:37:45.000000 abstract_pandas-0.0.0.94/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:37:58.578519 abstract_pandas-0.0.0.94/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:37:58.582519 abstract_pandas-0.0.0.94/src/abstract_pandas/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       29 2024-05-10 04:14:51.000000 abstract_pandas-0.0.0.94/src/abstract_pandas/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5943 2024-05-10 08:14:17.000000 abstract_pandas-0.0.0.94/src/abstract_pandas/abstractLandManager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.0.94/src/abstract_pandas/depriciated.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     6290 2024-05-10 04:15:06.000000 abstract_pandas-0.0.0.94/src/abstract_pandas/excel_classes.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.0.94/src/abstract_pandas/excel_gui.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    13418 2024-05-15 09:12:52.000000 abstract_pandas-0.0.0.94/src/abstract_pandas/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    14964 2024-05-15 10:37:38.000000 abstract_pandas-0.0.0.94/src/abstract_pandas/file_utils.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-06 03:12:41.000000 abstract_pandas-0.0.0.94/src/abstract_pandas/functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     7459 2024-05-06 03:49:09.000000 abstract_pandas-0.0.0.94/src/abstract_pandas/general_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1745 2024-05-10 04:14:25.000000 abstract_pandas-0.0.0.94/src/abstract_pandas/location_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     2861 2024-05-15 10:34:45.000000 abstract_pandas-0.0.0.94/src/abstract_pandas/proj_tools.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8552 2024-05-10 04:14:42.000000 abstract_pandas-0.0.0.94/src/abstract_pandas/query_tools.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:37:58.582519 abstract_pandas-0.0.0.94/src/abstract_pandas.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-15 10:37:58.000000 abstract_pandas-0.0.0.94/src/abstract_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      667 2024-05-15 10:37:58.000000 abstract_pandas-0.0.0.94/src/abstract_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-15 10:37:58.000000 abstract_pandas-0.0.0.94/src/abstract_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      108 2024-05-15 10:37:58.000000 abstract_pandas-0.0.0.94/src/abstract_pandas.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-15 10:37:58.000000 abstract_pandas-0.0.0.94/src/abstract_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:44:06.877918 abstract_pandas-0.0.0.95/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-15 10:44:06.877918 abstract_pandas-0.0.0.95/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.95/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-15 10:44:06.877918 abstract_pandas-0.0.0.95/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1036 2024-05-15 10:43:53.000000 abstract_pandas-0.0.0.95/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:44:06.873918 abstract_pandas-0.0.0.95/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:44:06.873918 abstract_pandas-0.0.0.95/src/abstract_pandas/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       29 2024-05-10 04:14:51.000000 abstract_pandas-0.0.0.95/src/abstract_pandas/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5943 2024-05-10 08:14:17.000000 abstract_pandas-0.0.0.95/src/abstract_pandas/abstractLandManager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.0.95/src/abstract_pandas/depriciated.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     6290 2024-05-10 04:15:06.000000 abstract_pandas-0.0.0.95/src/abstract_pandas/excel_classes.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.0.95/src/abstract_pandas/excel_gui.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    13418 2024-05-15 09:12:52.000000 abstract_pandas-0.0.0.95/src/abstract_pandas/excel_module.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    15076 2024-05-15 10:43:46.000000 abstract_pandas-0.0.0.95/src/abstract_pandas/file_utils.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-06 03:12:41.000000 abstract_pandas-0.0.0.95/src/abstract_pandas/functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7459 2024-05-06 03:49:09.000000 abstract_pandas-0.0.0.95/src/abstract_pandas/general_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1745 2024-05-10 04:14:25.000000 abstract_pandas-0.0.0.95/src/abstract_pandas/location_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2861 2024-05-15 10:34:45.000000 abstract_pandas-0.0.0.95/src/abstract_pandas/proj_tools.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8552 2024-05-10 04:14:42.000000 abstract_pandas-0.0.0.95/src/abstract_pandas/query_tools.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:44:06.877918 abstract_pandas-0.0.0.95/src/abstract_pandas.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-15 10:44:06.000000 abstract_pandas-0.0.0.95/src/abstract_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      667 2024-05-15 10:44:06.000000 abstract_pandas-0.0.0.95/src/abstract_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-15 10:44:06.000000 abstract_pandas-0.0.0.95/src/abstract_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      108 2024-05-15 10:44:06.000000 abstract_pandas-0.0.0.95/src/abstract_pandas.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-15 10:44:06.000000 abstract_pandas-0.0.0.95/src/abstract_pandas.egg-info/top_level.txt
```

### Comparing `abstract_pandas-0.0.0.94/PKG-INFO` & `abstract_pandas-0.0.0.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.94
+Version: 0.0.0.95
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.94/setup.py` & `abstract_pandas-0.0.0.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_pandas',
-    version='0.0.0.94',
+    version='0.0.0.95',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas/abstractLandManager.py` & `abstract_pandas-0.0.0.95/src/abstract_pandas/abstractLandManager.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas/depriciated.py` & `abstract_pandas-0.0.0.95/src/abstract_pandas/depriciated.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas/excel_classes.py` & `abstract_pandas-0.0.0.95/src/abstract_pandas/excel_classes.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas/excel_gui.py` & `abstract_pandas-0.0.0.95/src/abstract_pandas/excel_gui.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas/excel_module.py` & `abstract_pandas-0.0.0.95/src/abstract_pandas/excel_module.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas/file_utils.py` & `abstract_pandas-0.0.0.95/src/abstract_pandas/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,14 +124,16 @@
                 df = pd.read_excel(source,  skiprows=skiprows, engine=engine, nrows=nrows)
             elif file_ext == '.json':
                 df = pd.read_json(source, nrows=nrows)
             elif file_ext == '.parquet':
                 df = pd.read_parquet(source, nrows=nrows)
             elif file_ext in ['.shp', '.cpg', '.dbf', '.shx','.geojson']:
                 df = read_shape_file(source)
+                df = filter_df(df, nrows=nrows, condition=condition, indices=indices)
+                return df
             elif file_ext == '.prj':
                 with open(source, "r") as file:
                     return file.read()
             else:
                 try:
                     df = read_from_file(source)
                 except:
```

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas/functions.py` & `abstract_pandas-0.0.0.95/src/abstract_pandas/functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas/general_functions.py` & `abstract_pandas-0.0.0.95/src/abstract_pandas/general_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas/location_functions.py` & `abstract_pandas-0.0.0.95/src/abstract_pandas/location_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas/proj_tools.py` & `abstract_pandas-0.0.0.95/src/abstract_pandas/proj_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas/query_tools.py` & `abstract_pandas-0.0.0.95/src/abstract_pandas/query_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas.egg-info/PKG-INFO` & `abstract_pandas-0.0.0.95/src/abstract_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.94
+Version: 0.0.0.95
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.94/src/abstract_pandas.egg-info/SOURCES.txt` & `abstract_pandas-0.0.0.95/src/abstract_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

