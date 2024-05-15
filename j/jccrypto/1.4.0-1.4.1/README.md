# Comparing `tmp/jccrypto-1.4.0-py3-none-any.whl.zip` & `tmp/jccrypto-1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4530 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     3051 b- defN 24-May-15 06:44 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     6240 b- defN 24-May-15 06:44 jccrypto-1.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 06:44 jccrypto-1.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-15 06:44 jccrypto-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-15 06:44 jccrypto-1.4.0.dist-info/RECORD
-5 files, 9770 bytes uncompressed, 3824 bytes compressed:  60.9%
+Zip file size: 4528 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     3058 b- defN 24-May-15 06:46 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     6240 b- defN 24-May-15 06:46 jccrypto-1.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 06:46 jccrypto-1.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-15 06:46 jccrypto-1.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-15 06:46 jccrypto-1.4.1.dist-info/RECORD
+5 files, 9777 bytes uncompressed, 3822 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.4.0.dist-info/METADATA
+Filename: jccrypto-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.4.0.dist-info/WHEEL
+Filename: jccrypto-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.4.0.dist-info/top_level.txt
+Filename: jccrypto-1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.4.0.dist-info/RECORD
+Filename: jccrypto-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jccrypto/__init__.py

```diff
@@ -1,20 +1,20 @@
 # pip install PyCryptoDome
 from Crypto.Cipher import AES as ___AES__
 import base64
 import hashlib
 import pickle
 
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.4.0'
+__version__      = '1.4.1'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
-__all__ = ['JcCrypto', 'AES128FromString', 'AES256FromString']
+__all__ = ['JcCrypto', 'AES', 'AES128FromString', 'AES256FromString']
 
 def AES128FromString(str):
     sha256 = hashlib.sha256(str.encode())
     digets = sha256.digest()
     upper16 = digets[0:16]
     lower16 = digets[16:]
     return JcCrypto(upper16, lower16)
```

## Comparing `jccrypto-1.4.0.dist-info/METADATA` & `jccrypto-1.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jccrypto
-Version: 1.4.0
+Version: 1.4.1
 Summary: Simple crypto library
 Home-page: https://github.com/lang-library/py-jccrypto
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

