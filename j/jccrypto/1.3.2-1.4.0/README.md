# Comparing `tmp/jccrypto-1.3.2-py3-none-any.whl.zip` & `tmp/jccrypto-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4497 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     2915 b- defN 24-May-15 06:34 jccrypto/__init__.py
--rw-rw-rw-  2.0 fat     6250 b- defN 24-May-15 06:35 jccrypto-1.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 06:35 jccrypto-1.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-15 06:35 jccrypto-1.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-15 06:35 jccrypto-1.3.2.dist-info/RECORD
-5 files, 9644 bytes uncompressed, 3791 bytes compressed:  60.7%
+Zip file size: 4530 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     3051 b- defN 24-May-15 06:44 jccrypto/__init__.py
+-rw-rw-rw-  2.0 fat     6240 b- defN 24-May-15 06:44 jccrypto-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 06:44 jccrypto-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-15 06:44 jccrypto-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-15 06:44 jccrypto-1.4.0.dist-info/RECORD
+5 files, 9770 bytes uncompressed, 3824 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jccrypto/__init__.py
 Comment: 
 
-Filename: jccrypto-1.3.2.dist-info/METADATA
+Filename: jccrypto-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: jccrypto-1.3.2.dist-info/WHEEL
+Filename: jccrypto-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: jccrypto-1.3.2.dist-info/top_level.txt
+Filename: jccrypto-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: jccrypto-1.3.2.dist-info/RECORD
+Filename: jccrypto-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jccrypto/__init__.py

```diff
@@ -1,15 +1,15 @@
 # pip install PyCryptoDome
-from Crypto.Cipher import AES
+from Crypto.Cipher import AES as ___AES__
 import base64
 import hashlib
 import pickle
 
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.3.2'
+__version__      = '1.4.0'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-jccrypto'
 __all__ = ['JcCrypto', 'AES128FromString', 'AES256FromString']
 
 def AES128FromString(str):
@@ -24,47 +24,51 @@
     digets = sha384.digest()
     upper32 = digets[0:32]
     lower16 = digets[32:]
     return JcCrypto(upper32, lower16)
 
 class JcCrypto:
     def __init__(self, key, iv):
-        self.cipher = AES.new(key, AES.MODE_CBC, iv)
-        self.decipher = AES.new(key, AES.MODE_CBC, iv)
+        self.cipher = ___AES__.new(key, ___AES__.MODE_CBC, iv)
+        self.decipher = ___AES__.new(key, ___AES__.MODE_CBC, iv)
     def encode_text(self, plain_text):
         data = plain_text.encode()
-        block_size = AES.block_size
+        block_size = ___AES__.block_size
         padding_size = block_size - (len(data) % block_size)
         padded_data = data + bytes([padding_size]) * padding_size
         encrypted_data = self.cipher.encrypt(padded_data)
         return base64.b64encode(encrypted_data).decode()
     def decode_text(self, base64_text):
         encrypted_data = base64.b64decode(base64_text.encode())
         decrypted_data = self.decipher.decrypt(encrypted_data)
         padding_size = decrypted_data[-1]
         unpadded_data = decrypted_data[:-padding_size]
         return unpadded_data.decode()
     def encode_bytes(self, data):
-        block_size = AES.block_size
+        block_size = ___AES__.block_size
         padding_size = block_size - (len(data) % block_size)
         padded_data = data + bytes([padding_size]) * padding_size
         encrypted_data = self.cipher.encrypt(padded_data)
         return base64.b64encode(encrypted_data).decode()
     def decode_bytes(self, base64_text):
         encrypted_data = base64.b64decode(base64_text.encode())
         decrypted_data = self.decipher.decrypt(encrypted_data)
         padding_size = decrypted_data[-1]
         unpadded_data = decrypted_data[:-padding_size]
         return unpadded_data
     def encode_pickle(self, x, protocol=3):
         data = pickle.dumps(x, protocol=protocol)
-        block_size = AES.block_size
+        block_size = ___AES__.block_size
         padding_size = block_size - (len(data) % block_size)
         padded_data = data + bytes([padding_size]) * padding_size
         encrypted_data = self.cipher.encrypt(padded_data)
         return base64.b64encode(encrypted_data).decode()
     def decode_pickle(self, base64_text):
         encrypted_data = base64.b64decode(base64_text.encode())
         decrypted_data = self.decipher.decrypt(encrypted_data)
         padding_size = decrypted_data[-1]
         unpadded_data = decrypted_data[:-padding_size]
         return pickle.loads(unpadded_data)
+
+class AES(JcCrypto):
+    def __init__(self, key, iv):
+        super().__init__(key, iv)
```

## Comparing `jccrypto-1.3.2.dist-info/METADATA` & `jccrypto-1.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jccrypto
-Version: 1.3.2
+Version: 1.4.0
 Summary: Simple crypto library
 Home-page: https://github.com/lang-library/py-jccrypto
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -85,25 +85,25 @@
 
 ----
 ```
 
 ## Sample code
 
 ```
-from jccrypto import JcCrypto, AES128FromString, AES256FromString
+from jccrypto import AES, AES128FromString, AES256FromString
 
 text = "Pythonの暗号化ライブラリとそれらの概要を表にまとめました。非常にたくさんのライブラリがあることがわかりました。それぞれのライブラリが得手不得手を持っているためユースケースに応じて適切なライブラリを使用する必要があります。"
 
 # 鍵の生成
 #key = 'abcdefghijklmnop'.encode()
 key = '12345678901234567890123456789012'.encode()
 # IVの生成
 iv = '1234567890123456'.encode()
 
-cr = JcCrypto(key, iv)
+cr = AES(key, iv)
 
 print("")
 encoded = cr.encode_text(text)
 print("encoded={}".format(encoded))
 decoded = cr.decode_text(encoded)
 print("decoded={}".format(decoded))
```

