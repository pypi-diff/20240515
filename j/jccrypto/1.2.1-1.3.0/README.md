# Comparing `tmp/jccrypto-1.2.1-py3-none-any.whl.zip` & `tmp/jccrypto-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4418 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     2739 b- defN 24-May-15 05:04 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     5977 b- defN 24-May-15 05:04 jccrypto-1.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 05:04 jccrypto-1.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-15 05:04 jccrypto-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-15 05:04 jccrypto-1.2.1.dist-info/RECORD
-5 files, 9195 bytes uncompressed, 3712 bytes compressed:  59.6%
+Zip file size: 4505 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     2925 b- defN 24-May-15 05:30 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     6250 b- defN 24-May-15 05:31 jccrypto-1.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 05:31 jccrypto-1.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-15 05:31 jccrypto-1.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-15 05:31 jccrypto-1.3.0.dist-info/RECORD
+5 files, 9654 bytes uncompressed, 3799 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.2.1.dist-info/METADATA
+Filename: jccrypto-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.2.1.dist-info/WHEEL
+Filename: jccrypto-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.2.1.dist-info/top_level.txt
+Filename: jccrypto-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.2.1.dist-info/RECORD
+Filename: jccrypto-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jccrypto/__init__.py

```diff
@@ -2,28 +2,35 @@
 from Crypto.Cipher import AES
 import base64
 import hashlib
 import pickle
 
 __package_name__ = 'pycrypto'
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.2.1'
+__version__      = '1.3.0'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
-__all__ = ['JcCrypto', 'JcCryptoFromString']
+__all__ = ['JcCrypto', 'AES128FromString']
 
-def JcCryptoFromString(str):
+def AES128FromString(str):
     sha256 = hashlib.sha256(str.encode())
     digets = sha256.digest()
     upper16 = digets[0:16]
     lower16 = digets[16:]
     return JcCrypto(upper16, lower16)
 
+def AES256FromString(str):
+    sha384 = hashlib.sha384(str.encode())
+    digets = sha384.digest()
+    upper32 = digets[0:32]
+    lower16 = digets[32:]
+    return JcCrypto(upper32, lower16)
+
 class JcCrypto:
     def __init__(self, key, iv):
         self.cipher = AES.new(key, AES.MODE_CBC, iv)
         self.decipher = AES.new(key, AES.MODE_CBC, iv)
     def encode_text(self, plain_text):
         data = plain_text.encode()
         block_size = AES.block_size
```

## Comparing `jccrypto-1.2.1.dist-info/METADATA` & `jccrypto-1.3.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jccrypto
-Version: 1.2.1
+Version: 1.3.0
 Summary: Simple crypto library
 Home-page: https://github.com/lang-library/py-jccrypto
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -85,20 +85,21 @@
 
 ----
 ```
 
 ## Sample code
 
 ```
-from jccrypto import JcCrypto, JcCryptoFromString
+from jccrypto import JcCrypto, AES128FromString, AES256FromString
 
 text = "Pythonの暗号化ライブラリとそれらの概要を表にまとめました。非常にたくさんのライブラリがあることがわかりました。それぞれのライブラリが得手不得手を持っているためユースケースに応じて適切なライブラリを使用する必要があります。"
 
 # 鍵の生成
-key = 'abcdefghijklmnop'.encode()
+#key = 'abcdefghijklmnop'.encode()
+key = '12345678901234567890123456789012'.encode()
 # IVの生成
 iv = '1234567890123456'.encode()
 
 cr = JcCrypto(key, iv)
 
 print("")
 encoded = cr.encode_text(text)
@@ -123,13 +124,20 @@
 print("")
 list = [11, 22, 33]
 encoded = cr.encode_pickle(list)
 decoded = cr.decode_pickle(encoded)
 print("decoded={}".format(decoded))
 
 print("")
-cr2 = JcCryptoFromString("this is password!")
+cr2 = AES128FromString("this is password!")
 list = [111, 222, 333]
 encoded = cr2.encode_pickle(list, protocol=4)
 decoded = cr2.decode_pickle(encoded)
 print("decoded={}".format(decoded))
+
+print("")
+cr3 = AES256FromString("this is password!")
+list = [1111, 2222, 3333]
+encoded = cr3.encode_pickle(list, protocol=4)
+decoded = cr3.decode_pickle(encoded)
+print("decoded={}".format(decoded))
 ```
```

