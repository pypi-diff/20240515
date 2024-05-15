# Comparing `tmp/plingenn-0.0.1.tar.gz` & `tmp/plingenn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plingenn-0.0.1.tar", last modified: Wed May 15 18:48:39 2024, max compression
+gzip compressed data, was "plingenn-0.0.2.tar", last modified: Wed May 15 19:10:03 2024, max compression
```

## Comparing `plingenn-0.0.1.tar` & `plingenn-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 18:48:39.861851 plingenn-0.0.1/
--rw-rw-rw-   0        0        0       71 2024-05-15 18:33:51.000000 plingenn-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1071 2024-05-15 18:35:13.000000 plingenn-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2024-05-15 18:34:21.000000 plingenn-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      599 2024-05-15 18:48:39.819430 plingenn-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.1/README.txt
--rw-rw-rw-   0        0        0      112 2024-05-15 18:31:48.000000 plingenn-0.0.1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 18:48:39.743198 plingenn-0.0.1/plingenn.egg-info/
--rw-rw-rw-   0        0        0      599 2024-05-15 18:48:38.000000 plingenn-0.0.1/plingenn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-05-15 18:48:38.000000 plingenn-0.0.1/plingenn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 18:48:38.000000 plingenn-0.0.1/plingenn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 18:48:38.000000 plingenn-0.0.1/plingenn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 18:48:39.861851 plingenn-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      715 2024-05-15 18:48:18.000000 plingenn-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:10:03.601833 plingenn-0.0.2/
+-rw-rw-rw-   0        0        0       71 2024-05-15 18:33:51.000000 plingenn-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1071 2024-05-15 18:35:13.000000 plingenn-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-15 18:34:21.000000 plingenn-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      646 2024-05-15 19:10:03.558579 plingenn-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.2/README.txt
+-rw-rw-rw-   0        0        0      112 2024-05-15 18:31:48.000000 plingenn-0.0.2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:10:03.482523 plingenn-0.0.2/plingenn.egg-info/
+-rw-rw-rw-   0        0        0      646 2024-05-15 19:10:01.000000 plingenn-0.0.2/plingenn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2024-05-15 19:10:02.000000 plingenn-0.0.2/plingenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:10:02.000000 plingenn-0.0.2/plingenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 19:10:02.000000 plingenn-0.0.2/plingenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:10:02.000000 plingenn-0.0.2/plingenn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 19:10:03.602834 plingenn-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      732 2024-05-15 19:07:59.000000 plingenn-0.0.2/setup.py
```

### Comparing `plingenn-0.0.1/LICENCE.txt` & `plingenn-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `plingenn-0.0.1/PKG-INFO` & `plingenn-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.1
+Version: 0.0.2
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
-Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
+Requires-Dist: requests
+Requires-Dist: numpy
 
 This is a very simple library.
 
 Change Log
 ==========
 
 0.0.1 (Date)
```

### Comparing `plingenn-0.0.1/plingenn.egg-info/PKG-INFO` & `plingenn-0.0.2/plingenn.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.1
+Version: 0.0.2
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
-Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
+Requires-Dist: requests
+Requires-Dist: numpy
 
 This is a very simple library.
 
 Change Log
 ==========
 
 0.0.1 (Date)
```

