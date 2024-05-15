# Comparing `tmp/python_esios-0.1.3.tar.gz` & `tmp/python_esios-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_esios-0.1.3.tar", last modified: Wed May 15 06:42:23 2024, max compression
+gzip compressed data, was "python_esios-0.1.4.tar", last modified: Wed May 15 06:54:00 2024, max compression
```

## Comparing `python_esios-0.1.3.tar` & `python_esios-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:23.082380 python_esios-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:14.000000 python_esios-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 06:42:23.082380 python_esios-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-15 06:42:14.000000 python_esios-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:23.078380 python_esios-0.1.3/esios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:14.000000 python_esios-0.1.3/esios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-15 06:42:14.000000 python_esios-0.1.3/esios/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:23.078380 python_esios-0.1.3/esios/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 06:42:14.000000 python_esios-0.1.3/esios/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:23.078380 python_esios-0.1.3/esios/endpoints/indicators/
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-15 06:42:15.000000 python_esios-0.1.3/esios/endpoints/indicators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:23.082380 python_esios-0.1.3/python_esios.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 06:42:23.000000 python_esios-0.1.3/python_esios.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 06:42:23.000000 python_esios-0.1.3/python_esios.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:42:23.000000 python_esios-0.1.3/python_esios.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 06:42:23.000000 python_esios-0.1.3/python_esios.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 06:42:23.000000 python_esios-0.1.3/python_esios.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:42:23.082380 python_esios-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 06:42:15.000000 python_esios-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:54:00.589653 python_esios-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:53:51.000000 python_esios-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 06:54:00.589653 python_esios-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-15 06:53:51.000000 python_esios-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:54:00.585652 python_esios-0.1.4/esios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:53:51.000000 python_esios-0.1.4/esios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-15 06:53:51.000000 python_esios-0.1.4/esios/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:54:00.589653 python_esios-0.1.4/esios/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 06:53:51.000000 python_esios-0.1.4/esios/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:54:00.589653 python_esios-0.1.4/esios/endpoints/indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-15 06:53:51.000000 python_esios-0.1.4/esios/endpoints/indicators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:54:00.589653 python_esios-0.1.4/python_esios.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 06:54:00.000000 python_esios-0.1.4/python_esios.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 06:54:00.000000 python_esios-0.1.4/python_esios.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:54:00.000000 python_esios-0.1.4/python_esios.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 06:54:00.000000 python_esios-0.1.4/python_esios.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 06:54:00.000000 python_esios-0.1.4/python_esios.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:54:00.589653 python_esios-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 06:53:51.000000 python_esios-0.1.4/setup.py
```

### Comparing `python_esios-0.1.3/PKG-INFO` & `python_esios-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esios
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python wrapper for the ESIOS API
 Home-page: https://github.com/datons/python-esios
 Author: Jesús López
 Author-email: jesus.lopez@datons.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_esios-0.1.3/esios/api_client.py` & `python_esios-0.1.4/esios/api_client.py`

 * *Files identical despite different names*

### Comparing `python_esios-0.1.3/esios/endpoints/indicators/__init__.py` & `python_esios-0.1.4/esios/endpoints/indicators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -87,14 +87,18 @@
         response = self._api_call('GET', endpoint, params=params)
         return IndicatorData(response.json())
 
 class IndicatorData:
     def __init__(self, data):
         self.data = data
 
+class IndicatorData:
+    def __init__(self, data):
+        self.data = data
+
     def to_dataframe(self, column_name='value'):
         """
         Converts the indicator values data to a Pandas DataFrame.
 
         Parameters
         -------
         column_name : {'value', 'id', 'short_name'}, default 'value'
@@ -105,37 +109,36 @@
             A DataFrame containing the indicator values.
         """
         data = self.data.get('indicator', {})
         values = data.get('values', [])
         
         if values:
             df = pd.DataFrame(values)
-            df = df.set_index('datetime')
-            df.index = pd.to_datetime(df.index, utc=True)
-            
-            columns = df.columns
-            mask = columns.str.contains('time')
+            if 'datetime' in df.columns:
+                df['datetime'] = pd.to_datetime(df['datetime'], utc=True)
+                df = df.set_index('datetime')
+                df.index = df.index.tz_convert('Europe/Madrid')
             
-            df.drop(columns=columns[mask], inplace=True)
+            # Drop all columns that contain the word 'time' in them
+            df = df[[col for col in df.columns if not 'time' in col]]
             
-            if column_name != 'value':
-                df = df.rename(columns={'value': data[column_name]})
+            # Rename 'value' column if a different column_name is requested
+            if column_name in data and column_name != 'value':
+                df.rename(columns={'value': data[column_name]}, inplace=True)
             
-            return df.tz_convert('Europe/Madrid')
+            return df
         else:
             return pd.DataFrame()
 
     def get_metadata(self):
         """
         Extracts metadata from the indicator data.
 
         Returns
         -------
         dict
             A dictionary containing the metadata of the indicator.
         """
+        metadata = self.data.get('indicator', {}).copy()  # Use a copy to avoid mutating original data
+        metadata.pop('values', None)  # Remove values key to extract only metadata
         
-        # extract all inside indicator key, except values
-        metadata = self.data.get('indicator', {})
-        metadata.pop('values', None)
-        
-        return metadata
+        return metadata
```

### Comparing `python_esios-0.1.3/python_esios.egg-info/PKG-INFO` & `python_esios-0.1.4/python_esios.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esios
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python wrapper for the ESIOS API
 Home-page: https://github.com/datons/python-esios
 Author: Jesús López
 Author-email: jesus.lopez@datons.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_esios-0.1.3/setup.py` & `python_esios-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 setup(
     name='python-esios',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'requests',
         'pandas',
     ],
     author="Jesús López",
     author_email="jesus.lopez@datons.ai",
```

