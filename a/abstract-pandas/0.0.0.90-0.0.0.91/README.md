# Comparing `tmp/abstract_pandas-0.0.0.90.tar.gz` & `tmp/abstract_pandas-0.0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_pandas-0.0.0.90.tar", last modified: Wed May 15 10:25:32 2024, max compression
+gzip compressed data, was "abstract_pandas-0.0.0.91.tar", last modified: Wed May 15 10:27:40 2024, max compression
```

## Comparing `abstract_pandas-0.0.0.90.tar` & `abstract_pandas-0.0.0.91.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:25:32.915782 abstract_pandas-0.0.0.90/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-15 10:25:32.915782 abstract_pandas-0.0.0.90/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.90/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-15 10:25:32.915782 abstract_pandas-0.0.0.90/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1036 2024-05-15 10:25:27.000000 abstract_pandas-0.0.0.90/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:25:32.915782 abstract_pandas-0.0.0.90/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:25:32.915782 abstract_pandas-0.0.0.90/src/abstract_pandas/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       29 2024-05-10 04:14:51.000000 abstract_pandas-0.0.0.90/src/abstract_pandas/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5943 2024-05-10 08:14:17.000000 abstract_pandas-0.0.0.90/src/abstract_pandas/abstractLandManager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.0.90/src/abstract_pandas/depriciated.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     6290 2024-05-10 04:15:06.000000 abstract_pandas-0.0.0.90/src/abstract_pandas/excel_classes.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.0.90/src/abstract_pandas/excel_gui.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    13418 2024-05-15 09:12:52.000000 abstract_pandas-0.0.0.90/src/abstract_pandas/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    14885 2024-05-15 10:24:44.000000 abstract_pandas-0.0.0.90/src/abstract_pandas/file_utils.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-06 03:12:41.000000 abstract_pandas-0.0.0.90/src/abstract_pandas/functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     7459 2024-05-06 03:49:09.000000 abstract_pandas-0.0.0.90/src/abstract_pandas/general_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1745 2024-05-10 04:14:25.000000 abstract_pandas-0.0.0.90/src/abstract_pandas/location_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     2851 2024-05-15 09:36:55.000000 abstract_pandas-0.0.0.90/src/abstract_pandas/proj_tools.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8552 2024-05-10 04:14:42.000000 abstract_pandas-0.0.0.90/src/abstract_pandas/query_tools.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:25:32.915782 abstract_pandas-0.0.0.90/src/abstract_pandas.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-15 10:25:32.000000 abstract_pandas-0.0.0.90/src/abstract_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      667 2024-05-15 10:25:32.000000 abstract_pandas-0.0.0.90/src/abstract_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-15 10:25:32.000000 abstract_pandas-0.0.0.90/src/abstract_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      108 2024-05-15 10:25:32.000000 abstract_pandas-0.0.0.90/src/abstract_pandas.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-15 10:25:32.000000 abstract_pandas-0.0.0.90/src/abstract_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:27:40.082211 abstract_pandas-0.0.0.91/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-15 10:27:40.082211 abstract_pandas-0.0.0.91/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.91/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-15 10:27:40.082211 abstract_pandas-0.0.0.91/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1036 2024-05-15 10:27:33.000000 abstract_pandas-0.0.0.91/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:27:40.078211 abstract_pandas-0.0.0.91/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:27:40.078211 abstract_pandas-0.0.0.91/src/abstract_pandas/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       29 2024-05-10 04:14:51.000000 abstract_pandas-0.0.0.91/src/abstract_pandas/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5943 2024-05-10 08:14:17.000000 abstract_pandas-0.0.0.91/src/abstract_pandas/abstractLandManager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.0.91/src/abstract_pandas/depriciated.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     6290 2024-05-10 04:15:06.000000 abstract_pandas-0.0.0.91/src/abstract_pandas/excel_classes.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.0.91/src/abstract_pandas/excel_gui.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    13418 2024-05-15 09:12:52.000000 abstract_pandas-0.0.0.91/src/abstract_pandas/excel_module.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    14864 2024-05-15 10:27:28.000000 abstract_pandas-0.0.0.91/src/abstract_pandas/file_utils.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-06 03:12:41.000000 abstract_pandas-0.0.0.91/src/abstract_pandas/functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7459 2024-05-06 03:49:09.000000 abstract_pandas-0.0.0.91/src/abstract_pandas/general_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1745 2024-05-10 04:14:25.000000 abstract_pandas-0.0.0.91/src/abstract_pandas/location_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2851 2024-05-15 09:36:55.000000 abstract_pandas-0.0.0.91/src/abstract_pandas/proj_tools.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8552 2024-05-10 04:14:42.000000 abstract_pandas-0.0.0.91/src/abstract_pandas/query_tools.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:27:40.082211 abstract_pandas-0.0.0.91/src/abstract_pandas.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-15 10:27:40.000000 abstract_pandas-0.0.0.91/src/abstract_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      667 2024-05-15 10:27:40.000000 abstract_pandas-0.0.0.91/src/abstract_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-15 10:27:40.000000 abstract_pandas-0.0.0.91/src/abstract_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      108 2024-05-15 10:27:40.000000 abstract_pandas-0.0.0.91/src/abstract_pandas.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-15 10:27:40.000000 abstract_pandas-0.0.0.91/src/abstract_pandas.egg-info/top_level.txt
```

### Comparing `abstract_pandas-0.0.0.90/PKG-INFO` & `abstract_pandas-0.0.0.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.90
+Version: 0.0.0.91
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.90/setup.py` & `abstract_pandas-0.0.0.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_pandas',
-    version='0.0.0.90',
+    version='0.0.0.91',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas/abstractLandManager.py` & `abstract_pandas-0.0.0.91/src/abstract_pandas/abstractLandManager.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas/depriciated.py` & `abstract_pandas-0.0.0.91/src/abstract_pandas/depriciated.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas/excel_classes.py` & `abstract_pandas-0.0.0.91/src/abstract_pandas/excel_classes.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas/excel_gui.py` & `abstract_pandas-0.0.0.91/src/abstract_pandas/excel_gui.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas/excel_module.py` & `abstract_pandas-0.0.0.91/src/abstract_pandas/excel_module.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas/file_utils.py` & `abstract_pandas-0.0.0.91/src/abstract_pandas/file_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,14 @@
     return df
 def read_shape_file(source):
     file_ext = is_file(source)
     if file_ext:
         if file_ext in ['.shp', '.cpg', '.dbf', '.shx','.geojson']:
             df = gpd.read_file(source,driver=source_ext(file_ext))
             return df
