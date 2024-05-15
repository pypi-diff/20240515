# Comparing `tmp/printmate-1.2.2.tar.gz` & `tmp/printmate-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printmate-1.2.2.tar", last modified: Wed May 15 20:48:40 2024, max compression
+gzip compressed data, was "printmate-1.2.6.tar", last modified: Wed May 15 21:11:16 2024, max compression
```

## Comparing `printmate-1.2.2.tar` & `printmate-1.2.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 20:48:40.686455 printmate-1.2.2/
--rw-rw-rw-   0        0        0      308 2024-05-15 20:48:40.681391 printmate-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1103 2024-05-15 20:36:00.000000 printmate-1.2.2/license
-drwxrwxrwx   0        0        0        0 2024-05-15 20:48:40.681391 printmate-1.2.2/printmate.egg-info/
--rw-rw-rw-   0        0        0      308 2024-05-15 20:48:40.000000 printmate-1.2.2/printmate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-05-15 20:48:40.000000 printmate-1.2.2/printmate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 20:48:40.000000 printmate-1.2.2/printmate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-15 20:48:40.000000 printmate-1.2.2/printmate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-15 20:48:40.000000 printmate-1.2.2/printmate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 20:48:40.000000 printmate-1.2.2/printmate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 20:48:40.686455 printmate-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      530 2024-05-15 20:36:00.000000 printmate-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 21:11:16.728158 printmate-1.2.6/
+-rw-rw-rw-   0        0        0      308 2024-05-15 21:11:16.721074 printmate-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1103 2024-05-15 21:05:01.000000 printmate-1.2.6/license
+drwxrwxrwx   0        0        0        0 2024-05-15 21:11:16.721074 printmate-1.2.6/printmate.egg-info/
+-rw-rw-rw-   0        0        0      308 2024-05-15 21:11:16.000000 printmate-1.2.6/printmate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-05-15 21:11:16.000000 printmate-1.2.6/printmate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 21:11:16.000000 printmate-1.2.6/printmate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-15 21:11:16.000000 printmate-1.2.6/printmate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-15 21:11:16.000000 printmate-1.2.6/printmate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 21:11:16.000000 printmate-1.2.6/printmate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 21:11:16.728158 printmate-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-15 21:10:23.000000 printmate-1.2.6/setup.py
```

### Comparing `printmate-1.2.2/license` & `printmate-1.2.6/license`

 * *Files identical despite different names*

### Comparing `printmate-1.2.2/setup.py` & `printmate-1.2.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='printmate',
-    version='1.2.2',
+    version='1.2.6',
     packages=find_packages(),
     install_requires=[
         "colorama"],
     entry_points={
         'console_scripts': [
-            'vardll = vardll.__main__:main',
+            'printmate = printmate.__main__:main',
         ],
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication',
         'Operating System :: Microsoft :: Windows',
     ],
```

