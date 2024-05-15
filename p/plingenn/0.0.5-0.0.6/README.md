# Comparing `tmp/plingenn-0.0.5.tar.gz` & `tmp/plingenn-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plingenn-0.0.5.tar", last modified: Wed May 15 19:26:16 2024, max compression
+gzip compressed data, was "plingenn-0.0.6.tar", last modified: Wed May 15 19:30:45 2024, max compression
```

## Comparing `plingenn-0.0.5.tar` & `plingenn-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 19:26:15.994796 plingenn-0.0.5/
--rw-rw-rw-   0        0        0      619 2024-05-15 19:26:15.954831 plingenn-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 19:26:15.390586 plingenn-0.0.5/plingenn/
--rw-rw-rw-   0        0        0      112 2024-05-15 18:31:48.000000 plingenn-0.0.5/plingenn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 19:26:15.877003 plingenn-0.0.5/plingenn.egg-info/
--rw-rw-rw-   0        0        0      619 2024-05-15 19:26:14.000000 plingenn-0.0.5/plingenn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2024-05-15 19:26:15.000000 plingenn-0.0.5/plingenn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 19:26:15.000000 plingenn-0.0.5/plingenn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 19:26:15.000000 plingenn-0.0.5/plingenn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 19:26:15.000000 plingenn-0.0.5/plingenn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 19:26:15.995795 plingenn-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-15 19:25:56.000000 plingenn-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:30:45.871017 plingenn-0.0.6/
+-rw-rw-rw-   0        0        0       71 2024-05-15 18:33:51.000000 plingenn-0.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1071 2024-05-15 18:35:13.000000 plingenn-0.0.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-15 18:34:21.000000 plingenn-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      646 2024-05-15 19:30:45.829190 plingenn-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 19:30:45.030900 plingenn-0.0.6/plingenn/
+-rw-rw-rw-   0        0        0      112 2024-05-15 18:31:48.000000 plingenn-0.0.6/plingenn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:30:45.673497 plingenn-0.0.6/plingenn/plingenn.egg-info/
+-rw-rw-rw-   0        0        0        0 2024-05-15 19:27:48.000000 plingenn-0.0.6/plingenn/plingenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:27:48.000000 plingenn-0.0.6/plingenn/plingenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 19:27:48.000000 plingenn-0.0.6/plingenn/plingenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 19:27:48.000000 plingenn-0.0.6/plingenn/plingenn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 19:30:45.753261 plingenn-0.0.6/plingenn.egg-info/
+-rw-rw-rw-   0        0        0      646 2024-05-15 19:30:44.000000 plingenn-0.0.6/plingenn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-05-15 19:30:44.000000 plingenn-0.0.6/plingenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:30:44.000000 plingenn-0.0.6/plingenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 19:30:44.000000 plingenn-0.0.6/plingenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 19:30:44.000000 plingenn-0.0.6/plingenn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 19:30:45.871017 plingenn-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-15 19:30:30.000000 plingenn-0.0.6/setup.py
```

### Comparing `plingenn-0.0.5/PKG-INFO` & `plingenn-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.5
+Version: 0.0.6
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+License-File: LICENCE.txt
 Requires-Dist: requests
 Requires-Dist: numpy
 
 This is a very simple library.
 
 Change Log
 ==========
```

### Comparing `plingenn-0.0.5/plingenn.egg-info/PKG-INFO` & `plingenn-0.0.6/plingenn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.5
+Version: 0.0.6
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+License-File: LICENCE.txt
 Requires-Dist: requests
 Requires-Dist: numpy
 
 This is a very simple library.
 
 Change Log
 ==========
```

