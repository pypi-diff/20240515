# Comparing `tmp/plingenn-0.0.4.tar.gz` & `tmp/plingenn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plingenn-0.0.4.tar", last modified: Wed May 15 19:24:05 2024, max compression
+gzip compressed data, was "plingenn-0.0.5.tar", last modified: Wed May 15 19:26:16 2024, max compression
```

## Comparing `plingenn-0.0.4.tar` & `plingenn-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 19:24:05.512448 plingenn-0.0.4/
--rw-rw-rw-   0        0        0      619 2024-05-15 19:24:05.472434 plingenn-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.4/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 19:24:04.953518 plingenn-0.0.4/plingenn/
--rw-rw-rw-   0        0        0      112 2024-05-15 18:31:48.000000 plingenn-0.0.4/plingenn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 19:24:05.407064 plingenn-0.0.4/plingenn.egg-info/
--rw-rw-rw-   0        0        0      619 2024-05-15 19:24:03.000000 plingenn-0.0.4/plingenn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2024-05-15 19:24:04.000000 plingenn-0.0.4/plingenn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 19:24:04.000000 plingenn-0.0.4/plingenn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 19:24:04.000000 plingenn-0.0.4/plingenn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 19:24:04.000000 plingenn-0.0.4/plingenn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 19:24:05.513449 plingenn-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-15 19:23:57.000000 plingenn-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:26:15.994796 plingenn-0.0.5/
+-rw-rw-rw-   0        0        0      619 2024-05-15 19:26:15.954831 plingenn-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.5/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 19:26:15.390586 plingenn-0.0.5/plingenn/
+-rw-rw-rw-   0        0        0      112 2024-05-15 18:31:48.000000 plingenn-0.0.5/plingenn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:26:15.877003 plingenn-0.0.5/plingenn.egg-info/
+-rw-rw-rw-   0        0        0      619 2024-05-15 19:26:14.000000 plingenn-0.0.5/plingenn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2024-05-15 19:26:15.000000 plingenn-0.0.5/plingenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:26:15.000000 plingenn-0.0.5/plingenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 19:26:15.000000 plingenn-0.0.5/plingenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 19:26:15.000000 plingenn-0.0.5/plingenn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 19:26:15.995795 plingenn-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-15 19:25:56.000000 plingenn-0.0.5/setup.py
```

### Comparing `plingenn-0.0.4/PKG-INFO` & `plingenn-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.4
+Version: 0.0.5
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plingenn-0.0.4/plingenn.egg-info/PKG-INFO` & `plingenn-0.0.5/plingenn.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.4
+Version: 0.0.5
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plingenn-0.0.4/setup.py` & `plingenn-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='plingenn',
-    version='0.0.4',
+    version='0.0.5',
     description='A very basic package',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Plingenn Plingsson',
     author_email='Plingenn12@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

