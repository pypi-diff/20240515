# Comparing `tmp/abstract_pandas-0.0.0.89.tar.gz` & `tmp/abstract_pandas-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_pandas-0.0.0.89.tar", last modified: Wed May 15 10:20:28 2024, max compression
+gzip compressed data, was "abstract_pandas-0.0.0.9.tar", last modified: Sun May  5 07:38:06 2024, max compression
```

## Comparing `abstract_pandas-0.0.0.89.tar` & `abstract_pandas-0.0.0.9.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:20:28.567511 abstract_pandas-0.0.0.89/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-15 10:20:28.567511 abstract_pandas-0.0.0.89/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.89/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-15 10:20:28.567511 abstract_pandas-0.0.0.89/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1036 2024-05-15 10:20:19.000000 abstract_pandas-0.0.0.89/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:20:28.563511 abstract_pandas-0.0.0.89/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:20:28.567511 abstract_pandas-0.0.0.89/src/abstract_pandas/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       29 2024-05-10 04:14:51.000000 abstract_pandas-0.0.0.89/src/abstract_pandas/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5943 2024-05-10 08:14:17.000000 abstract_pandas-0.0.0.89/src/abstract_pandas/abstractLandManager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.0.89/src/abstract_pandas/depriciated.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     6290 2024-05-10 04:15:06.000000 abstract_pandas-0.0.0.89/src/abstract_pandas/excel_classes.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.0.89/src/abstract_pandas/excel_gui.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    13418 2024-05-15 09:12:52.000000 abstract_pandas-0.0.0.89/src/abstract_pandas/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    14778 2024-05-15 10:19:42.000000 abstract_pandas-0.0.0.89/src/abstract_pandas/file_utils.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-06 03:12:41.000000 abstract_pandas-0.0.0.89/src/abstract_pandas/functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     7459 2024-05-06 03:49:09.000000 abstract_pandas-0.0.0.89/src/abstract_pandas/general_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1745 2024-05-10 04:14:25.000000 abstract_pandas-0.0.0.89/src/abstract_pandas/location_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     2851 2024-05-15 09:36:55.000000 abstract_pandas-0.0.0.89/src/abstract_pandas/proj_tools.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8552 2024-05-10 04:14:42.000000 abstract_pandas-0.0.0.89/src/abstract_pandas/query_tools.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 10:20:28.567511 abstract_pandas-0.0.0.89/src/abstract_pandas.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-15 10:20:28.000000 abstract_pandas-0.0.0.89/src/abstract_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      667 2024-05-15 10:20:28.000000 abstract_pandas-0.0.0.89/src/abstract_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-15 10:20:28.000000 abstract_pandas-0.0.0.89/src/abstract_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      108 2024-05-15 10:20:28.000000 abstract_pandas-0.0.0.89/src/abstract_pandas.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-15 10:20:28.000000 abstract_pandas-0.0.0.89/src/abstract_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 07:38:06.523038 abstract_pandas-0.0.0.9/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-05-05 07:38:06.523038 abstract_pandas-0.0.0.9/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.9/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-05 07:38:06.523038 abstract_pandas-0.0.0.9/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      979 2024-05-05 07:37:55.000000 abstract_pandas-0.0.0.9/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 07:38:06.519038 abstract_pandas-0.0.0.9/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 07:38:06.523038 abstract_pandas-0.0.0.9/src/abstract_pandas/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       54 2024-05-05 03:13:48.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/depriciated.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     6291 2024-05-05 07:04:33.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/excel_classes.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/excel_gui.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    23630 2024-05-05 07:26:06.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/excel_module.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8967 2024-05-05 07:35:43.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/file_utils.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7154 2024-05-05 07:23:50.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/general_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2731 2024-05-05 06:13:53.000000 abstract_pandas-0.0.0.9/src/abstract_pandas/landManager.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 07:38:06.523038 abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-05-05 07:38:06.000000 abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      515 2024-05-05 07:38:06.000000 abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-05 07:38:06.000000 abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-05-05 07:38:06.000000 abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-05 07:38:06.000000 abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/top_level.txt
```

### Comparing `abstract_pandas-0.0.0.89/setup.py` & `abstract_pandas-0.0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_pandas',
-    version='0.0.0.89',
+    version='0.0.0.9',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.11',
       ],
