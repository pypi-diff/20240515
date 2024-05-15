# Comparing `tmp/lusid_express-1.1.7.tar.gz` & `tmp/lusid_express-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-1.1.7.tar", last modified: Wed May  8 16:47:49 2024, max compression
+gzip compressed data, was "lusid_express-1.1.8.tar", last modified: Wed May 15 14:31:34 2024, max compression
```

## Comparing `lusid_express-1.1.7.tar` & `lusid_express-1.1.8.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:47:49.265409 lusid_express-1.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-08 16:47:03.000000 lusid_express-1.1.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-08 16:47:03.000000 lusid_express-1.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8202 2024-05-08 16:47:49.264409 lusid_express-1.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7562 2024-05-08 16:47:03.000000 lusid_express-1.1.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 16:47:49.265409 lusid_express-1.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-08 16:47:03.000000 lusid_express-1.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:47:49.259409 lusid_express-1.1.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:47:49.261409 lusid_express-1.1.7/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-08 16:47:03.000000 lusid_express-1.1.7/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5913 2024-05-08 16:47:03.000000 lusid_express-1.1.7/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:47:49.262409 lusid_express-1.1.7/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-05-08 16:47:48.000000 lusid_express-1.1.7/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:47:49.264409 lusid_express-1.1.7/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-08 16:47:03.000000 lusid_express-1.1.7/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:47:49.264409 lusid_express-1.1.7/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-08 16:47:03.000000 lusid_express-1.1.7/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)    11360 2024-05-08 16:47:03.000000 lusid_express-1.1.7/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3157 2024-05-08 16:47:03.000000 lusid_express-1.1.7/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:47:49.264409 lusid_express-1.1.7/src/lusid_express/utils/
--rw-rw-rw-   0 root         (0) root         (0)     2172 2024-05-08 16:47:03.000000 lusid_express-1.1.7/src/lusid_express/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:47:49.262409 lusid_express-1.1.7/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8202 2024-05-08 16:47:49.000000 lusid_express-1.1.7/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      518 2024-05-08 16:47:49.000000 lusid_express-1.1.7/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 16:47:49.000000 lusid_express-1.1.7/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-08 16:47:49.000000 lusid_express-1.1.7/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-08 16:47:49.000000 lusid_express-1.1.7/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.243222 lusid_express-1.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-15 14:30:45.000000 lusid_express-1.1.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-15 14:30:45.000000 lusid_express-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8202 2024-05-15 14:31:34.242222 lusid_express-1.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7562 2024-05-15 14:30:45.000000 lusid_express-1.1.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 14:31:34.243222 lusid_express-1.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-15 14:30:45.000000 lusid_express-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.235222 lusid_express-1.1.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.237222 lusid_express-1.1.8/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5913 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.238222 lusid_express-1.1.8/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-05-15 14:31:33.000000 lusid_express-1.1.8/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.241222 lusid_express-1.1.8/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.242222 lusid_express-1.1.8/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3157 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.242222 lusid_express-1.1.8/src/lusid_express/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     2172 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.242222 lusid_express-1.1.8/src/lusid_express/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     7731 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.238222 lusid_express-1.1.8/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8202 2024-05-15 14:31:34.000000 lusid_express-1.1.8/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2024-05-15 14:31:34.000000 lusid_express-1.1.8/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 14:31:34.000000 lusid_express-1.1.8/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-15 14:31:34.000000 lusid_express-1.1.8/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-15 14:31:34.000000 lusid_express-1.1.8/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-1.1.7/LICENSE` & `lusid_express-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.7/PKG-INFO` & `lusid_express-1.1.8/src/lusid_express.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lusid_express
-Version: 1.1.7
+Name: lusid-express
+Version: 1.1.8
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-1.1.7/README.md` & `lusid_express-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.7/setup.py` & `lusid_express-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='1.1.7',
+    version='1.1.8',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-1.1.7/src/lusid_express/__main__.py` & `lusid_express-1.1.8/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.7/src/lusid_express/apis/__init__.py` & `lusid_express-1.1.8/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.7/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-1.1.8/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.7/src/lusid_express/display/__init__.py` & `lusid_express-1.1.8/src/lusid_express/display/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.7/src/lusid_express/load.le` & `lusid_express-1.1.8/src/lusid_express/load.le`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.7/src/lusid_express/utils/__init__.py` & `lusid_express-1.1.8/src/lusid_express/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.7/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lusid-express
-Version: 1.1.7
+Name: lusid_express
+Version: 1.1.8
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-1.1.7/src/lusid_express.egg-info/SOURCES.txt` & `lusid_express-1.1.8/src/lusid_express.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 src/lusid_express.egg-info/dependency_links.txt
 src/lusid_express.egg-info/requires.txt
 src/lusid_express.egg-info/top_level.txt
 src/lusid_express/apis/__init__.py
 src/lusid_express/config/__init__.py
 src/lusid_express/display/PRELOADED_VARS.md
 src/lusid_express/display/__init__.py
-src/lusid_express/utils/__init__.py
+src/lusid_express/utils/__init__.py
+src/lusid_express/widgets/__init__.py
```

