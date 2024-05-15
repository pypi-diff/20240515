# Comparing `tmp/plingenn-0.0.3.tar.gz` & `tmp/plingenn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plingenn-0.0.3.tar", last modified: Wed May 15 19:20:19 2024, max compression
+gzip compressed data, was "plingenn-0.0.4.tar", last modified: Wed May 15 19:24:05 2024, max compression
```

## Comparing `plingenn-0.0.3.tar` & `plingenn-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 19:20:19.158379 plingenn-0.0.3/
--rw-rw-rw-   0        0        0      619 2024-05-15 19:20:19.117649 plingenn-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 19:20:18.536783 plingenn-0.0.3/plingenn/
--rw-rw-rw-   0        0        0      112 2024-05-15 18:31:48.000000 plingenn-0.0.3/plingenn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 19:20:19.041118 plingenn-0.0.3/plingenn.egg-info/
--rw-rw-rw-   0        0        0      619 2024-05-15 19:20:17.000000 plingenn-0.0.3/plingenn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-15 19:20:18.000000 plingenn-0.0.3/plingenn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 19:20:17.000000 plingenn-0.0.3/plingenn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 19:20:18.000000 plingenn-0.0.3/plingenn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 19:20:18.000000 plingenn-0.0.3/plingenn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 19:20:19.159891 plingenn-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      747 2024-05-15 19:19:12.000000 plingenn-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:24:05.512448 plingenn-0.0.4/
+-rw-rw-rw-   0        0        0      619 2024-05-15 19:24:05.472434 plingenn-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-15 18:32:53.000000 plingenn-0.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 19:24:04.953518 plingenn-0.0.4/plingenn/
+-rw-rw-rw-   0        0        0      112 2024-05-15 18:31:48.000000 plingenn-0.0.4/plingenn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 19:24:05.407064 plingenn-0.0.4/plingenn.egg-info/
+-rw-rw-rw-   0        0        0      619 2024-05-15 19:24:03.000000 plingenn-0.0.4/plingenn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2024-05-15 19:24:04.000000 plingenn-0.0.4/plingenn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 19:24:04.000000 plingenn-0.0.4/plingenn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 19:24:04.000000 plingenn-0.0.4/plingenn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 19:24:04.000000 plingenn-0.0.4/plingenn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 19:24:05.513449 plingenn-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-15 19:23:57.000000 plingenn-0.0.4/setup.py
```

### Comparing `plingenn-0.0.3/PKG-INFO` & `plingenn-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.3
+Version: 0.0.4
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `plingenn-0.0.3/plingenn.egg-info/PKG-INFO` & `plingenn-0.0.4/plingenn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plingenn
-Version: 0.0.3
+Version: 0.0.4
 Summary: A very basic package
 Home-page: 
 Author: Plingenn Plingsson
 Author-email: Plingenn12@gmail.com
 License: MIT
 Keywords: none
 Classifier: Development Status :: 5 - Production/Stable
```

