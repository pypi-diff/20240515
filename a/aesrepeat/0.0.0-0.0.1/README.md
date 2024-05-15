# Comparing `tmp/aesrepeat-0.0.0-py3-none-any.whl.zip` & `tmp/aesrepeat-0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2053 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     2943 b- defN 24-May-15 13:13 aesrepeat/__init__.py
--rw-rw-rw-  2.0 fat      573 b- defN 24-May-15 13:13 aesrepeat-0.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 13:13 aesrepeat-0.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-May-15 13:13 aesrepeat-0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      383 b- defN 24-May-15 13:13 aesrepeat-0.0.0.dist-info/RECORD
-5 files, 4001 bytes uncompressed, 1337 bytes compressed:  66.6%
+Zip file size: 2307 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     2548 b- defN 24-May-15 14:30 aesrepeat/__init__.py
+-rw-rw-rw-  2.0 fat     1870 b- defN 24-May-15 14:30 aesrepeat-0.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 14:30 aesrepeat-0.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-15 14:30 aesrepeat-0.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      384 b- defN 24-May-15 14:30 aesrepeat-0.0.1.dist-info/RECORD
+5 files, 4904 bytes uncompressed, 1591 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: aesrepeat/__init__.py
 Comment: 
 
-Filename: aesrepeat-0.0.0.dist-info/METADATA
+Filename: aesrepeat-0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: aesrepeat-0.0.0.dist-info/WHEEL
+Filename: aesrepeat-0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: aesrepeat-0.0.0.dist-info/top_level.txt
+Filename: aesrepeat-0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: aesrepeat-0.0.0.dist-info/RECORD
+Filename: aesrepeat-0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aesrepeat/__init__.py

```diff
@@ -1,70 +1,68 @@
-# pip install PyCryptoDome
-from Crypto.Cipher import AES as ___AES__
+from aesrepeat.internal import *
 import base64
-import hashlib
 import pickle
 
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '0.0.0'
+__version__      = '0.0.1'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/lang-library/py-aesrepeat'
-__all__ = ['AES', 'AES128FromString', 'AES256FromString']
+__all__ = ['AES128', 'AES256']
 
-def AES128FromString(str):
-    sha256 = hashlib.sha256(str.encode())
-    digets = sha256.digest()
-    upper16 = digets[0:16]
-    lower16 = digets[16:]
-    return AES(upper16, lower16)
-
-def AES256FromString(str):
-    sha384 = hashlib.sha384(str.encode())
-    digets = sha384.digest()
-    upper32 = digets[0:32]
-    lower16 = digets[32:]
-    return AES(upper32, lower16)
-
-class AES:
-    def __init__(self, key, iv):
-        self.cipher = ___AES__.new(key, ___AES__.MODE_CBC, iv)
-        self.decipher = ___AES__.new(key, ___AES__.MODE_CBC, iv)
+class AES128:
+    def __init__(self, password_list):
+        self.password_list = password_list
+        self.reverse_password_list = list(reversed(self.password_list))
+    def encode_bytes(self, data):
+        for p in self.password_list:
+            aes = AES128FromString(p)
+            data = aes.encode_bytes(data)
+        return base64.b64encode(data).decode()
+    def decode_bytes(self, base64_text):
+        data = base64.b64decode(base64_text.encode())
+        for p in self.reverse_password_list:
+            aes = AES128FromString(p)
+            data = aes.decode_bytes(data)
+        return data
     def encode_text(self, plain_text):
         data = plain_text.encode()
-        block_size = ___AES__.block_size
-        padding_size = block_size - (len(data) % block_size)
-        padded_data = data + bytes([padding_size]) * padding_size
-        encrypted_data = self.cipher.encrypt(padded_data)
-        return base64.b64encode(encrypted_data).decode()
+        return self.encode_bytes(data)
     def decode_text(self, base64_text):
-        encrypted_data = base64.b64decode(base64_text.encode())
-        decrypted_data = self.decipher.decrypt(encrypted_data)
-        padding_size = decrypted_data[-1]
-        unpadded_data = decrypted_data[:-padding_size]
-        return unpadded_data.decode()
+        data = self.decode_bytes(base64_text)
+        return data.decode()
+    def encode_pickle(self, x, protocol=3):
+        data = pickle.dumps(x, protocol=protocol)
+        return self.encode_bytes(data)
+    def decode_pickle(self, base64_text):
+        data = self.decode_bytes(base64_text)
+        return pickle.loads(data)
+ 
+class AES256:
+    def __init__(self, password_list):
+        self.password_list = password_list
+        self.reverse_password_list = list(reversed(self.password_list))
     def encode_bytes(self, data):
-        block_size = ___AES__.block_size
-        padding_size = block_size - (len(data) % block_size)
-        padded_data = data + bytes([padding_size]) * padding_size
-        encrypted_data = self.cipher.encrypt(padded_data)
-        return base64.b64encode(encrypted_data).decode()
+        for p in self.password_list:
+            aes = AES256FromString(p)
+            data = aes.encode_bytes(data)
+        return base64.b64encode(data).decode()
     def decode_bytes(self, base64_text):
-        encrypted_data = base64.b64decode(base64_text.encode())
-        decrypted_data = self.decipher.decrypt(encrypted_data)
-        padding_size = decrypted_data[-1]
-        unpadded_data = decrypted_data[:-padding_size]
-        return unpadded_data
+        data = base64.b64decode(base64_text.encode())
+        for p in self.reverse_password_list:
+            aes = AES256FromString(p)
+            data = aes.decode_bytes(data)
+        return data
+    def encode_text(self, plain_text):
+        data = plain_text.encode()
+        return self.encode_bytes(data)
+    def decode_text(self, base64_text):
+        data = self.decode_bytes(base64_text)
+        return data.decode()
     def encode_pickle(self, x, protocol=3):
         data = pickle.dumps(x, protocol=protocol)
-        block_size = ___AES__.block_size
-        padding_size = block_size - (len(data) % block_size)
-        padded_data = data + bytes([padding_size]) * padding_size
-        encrypted_data = self.cipher.encrypt(padded_data)
-        return base64.b64encode(encrypted_data).decode()
+        return self.encode_bytes(data)
     def decode_pickle(self, base64_text):
-        encrypted_data = base64.b64decode(base64_text.encode())
-        decrypted_data = self.decipher.decrypt(encrypted_data)
-        padding_size = decrypted_data[-1]
-        unpadded_data = decrypted_data[:-padding_size]
-        return pickle.loads(unpadded_data)
+        data = self.decode_bytes(base64_text)
+        return pickle.loads(data)
+
```

