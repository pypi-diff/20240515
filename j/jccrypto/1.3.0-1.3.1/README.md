# Comparing `tmp/jccrypto-1.3.0-py3-none-any.whl.zip` & `tmp/jccrypto-1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4505 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     2925 b- defN 24-May-15 05:30 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     6250 b- defN 24-May-15 05:31 jccrypto-1.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 05:31 jccrypto-1.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-15 05:31 jccrypto-1.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-15 05:31 jccrypto-1.3.0.dist-info/RECORD
-5 files, 9654 bytes uncompressed, 3799 bytes compressed:  60.6%
+Zip file size: 4508 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     2945 b- defN 24-May-15 05:36 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     6250 b- defN 24-May-15 05:36 jccrypto-1.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 05:36 jccrypto-1.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-15 05:36 jccrypto-1.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-15 05:36 jccrypto-1.3.1.dist-info/RECORD
+5 files, 9674 bytes uncompressed, 3802 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.3.0.dist-info/METADATA
+Filename: jccrypto-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.3.0.dist-info/WHEEL
+Filename: jccrypto-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.3.0.dist-info/top_level.txt
+Filename: jccrypto-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.3.0.dist-info/RECORD
+Filename: jccrypto-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jccrypto/__init__.py

```diff
@@ -2,20 +2,20 @@
 from Crypto.Cipher import AES
 import base64
 import hashlib
 import pickle
 
 __package_name__ = 'pycrypto'
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.3.0'
+__version__      = '1.3.1'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
-__all__ = ['JcCrypto', 'AES128FromString']
+__all__ = ['JcCrypto', 'AES128FromString', 'AES256FromString']
 
 def AES128FromString(str):
     sha256 = hashlib.sha256(str.encode())
     digets = sha256.digest()
     upper16 = digets[0:16]
     lower16 = digets[16:]
     return JcCrypto(upper16, lower16)
```

## Comparing `jccrypto-1.3.0.dist-info/METADATA` & `jccrypto-1.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jccrypto
-Version: 1.3.0
+Version: 1.3.1
 Summary: Simple crypto library
 Home-page: https://github.com/lang-library/py-jccrypto
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

