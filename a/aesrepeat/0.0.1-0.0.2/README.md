# Comparing `tmp/aesrepeat-0.0.1-py3-none-any.whl.zip` & `tmp/aesrepeat-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 2307 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     2548 b- defN 24-May-15 14:30 aesrepeat/__init__.py
--rw-rw-rw-  2.0 fat     1870 b- defN 24-May-15 14:30 aesrepeat-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 14:30 aesrepeat-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-May-15 14:30 aesrepeat-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      384 b- defN 24-May-15 14:30 aesrepeat-0.0.1.dist-info/RECORD
-5 files, 4904 bytes uncompressed, 1591 bytes compressed:  67.6%
+Zip file size: 2876 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     2548 b- defN 24-May-15 14:56 aesrepeat/__init__.py
+-rw-rw-rw-  2.0 fat      948 b- defN 24-May-15 14:47 aesrepeat/internal/__init__.py
+-rw-rw-rw-  2.0 fat     1870 b- defN 24-May-15 14:56 aesrepeat-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 14:56 aesrepeat-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-15 14:56 aesrepeat-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      470 b- defN 24-May-15 14:56 aesrepeat-0.0.2.dist-info/RECORD
+6 files, 5938 bytes uncompressed, 2024 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
 Filename: aesrepeat/__init__.py
 Comment: 
 
-Filename: aesrepeat-0.0.1.dist-info/METADATA
+Filename: aesrepeat/internal/__init__.py
 Comment: 
 
-Filename: aesrepeat-0.0.1.dist-info/WHEEL
+Filename: aesrepeat-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: aesrepeat-0.0.1.dist-info/top_level.txt
+Filename: aesrepeat-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: aesrepeat-0.0.1.dist-info/RECORD
+Filename: aesrepeat-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: aesrepeat-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aesrepeat/__init__.py

```diff
@@ -1,13 +1,13 @@
 from aesrepeat.internal import *
 import base64
 import pickle
 
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '0.0.1'
+__version__      = '0.0.2'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-aesrepeat'
 __all__ = ['AES128', 'AES256']
 
 class AES128:
```

## Comparing `aesrepeat-0.0.1.dist-info/METADATA` & `aesrepeat-0.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aesrepeat
-Version: 0.0.1
+Version: 0.0.2
 Summary: Multiple encryption library
 Home-page: https://github.com/lang-library/py-aesrepeat
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

