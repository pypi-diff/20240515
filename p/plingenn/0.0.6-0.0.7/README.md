# Comparing `tmp/plingenn-0.0.6.tar.gz` & `tmp/plingenn-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plingenn-0.0.6.tar", last modified: Wed May 15 19:30:45 2024, max compression
+gzip compressed data, was "plingenn-0.0.7.tar", last modified: Wed May 15 19:41:41 2024, max compression
```

## Comparing `plingenn-0.0.6.tar` & `plingenn-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 19:30:45.871017 plingenn-0.0.6/
--rw-rw-rw-   0        0        0       71 2024-05-15 18:33:51.000000 plingenn-0.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1071 2024-05-15 18:35:13.000000 plingenn-0.0.6/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2024-05-15 18:34:21.000000 plingenn-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      646 2024-05-15 19:30:45.829190 plingenn-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 19:30:45.030900 plingenn-0.0.6/plingenn/
--rw-rw-rw-   0        0        0      112 2024-05-15 18:31:48.000000 plingenn-0.0.6/plingenn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 19:30:45.673497 plingenn-0.0.6/plingenn/plingenn.egg-info/
--rw-rw-rw-   0        0        0        0 2024-05-15 19:27:48.000000 plingenn-0.0.6/plingenn/plingenn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 19:27:48.000000 plingenn-0.0.6/plingenn/plingenn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 19:27:48.000000 plingenn-0.0.6/plingenn/plingenn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 19:27:48.000000 plingenn-0.0.6/plingenn/plingenn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 19:30:45.753261 plingenn-0.0.6/plingenn.egg-info/
--rw-rw-rw-   0        0        0      646 2024-05-15 19:30:44.000000 plingenn-0.0.6/plingenn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-05-15 19:30:44.000000 plingenn-0.0.6/plingenn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 19:30:44.000000 plingenn-0.0.6/plingenn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 19:30:44.000000 plingenn-0.0.6/plingenn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 19:30:44.000000 plingenn-0.0.6/plingenn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 19:30:45.871017 plingenn-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-15 19:30:30.000000 plingenn-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:41:41.539846 plingenn-0.0.7/
+-rw-rw-rw-   0        0        0       71 2024-05-15 18:33:51.000000 plingenn-0.0.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1071 2024-05-15 18:35:13.000000 plingenn-0.0.7/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-15 18:34:21.000000 plingenn-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      646 2024-05-15 19:41:41.498473 plingenn-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 19:41:40.800649 plingenn-0.0.7/plingenn/
+-rw-rw-rw-   0        0        0      912 2024-05-15 19:41:03.000000 plingenn-0.0.7/plingenn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:41:41.354613 plingenn-0.0.7/plingenn/plingenn.egg-info/
+-rw-rw-rw-   0        0        0        0 2024-05-15 19:27:48.000000 plingenn-0.0.7/plingenn/plingenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:27:48.000000 plingenn-0.0.7/plingenn/plingenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 19:27:48.000000 plingenn-0.0.7/plingenn/plingenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 19:27:48.000000 plingenn-0.0.7/plingenn/plingenn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 19:41:41.422287 plingenn-0.0.7/plingenn.egg-info/
+-rw-rw-rw-   0        0        0      646 2024-05-15 19:41:40.000000 plingenn-0.0.7/plingenn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-05-15 19:41:40.000000 plingenn-0.0.7/plingenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:41:40.000000 plingenn-0.0.7/plingenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 19:41:40.000000 plingenn-0.0.7/plingenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 19:41:40.000000 plingenn-0.0.7/plingenn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 19:41:41.540931 plingenn-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-15 19:41:34.000000 plingenn-0.0.7/setup.py
```

### Comparing `plingenn-0.0.6/LICENCE.txt` & `plingenn-0.0.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `plingenn-0.0.6/PKG-INFO` & `plingenn-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.6
+Version: 0.0.7
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plingenn-0.0.6/plingenn.egg-info/PKG-INFO` & `plingenn-0.0.7/plingenn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.6
+Version: 0.0.7
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plingenn-0.0.6/setup.py` & `plingenn-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='plingenn',
-    version='0.0.6',
+    version='0.0.7',
     description='A very basic package',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Plingenn Plingsson',
     author_email='Plingenn12@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

