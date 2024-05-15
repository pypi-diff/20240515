# Comparing `tmp/di-compression-0.0.4.tar.gz` & `tmp/di_compression-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "di-compression-0.0.4.tar", last modified: Wed May 15 02:02:45 2024, max compression
+gzip compressed data, was "di_compression-0.1.0.tar", last modified: Wed May 15 02:15:17 2024, max compression
```

## Comparing `di-compression-0.0.4.tar` & `di_compression-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-15 02:02:45.234348 di-compression-0.0.4/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      839 2024-05-15 02:02:45.234348 di-compression-0.0.4/PKG-INFO
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)    25793 2024-05-15 02:00:03.000000 di-compression-0.0.4/README.md
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-15 02:02:45.233348 di-compression-0.0.4/algorithms/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      186 2024-05-14 07:20:32.000000 di-compression-0.0.4/algorithms/__init__.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2652 2024-05-14 07:38:47.000000 di-compression-0.0.4/algorithms/deflate.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     9278 2024-05-14 07:18:58.000000 di-compression-0.0.4/algorithms/huffman.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     3793 2024-05-14 06:39:51.000000 di-compression-0.0.4/algorithms/lz77.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2370 2024-05-14 07:15:34.000000 di-compression-0.0.4/algorithms/lz78.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2201 2024-05-14 00:23:21.000000 di-compression-0.0.4/algorithms/lzw.py
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-15 02:02:45.234348 di-compression-0.0.4/di_compression.egg-info/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      839 2024-05-15 02:02:45.000000 di-compression-0.0.4/di_compression.egg-info/PKG-INFO
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      330 2024-05-15 02:02:45.000000 di-compression-0.0.4/di_compression.egg-info/SOURCES.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)        1 2024-05-15 02:02:45.000000 di-compression-0.0.4/di_compression.egg-info/dependency_links.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       30 2024-05-15 02:02:45.000000 di-compression-0.0.4/di_compression.egg-info/requires.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       11 2024-05-15 02:02:45.000000 di-compression-0.0.4/di_compression.egg-info/top_level.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       38 2024-05-15 02:02:45.234348 di-compression-0.0.4/setup.cfg
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     1087 2024-05-15 02:02:03.000000 di-compression-0.0.4/setup.py
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-15 02:15:17.595731 di_compression-0.1.0/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      839 2024-05-15 02:15:17.594731 di_compression-0.1.0/PKG-INFO
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)    25793 2024-05-15 02:00:03.000000 di_compression-0.1.0/README.md
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-15 02:15:17.592731 di_compression-0.1.0/di_compression/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      206 2024-05-15 02:09:23.000000 di_compression-0.1.0/di_compression/__init__.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2652 2024-05-14 07:38:47.000000 di_compression-0.1.0/di_compression/deflate.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     9278 2024-05-14 07:18:58.000000 di_compression-0.1.0/di_compression/huffman.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     3793 2024-05-14 06:39:51.000000 di_compression-0.1.0/di_compression/lz77.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2370 2024-05-14 07:15:34.000000 di_compression-0.1.0/di_compression/lz78.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2201 2024-05-14 00:23:21.000000 di_compression-0.1.0/di_compression/lzw.py
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-15 02:15:17.594731 di_compression-0.1.0/di_compression.egg-info/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      839 2024-05-15 02:15:17.000000 di_compression-0.1.0/di_compression.egg-info/PKG-INFO
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      354 2024-05-15 02:15:17.000000 di_compression-0.1.0/di_compression.egg-info/SOURCES.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)        1 2024-05-15 02:15:17.000000 di_compression-0.1.0/di_compression.egg-info/dependency_links.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       30 2024-05-15 02:15:17.000000 di_compression-0.1.0/di_compression.egg-info/requires.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       15 2024-05-15 02:15:17.000000 di_compression-0.1.0/di_compression.egg-info/top_level.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       38 2024-05-15 02:15:17.595731 di_compression-0.1.0/setup.cfg
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     1087 2024-05-15 02:14:50.000000 di_compression-0.1.0/setup.py
```

### Comparing `di-compression-0.0.4/PKG-INFO` & `di_compression-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: di-compression
-Version: 0.0.4
+Version: 0.1.0
 Summary: Compress algorithms
 Home-page: https://github.com/UCUgllekk/compression_research
 Author: UCUgllekk
 Author-email: pavlosiuk.pn@ucu.edu.ua
 Keywords: python,compress,compression,algorithm,lz78,lzw,huffman,deflate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `di-compression-0.0.4/README.md` & `di_compression-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `di-compression-0.0.4/algorithms/deflate.py` & `di_compression-0.1.0/di_compression/deflate.py`

 * *Files identical despite different names*

### Comparing `di-compression-0.0.4/algorithms/huffman.py` & `di_compression-0.1.0/di_compression/huffman.py`

 * *Files identical despite different names*

### Comparing `di-compression-0.0.4/algorithms/lz77.py` & `di_compression-0.1.0/di_compression/lz77.py`

 * *Files identical despite different names*

### Comparing `di-compression-0.0.4/algorithms/lz78.py` & `di_compression-0.1.0/di_compression/lz78.py`

 * *Files identical despite different names*

### Comparing `di-compression-0.0.4/algorithms/lzw.py` & `di_compression-0.1.0/di_compression/lzw.py`

 * *Files identical despite different names*

### Comparing `di-compression-0.0.4/di_compression.egg-info/PKG-INFO` & `di_compression-0.1.0/di_compression.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: di-compression
-Version: 0.0.4
+Version: 0.1.0
 Summary: Compress algorithms
 Home-page: https://github.com/UCUgllekk/compression_research
 Author: UCUgllekk
 Author-email: pavlosiuk.pn@ucu.edu.ua
 Keywords: python,compress,compression,algorithm,lz78,lzw,huffman,deflate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `di-compression-0.0.4/setup.py` & `di_compression-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''Setup'''
 from setuptools import setup, find_packages
 
 LONG_DESCRIPTION = 'A package that allows to compress different types of data using different algorithms such as LZW, LZ78, Deflate, Huffman'
 
 setup(
     name="di-compression",
-    version="0.0.4",
+    version="0.1.0",
     author="UCUgllekk",
     author_email="pavlosiuk.pn@ucu.edu.ua",
     description='Compress algorithms',
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     url="https://github.com/UCUgllekk/compression_research",
```

