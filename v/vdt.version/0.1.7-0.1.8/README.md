# Comparing `tmp/vdt.version-0.1.7.tar.gz` & `tmp/vdt.version-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdt.version-0.1.7.tar", last modified: Tue May 14 07:36:19 2024, max compression
+gzip compressed data, was "vdt.version-0.1.8.tar", last modified: Wed May 15 09:05:56 2024, max compression
```

## Comparing `vdt.version-0.1.7.tar` & `vdt.version-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:36:19.614934 vdt.version-0.1.7/
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     1491 2024-05-14 07:17:41.000000 vdt.version-0.1.7/LICENSE
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      318 2024-05-14 07:36:19.614814 vdt.version-0.1.7/PKG-INFO
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     4380 2024-05-14 07:17:41.000000 vdt.version-0.1.7/README.rst
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       38 2024-05-14 07:36:19.614973 vdt.version-0.1.7/setup.cfg
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      798 2024-05-14 07:17:41.000000 vdt.version-0.1.7/setup.py
-drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:36:19.612962 vdt.version-0.1.7/vdt/
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       56 2024-05-14 07:17:41.000000 vdt.version-0.1.7/vdt/__init__.py
-drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:36:19.614657 vdt.version-0.1.7/vdt/version/
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        1 2024-05-14 07:17:41.000000 vdt.version-0.1.7/vdt/version/__init__.py
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     2919 2024-05-14 07:17:41.000000 vdt.version-0.1.7/vdt/version/main.py
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     2215 2024-05-14 07:17:41.000000 vdt.version-0.1.7/vdt/version/repo.py
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     4284 2024-05-14 07:17:41.000000 vdt.version-0.1.7/vdt/version/shared.py
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     2965 2024-05-14 07:17:41.000000 vdt.version-0.1.7/vdt/version/utils.py
-drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:36:19.613996 vdt.version-0.1.7/vdt.version.egg-info/
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      318 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/PKG-INFO
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      436 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/SOURCES.txt
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        1 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/dependency_links.txt
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       50 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/entry_points.txt
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        4 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/namespace_packages.txt
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       67 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/requires.txt
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        4 2024-05-14 07:36:19.000000 vdt.version-0.1.7/vdt.version.egg-info/top_level.txt
--rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        1 2024-05-14 07:18:21.000000 vdt.version-0.1.7/vdt.version.egg-info/zip-safe
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-15 09:05:56.058532 vdt.version-0.1.8/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     1491 2024-05-14 07:17:41.000000 vdt.version-0.1.8/LICENSE
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      318 2024-05-15 09:05:56.058409 vdt.version-0.1.8/PKG-INFO
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     4380 2024-05-14 07:17:41.000000 vdt.version-0.1.8/README.rst
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       38 2024-05-15 09:05:56.058570 vdt.version-0.1.8/setup.cfg
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      798 2024-05-15 09:04:35.000000 vdt.version-0.1.8/setup.py
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-15 09:05:56.056608 vdt.version-0.1.8/vdt/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       56 2024-05-14 07:17:41.000000 vdt.version-0.1.8/vdt/__init__.py
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-15 09:05:56.058255 vdt.version-0.1.8/vdt/version/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        1 2024-05-14 07:17:41.000000 vdt.version-0.1.8/vdt/version/__init__.py
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     2919 2024-05-14 07:17:41.000000 vdt.version-0.1.8/vdt/version/main.py
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     2215 2024-05-14 07:17:41.000000 vdt.version-0.1.8/vdt/version/repo.py
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     4379 2024-05-15 09:04:25.000000 vdt.version-0.1.8/vdt/version/shared.py
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     2965 2024-05-14 07:17:41.000000 vdt.version-0.1.8/vdt/version/utils.py
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-15 09:05:56.057630 vdt.version-0.1.8/vdt.version.egg-info/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      318 2024-05-15 09:05:56.000000 vdt.version-0.1.8/vdt.version.egg-info/PKG-INFO
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      436 2024-05-15 09:05:56.000000 vdt.version-0.1.8/vdt.version.egg-info/SOURCES.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        1 2024-05-15 09:05:56.000000 vdt.version-0.1.8/vdt.version.egg-info/dependency_links.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       50 2024-05-15 09:05:56.000000 vdt.version-0.1.8/vdt.version.egg-info/entry_points.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        4 2024-05-15 09:05:56.000000 vdt.version-0.1.8/vdt.version.egg-info/namespace_packages.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       67 2024-05-15 09:05:56.000000 vdt.version-0.1.8/vdt.version.egg-info/requires.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        4 2024-05-15 09:05:56.000000 vdt.version-0.1.8/vdt.version.egg-info/top_level.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        1 2024-05-14 07:18:21.000000 vdt.version-0.1.8/vdt.version.egg-info/zip-safe
```

### Comparing `vdt.version-0.1.7/LICENSE` & `vdt.version-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vdt.version-0.1.7/README.rst` & `vdt.version-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `vdt.version-0.1.7/setup.py` & `vdt.version-0.1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 from setuptools import find_packages, setup
 
 pkgname = "vdt.version"
 
 setup(name=pkgname,
-      version="0.1.7",
+      version="0.1.8",
       description="Version Increment Tool for GIT",
       author="Lars van de Kerkhof",
       author_email="lars@devopsconsulting.nl",
       maintainer="Lars van de Kerkhof",
       maintainer_email="lars@devopsconsulting.nl",
       url="https://github.com/devopsconsulting/vdt.version",
       packages=find_packages(),
```

### Comparing `vdt.version-0.1.7/vdt/version/main.py` & `vdt.version-0.1.8/vdt/version/main.py`

 * *Files identical despite different names*

### Comparing `vdt.version-0.1.7/vdt/version/repo.py` & `vdt.version-0.1.8/vdt/version/repo.py`

 * *Files identical despite different names*

### Comparing `vdt.version-0.1.7/vdt/version/shared.py` & `vdt.version-0.1.8/vdt/version/shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 The functions and objects in this file can be used in your plugins.
 """
 from functools import total_ordering
+from packaging.version import Version as VersionParser
 import contextlib
 import logging
 import os.path
 import subprocess
 import sys
 
 
@@ -17,16 +18,19 @@
     Parse a version string into it's components.
     
     >>> parse_version_string("0.1")
     ([0, 1], 'jenkins', None)
     >>> parse_version_string("0.3.2-jenkins-3447876")
     ([0, 3, 2], 'jenkins', 3447876)
     """
+
     components = version_string.split('-') + [None, None]
-    version = list(map(int, components[0].split('.')))
+
+    parsed_version = VersionParser(components[0])
+    version = list(parsed_version.release)
     build_tag = components[1] if components[1] else BUILD_TAG
     build_number = int(components[2]) if components[2] else components[2]
 
     return (version, build_tag, build_number)
 
 
 def format_version(version, build_number=None, build_tag=BUILD_TAG):
```

### Comparing `vdt.version-0.1.7/vdt/version/utils.py` & `vdt.version-0.1.8/vdt/version/utils.py`

 * *Files identical despite different names*

