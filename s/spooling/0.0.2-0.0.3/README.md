# Comparing `tmp/spooling-0.0.2.tar.gz` & `tmp/spooling-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spooling-0.0.2.tar", last modified: Tue May 14 20:09:00 2024, max compression
+gzip compressed data, was "spooling-0.0.3.tar", last modified: Tue May 14 20:18:57 2024, max compression
```

## Comparing `spooling-0.0.2.tar` & `spooling-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 20:09:00.202671 spooling-0.0.2/
--rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 spooling-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 spooling-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 spooling-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      600 2024-05-14 20:09:00.201664 spooling-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       38 2024-05-14 19:52:48.000000 spooling-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 20:09:00.148670 spooling-0.0.2/daiexperiments/
--rw-rw-rw-   0        0        0      239 2024-05-14 20:08:49.000000 spooling-0.0.2/daiexperiments/__init__.py
--rw-rw-rw-   0        0        0    20539 2024-05-14 20:00:19.000000 spooling-0.0.2/daiexperiments/main.py
-drwxrwxrwx   0        0        0        0 2024-05-14 20:09:00.157669 spooling-0.0.2/daiexperiments.egg-info/
--rw-rw-rw-   0        0        0      393 2024-05-14 07:40:34.000000 spooling-0.0.2/daiexperiments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 07:40:34.000000 spooling-0.0.2/daiexperiments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-14 07:40:34.000000 spooling-0.0.2/daiexperiments.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 20:09:00.164669 spooling-0.0.2/ishandaiexperiments.egg-info/
--rw-rw-rw-   0        0        0      289 2024-05-13 20:00:47.000000 spooling-0.0.2/ishandaiexperiments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 20:00:47.000000 spooling-0.0.2/ishandaiexperiments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-13 20:00:47.000000 spooling-0.0.2/ishandaiexperiments.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 20:09:00.172711 spooling-0.0.2/pooLing.egg-info/
--rw-rw-rw-   0        0        0      484 2024-05-14 20:00:32.000000 spooling-0.0.2/pooLing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 20:00:32.000000 spooling-0.0.2/pooLing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-14 20:00:32.000000 spooling-0.0.2/pooLing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 20:09:00.203667 spooling-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      701 2024-05-14 20:08:54.000000 spooling-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 20:09:00.199666 spooling-0.0.2/spooling.egg-info/
--rw-rw-rw-   0        0        0      600 2024-05-14 20:08:59.000000 spooling-0.0.2/spooling.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2024-05-14 20:09:00.000000 spooling-0.0.2/spooling.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 20:08:59.000000 spooling-0.0.2/spooling.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-14 20:08:59.000000 spooling-0.0.2/spooling.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 20:18:57.830631 spooling-0.0.3/
+-rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 spooling-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 spooling-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 spooling-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      600 2024-05-14 20:18:57.829631 spooling-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2024-05-14 19:52:48.000000 spooling-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 20:18:57.775631 spooling-0.0.3/daiexperiments.egg-info/
+-rw-rw-rw-   0        0        0      393 2024-05-14 07:40:34.000000 spooling-0.0.3/daiexperiments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 07:40:34.000000 spooling-0.0.3/daiexperiments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 07:40:34.000000 spooling-0.0.3/daiexperiments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 20:18:57.781636 spooling-0.0.3/ishandaiexperiments.egg-info/
+-rw-rw-rw-   0        0        0      289 2024-05-13 20:00:47.000000 spooling-0.0.3/ishandaiexperiments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 20:00:47.000000 spooling-0.0.3/ishandaiexperiments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-13 20:00:47.000000 spooling-0.0.3/ishandaiexperiments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 20:18:57.790631 spooling-0.0.3/pooLing.egg-info/
+-rw-rw-rw-   0        0        0      484 2024-05-14 20:00:32.000000 spooling-0.0.3/pooLing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 20:00:32.000000 spooling-0.0.3/pooLing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 20:00:32.000000 spooling-0.0.3/pooLing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 20:18:57.830631 spooling-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      701 2024-05-14 20:18:52.000000 spooling-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:18:57.794670 spooling-0.0.3/spooling/
+-rw-rw-rw-   0        0        0      239 2024-05-14 20:17:25.000000 spooling-0.0.3/spooling/__init__.py
+-rw-rw-rw-   0        0        0    20539 2024-05-14 20:00:19.000000 spooling-0.0.3/spooling/main.py
+drwxrwxrwx   0        0        0        0 2024-05-14 20:18:57.827636 spooling-0.0.3/spooling.egg-info/
+-rw-rw-rw-   0        0        0      600 2024-05-14 20:18:57.000000 spooling-0.0.3/spooling.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2024-05-14 20:18:57.000000 spooling-0.0.3/spooling.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 20:18:57.000000 spooling-0.0.3/spooling.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-14 20:18:57.000000 spooling-0.0.3/spooling.egg-info/top_level.txt
```

### Comparing `spooling-0.0.2/LICENSE.txt` & `spooling-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spooling-0.0.2/PKG-INFO` & `spooling-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spooling
-Version: 0.0.2
+Version: 0.0.3
 Summary: rl experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spooling-0.0.2/daiexperiments/main.py` & `spooling-0.0.3/spooling/main.py`

 * *Files identical despite different names*

### Comparing `spooling-0.0.2/setup.py` & `spooling-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='spooling',
-  version='0.0.2',
+  version='0.0.3',
   description='rl experiments',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='S Ishan',
   author_email='is9678@srmist.edu.in',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `spooling-0.0.2/spooling.egg-info/PKG-INFO` & `spooling-0.0.3/spooling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spooling
-Version: 0.0.2
+Version: 0.0.3
 Summary: rl experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

