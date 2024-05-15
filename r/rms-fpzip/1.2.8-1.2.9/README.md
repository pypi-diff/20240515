# Comparing `tmp/rms_fpzip-1.2.8-cp39-cp39-win_amd64.whl.zip` & `tmp/rms_fpzip-1.2.9-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 99064 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat   299008 b- defN 23-Oct-24 22:53 fpzip.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      148 b- defN 23-Oct-24 22:53 rms_fpzip-1.2.8.dist-info/AUTHORS
--rw-rw-rw-  2.0 fat     1556 b- defN 23-Oct-24 22:53 rms_fpzip-1.2.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4293 b- defN 23-Oct-24 22:53 rms_fpzip-1.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Oct-24 22:53 rms_fpzip-1.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Oct-24 22:53 rms_fpzip-1.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      569 b- defN 23-Oct-24 22:53 rms_fpzip-1.2.8.dist-info/RECORD
-7 files, 305691 bytes uncompressed, 98058 bytes compressed:  67.9%
+Zip file size: 98835 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat   297472 b- defN 23-Dec-13 23:03 fpzip.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      148 b- defN 23-Dec-13 23:03 rms_fpzip-1.2.9.dist-info/AUTHORS
+-rw-rw-rw-  2.0 fat     1556 b- defN 23-Dec-13 23:03 rms_fpzip-1.2.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4276 b- defN 23-Dec-13 23:03 rms_fpzip-1.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Dec-13 23:03 rms_fpzip-1.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Dec-13 23:03 rms_fpzip-1.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      569 b- defN 23-Dec-13 23:03 rms_fpzip-1.2.9.dist-info/RECORD
+7 files, 304138 bytes uncompressed, 97829 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: fpzip.cp39-win_amd64.pyd
 Comment: 
 
-Filename: rms_fpzip-1.2.8.dist-info/AUTHORS
+Filename: rms_fpzip-1.2.9.dist-info/AUTHORS
 Comment: 
 
-Filename: rms_fpzip-1.2.8.dist-info/LICENSE
+Filename: rms_fpzip-1.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: rms_fpzip-1.2.8.dist-info/METADATA
+Filename: rms_fpzip-1.2.9.dist-info/METADATA
 Comment: 
 
-Filename: rms_fpzip-1.2.8.dist-info/WHEEL
+Filename: rms_fpzip-1.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: rms_fpzip-1.2.8.dist-info/top_level.txt
+Filename: rms_fpzip-1.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: rms_fpzip-1.2.8.dist-info/RECORD
+Filename: rms_fpzip-1.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rms_fpzip-1.2.8.dist-info/LICENSE` & `rms_fpzip-1.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rms_fpzip-1.2.8.dist-info/METADATA` & `rms_fpzip-1.2.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-fpzip
-Version: 1.2.8
+Version: 1.2.9
 Summary: Numpy wrapper for fpzip algorithm (P. Lindstrom & M. Isenburg, 2006) RMS Fork
 Home-page: https://github.com/SETI/rms-fpzip/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 Maintainer: Robert French
 Maintainer-email: rfrench@seti.org
 License: BSD
@@ -27,15 +27,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: oldest-supported-numpy
+Requires-Dist: numpy
 
 | PyPI Release | Test Status |
 | ------------ | ----------- |
 | [![PyPI version](https://badge.fury.io/py/rms-fpzip.svg)](https://badge.fury.io/py/rms-fpzip) | [![Build status](https://img.shields.io/github/actions/workflow/status/SETI/rms-fpzip/run-tests.yml?branch=master)](https://github.com/SETI/rms-fpzip/actions) |
 
 # Introduction
```

## Comparing `rms_fpzip-1.2.8.dist-info/RECORD` & `rms_fpzip-1.2.9.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-fpzip.cp39-win_amd64.pyd,sha256=pkCSBwH1hk7rMJV3IwuGmaMZnfRyhJ7YALVU8U81ceo,299008
-rms_fpzip-1.2.8.dist-info/AUTHORS,sha256=DWcBA-LLUE0rjzUE8xVO4sA1KzwxWIja0Iu7M1XhvGo,148
-rms_fpzip-1.2.8.dist-info/LICENSE,sha256=8BpZRbaM_5v8SwQlwhblgue4osr-URIVpjiJ7R-Iec8,1556
-rms_fpzip-1.2.8.dist-info/METADATA,sha256=-GChVVpYcdmpcMXkiGlv3ZKMC1O7kbMFZmM9W-tn9Bc,4293
-rms_fpzip-1.2.8.dist-info/WHEEL,sha256=2xSj8c4s_gFbWpcImYQptdXS3JLuzC2uK5Om8I_SEKg,100
-rms_fpzip-1.2.8.dist-info/top_level.txt,sha256=uEP3zKKR8Qo6aKJDXZrIXTDZdsszpOstYi14B4jRUsQ,17
-rms_fpzip-1.2.8.dist-info/RECORD,,
+fpzip.cp39-win_amd64.pyd,sha256=zeNJtc0xOeFk3T5PGIyc0JJtXk7PHIKhhi8Q7kRwu2Q,297472
+rms_fpzip-1.2.9.dist-info/AUTHORS,sha256=DWcBA-LLUE0rjzUE8xVO4sA1KzwxWIja0Iu7M1XhvGo,148
+rms_fpzip-1.2.9.dist-info/LICENSE,sha256=8BpZRbaM_5v8SwQlwhblgue4osr-URIVpjiJ7R-Iec8,1556
+rms_fpzip-1.2.9.dist-info/METADATA,sha256=VguC6cl_2L-nuwwfaVkOmj0O3Cy1WEFgziRRY1WouXc,4276
+rms_fpzip-1.2.9.dist-info/WHEEL,sha256=GZFS91_ufm4WrNPBaFVPB9MvOXR6bMZQhPcZRRTN5YM,100
+rms_fpzip-1.2.9.dist-info/top_level.txt,sha256=uEP3zKKR8Qo6aKJDXZrIXTDZdsszpOstYi14B4jRUsQ,17
+rms_fpzip-1.2.9.dist-info/RECORD,,
```

