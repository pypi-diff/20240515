# Comparing `tmp/oeel-0.9.8.6.tar.gz` & `tmp/oeel-0.9.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oeel-0.9.8.6.tar", last modified: Sat Sep 23 18:34:08 2023, max compression
+gzip compressed data, was "oeel-0.9.8.7.tar", last modified: Wed May 15 08:03:34 2024, max compression
```

## Comparing `oeel-0.9.8.6.tar` & `oeel-0.9.8.7.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 18:34:08.100921 oeel-0.9.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35146 2023-09-23 18:33:59.000000 oeel-0.9.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-09-23 18:34:08.100921 oeel-0.9.8.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 18:34:08.100921 oeel-0.9.8.6/oeel/
--rw-r--r--   0 runner    (1001) docker     (127)     9339 2023-09-23 18:33:59.000000 oeel-0.9.8.6/oeel/EE_node_server.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 18:33:59.000000 oeel-0.9.8.6/oeel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-09-23 18:33:59.000000 oeel-0.9.8.6/oeel/colab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2023-09-23 18:33:59.000000 oeel-0.9.8.6/oeel/external.py
--rw-r--r--   0 runner    (1001) docker     (127)    10984 2023-09-23 18:33:59.000000 oeel-0.9.8.6/oeel/oeel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 18:34:08.100921 oeel-0.9.8.6/oeel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-09-23 18:34:08.000000 oeel-0.9.8.6/oeel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-09-23 18:34:08.000000 oeel-0.9.8.6/oeel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-23 18:34:08.000000 oeel-0.9.8.6/oeel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-23 18:34:08.000000 oeel-0.9.8.6/oeel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-09-23 18:34:08.000000 oeel-0.9.8.6/oeel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-23 18:34:08.100921 oeel-0.9.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-09-23 18:33:59.000000 oeel-0.9.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:03:34.672004 oeel-0.9.8.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-05-15 08:03:28.000000 oeel-0.9.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-15 08:03:34.672004 oeel-0.9.8.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:03:34.672004 oeel-0.9.8.7/oeel/
+-rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-15 08:03:28.000000 oeel-0.9.8.7/oeel/EE_node_server.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:03:28.000000 oeel-0.9.8.7/oeel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-15 08:03:28.000000 oeel-0.9.8.7/oeel/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-05-15 08:03:28.000000 oeel-0.9.8.7/oeel/oeel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:03:34.672004 oeel-0.9.8.7/oeel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-15 08:03:34.000000 oeel-0.9.8.7/oeel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 08:03:34.000000 oeel-0.9.8.7/oeel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:03:34.000000 oeel-0.9.8.7/oeel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 08:03:34.000000 oeel-0.9.8.7/oeel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 08:03:34.000000 oeel-0.9.8.7/oeel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:03:34.672004 oeel-0.9.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-15 08:03:28.000000 oeel-0.9.8.7/setup.py
```

### Comparing `oeel-0.9.8.6/LICENSE` & `oeel-0.9.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oeel-0.9.8.6/PKG-INFO` & `oeel-0.9.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oeel
-Version: 0.9.8.6
+Version: 0.9.8.7
 Summary: The Open Earth Engine Library Python interface
 Home-page: https://www.open-geocomputing.org/OpenEarthEngineLibrary/
 Author: Mathieu Gravey
 Author-email: research@mgravey.com
 License: GPLv3
 Keywords: Earth Engine,OEEL,Open Earth Engine Library
 Platform: UNKNOWN
```

### Comparing `oeel-0.9.8.6/oeel/EE_node_server.js` & `oeel-0.9.8.7/oeel/EE_node_server.js`

 * *Files identical despite different names*

### Comparing `oeel-0.9.8.6/oeel/external.py` & `oeel-0.9.8.7/oeel/external.py`

 * *Files identical despite different names*

### Comparing `oeel-0.9.8.6/oeel/oeel.py` & `oeel-0.9.8.7/oeel/oeel.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,19 @@
 import time
 import inspect
 import types
 import ctypes
 from shutil import which
 
 from . import external
-from . import colab
 oeelLibPath=os.path.dirname(__file__)
 
 class oeelMissingExternalCommand(Exception):
 		pass
 
-import sys
-IN_COLAB = 'google.colab' in sys.modules
-if IN_COLAB:
-	from . import colab
-
 def initialize():
 	if(os.path.exists(oeelLibPath+'/initialized')):
 		subprocess.Popen(['git', 'pull'], cwd=oeelLibPath+'/OEEL',stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 		if(os.path.getmtime(oeelLibPath+'/initialized')<os.path.getmtime(__file__)): # updated
 			os.remove(oeelLibPath+'/initialized')
 			initialize();
 		return
```

### Comparing `oeel-0.9.8.6/oeel.egg-info/PKG-INFO` & `oeel-0.9.8.7/oeel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oeel
-Version: 0.9.8.6
+Version: 0.9.8.7
 Summary: The Open Earth Engine Library Python interface
 Home-page: https://www.open-geocomputing.org/OpenEarthEngineLibrary/
 Author: Mathieu Gravey
 Author-email: research@mgravey.com
 License: GPLv3
 Keywords: Earth Engine,OEEL,Open Earth Engine Library
 Platform: UNKNOWN
```

### Comparing `oeel-0.9.8.6/setup.py` & `oeel-0.9.8.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='oeel',
-    version='0.9.8.6',
+    version='0.9.8.7',
     author='Mathieu Gravey',
     author_email='research@mgravey.com',
     url='https://www.open-geocomputing.org/OpenEarthEngineLibrary/',
     description='The Open Earth Engine Library Python interface',
     long_description='Python interface for the OpenEarthEngineLibrary and JS Earth Engine code.',
     classifiers=['Development Status :: 3 - Alpha','License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)','Programming Language :: Python :: 3','Programming Language :: JavaScript','Topic :: Scientific/Engineering :: GIS'],
     packages=['oeel'],
```

