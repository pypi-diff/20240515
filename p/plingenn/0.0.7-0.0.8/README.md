# Comparing `tmp/plingenn-0.0.7.tar.gz` & `tmp/plingenn-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plingenn-0.0.7.tar", last modified: Wed May 15 19:41:41 2024, max compression
+gzip compressed data, was "plingenn-0.0.8.tar", last modified: Wed May 15 19:53:26 2024, max compression
```

## Comparing `plingenn-0.0.7.tar` & `plingenn-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 19:41:41.539846 plingenn-0.0.7/
--rw-rw-rw-   0        0        0       71 2024-05-15 18:33:51.000000 plingenn-0.0.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1071 2024-05-15 18:35:13.000000 plingenn-0.0.7/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2024-05-15 18:34:21.000000 plingenn-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      646 2024-05-15 19:41:41.498473 plingenn-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.7/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 19:41:40.800649 plingenn-0.0.7/plingenn/
--rw-rw-rw-   0        0        0      912 2024-05-15 19:41:03.000000 plingenn-0.0.7/plingenn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 19:41:41.354613 plingenn-0.0.7/plingenn/plingenn.egg-info/
--rw-rw-rw-   0        0        0        0 2024-05-15 19:27:48.000000 plingenn-0.0.7/plingenn/plingenn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 19:27:48.000000 plingenn-0.0.7/plingenn/plingenn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 19:27:48.000000 plingenn-0.0.7/plingenn/plingenn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 19:27:48.000000 plingenn-0.0.7/plingenn/plingenn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 19:41:41.422287 plingenn-0.0.7/plingenn.egg-info/
--rw-rw-rw-   0        0        0      646 2024-05-15 19:41:40.000000 plingenn-0.0.7/plingenn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-05-15 19:41:40.000000 plingenn-0.0.7/plingenn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 19:41:40.000000 plingenn-0.0.7/plingenn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 19:41:40.000000 plingenn-0.0.7/plingenn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 19:41:40.000000 plingenn-0.0.7/plingenn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 19:41:41.540931 plingenn-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-15 19:41:34.000000 plingenn-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:53:26.704702 plingenn-0.0.8/
+-rw-rw-rw-   0        0        0       71 2024-05-15 18:33:51.000000 plingenn-0.0.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1071 2024-05-15 18:35:13.000000 plingenn-0.0.8/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-15 18:34:21.000000 plingenn-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      646 2024-05-15 19:53:26.662757 plingenn-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.8/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 19:53:25.944435 plingenn-0.0.8/plingenn/
+-rw-rw-rw-   0        0        0     1705 2024-05-15 19:52:19.000000 plingenn-0.0.8/plingenn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:53:26.519026 plingenn-0.0.8/plingenn/plingenn.egg-info/
+-rw-rw-rw-   0        0        0        0 2024-05-15 19:27:48.000000 plingenn-0.0.8/plingenn/plingenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:27:48.000000 plingenn-0.0.8/plingenn/plingenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 19:27:48.000000 plingenn-0.0.8/plingenn/plingenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 19:27:48.000000 plingenn-0.0.8/plingenn/plingenn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 19:53:26.597178 plingenn-0.0.8/plingenn.egg-info/
+-rw-rw-rw-   0        0        0      646 2024-05-15 19:53:25.000000 plingenn-0.0.8/plingenn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-05-15 19:53:25.000000 plingenn-0.0.8/plingenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:53:25.000000 plingenn-0.0.8/plingenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 19:53:25.000000 plingenn-0.0.8/plingenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 19:53:25.000000 plingenn-0.0.8/plingenn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 19:53:26.704702 plingenn-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-15 19:52:58.000000 plingenn-0.0.8/setup.py
```

### Comparing `plingenn-0.0.7/LICENCE.txt` & `plingenn-0.0.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `plingenn-0.0.7/PKG-INFO` & `plingenn-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.7
+Version: 0.0.8
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plingenn-0.0.7/plingenn.egg-info/PKG-INFO` & `plingenn-0.0.8/plingenn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.7
+Version: 0.0.8
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plingenn-0.0.7/setup.py` & `plingenn-0.0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='plingenn',
-    version='0.0.7',
+    version='0.0.8',
     description='A very basic package',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Plingenn Plingsson',
     author_email='Plingenn12@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

