# Comparing `tmp/meapy-0.0.8.tar.gz` & `tmp/meapy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\meapy-0.0.8.tar", last modified: Thu Nov 12 17:32:46 2020, max compression
+gzip compressed data, was "dist\meapy-0.0.9.tar", last modified: Fri Nov 13 05:06:44 2020, max compression
```

## Comparing `meapy-0.0.8.tar` & `meapy-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2020-11-12 17:32:46.346374 meapy-0.0.8/
--rw-rw-rw-   0        0        0     4196 2020-11-12 17:32:46.346374 meapy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2402 2020-11-12 17:09:01.000000 meapy-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2020-11-12 17:32:46.323375 meapy-0.0.8/meapy/
--rw-rw-rw-   0        0        0      302 2020-03-25 08:49:25.000000 meapy-0.0.8/meapy/__init__.py
--rw-rw-rw-   0        0        0     1202 2020-10-24 09:14:39.000000 meapy-0.0.8/meapy/loadingconfig.py
--rw-rw-rw-   0        0        0    10139 2020-11-12 17:01:12.000000 meapy-0.0.8/meapy/meapy.py
--rw-rw-rw-   0        0        0      605 2020-10-24 09:14:39.000000 meapy-0.0.8/meapy/measurement.py
--rw-rw-rw-   0        0        0      585 2020-10-24 09:14:39.000000 meapy-0.0.8/meapy/measurementlist.py
--rw-rw-rw-   0        0        0      665 2020-11-12 17:27:38.000000 meapy-0.0.8/meapy/signaldata.py
-drwxrwxrwx   0        0        0        0 2020-11-12 17:32:46.345374 meapy-0.0.8/meapy.egg-info/
--rw-rw-rw-   0        0        0     4196 2020-11-12 17:32:45.000000 meapy-0.0.8/meapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2020-11-12 17:32:46.000000 meapy-0.0.8/meapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-11-12 17:32:45.000000 meapy-0.0.8/meapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-03-25 13:51:47.000000 meapy-0.0.8/meapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2020-11-12 17:32:45.000000 meapy-0.0.8/meapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2020-11-12 17:32:45.000000 meapy-0.0.8/meapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2020-11-12 17:32:46.352374 meapy-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1467 2020-11-12 17:32:16.000000 meapy-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-11-13 05:06:44.379062 meapy-0.0.9/
+-rw-rw-rw-   0        0        0     4196 2020-11-13 05:06:44.379062 meapy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2402 2020-11-12 17:09:01.000000 meapy-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2020-11-13 05:06:44.357062 meapy-0.0.9/meapy/
+-rw-rw-rw-   0        0        0      302 2020-03-25 08:49:25.000000 meapy-0.0.9/meapy/__init__.py
+-rw-rw-rw-   0        0        0     1202 2020-10-24 09:14:39.000000 meapy-0.0.9/meapy/loadingconfig.py
+-rw-rw-rw-   0        0        0    10254 2020-11-13 05:04:45.000000 meapy-0.0.9/meapy/meapy.py
+-rw-rw-rw-   0        0        0      605 2020-10-24 09:14:39.000000 meapy-0.0.9/meapy/measurement.py
+-rw-rw-rw-   0        0        0      585 2020-10-24 09:14:39.000000 meapy-0.0.9/meapy/measurementlist.py
+-rw-rw-rw-   0        0        0      665 2020-11-12 17:27:38.000000 meapy-0.0.9/meapy/signaldata.py
+drwxrwxrwx   0        0        0        0 2020-11-13 05:06:44.378062 meapy-0.0.9/meapy.egg-info/
+-rw-rw-rw-   0        0        0     4196 2020-11-13 05:06:44.000000 meapy-0.0.9/meapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2020-11-13 05:06:44.000000 meapy-0.0.9/meapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-11-13 05:06:44.000000 meapy-0.0.9/meapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-03-25 13:51:47.000000 meapy-0.0.9/meapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2020-11-13 05:06:44.000000 meapy-0.0.9/meapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2020-11-13 05:06:44.000000 meapy-0.0.9/meapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2020-11-13 05:06:44.381062 meapy-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1467 2020-11-13 05:05:58.000000 meapy-0.0.9/setup.py
```

### Comparing `meapy-0.0.8/PKG-INFO` & `meapy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meapy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python API Wrapper for Measurement Data
 Home-page: https://bitbucket.chemnitz.kistler.com/projects/MDM/repos/meapy
 Author: Philipp Oehme
 Author-email: philipp.oehme@kistler.com
 License: UNKNOWN
 Download-URL: https://pypi.python.org/pypi/meapy
 Description: ![PyPI](https://img.shields.io/pypi/v/meapy?style=flat-square)
```

### Comparing `meapy-0.0.8/README.md` & `meapy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `meapy-0.0.8/meapy/loadingconfig.py` & `meapy-0.0.9/meapy/loadingconfig.py`

 * *Files identical despite different names*

### Comparing `meapy-0.0.8/meapy/meapy.py` & `meapy-0.0.9/meapy/meapy.py`

 * *Files 10% similar despite different names*

```diff
@@ -203,15 +203,15 @@
             if responseJson.get('errorId') is not None:
                 raise Exception(responseJson.get('errorId')+': ' +
                                 responseJson.get('localizedErrorMessage'))
             return False
 
         return True
 
-    def upload(self, filename: str, df: pd.DataFrame, metadata: dict = {}) -> bool:
+    def upload(self, filename: str, df: pd.DataFrame, metadata: dict = {}, testType: str = 'Test') -> bool:
         """Uploads a file as a new measurement together with the given metadata
 
         Parameters
         ----------
         file : str
             Path to the file which should be uploaded
         metadata : dict
@@ -220,32 +220,31 @@
         Returns
         -------
         bool
             Signals if the upload was successful
         """
 
         outputFilename = filename + '.csv'
-        df.to_csv(outputFilename)
+        fileContent = df.to_csv()
         dataObjects = []
 
         # get columns and generate DO
         for col in list(df):
             _id = str(uuid.uuid4())
             dataObjects.append({
                 'type': 'DataObject',
                 'id': _id,
                 'fields': {
                     'Type': 'DataObject',
                     'Id': _id,
                     'Name': col,
-                    'DataType': 802,
-                    'Maximum': float(df[col].max()),
-                    'Minimum': float(df[col].min()),
-                    'Average': float(df[col].sum() / df[col].count()),
-                    'StandardDeviation': float(df[col].std())
+                    'Maximum': df[col].max().astype(float) if pd.api.types.is_numeric_dtype(df[col]) else None,
+                    'Minimum': df[col].min().astype(float) if pd.api.types.is_numeric_dtype(df[col]) else None,
+                    'Average': df[col].mean() if pd.api.types.is_numeric_dtype(df[col]) else None,
+                    'StandardDeviation': df[col].std() if pd.api.types.is_numeric_dtype(df[col]) else None
                 }
             })
 
         dataObjectRefs = []
         for do in dataObjects:
             dataObjectRefs.append({
                 'type': 'DataObject',
@@ -259,31 +258,30 @@
             'relativePath': outputFilename,
             'originalFileName': outputFilename
         }
 
         testId = str(uuid.uuid4())
 
         data = {
-            'Type': 'Test',
+            'Type': testType,
             'Id': testId,
             'DataObjects': dataObjectRefs,
-            'Owner': 'MaDaM_DemoUser',
-            'Name': 'generated test by Meapy',
+            'Name': outputFilename,
             'MainFile': [fileRef],
             'MeasurementData': [fileRef],
             'SourcePath': 'meapy/'+outputFilename
         }
 
         data.update(metadata)
 
         filesToUpload = {}
-        filesToUpload[uploadId] = (outputFilename, open(outputFilename, 'rb'), 'text/csv')
+        filesToUpload[uploadId] = (outputFilename, fileContent, 'text/csv')
 
         docs = dataObjects
         measurementDto = {
-            'type': 'Test',
+            'type': testType,
             'id': testId,
             'fields': data
         }
         status = self.update(Measurement(measurementDto), data, filesToUpload, docs)
 
         return status
```

### Comparing `meapy-0.0.8/meapy/measurement.py` & `meapy-0.0.9/meapy/measurement.py`

 * *Files identical despite different names*

### Comparing `meapy-0.0.8/meapy/measurementlist.py` & `meapy-0.0.9/meapy/measurementlist.py`

 * *Files identical despite different names*

### Comparing `meapy-0.0.8/meapy/signaldata.py` & `meapy-0.0.9/meapy/signaldata.py`

 * *Files identical despite different names*

### Comparing `meapy-0.0.8/meapy.egg-info/PKG-INFO` & `meapy-0.0.9/meapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meapy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python API Wrapper for Measurement Data
 Home-page: https://bitbucket.chemnitz.kistler.com/projects/MDM/repos/meapy
 Author: Philipp Oehme
 Author-email: philipp.oehme@kistler.com
 License: UNKNOWN
 Download-URL: https://pypi.python.org/pypi/meapy
 Description: ![PyPI](https://img.shields.io/pypi/v/meapy?style=flat-square)
```

### Comparing `meapy-0.0.8/setup.py` & `meapy-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='meapy',
-      version='0.0.8',
+      version='0.0.9',
       description='Python API Wrapper for Measurement Data',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       url='https://bitbucket.chemnitz.kistler.com/projects/MDM/repos/meapy',
       author='Philipp Oehme',
       author_email='philipp.oehme@kistler.com',
       download_url="https://pypi.python.org/pypi/meapy",
```