-    install_requires=['abstract_utilities', 'pandas', 'openpyxl','abstract_security','Werkzeug','odfpy','ezodf','lxml','geopandas','abstract_distances'],
+    install_requires=['abstract_utilities', 'pandas', 'openpyxl','abstract_security','requests'],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     # Add this line to include wheel format in your distribution
     setup_requires=['wheel'],
 )
```

### Comparing `abstract_pandas-0.0.0.89/src/abstract_pandas/depriciated.py` & `abstract_pandas-0.0.0.9/src/abstract_pandas/depriciated.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.89/src/abstract_pandas/excel_classes.py` & `abstract_pandas-0.0.0.9/src/abstract_pandas/excel_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 from .excel_module import *
 class SingletonMeta(type):
     _instances = {}
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(SingletonMeta, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
```

### Comparing `abstract_pandas-0.0.0.89/src/abstract_pandas/excel_gui.py` & `abstract_pandas-0.0.0.9/src/abstract_pandas/excel_gui.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.89/src/abstract_pandas/file_utils.py` & `abstract_pandas-0.0.0.9/src/abstract_pandas/file_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,15 @@
 from odf.table import Table, TableRow, TableCell
 from odf.opendocument import load
 import pandas as pd
-import geopandas as gpd
-from .proj_tools import *
-from abstract_utilities import *
 from odf import text, teletype
 from datetime import datetime
-from openpyxl import load_workbook, utils
-from difflib import get_close_matches
-from werkzeug.utils import secure_filename
-from werkzeug.datastructures import FileStorage
-import tempfile,shutil,os,ezodf,inspect,logging,logging
-from .general_functions import split_and_clean_lines,make_type,convert_column,return_float_or_int,safe_get,get_number
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-def source_ext(typ=None):
-    source_js = {'.parquet':'pyarrow','.txt':'python','.xlsx':'openpyxl','.xls':'openpyxl','.xlsb':'pyxlsb','.ods':'odf','.geojson':'GeoJSON'}
-    if typ:
-        source_js = source_js.get(typ)
-    return source_js
-def is_file(file_path):
-    if file_path and isinstance(file_path, str) and os.path.isfile(file_path):
-        return os.path.splitext(file_path)[-1].lower()
-def isDataFrame(obj):
-    return isinstance(obj, pd.DataFrame)
-def create_dataframe(new_data=None,columns=None):
-    if isDataFrame(new_data):
-        return new_data
-    new_data = new_data or {}
-    if isinstance(new_data,dict):
-        new_data=[new_data]
-        if columns == None:
-            columns=[]
-            for datas in new_data:
-                if isinstance(datas,dict):
-                    columns=list(set(columns+list(datas.keys())))
-        if columns ==False:
-            columns=None
-    if isinstance(new_data,list):
-        return pd.DataFrame(new_data,columns=columns)
+import tempfile,shutil,os,ezodf,inspect
+def source_ext():
+    return {'.parquet':'pyarrow','.txt':'python','.xlsx':'openpyxl','.xls':'openpyxl','.xlsb':'pyxlsb','.ods':'odf'}
 def read_ods_file(file_path):
     doc = ezodf.opendoc(file_path)
     sheets = {}
     
     for sheet in doc.sheets:
         data = []
         for row in sheet.rows():
@@ -58,147 +26,43 @@
         df = pd.DataFrame(data)
         sheets[sheet.name] = df
         print(f"Processed sheet: {sheet.name}")
     return sheets
 def read_ods(file_path,xlsx_path=None):
     ods_to_xlsx(file_path,xlsx_path)
     return pd.read_excel(xlsx_path)
-def filter_df(df, nrows=None, condition=None, indices=None):
-    """
-    Apply filtering to a DataFrame based on specified criteria.
-
-    Parameters:
-    - df (DataFrame): The DataFrame to filter.
-    - nrows (int, optional): Number of rows to return from the start.
-    - condition (pd.Series, optional): Boolean series for row filtering.
-    - indices (list of int, optional): Row indices to select.
-
-    Returns:
-    - DataFrame: Filtered DataFrame.
-    """
-    if nrows is not None:
-        df = df.head(nrows)
-    if condition is not None:
-        df = df[condition]
-    if indices is not None:
-        df = df.iloc[indices]
-    return df
-def read_shape_file(source):
-    file_ext = is_file(source)
-    if file_ext:
-        if file_ext in ['.shp', '.cpg', '.dbf', '.shx','.geojson']:
-            df = gpd.read_file(source,driver=source_ext(file_ext))
-            return df
-        elif file_ext in ['.prj']:
-            df = get_wkt_string(source)
-            return df
-    return False
-def get_df(source=None, nrows=None, skiprows=None, condition=None, indices=None):
-    """
-    Load a DataFrame from various sources with optional filtering.
-
-    Parameters:
-    - source (str, pd.DataFrame, gpd.GeoDataFrame, dict, list, FileStorage): Source of the data.
-    - nrows (int, optional): Number of rows to load.
-    - header (int, list of int, 'infer', optional): Row(s) to use as the header.
-    - skiprows (list-like, int, optional): Rows to skip at the beginning.
-    - condition (pd.Series, optional): Condition for filtering rows.
-    - indices (list of int, optional): Indices of rows to select.
-
-    Returns:
-    - pd.DataFrame or gpd.GeoDataFrame: Loaded and optionally filtered data.
-    """
-    if isinstance(source, (pd.DataFrame, gpd.GeoDataFrame)):
-        return filter_df(source, nrows=nrows, condition=condition, indices=indices)
-
-    if source is None:
-        logging.error("No source provided for loading data.")
-        return create_dataframe()
-    file_ext = is_file(source)
-    if file_ext:
-        
-        
-            logging.info(f"Loading data from file with extension: {file_ext}")
-            if file_ext in ['.csv', '.tsv', '.txt']:
-                sep = {'csv': ',', 'tsv': '\t'}.get(file_ext.strip('.'), None)
-                df = pd.read_csv(source,  skiprows=skiprows, sep=sep, nrows=nrows)
-            elif file_ext in ['.ods', '.xlsx', '.xls', '.xlsb']:
-                engine = {'ods': 'odf', 'xlsx': 'openpyxl', 'xls': 'xlrd', 'xlsb': 'pyxlsb'}.get(file_ext.strip('.'))
-                df = pd.read_excel(source,  skiprows=skiprows, engine=engine, nrows=nrows)
-            elif file_ext == '.json':
-                df = pd.read_json(source, nrows=nrows)
-            elif file_ext == '.parquet':
-                df = pd.read_parquet(source, nrows=nrows)
-            elif file_ext in ['.shp', '.cpg', '.dbf', '.shx','.geojson','.prj']:
-                df = read_shape_file(source)
-            else:
-                try:
-                    df = read_from_file(source)
-                except:                
-                    raise logging.info(f"Unsupported file extension: {file_ext}")
-            if not isinstance(df, (dict, list,FileStorage)):
-                return filter_df(df, nrows=nrows, condition=condition, indices=indices)
-            source = df
-        
-
-    if isinstance(source, FileStorage):
-        try:
-            logging.info(f"Reading from FileStorage: {secure_filename(source.filename)}")
-            df = pd.read_excel(source.stream, nrows=nrows)
-            return filter_df(df, nrows=nrows, condition=condition, indices=indices)
-        except Exception as e:
-            logging.error(f"Failed to read from FileStorage: {e}")
-            return None
-
-    if isinstance(source, (dict, list)):
-        logging.info("Creating DataFrame from in-memory data structure.")
-        df = pd.DataFrame(source)
-        return filter_df(df, nrows=nrows, condition=condition, indices=indices)
-
-    logging.error("Invalid data source type provided.")
-    return None
 def save_df(df,file_path,index=None,suffix=None,engine=None):
     df = get_df(df)
-    suffix = suffix or os.path.splitext(file_path)[-1] or '.xlsx'
-    logging.info(f"saving df with suffix {suffix} to {file_path}")
+    suffix = suffix or os.path.splitext(original_file_path)[-1] or '.xlsx'
+    logging.info(f"saving df with suffix {file_ext} to {file_path}")
     try:
-        if suffix in ['.ods','.xlsx', '.xls','.xlsb']:
-            df.to_excel(file_path,  engine=engine or source_ext(suffix))
-            
-        elif suffix in ['.csv','.tsv','.txt']:
-            df.to_csv(file_path,  engine=engine or source_ext(suffix))
-        elif suffix in [".shp", ".cpg", ".dbf", ".shx",'.geojson']:
-            df.to_file(file_path,driver=source_ext(suffix))
-        elif suffix in ['.prj']:
-            save_valid_crs(df, file_path=file_path)
-        elif suffix == '.parquet':
-            df.to_parquet(file_path, engine=engine or source_ext(suffix))
+        if file_ext in ['.ods','.xlsx', '.xls','.xlsb']:
+            pd.to_excel(df,  engine=engine or source_ext().get(file_ext))
+        elif file_ext in ['.csv','.tsv','.txt']:
+            pd.to_csv(df,  engine=engine or source_ext().get(file_ext))
+        elif file_ext in [".shp", ".cpg", ".dbf", ".shx"]:
+            gpd.save_file(df, file_path)
+        elif file_ext == '.parquet':
+            pd.to_parquet(df, engine=engine or source_ext().get(file_ext))
         else:
             logging.info(f"could not find appropriate file type, attempting generic file save")
             try:
-                save_to_file(df,file_path)
-                logging.info(f"file save for file path {file_path} succesful")
-                return True
+                df = save_to_file(file_path)
             except Exception as e:
                 logging.info(f"file save for file path {file_path} unsuccesful:\n {e}")
                 return False
-        logging.info(f"file save for file path {file_path} succesful")
-        return True
     except Exception as e:
         logging.info(f"Failed to read file: {e}")
         return False
+    logging.info(f"file save for file path {file_path} succesful")
     return True
-    
 def safe_excel_save(df,original_file_path,index=False,suffix=None,engine=None):
-    suffix = suffix or os.path.splitext(original_file_path)[-1] or '.xlsx'
-    result = None
     with tempfile.NamedTemporaryFile(delete=False, suffix=suffix) as tmp:
         temp_file_name = tmp.name
-        result = save_df(df,temp_file_name,index=index,suffix=suffix,engine=engine)  # Save your DataFrame to the temp file
-        logging.info(f"{temp_file_name} {os.path.isfile(temp_file_name)},{os.path.getsize(temp_file_name)}")
+        result = save_df(df,file_path,index=index,suffix=suffix,engine=engine)  # Save your DataFrame to the temp file
     if result and os.path.getsize(temp_file_name) > 0:
         shutil.move(temp_file_name, original_file_path)
     else:
        logging.info("Temporary file is empty or wasn't written correctly. Original file is unchanged.")
     # Cleanup: Ensure the temporary file is deleted if it hasn't been moved
     if os.path.exists(temp_file_name):
         os.remove(temp_file_name)
```

### Comparing `abstract_pandas-0.0.0.89/src/abstract_pandas/general_functions.py` & `abstract_pandas-0.0.0.9/src/abstract_pandas/general_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abstract_security import *
 import os, time
 from datetime import datetime, timedelta
 from itertools import permutations
-from abstract_utilities import eatAll
+
 def capitalize(string):
    string = str(string)
    return  string[0].upper()+string[1:]
 def add_to_dict(key,value,_dict={}):
    _dict[key]=value
    return _dict
 def get_dict(is_true=False,*args,**kwargs):
@@ -120,21 +120,14 @@
 
     :param strings: A list of strings for which we want to generate all combinations.
     :return: A list of strings representing all possible combinations.
     """
     all_perms = permutations(strings)
     combinations = [''.join(perm) for perm in all_perms]
     return combinations
-def clean_list(list_obj):
-    while '' in list_obj:
-        list_obj.remove('')
-    return list_obj
-def split_and_clean_lines(query):
-    query = query.replace('\n',',')
-    return list(set([eatAll(quer,[',',' ','\t','\n']) for quer in clean_list(query.split(','))]))
 
 def all_date_formats():
     date_formats = []
     for part in all_combinations_of_strings("Ymd"):
         for separator in ['/', '-', '_']:
             date_pattern = ''
             for piece in part:
```

### Comparing `abstract_pandas-0.0.0.89/src/abstract_pandas.egg-info/SOURCES.txt` & `abstract_pandas-0.0.0.9/src/abstract_pandas.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 README.md
 setup.py
 src/abstract_pandas/__init__.py
-src/abstract_pandas/abstractLandManager.py
 src/abstract_pandas/depriciated.py
 src/abstract_pandas/excel_classes.py
 src/abstract_pandas/excel_gui.py
 src/abstract_pandas/excel_module.py
 src/abstract_pandas/file_utils.py
-src/abstract_pandas/functions.py
 src/abstract_pandas/general_functions.py
-src/abstract_pandas/location_functions.py
-src/abstract_pandas/proj_tools.py
-src/abstract_pandas/query_tools.py
+src/abstract_pandas/landManager.py
 src/abstract_pandas.egg-info/PKG-INFO
 src/abstract_pandas.egg-info/SOURCES.txt
 src/abstract_pandas.egg-info/dependency_links.txt
 src/abstract_pandas.egg-info/requires.txt
 src/abstract_pandas.egg-info/top_level.txt
```

