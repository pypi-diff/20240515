# Comparing `tmp/cryptojwt-1.9.0.tar.gz` & `tmp/cryptojwt-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptojwt-1.9.0.tar", max compression
+gzip compressed data, was "cryptojwt-1.9.1.tar", max compression
```

## Comparing `cryptojwt-1.9.0.tar` & `cryptojwt-1.9.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rwxr-xr-x   0        0        0    10759 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/LICENSE
--rw-r--r--   0        0        0      576 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/README.md
--rw-r--r--   0        0        0     1317 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      877 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/__init__.py
--rw-r--r--   0        0        0     1872 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/exception.py
--rw-r--r--   0        0        0     1119 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/__init__.py
--rw-r--r--   0        0        0     4388 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/aes.py
--rw-r--r--   0        0        0      606 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/exception.py
--rw-r--r--   0        0        0     2064 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/fernet.py
--rw-r--r--   0        0        0     7204 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/jwe.py
--rw-r--r--   0        0        0     7769 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/jwe_ec.py
--rw-r--r--   0        0        0     3050 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/jwe_hmac.py
--rw-r--r--   0        0        0     3638 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/jwe_rsa.py
--rw-r--r--   0        0        0     2749 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/jwekey.py
--rw-r--r--   0        0        0     1414 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/jwenc.py
--rw-r--r--   0        0        0     1775 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/rsa.py
--rw-r--r--   0        0        0     2910 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/utils.py
--rw-r--r--   0        0        0    10835 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/__init__.py
--rw-r--r--   0        0        0     1906 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/asym.py
--rw-r--r--   0        0        0    11294 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/ec.py
--rw-r--r--   0        0        0     4607 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/hmac.py
--rw-r--r--   0        0        0     8078 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/jwk.py
--rw-r--r--   0        0        0    11985 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/okp.py
--rw-r--r--   0        0        0    15334 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/rsa.py
--rw-r--r--   0        0        0      728 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/utils.py
--rw-r--r--   0        0        0      905 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/wrap.py
--rw-r--r--   0        0        0     4102 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/x509.py
--rw-r--r--   0        0        0      354 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/__init__.py
--rw-r--r--   0        0        0     3962 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/dsa.py
--rw-r--r--   0        0        0     2630 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/eddsa.py
--rw-r--r--   0        0        0      329 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/exception.py
--rw-r--r--   0        0        0     1535 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/hmac.py
--rw-r--r--   0        0        0    15416 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/jws.py
--rw-r--r--   0        0        0     2183 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/pss.py
--rw-r--r--   0        0        0     1580 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/rsa.py
--rw-r--r--   0        0        0     2831 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/jws/utils.py
--rwxr-xr-x   0        0        0    14149 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/jwt.py
--rw-r--r--   0        0        0     8719 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/jwx.py
--rwxr-xr-x   0        0        0    40515 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/key_bundle.py
--rwxr-xr-x   0        0        0    21135 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/key_issuer.py
--rwxr-xr-x   0        0        0    29558 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/key_jar.py
--rw-r--r--   0        0        0        0 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/serialize/__init__.py
--rw-r--r--   0        0        0      472 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/serialize/item.py
--rw-r--r--   0        0        0     4504 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/simple_jwt.py
--rw-r--r--   0        0        0        0 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/tools/__init__.py
--rwxr-xr-x   0        0        0     4221 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/tools/jwtpeek.py
--rw-r--r--   0        0        0     7481 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/tools/keyconv.py
--rw-r--r--   0        0        0     2522 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/tools/keygen.py
--rw-r--r--   0        0        0     8709 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/utils.py
--rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 cryptojwt-1.9.0/PKG-INFO
+-rwxr-xr-x   0        0        0    10759 2024-05-15 07:35:51.528498 cryptojwt-1.9.1/LICENSE
+-rw-r--r--   0        0        0      576 2024-05-15 07:35:51.528498 cryptojwt-1.9.1/README.md
+-rw-r--r--   0        0        0     1317 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      878 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/__init__.py
+-rw-r--r--   0        0        0     1872 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/exception.py
+-rw-r--r--   0        0        0     1119 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwe/__init__.py
+-rw-r--r--   0        0        0     4250 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwe/aes.py
+-rw-r--r--   0        0        0      606 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwe/exception.py
+-rw-r--r--   0        0        0     2064 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwe/fernet.py
+-rw-r--r--   0        0        0     7204 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwe/jwe.py
+-rw-r--r--   0        0        0     7663 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwe/jwe_ec.py
+-rw-r--r--   0        0        0     2955 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwe/jwe_hmac.py
+-rw-r--r--   0        0        0     3638 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwe/jwe_rsa.py
+-rw-r--r--   0        0        0     2749 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwe/jwekey.py
+-rw-r--r--   0        0        0     1414 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwe/jwenc.py
+-rw-r--r--   0        0        0     1775 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwe/rsa.py
+-rw-r--r--   0        0        0     2826 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwe/utils.py
+-rw-r--r--   0        0        0    10835 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwk/__init__.py
+-rw-r--r--   0        0        0     1906 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwk/asym.py
+-rw-r--r--   0        0        0    11178 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwk/ec.py
+-rw-r--r--   0        0        0     4607 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwk/hmac.py
+-rw-r--r--   0        0        0     7901 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwk/jwk.py
+-rw-r--r--   0        0        0    11985 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwk/okp.py
+-rw-r--r--   0        0        0    15161 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwk/rsa.py
+-rw-r--r--   0        0        0      728 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwk/utils.py
+-rw-r--r--   0        0        0      905 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwk/wrap.py
+-rw-r--r--   0        0        0     3904 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwk/x509.py
+-rw-r--r--   0        0        0      354 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jws/__init__.py
+-rw-r--r--   0        0        0     3962 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jws/dsa.py
+-rw-r--r--   0        0        0     2630 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jws/eddsa.py
+-rw-r--r--   0        0        0      329 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jws/exception.py
+-rw-r--r--   0        0        0     1440 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jws/hmac.py
+-rw-r--r--   0        0        0    15417 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jws/jws.py
+-rw-r--r--   0        0        0     2099 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jws/pss.py
+-rw-r--r--   0        0        0     1580 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jws/rsa.py
+-rw-r--r--   0        0        0     2831 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jws/utils.py
+-rwxr-xr-x   0        0        0    14150 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwt.py
+-rw-r--r--   0        0        0     8720 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/jwx.py
+-rwxr-xr-x   0        0        0    40515 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/key_bundle.py
+-rwxr-xr-x   0        0        0    21135 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/key_issuer.py
+-rwxr-xr-x   0        0        0    29558 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/key_jar.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/serialize/__init__.py
+-rw-r--r--   0        0        0      472 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/serialize/item.py
+-rw-r--r--   0        0        0     4504 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/simple_jwt.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/tools/__init__.py
+-rwxr-xr-x   0        0        0     4221 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/tools/jwtpeek.py
+-rw-r--r--   0        0        0     7481 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/tools/keyconv.py
+-rw-r--r--   0        0        0     2522 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/tools/keygen.py
+-rw-r--r--   0        0        0     8709 2024-05-15 07:35:51.532498 cryptojwt-1.9.1/src/cryptojwt/utils.py
+-rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 cryptojwt-1.9.1/PKG-INFO
```

### Comparing `cryptojwt-1.9.0/LICENSE` & `cryptojwt-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/README.md` & `cryptojwt-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/pyproject.toml` & `cryptojwt-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 exclude_lines = [
     "pragma: no cover",
     "raise NotImplementedError",
 ]
 
 [tool.poetry]
 name = "cryptojwt"
