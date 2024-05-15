# Comparing `tmp/healmatcher-0.0.7.tar.gz` & `tmp/healmatcher-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/healmatcher-0.0.7.tar", last modified: Wed May 15 16:49:40 2024, max compression
+gzip compressed data, was "dist/healmatcher-0.0.8.tar", last modified: Wed May 15 16:57:44 2024, max compression
```

## Comparing `healmatcher-0.0.7.tar` & `healmatcher-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-15 16:49:40.473170 healmatcher-0.0.7/
--rw-r--r--   0 kwanbo     (501) staff       (20)     2969 2024-05-15 16:49:40.473009 healmatcher-0.0.7/PKG-INFO
--rw-r--r--   0 kwanbo     (501) staff       (20)     1851 2024-05-15 16:11:19.000000 healmatcher-0.0.7/README.md
-drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-15 16:49:40.472774 healmatcher-0.0.7/healmatcher.egg-info/
--rw-r--r--   0 kwanbo     (501) staff       (20)     2969 2024-05-15 16:49:40.000000 healmatcher-0.0.7/healmatcher.egg-info/PKG-INFO
--rw-r--r--   0 kwanbo     (501) staff       (20)      192 2024-05-15 16:49:40.000000 healmatcher-0.0.7/healmatcher.egg-info/SOURCES.txt
--rw-r--r--   0 kwanbo     (501) staff       (20)        1 2024-05-15 16:49:40.000000 healmatcher-0.0.7/healmatcher.egg-info/dependency_links.txt
--rw-r--r--   0 kwanbo     (501) staff       (20)       20 2024-05-15 16:49:40.000000 healmatcher-0.0.7/healmatcher.egg-info/requires.txt
--rw-r--r--   0 kwanbo     (501) staff       (20)        1 2024-05-15 16:49:40.000000 healmatcher-0.0.7/healmatcher.egg-info/top_level.txt
--rw-r--r--   0 kwanbo     (501) staff       (20)       38 2024-05-15 16:49:40.473226 healmatcher-0.0.7/setup.cfg
--rw-r--r--   0 kwanbo     (501) staff       (20)     1065 2024-05-15 16:49:20.000000 healmatcher-0.0.7/setup.py
+drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-15 16:57:44.976309 healmatcher-0.0.8/
+-rw-r--r--   0 kwanbo     (501) staff       (20)     2969 2024-05-15 16:57:44.976081 healmatcher-0.0.8/PKG-INFO
+-rw-r--r--   0 kwanbo     (501) staff       (20)     1851 2024-05-15 16:11:19.000000 healmatcher-0.0.8/README.md
+drwxr-xr-x   0 kwanbo     (501) staff       (20)        0 2024-05-15 16:57:44.975721 healmatcher-0.0.8/healmatcher.egg-info/
+-rw-r--r--   0 kwanbo     (501) staff       (20)     2969 2024-05-15 16:57:44.000000 healmatcher-0.0.8/healmatcher.egg-info/PKG-INFO
+-rw-r--r--   0 kwanbo     (501) staff       (20)      192 2024-05-15 16:57:44.000000 healmatcher-0.0.8/healmatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 kwanbo     (501) staff       (20)        1 2024-05-15 16:57:44.000000 healmatcher-0.0.8/healmatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 kwanbo     (501) staff       (20)       20 2024-05-15 16:57:44.000000 healmatcher-0.0.8/healmatcher.egg-info/requires.txt
+-rw-r--r--   0 kwanbo     (501) staff       (20)        1 2024-05-15 16:57:44.000000 healmatcher-0.0.8/healmatcher.egg-info/top_level.txt
+-rw-r--r--   0 kwanbo     (501) staff       (20)       38 2024-05-15 16:57:44.976410 healmatcher-0.0.8/setup.cfg
+-rw-r--r--   0 kwanbo     (501) staff       (20)     1065 2024-05-15 16:56:58.000000 healmatcher-0.0.8/setup.py
```

### Comparing `healmatcher-0.0.7/PKG-INFO` & `healmatcher-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healmatcher
-Version: 0.0.7
+Version: 0.0.8
 Summary: Fast and simple probabilistic data matching package
 Home-page: UNKNOWN
 Author: Joseph Shim github.com/JosephKBS
 Author-email: <joseph.shim.rok@gmail.com>
 License: UNKNOWN
 Description: # healmatcher
         - `healmatcher` is a simple but fast probabilistic matching package developed by NYULH HEAL Lab.
```

### Comparing `healmatcher-0.0.7/README.md` & `healmatcher-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `healmatcher-0.0.7/healmatcher.egg-info/PKG-INFO` & `healmatcher-0.0.8/healmatcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healmatcher
-Version: 0.0.7
+Version: 0.0.8
 Summary: Fast and simple probabilistic data matching package
 Home-page: UNKNOWN
 Author: Joseph Shim github.com/JosephKBS
 Author-email: <joseph.shim.rok@gmail.com>
 License: UNKNOWN
 Description: # healmatcher
         - `healmatcher` is a simple but fast probabilistic matching package developed by NYULH HEAL Lab.
```

### Comparing `healmatcher-0.0.7/setup.py` & `healmatcher-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7' 
+VERSION = '0.0.8' 
 DESCRIPTION = 'Fast and simple probabilistic data matching package'
 
 # Setting up
 setup(
         name="healmatcher", 
         version=VERSION,
         author="Joseph Shim github.com/JosephKBS",
```

