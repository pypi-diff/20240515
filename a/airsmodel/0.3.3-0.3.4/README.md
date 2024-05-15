# Comparing `tmp/airsmodel-0.3.3.tar.gz` & `tmp/airsmodel-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airsmodel-0.3.3.tar", last modified: Tue May 14 09:46:43 2024, max compression
+gzip compressed data, was "dist/airsmodel-0.3.4.tar", last modified: Wed May 15 08:00:25 2024, max compression
```

## Comparing `airsmodel-0.3.3.tar` & `airsmodel-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2024-05-14 09:46:43.000000 airsmodel-0.3.3/
--rw-r--r--   0 container  (1000) container  (1000)   281590 2024-05-14 09:46:43.000000 airsmodel-0.3.3/PKG-INFO
--rw-rw-r--   0 container  (1000) container  (1000)   246982 2024-05-14 09:46:42.000000 airsmodel-0.3.3/README.md
--rw-r--r--   0 container  (1000) container  (1000)       38 2024-05-14 09:46:43.000000 airsmodel-0.3.3/setup.cfg
--rw-rw-r--   0 container  (1000) container  (1000)      575 2024-05-14 09:46:42.000000 airsmodel-0.3.3/setup.py
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2024-05-14 09:46:43.000000 airsmodel-0.3.3/src/
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2024-05-14 09:46:43.000000 airsmodel-0.3.3/src/airs/
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2024-05-14 09:46:43.000000 airsmodel-0.3.3/src/airs/core/
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2024-05-14 09:46:43.000000 airsmodel-0.3.3/src/airs/core/models/
--rw-rw-r--   0 container  (1000) container  (1000)        0 2024-05-14 09:46:42.000000 airsmodel-0.3.3/src/airs/core/models/__init__.py
--rw-rw-r--   0 container  (1000) container  (1000)     3082 2024-05-14 09:46:42.000000 airsmodel-0.3.3/src/airs/core/models/mapper.py
--rw-rw-r--   0 container  (1000) container  (1000)    26093 2024-05-14 09:46:42.000000 airsmodel-0.3.3/src/airs/core/models/model.py
-drwxr-xr-x   0 container  (1000) container  (1000)        0 2024-05-14 09:46:43.000000 airsmodel-0.3.3/src/airsmodel.egg-info/
--rw-r--r--   0 container  (1000) container  (1000)   281590 2024-05-14 09:46:43.000000 airsmodel-0.3.3/src/airsmodel.egg-info/PKG-INFO
--rw-r--r--   0 container  (1000) container  (1000)      260 2024-05-14 09:46:43.000000 airsmodel-0.3.3/src/airsmodel.egg-info/SOURCES.txt
--rw-r--r--   0 container  (1000) container  (1000)        1 2024-05-14 09:46:43.000000 airsmodel-0.3.3/src/airsmodel.egg-info/dependency_links.txt
--rw-r--r--   0 container  (1000) container  (1000)        5 2024-05-14 09:46:43.000000 airsmodel-0.3.3/src/airsmodel.egg-info/top_level.txt
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2024-05-15 08:00:25.000000 airsmodel-0.3.4/
+-rw-r--r--   0 container  (1000) container  (1000)   281590 2024-05-15 08:00:25.000000 airsmodel-0.3.4/PKG-INFO
+-rw-rw-r--   0 container  (1000) container  (1000)   246982 2024-05-15 08:00:23.000000 airsmodel-0.3.4/README.md
+-rw-r--r--   0 container  (1000) container  (1000)       38 2024-05-15 08:00:25.000000 airsmodel-0.3.4/setup.cfg
+-rw-rw-r--   0 container  (1000) container  (1000)      575 2024-05-15 08:00:23.000000 airsmodel-0.3.4/setup.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2024-05-15 08:00:25.000000 airsmodel-0.3.4/src/
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2024-05-15 08:00:25.000000 airsmodel-0.3.4/src/airs/
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2024-05-15 08:00:25.000000 airsmodel-0.3.4/src/airs/core/
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2024-05-15 08:00:25.000000 airsmodel-0.3.4/src/airs/core/models/
+-rw-rw-r--   0 container  (1000) container  (1000)        0 2024-05-15 08:00:23.000000 airsmodel-0.3.4/src/airs/core/models/__init__.py
+-rw-rw-r--   0 container  (1000) container  (1000)     3082 2024-05-15 08:00:23.000000 airsmodel-0.3.4/src/airs/core/models/mapper.py
+-rw-rw-r--   0 container  (1000) container  (1000)    26093 2024-05-15 08:00:23.000000 airsmodel-0.3.4/src/airs/core/models/model.py
+drwxr-xr-x   0 container  (1000) container  (1000)        0 2024-05-15 08:00:25.000000 airsmodel-0.3.4/src/airsmodel.egg-info/
+-rw-r--r--   0 container  (1000) container  (1000)   281590 2024-05-15 08:00:25.000000 airsmodel-0.3.4/src/airsmodel.egg-info/PKG-INFO
+-rw-r--r--   0 container  (1000) container  (1000)      260 2024-05-15 08:00:25.000000 airsmodel-0.3.4/src/airsmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 container  (1000) container  (1000)        1 2024-05-15 08:00:25.000000 airsmodel-0.3.4/src/airsmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 container  (1000) container  (1000)        5 2024-05-15 08:00:25.000000 airsmodel-0.3.4/src/airsmodel.egg-info/top_level.txt
```

### Comparing `airsmodel-0.3.3/PKG-INFO` & `airsmodel-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airsmodel
-Version: 0.3.3
+Version: 0.3.4
 Summary: ARLAS Item Registration Service Model
 Home-page: UNKNOWN
 Author: Gisaïa
 License: UNKNOWN
 Description: # AIRS Model
         
         This package contains the data model for sending requests to ARLAS Item Registration Services.
```

### Comparing `airsmodel-0.3.3/README.md` & `airsmodel-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `airsmodel-0.3.3/setup.py` & `airsmodel-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="airsmodel",
-    version="0.3.3",                        
+    version="0.3.4",                        
     author="Gisaïa",                     
     description="ARLAS Item Registration Service Model",
     long_description=long_description,      
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    
     python_requires='>=3.11',     
     py_modules=["airs.core.models.model","airs.core.models.mapper"],
```

### Comparing `airsmodel-0.3.3/src/airs/core/models/mapper.py` & `airsmodel-0.3.4/src/airs/core/models/mapper.py`

 * *Files identical despite different names*

### Comparing `airsmodel-0.3.3/src/airs/core/models/model.py` & `airsmodel-0.3.4/src/airs/core/models/model.py`

 * *Files identical despite different names*

### Comparing `airsmodel-0.3.3/src/airsmodel.egg-info/PKG-INFO` & `airsmodel-0.3.4/src/airsmodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airsmodel
-Version: 0.3.3
+Version: 0.3.4
 Summary: ARLAS Item Registration Service Model
 Home-page: UNKNOWN
 Author: Gisaïa
 License: UNKNOWN
 Description: # AIRS Model
         
         This package contains the data model for sending requests to ARLAS Item Registration Services.
```