-version = "1.9.0"
+version = "1.9.1"
 description = "Python implementation of JWT, JWE, JWS and JWK"
 authors = ["Roland Hedberg <roland@catalogix.se>"]
 license = "Apache-2.0"
 repository = "https://github.com/IdentityPython/JWTConnect-Python-CryptoJWT"
 readme = "README.md"
 packages = [
     { include = "cryptojwt", from = "src" }
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/__init__.py` & `cryptojwt-1.9.1/src/cryptojwt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """JSON Web Token"""
+
 import logging
 
 import pkg_resources
 
 from cryptojwt.jwe.jwe import JWE
 from cryptojwt.jwk import JWK
 from cryptojwt.jws.jws import JWS
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/exception.py` & `cryptojwt-1.9.1/src/cryptojwt/exception.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwe/__init__.py` & `cryptojwt-1.9.1/src/cryptojwt/jwe/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwe/aes.py` & `cryptojwt-1.9.1/src/cryptojwt/jwe/aes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 from struct import pack
 
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hmac
 from cryptography.hazmat.primitives.ciphers import Cipher
 from cryptography.hazmat.primitives.ciphers import algorithms
 from cryptography.hazmat.primitives.ciphers import modes
 from cryptography.hazmat.primitives.ciphers.aead import AESGCM
 from cryptography.hazmat.primitives.padding import PKCS7
 
@@ -33,15 +32,15 @@
         else:
             raise Unsupported("Message padding: {}".format(msg_padding))
 
         self.iv = None
 
     def _mac(self, hash_key, hash_func, auth_data, iv, enc_msg, key_len):
         al = pack("!Q", 8 * len(auth_data))
-        h = hmac.HMAC(hash_key, hash_func(), backend=default_backend())
+        h = hmac.HMAC(hash_key, hash_func())
         h.update(auth_data)
         h.update(iv)
         h.update(enc_msg)
         h.update(al)
         m = h.finalize()
         return m[:key_len]
 
@@ -50,15 +49,15 @@
             iv = os.urandom(16)
             self.iv = iv
         else:
             self.iv = iv
 
         hash_key, enc_key, key_len, hash_func = get_keys_seclen_dgst(self.key, iv)
 
-        cipher = Cipher(algorithms.AES(enc_key), modes.CBC(iv), backend=default_backend())
+        cipher = Cipher(algorithms.AES(enc_key), modes.CBC(iv))
         encryptor = cipher.encryptor()
 
         pmsg = self.padder.update(msg)
         pmsg += self.padder.finalize()
         ct = encryptor.update(pmsg)
         ct += encryptor.finalize()
         tag = self._mac(hash_key, hash_func, auth_data, iv, ct, key_len)
@@ -73,15 +72,15 @@
 
         hash_key, enc_key, key_len, hash_func = get_keys_seclen_dgst(key, iv)
 
         comp_tag = self._mac(hash_key, hash_func, auth_data, iv, msg, key_len)
         if comp_tag != tag:
             raise VerificationError("AES-CBC HMAC")
 
-        cipher = Cipher(algorithms.AES(enc_key), modes.CBC(iv), backend=default_backend())
+        cipher = Cipher(algorithms.AES(enc_key), modes.CBC(iv))
         decryptor = cipher.decryptor()
 
         ctext = decryptor.update(msg)
         ctext += decryptor.finalize()
         unpad = self.unpadder.update(ctext)
         unpad += self.unpadder.finalize()
         return unpad
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwe/exception.py` & `cryptojwt-1.9.1/src/cryptojwt/jwe/exception.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwe/fernet.py` & `cryptojwt-1.9.1/src/cryptojwt/jwe/fernet.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwe/jwe.py` & `cryptojwt-1.9.1/src/cryptojwt/jwe/jwe.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwe/jwe_ec.py` & `cryptojwt-1.9.1/src/cryptojwt/jwe/jwe_ec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import struct
 
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.keywrap import aes_key_unwrap
 from cryptography.hazmat.primitives.keywrap import aes_key_wrap
 
 from ..jwk.ec import NIST2SEC
 from ..jwk.ec import ECKey
 from ..utils import as_bytes
@@ -83,15 +82,15 @@
             raise ValueError("EC Key Required for ECDH-ES JWE Encryption Setup")
 
         # epk is either an Elliptic curve key instance or a JWK description of
         # one. This key belongs to the entity on the other side.
         try:
             _epk = kwargs["epk"]
         except KeyError:
-            _epk = ec.generate_private_key(NIST2SEC[as_unicode(key.crv)], default_backend())
+            _epk = ec.generate_private_key(curve=NIST2SEC[as_unicode(key.crv)]())
             epk = ECKey().load_key(_epk.public_key())
         else:
             if isinstance(_epk, ec.EllipticCurvePrivateKey):
                 epk = ECKey().load_key(_epk)
             elif isinstance(_epk, ECKey):
                 epk = _epk
                 _epk = epk.private_key()
@@ -116,15 +115,15 @@
 
             cek = ecdh_derive_key(_epk, key.pub_key, apu, apv, str(self.enc).encode(), dk_len)
         elif self.alg in ["ECDH-ES+A128KW", "ECDH-ES+A192KW", "ECDH-ES+A256KW"]:
             _pre, _post = self.alg.split("+")
             klen = int(_post[1:4])
             kek = ecdh_derive_key(_epk, key.pub_key, apu, apv, str(_post).encode(), klen)
             cek = self._generate_key(self.enc, cek=cek)
-            encrypted_key = aes_key_wrap(kek, cek, default_backend())
+            encrypted_key = aes_key_wrap(kek, cek)
         else:
             raise Exception("Unsupported algorithm %s" % self.alg)
 
         return cek, encrypted_key, iv, params, epk
 
     def dec_setup(self, token, key=None, **kwargs):
         """
@@ -168,15 +167,15 @@
             "ECDH-ES+A128KW",
             "ECDH-ES+A192KW",
             "ECDH-ES+A256KW",
         ]:
             _pre, _post = self.headers["alg"].split("+")
             klen = int(_post[1:4])
             kek = ecdh_derive_key(key, epubkey.pub_key, apu, apv, str(_post).encode(), klen)
-            self.cek = aes_key_unwrap(kek, token.encrypted_key(), default_backend())
+            self.cek = aes_key_unwrap(kek, token.encrypted_key())
         else:
             raise Exception("Unsupported algorithm %s" % self.headers["alg"])
 
         return self.cek
 
     def encrypt(self, key=None, iv="", cek="", **kwargs):
         """
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwe/jwe_hmac.py` & `cryptojwt-1.9.1/src/cryptojwt/jwe/jwe_hmac.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import zlib
 
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.keywrap import aes_key_unwrap
 from cryptography.hazmat.primitives.keywrap import aes_key_wrap
 
 from ..exception import MissingKey
 from ..exception import WrongNumberOfParts
 from ..jwk.hmac import SYMKey
 from ..utils import as_bytes
@@ -53,15 +52,15 @@
         elif isinstance(key, bytes):
             kek = key
         else:
             kek = intarr2str(key)
 
         # The iv for this function must be 64 bit
         # Which is certainly different from the one above
-        jek = aes_key_wrap(kek, cek, default_backend())
+        jek = aes_key_wrap(kek, cek)
 
         _enc = self["enc"]
         _auth_data = jwe.b64_encode_header()
         ctxt, tag, cek = self.enc_setup(_enc, _msg, auth_data=_auth_data, key=cek, iv=iv)
         return jwe.pack(parts=[jek, iv, ctxt, tag])
 
     def decrypt(self, token, key=None, cek=None):
@@ -81,15 +80,15 @@
             jek = jwe.encrypted_key()
             if isinstance(key, SYMKey):
                 try:
                     key = key.key.encode("utf8")
                 except AttributeError:
                     key = key.key
             # The iv for this function must be 64 bit
-            cek = aes_key_unwrap(key, jek, default_backend())
+            cek = aes_key_unwrap(key, jek)
 
         auth_data = jwe.b64_protected_header()
         msg = self._decrypt(
             jwe.headers["enc"],
             cek,
             jwe.ciphertext(),
             auth_data=auth_data,
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwe/jwe_rsa.py` & `cryptojwt-1.9.1/src/cryptojwt/jwe/jwe_rsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwe/jwekey.py` & `cryptojwt-1.9.1/src/cryptojwt/jwe/jwekey.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwe/jwenc.py` & `cryptojwt-1.9.1/src/cryptojwt/jwe/jwenc.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwe/rsa.py` & `cryptojwt-1.9.1/src/cryptojwt/jwe/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwe/utils.py` & `cryptojwt-1.9.1/src/cryptojwt/jwe/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import struct
 from math import ceil
 
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.hashes import SHA256
 from cryptography.hazmat.primitives.hashes import SHA384
 from cryptography.hazmat.primitives.hashes import SHA512
 
 from ..utils import b64e
 
@@ -103,13 +102,13 @@
     """
     dkm = b""
     dk_bytes = int(ceil(dk_len / 8.0))
     counter = 0
     while len(dkm) < dk_bytes:
         counter += 1
         counter_bytes = struct.pack("!I", counter)
-        digest = hashes.Hash(hashes.SHA256(), backend=default_backend())
+        digest = hashes.Hash(hashes.SHA256())
         digest.update(counter_bytes)
         digest.update(secret)
         digest.update(other_info)
         dkm += digest.finalize()
     return dkm[:dk_bytes]
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwk/__init__.py` & `cryptojwt-1.9.1/src/cryptojwt/jwk/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwk/asym.py` & `cryptojwt-1.9.1/src/cryptojwt/jwk/asym.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwk/ec.py` & `cryptojwt-1.9.1/src/cryptojwt/jwk/ec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric import ec
 
 from cryptojwt.exception import KeyNotFound
 
 from ..exception import DeSerializationNotPossible
 from ..exception import JWKESTException
 from ..exception import UnsupportedECurve
@@ -46,29 +45,29 @@
     """
     try:
         _sec_crv = NIST2SEC[as_unicode(num["crv"])]
     except KeyError:
         raise UnsupportedECurve("Unsupported elliptic curve: {}".format(num["crv"]))
 
     ecpn = ec.EllipticCurvePublicNumbers(num["x"], num["y"], _sec_crv())
-    return ecpn.public_key(default_backend())
+    return ecpn.public_key()
 
 
 def ec_construct_private(num):
     """
     Given a set of values on public and private attributes build an elliptic
     curve private key instance.
 
     :param num: A dictionary with public and private attributes and their values
     :return: A cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey
         instance.
     """
     pub_ecpn = ec.EllipticCurvePublicNumbers(num["x"], num["y"], NIST2SEC[as_unicode(num["crv"])]())
     priv_ecpn = ec.EllipticCurvePrivateNumbers(num["d"], pub_ecpn)
-    return priv_ecpn.private_key(default_backend())
+    return priv_ecpn.private_key()
 
 
 class ECKey(AsymmetricKey):
     """
     JSON Web key representation of a Elliptic curve key.
     According to RFC 7517 a JWK representation of a EC key can look like
     this::
@@ -281,15 +280,15 @@
                     return False
             return True
 
     return False
 
 
 def new_ec_key(crv, kid="", **kwargs):
-    _key = ec.generate_private_key(curve=NIST2SEC[crv], backend=default_backend())
+    _key = ec.generate_private_key(curve=NIST2SEC[crv]())
 
     _rk = ECKey(priv_key=_key, kid=kid, **kwargs)
     if not kid:
         _rk.add_kid()
 
     return _rk
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwk/hmac.py` & `cryptojwt-1.9.1/src/cryptojwt/jwk/hmac.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwk/jwk.py` & `cryptojwt-1.9.1/src/cryptojwt/jwk/jwk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import copy
 import json
 import os
 
-from cryptography.hazmat import backends
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.asymmetric import ed448
 from cryptography.hazmat.primitives.asymmetric import ed25519
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.hazmat.primitives.asymmetric.rsa import rsa_crt_dmp1
 from cryptography.hazmat.primitives.asymmetric.rsa import rsa_crt_dmq1
 from cryptography.hazmat.primitives.asymmetric.rsa import rsa_crt_iqmp
@@ -101,26 +100,24 @@
         if _jwk_dict["crv"] in NIST2SEC:
             curve = NIST2SEC[_jwk_dict["crv"]]()
         else:
             raise UnsupportedAlgorithm("Unknown curve: %s" % (_jwk_dict["crv"]))
 
         if _jwk_dict.get("d", None) is not None:
             # Ecdsa private key.
-            _jwk_dict["priv_key"] = ec.derive_private_key(
-                base64url_to_long(_jwk_dict["d"]), curve, backends.default_backend()
-            )
+            _jwk_dict["priv_key"] = ec.derive_private_key(base64url_to_long(_jwk_dict["d"]), curve)
             _jwk_dict["pub_key"] = _jwk_dict["priv_key"].public_key()
         else:
             # Ecdsa public key.
             ec_pub_numbers = ec.EllipticCurvePublicNumbers(
                 base64url_to_long(_jwk_dict["x"]),
                 base64url_to_long(_jwk_dict["y"]),
                 curve,
             )
-            _jwk_dict["pub_key"] = ec_pub_numbers.public_key(backends.default_backend())
+            _jwk_dict["pub_key"] = ec_pub_numbers.public_key()
         return ECKey(**_jwk_dict)
     elif _jwk_dict["kty"] == "RSA":
         ensure_rsa_params(_jwk_dict, private)
 
         if private is not None and not private:
             # remove private components
             for v in RSA_PRIVATE:
@@ -147,18 +144,18 @@
                 qi_long = rsa_crt_iqmp(p_long, q_long)
             else:
                 qi_long = base64url_to_long(_jwk_dict["qi"])
 
             rsa_priv_numbers = rsa.RSAPrivateNumbers(
                 p_long, q_long, d_long, dp_long, dq_long, qi_long, rsa_pub_numbers
             )
-            _jwk_dict["priv_key"] = rsa_priv_numbers.private_key(backends.default_backend())
+            _jwk_dict["priv_key"] = rsa_priv_numbers.private_key()
             _jwk_dict["pub_key"] = _jwk_dict["priv_key"].public_key()
         else:
-            _jwk_dict["pub_key"] = rsa_pub_numbers.public_key(backends.default_backend())
+            _jwk_dict["pub_key"] = rsa_pub_numbers.public_key()
 
         if _jwk_dict["kty"] != "RSA":
             raise WrongKeyType('"{}" should have been "RSA"'.format(_jwk_dict["kty"]))
         return RSAKey(**_jwk_dict)
     elif _jwk_dict["kty"] == "OKP":
         ensure_okp_params(_jwk_dict, private)
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwk/okp.py` & `cryptojwt-1.9.1/src/cryptojwt/jwk/okp.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwk/rsa.py` & `cryptojwt-1.9.1/src/cryptojwt/jwk/rsa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import base64
 import logging
 
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 
 from cryptojwt.exception import KeyNotFound
 
 from ..exception import DeSerializationNotPossible
 from ..exception import JWKESTException
@@ -36,17 +35,15 @@
     :param key_size: The size of the key, default 2048 bytes.
     :param filename: The name of the file to which the key should be written
     :param passphrase: If the PEM representation should be protected with a
         pass phrase.
     :return: A
         cryptography.hazmat.primitives.asymmetric.rsa.RSAPrivateKey instance
     """
-    private_key = rsa.generate_private_key(
-        public_exponent=65537, key_size=key_size, backend=default_backend()
-    )
+    private_key = rsa.generate_private_key(public_exponent=65537, key_size=key_size)
 
     with open(filename, "wb") as keyfile:
         if passphrase:
             pem = private_key.private_bytes(
                 encoding=serialization.Encoding.PEM,
                 format=serialization.PrivateFormat.PKCS8,
                 encryption_algorithm=serialization.BestAvailableEncryption(passphrase),
@@ -137,15 +134,15 @@
     pub_key = import_rsa_key(txt)
     if isinstance(pub_key, rsa.RSAPublicKey):
         return [("rsa", pub_key)]
 
 
 def rsa_construct_public(numbers):
     rpn = rsa.RSAPublicNumbers(**numbers)
-    return rpn.public_key(default_backend())
+    return rpn.public_key()
 
 
 def rsa_construct_private(numbers):
     args = dict([(k, v) for k, v in numbers.items() if k in ["n", "e", "d"]])
     cnum = {"d": numbers["d"]}
     if "p" not in numbers and "q" not in numbers:
         (p, q) = rsa.rsa_recover_prime_factors(**args)
@@ -177,15 +174,15 @@
         cnum["iqmp"] = rsa.rsa_crt_iqmp(cnum["p"], cnum["q"])
     else:
         if not numbers["di"]:
             cnum["iqmp"] = rsa.rsa_crt_iqmp(cnum["p"], cnum["q"])
 
     rpubn = rsa.RSAPublicNumbers(e=numbers["e"], n=numbers["n"])
     rprivn = rsa.RSAPrivateNumbers(public_numbers=rpubn, **cnum)
-    return rprivn.private_key(default_backend())
+    return rprivn.private_key()
 
 
 def cmp_public_numbers(pn1, pn2):
     """
     Compare 2 sets of public numbers. These is a way to compare
     2 public RSA keys. If the sets are the same then the keys are the same.
 
@@ -488,16 +485,14 @@
 
     :param key_size: The size of the key
     :param kid: The key ID
     :param public_exponent: The value of the public exponent.
     :return: A :py:class:`cryptojwt.jwk.rsa.RSAKey` instance
     """
 
-    _key = rsa.generate_private_key(
-        public_exponent=public_exponent, key_size=key_size, backend=default_backend()
-    )
+    _key = rsa.generate_private_key(public_exponent=public_exponent, key_size=key_size)
 
     _rk = RSAKey(priv_key=_key, kid=kid, **kwargs)
     if not _rk.kid:
         _rk.add_kid()
 
     return _rk
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwk/utils.py` & `cryptojwt-1.9.1/src/cryptojwt/jwk/utils.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwk/wrap.py` & `cryptojwt-1.9.1/src/cryptojwt/jwk/wrap.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwk/x509.py` & `cryptojwt-1.9.1/src/cryptojwt/jwk/x509.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import base64
 import hashlib
 import logging
 
 from cryptography import x509
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.asymmetric import rsa
 
 from cryptojwt.utils import b64e
 
 logger = logging.getLogger(__name__)
@@ -18,30 +17,28 @@
     Read a public RSA key from a PEM file.
 
     :param filename: The name of the file
     :param passphrase: A pass phrase to use to unpack the PEM file.
     :return: A public key instance
     """
     with open(filename, "rb") as key_file:
-        public_key = serialization.load_pem_public_key(key_file.read(), backend=default_backend())
+        public_key = serialization.load_pem_public_key(key_file.read())
     return public_key
 
 
 def import_private_key_from_pem_file(filename, passphrase=None):
     """
     Read a private RSA key from a PEM file.
 
     :param filename: The name of the file
     :param passphrase: A pass phrase to use to unpack the PEM file.
     :return: A private key instance
     """
     with open(filename, "rb") as key_file:
-        private_key = serialization.load_pem_private_key(
-            key_file.read(), password=passphrase, backend=default_backend()
-        )
+        private_key = serialization.load_pem_private_key(key_file.read(), password=passphrase)
     return private_key
 
 
 PREFIX = "-----BEGIN CERTIFICATE-----"
 POSTFIX = "-----END CERTIFICATE-----"
 
 
@@ -52,40 +49,40 @@
     :param pem_data: RSA key encoded in standard form
     :return: rsa.RSAPublicKey instance
     """
     if not pem_data.startswith(PREFIX):
         pem_data = bytes("{}\n{}\n{}".format(PREFIX, pem_data, POSTFIX), "utf-8")
     else:
         pem_data = bytes(pem_data, "utf-8")
-    cert = x509.load_pem_x509_certificate(pem_data, default_backend())
+    cert = x509.load_pem_x509_certificate(pem_data)
     return cert.public_key()
 
 
 def import_public_key_from_cert_file(filename):
     """
     Read a public key from a certificate file.
 
     :param filename: The name of the file
     :return: A public key instance
     """
     with open(filename, "rb") as key_file:
-        cert = x509.load_pem_x509_certificate(key_file.read(), backend=default_backend())
+        cert = x509.load_pem_x509_certificate(key_file.read())
     return cert.public_key()
 
 
 def der_cert(der_data):
     """
     Load a DER encoded certificate
 
     :param der_data: DER-encoded certificate
     :return: A cryptography.x509.certificate instance
     """
     if isinstance(der_data, str):
         der_data = bytes(der_data, "utf-8")
-    return x509.load_der_x509_certificate(der_data, default_backend())
+    return x509.load_der_x509_certificate(der_data)
 
 
 def load_x509_cert(url, httpc, spec2key, **get_args):
     """
     Get and transform a X509 cert into a key.
 
     :param url: Where the X509 cert can be found
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jws/dsa.py` & `cryptojwt-1.9.1/src/cryptojwt/jws/dsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jws/eddsa.py` & `cryptojwt-1.9.1/src/cryptojwt/jws/eddsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jws/hmac.py` & `cryptojwt-1.9.1/src/cryptojwt/jws/hmac.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives import hmac
 
 from ..exception import Unsupported
 from . import Signer
 
 
@@ -22,28 +21,28 @@
         Create a signature over a message as defined in RFC7515 using a
         symmetric key
 
         :param msg: The message
         :param key: The key
         :return: A signature
         """
-        h = hmac.HMAC(key, self.algorithm(), default_backend())
+        h = hmac.HMAC(key, self.algorithm())
         h.update(msg)
         return h.finalize()
 
     def verify(self, msg, sig, key):
         """
         Verifies whether sig is the correct message authentication code of data.
 
         :param msg: The data
         :param sig: The message authentication code to verify against data.
         :param key: The key to use
         :return: Returns true if the mac was valid otherwise it will raise an
             Exception.
         """
         try:
-            h = hmac.HMAC(key, self.algorithm(), default_backend())
+            h = hmac.HMAC(key, self.algorithm())
             h.update(msg)
             h.verify(sig)
             return True
         except:
             return False
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jws/jws.py` & `cryptojwt-1.9.1/src/cryptojwt/jws/jws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """JSON Web Token"""
+
 import json
 import logging
 
 from cryptojwt.jws.exception import JWSException
 
 from ..exception import BadSignature
 from ..exception import UnknownAlgorithm
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jws/pss.py` & `cryptojwt-1.9.1/src/cryptojwt/jws/pss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 
 from cryptography.exceptions import InvalidSignature
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.hazmat.primitives.asymmetric import utils
 
 from ..exception import BadSignature
 from ..exception import Unsupported
 from . import Signer
@@ -28,15 +27,15 @@
         """
         Create a signature over a message
 
         :param msg: The message
         :param key: The key
         :return: A signature
         """
-        hasher = hashes.Hash(self.hash_algorithm(), backend=default_backend())
+        hasher = hashes.Hash(self.hash_algorithm())
         hasher.update(msg)
         digest = hasher.finalize()
         sig = key.sign(
             digest,
             padding.PSS(
                 mgf=padding.MGF1(self.hash_algorithm()),
                 salt_length=padding.PSS.MAX_LENGTH,
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jws/rsa.py` & `cryptojwt-1.9.1/src/cryptojwt/jws/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jws/utils.py` & `cryptojwt-1.9.1/src/cryptojwt/jws/utils.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwt.py` & `cryptojwt-1.9.1/src/cryptojwt/jwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Basic JSON Web Token implementation."""
+
 import json
 import logging
 import time
 import uuid
 from json import JSONDecodeError
 from typing import Dict
 from typing import List
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/jwx.py` & `cryptojwt-1.9.1/src/cryptojwt/jwx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A basic class on which to build the JWS and JWE classes."""
+
 import json
 import logging
 import warnings
 
 import requests
 
 from cryptojwt.jwk import JWK
```

### Comparing `cryptojwt-1.9.0/src/cryptojwt/key_bundle.py` & `cryptojwt-1.9.1/src/cryptojwt/key_bundle.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/key_issuer.py` & `cryptojwt-1.9.1/src/cryptojwt/key_issuer.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/key_jar.py` & `cryptojwt-1.9.1/src/cryptojwt/key_jar.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/simple_jwt.py` & `cryptojwt-1.9.1/src/cryptojwt/simple_jwt.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/tools/jwtpeek.py` & `cryptojwt-1.9.1/src/cryptojwt/tools/jwtpeek.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/tools/keyconv.py` & `cryptojwt-1.9.1/src/cryptojwt/tools/keyconv.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/tools/keygen.py` & `cryptojwt-1.9.1/src/cryptojwt/tools/keygen.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/src/cryptojwt/utils.py` & `cryptojwt-1.9.1/src/cryptojwt/utils.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.9.0/PKG-INFO` & `cryptojwt-1.9.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptojwt
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python implementation of JWT, JWE, JWS and JWK
 Home-page: https://github.com/IdentityPython/JWTConnect-Python-CryptoJWT
 License: Apache-2.0
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

