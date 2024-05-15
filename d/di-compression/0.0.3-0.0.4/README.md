# Comparing `tmp/di_compression-0.0.3.tar.gz` & `tmp/di-compression-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "di_compression-0.0.3.tar", last modified: Tue May 14 01:11:37 2024, max compression
+gzip compressed data, was "di-compression-0.0.4.tar", last modified: Wed May 15 02:02:45 2024, max compression
```

## Comparing `di_compression-0.0.3.tar` & `di-compression-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,18 @@
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-14 01:11:37.470168 di_compression-0.0.3/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      842 2024-05-14 01:11:37.470168 di_compression-0.0.3/PKG-INFO
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       22 2024-05-06 18:11:07.000000 di_compression-0.0.3/README.md
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-14 01:11:37.469168 di_compression-0.0.3/di_compression.egg-info/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      842 2024-05-14 01:11:37.000000 di_compression-0.0.3/di_compression.egg-info/PKG-INFO
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      207 2024-05-14 01:11:37.000000 di_compression-0.0.3/di_compression.egg-info/SOURCES.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)        1 2024-05-14 01:11:37.000000 di_compression-0.0.3/di_compression.egg-info/dependency_links.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       30 2024-05-14 01:11:37.000000 di_compression-0.0.3/di_compression.egg-info/requires.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)        1 2024-05-14 01:11:37.000000 di_compression-0.0.3/di_compression.egg-info/top_level.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       38 2024-05-14 01:11:37.470168 di_compression-0.0.3/setup.cfg
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     1097 2024-05-14 01:11:04.000000 di_compression-0.0.3/setup.py
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-15 02:02:45.234348 di-compression-0.0.4/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      839 2024-05-15 02:02:45.234348 di-compression-0.0.4/PKG-INFO
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)    25793 2024-05-15 02:00:03.000000 di-compression-0.0.4/README.md
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-15 02:02:45.233348 di-compression-0.0.4/algorithms/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      186 2024-05-14 07:20:32.000000 di-compression-0.0.4/algorithms/__init__.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2652 2024-05-14 07:38:47.000000 di-compression-0.0.4/algorithms/deflate.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     9278 2024-05-14 07:18:58.000000 di-compression-0.0.4/algorithms/huffman.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     3793 2024-05-14 06:39:51.000000 di-compression-0.0.4/algorithms/lz77.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2370 2024-05-14 07:15:34.000000 di-compression-0.0.4/algorithms/lz78.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2201 2024-05-14 00:23:21.000000 di-compression-0.0.4/algorithms/lzw.py
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-15 02:02:45.234348 di-compression-0.0.4/di_compression.egg-info/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      839 2024-05-15 02:02:45.000000 di-compression-0.0.4/di_compression.egg-info/PKG-INFO
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      330 2024-05-15 02:02:45.000000 di-compression-0.0.4/di_compression.egg-info/SOURCES.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)        1 2024-05-15 02:02:45.000000 di-compression-0.0.4/di_compression.egg-info/dependency_links.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       30 2024-05-15 02:02:45.000000 di-compression-0.0.4/di_compression.egg-info/requires.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       11 2024-05-15 02:02:45.000000 di-compression-0.0.4/di_compression.egg-info/top_level.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       38 2024-05-15 02:02:45.234348 di-compression-0.0.4/setup.cfg
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     1087 2024-05-15 02:02:03.000000 di-compression-0.0.4/setup.py
```

### Comparing `di_compression-0.0.3/PKG-INFO` & `di-compression-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: di_compression
-Version: 0.0.3
-Summary: compression algorithms
+Name: di-compression
+Version: 0.0.4
+Summary: Compress algorithms
 Home-page: https://github.com/UCUgllekk/compression_research
 Author: UCUgllekk
 Author-email: pavlosiuk.pn@ucu.edu.ua
 Keywords: python,compress,compression,algorithm,lz78,lzw,huffman,deflate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `di_compression-0.0.3/di_compression.egg-info/PKG-INFO` & `di-compression-0.0.4/di_compression.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: di_compression
-Version: 0.0.3
-Summary: compression algorithms
+Name: di-compression
+Version: 0.0.4
+Summary: Compress algorithms
 Home-page: https://github.com/UCUgllekk/compression_research
 Author: UCUgllekk
 Author-email: pavlosiuk.pn@ucu.edu.ua
 Keywords: python,compress,compression,algorithm,lz78,lzw,huffman,deflate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `di_compression-0.0.3/setup.py` & `di-compression-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+'''Setup'''
 from setuptools import setup, find_packages
 
 LONG_DESCRIPTION = 'A package that allows to compress different types of data using different algorithms such as LZW, LZ78, Deflate, Huffman'
 
 setup(
-    name="di_compression",
-    version="0.0.3",
+    name="di-compression",
+    version="0.0.4",
     author="UCUgllekk",
     author_email="pavlosiuk.pn@ucu.edu.ua",
-    description='compression algorithms',
+    description='Compress algorithms',
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
-    packages=find_packages(where="algorithms"),
+    packages=find_packages(),
     url="https://github.com/UCUgllekk/compression_research",
     install_requires=["tk>=0.1.0"],
     extras_require={
         "dev": ["twine>=4.0.2"]},
     keywords=['python', 'compress', 'compression', 'algorithm',
               'lz78', 'lzw', 'huffman', 'deflate'],
     classifiers=[
@@ -22,8 +23,8 @@
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     python_requires=">=3.11",
-)
+)
```