-        elif file_ext in ['.prj']:
-            df = get_wkt_string(source)
-            return df
     return False
 def get_df(source=None, nrows=None, skiprows=None, condition=None, indices=None):
     """
     Load a DataFrame from various sources with optional filtering.
 
     Parameters:
     - source (str, pd.DataFrame, gpd.GeoDataFrame, dict, list, FileStorage): Source of the data.
@@ -124,16 +121,18 @@
             elif file_ext in ['.ods', '.xlsx', '.xls', '.xlsb']:
                 engine = {'ods': 'odf', 'xlsx': 'openpyxl', 'xls': 'xlrd', 'xlsb': 'pyxlsb'}.get(file_ext.strip('.'))
                 df = pd.read_excel(source,  skiprows=skiprows, engine=engine, nrows=nrows)
             elif file_ext == '.json':
                 df = pd.read_json(source, nrows=nrows)
             elif file_ext == '.parquet':
                 df = pd.read_parquet(source, nrows=nrows)
-            elif file_ext in ['.shp', '.cpg', '.dbf', '.shx','.geojson','.prj']:
+            elif file_ext in ['.shp', '.cpg', '.dbf', '.shx','.geojson']:
                 df = read_shape_file(source)
+            elif file_ext == '.prj':
+                return get_wkt_string(source)
             else:
                 try:
                     df = read_from_file(source)
                 except:                
                     raise logging.info(f"Unsupported file extension: {file_ext}")
             if not isinstance(df, (dict, list,FileStorage)):
                 return filter_df(df, nrows=nrows, condition=condition, indices=indices)
```

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas/functions.py` & `abstract_pandas-0.0.0.91/src/abstract_pandas/functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas/general_functions.py` & `abstract_pandas-0.0.0.91/src/abstract_pandas/general_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas/location_functions.py` & `abstract_pandas-0.0.0.91/src/abstract_pandas/location_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas/proj_tools.py` & `abstract_pandas-0.0.0.91/src/abstract_pandas/proj_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas/query_tools.py` & `abstract_pandas-0.0.0.91/src/abstract_pandas/query_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas.egg-info/PKG-INFO` & `abstract_pandas-0.0.0.91/src/abstract_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.90
+Version: 0.0.0.91
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.90/src/abstract_pandas.egg-info/SOURCES.txt` & `abstract_pandas-0.0.0.91/src/abstract_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

