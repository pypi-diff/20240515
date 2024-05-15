# Comparing `tmp/jccrypto-1.1.1-py3-none-any.whl.zip` & `tmp/jccrypto-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4388 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     2686 b- defN 24-May-14 20:57 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     5965 b- defN 24-May-14 20:57 jccrypto-1.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 20:57 jccrypto-1.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 20:57 jccrypto-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-14 20:57 jccrypto-1.1.1.dist-info/RECORD
-5 files, 9130 bytes uncompressed, 3682 bytes compressed:  59.7%
+Zip file size: 4417 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     2717 b- defN 24-May-14 21:36 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     5977 b- defN 24-May-14 21:36 jccrypto-1.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 21:36 jccrypto-1.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-14 21:36 jccrypto-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-14 21:36 jccrypto-1.2.0.dist-info/RECORD
+5 files, 9173 bytes uncompressed, 3711 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.1.1.dist-info/METADATA
+Filename: jccrypto-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.1.1.dist-info/WHEEL
+Filename: jccrypto-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.1.1.dist-info/top_level.txt
+Filename: jccrypto-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.1.1.dist-info/RECORD
+Filename: jccrypto-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jccrypto/__init__.py

```diff
@@ -2,15 +2,15 @@
 from Crypto.Cipher import AES
 import base64
 import hashlib
 import pickle
 
 __package_name__ = 'pycrypto'
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.1.1'
+__version__      = '1.2.0'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
 __all__ = ['JcCrypto']
 
 def JcCryptoFromString(str):
@@ -45,16 +45,16 @@
         return base64.b64encode(encrypted_data).decode()
     def decode_bytes(self, base64_text):
         encrypted_data = base64.b64decode(base64_text.encode())
         decrypted_data = self.decipher.decrypt(encrypted_data)
         padding_size = decrypted_data[-1]
         unpadded_data = decrypted_data[:-padding_size]
         return unpadded_data
-    def encode_pickle(self, x):
-        data = pickle.dumps(x)
+    def encode_pickle(self, x, protocol=3):
+        data = pickle.dumps(x, protocol=protocol)
         block_size = AES.block_size
         padding_size = block_size - (len(data) % block_size)
         padded_data = data + bytes([padding_size]) * padding_size
         encrypted_data = self.cipher.encrypt(padded_data)
         return base64.b64encode(encrypted_data).decode()
     def decode_pickle(self, base64_text):
         encrypted_data = base64.b64decode(base64_text.encode())
```

## Comparing `jccrypto-1.1.1.dist-info/METADATA` & `jccrypto-1.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jccrypto
-Version: 1.1.1
+Version: 1.2.0
 Summary: Simple crypto library
 Home-page: https://github.com/lang-library/py-jccrypto
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -125,11 +125,11 @@
 encoded = cr.encode_pickle(list)
 decoded = cr.decode_pickle(encoded)
 print("decoded={}".format(decoded))
 
 print("")
 cr2 = JcCryptoFromString("this is password!")
 list = [111, 222, 333]
-encoded = cr2.encode_pickle(list)
+encoded = cr2.encode_pickle(list, protocol=4)
 decoded = cr2.decode_pickle(encoded)
 print("decoded={}".format(decoded))
 ```
```

