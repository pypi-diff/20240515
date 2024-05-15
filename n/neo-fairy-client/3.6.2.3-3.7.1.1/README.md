# Comparing `tmp/neo-fairy-client-3.6.2.3.tar.gz` & `tmp/neo_fairy_client-3.7.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo-fairy-client-3.6.2.3.tar", last modified: Tue Jan 30 05:02:01 2024, max compression
+gzip compressed data, was "neo_fairy_client-3.7.1.1.tar", last modified: Wed May 15 04:17:18 2024, max compression
```

## Comparing `neo-fairy-client-3.6.2.3.tar` & `neo_fairy_client-3.7.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-01-30 05:02:01.520897 neo-fairy-client-3.6.2.3/
--rw-rw-rw-   0        0        0     1085 2022-05-05 03:19:19.000000 neo-fairy-client-3.6.2.3/LICENSE
--rw-rw-rw-   0        0        0   139484 2024-01-30 05:02:01.519895 neo-fairy-client-3.6.2.3/PKG-INFO
--rw-rw-rw-   0        0        0   138993 2023-08-24 03:08:32.000000 neo-fairy-client-3.6.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-30 05:02:01.501552 neo-fairy-client-3.6.2.3/neo_fairy_client/
--rw-rw-rw-   0        0        0       74 2023-08-11 05:28:22.000000 neo-fairy-client-3.6.2.3/neo_fairy_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 05:02:01.509607 neo-fairy-client-3.6.2.3/neo_fairy_client/rpc/
--rw-rw-rw-   0        0        0       72 2023-08-11 05:33:48.000000 neo-fairy-client-3.6.2.3/neo_fairy_client/rpc/__init__.py
--rw-rw-rw-   0        0        0    59532 2024-01-30 05:01:38.000000 neo-fairy-client-3.6.2.3/neo_fairy_client/rpc/fairy_client.py
-drwxrwxrwx   0        0        0        0 2024-01-30 05:02:01.515617 neo-fairy-client-3.6.2.3/neo_fairy_client/utils/
--rw-rw-rw-   0        0        0     1379 2022-09-21 06:25:56.000000 neo-fairy-client-3.6.2.3/neo_fairy_client/utils/WitnessRule.py
--rw-rw-rw-   0        0        0      923 2023-08-11 05:25:04.000000 neo-fairy-client-3.6.2.3/neo_fairy_client/utils/__init__.py
--rw-rw-rw-   0        0        0     1368 2023-08-11 05:17:31.000000 neo-fairy-client-3.6.2.3/neo_fairy_client/utils/interpreters.py
--rw-rw-rw-   0        0        0      195 2022-09-28 04:32:29.000000 neo-fairy-client-3.6.2.3/neo_fairy_client/utils/misc.py
--rw-rw-rw-   0        0        0     1319 2022-10-25 06:12:11.000000 neo-fairy-client-3.6.2.3/neo_fairy_client/utils/timers.py
--rw-rw-rw-   0        0        0     7874 2023-09-20 07:36:06.000000 neo-fairy-client-3.6.2.3/neo_fairy_client/utils/types.py
-drwxrwxrwx   0        0        0        0 2024-01-30 05:02:01.517598 neo-fairy-client-3.6.2.3/neo_fairy_client/websocket/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:00:53.000000 neo-fairy-client-3.6.2.3/neo_fairy_client/websocket/__init__.py
--rw-rw-rw-   0        0        0     4694 2023-03-06 02:47:25.000000 neo-fairy-client-3.6.2.3/neo_fairy_client/websocket/fairy_websocket.py
-drwxrwxrwx   0        0        0        0 2024-01-30 05:02:01.518620 neo-fairy-client-3.6.2.3/neo_fairy_client.egg-info/
--rw-rw-rw-   0        0        0   139484 2024-01-30 05:02:01.000000 neo-fairy-client-3.6.2.3/neo_fairy_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2024-01-30 05:02:01.000000 neo-fairy-client-3.6.2.3/neo_fairy_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-30 05:02:01.000000 neo-fairy-client-3.6.2.3/neo_fairy_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-01-30 05:02:01.000000 neo-fairy-client-3.6.2.3/neo_fairy_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-01-30 05:02:01.000000 neo-fairy-client-3.6.2.3/neo_fairy_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-30 05:02:01.520897 neo-fairy-client-3.6.2.3/setup.cfg
--rw-rw-rw-   0        0        0      735 2024-01-16 05:11:54.000000 neo-fairy-client-3.6.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:17:18.691365 neo_fairy_client-3.7.1.1/
+-rw-rw-rw-   0        0        0     1085 2022-05-05 03:19:19.000000 neo_fairy_client-3.7.1.1/LICENSE
+-rw-rw-rw-   0        0        0   139484 2024-05-15 04:17:18.690366 neo_fairy_client-3.7.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0   138993 2023-08-24 03:08:32.000000 neo_fairy_client-3.7.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 04:17:18.674138 neo_fairy_client-3.7.1.1/neo_fairy_client/
+-rw-rw-rw-   0        0        0       74 2023-08-11 05:28:22.000000 neo_fairy_client-3.7.1.1/neo_fairy_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:17:18.681230 neo_fairy_client-3.7.1.1/neo_fairy_client/rpc/
+-rw-rw-rw-   0        0        0       72 2023-08-11 05:33:48.000000 neo_fairy_client-3.7.1.1/neo_fairy_client/rpc/__init__.py
+-rw-rw-rw-   0        0        0    61154 2024-05-15 03:39:18.000000 neo_fairy_client-3.7.1.1/neo_fairy_client/rpc/fairy_client.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:17:18.687212 neo_fairy_client-3.7.1.1/neo_fairy_client/utils/
+-rw-rw-rw-   0        0        0     1672 2024-03-22 07:23:02.000000 neo_fairy_client-3.7.1.1/neo_fairy_client/utils/WitnessRule.py
+-rw-rw-rw-   0        0        0     1299 2024-05-15 03:15:16.000000 neo_fairy_client-3.7.1.1/neo_fairy_client/utils/__init__.py
+-rw-rw-rw-   0        0        0     1368 2023-08-11 05:17:31.000000 neo_fairy_client-3.7.1.1/neo_fairy_client/utils/interpreters.py
+-rw-rw-rw-   0        0        0      195 2022-09-28 04:32:29.000000 neo_fairy_client-3.7.1.1/neo_fairy_client/utils/misc.py
+-rw-rw-rw-   0        0        0     1319 2022-10-25 06:12:11.000000 neo_fairy_client-3.7.1.1/neo_fairy_client/utils/timers.py
+-rw-rw-rw-   0        0        0     8086 2024-05-15 03:36:12.000000 neo_fairy_client-3.7.1.1/neo_fairy_client/utils/types.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:17:18.688213 neo_fairy_client-3.7.1.1/neo_fairy_client/websocket/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:00:53.000000 neo_fairy_client-3.7.1.1/neo_fairy_client/websocket/__init__.py
+-rw-rw-rw-   0        0        0     4694 2023-03-06 02:47:25.000000 neo_fairy_client-3.7.1.1/neo_fairy_client/websocket/fairy_websocket.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:17:18.689829 neo_fairy_client-3.7.1.1/neo_fairy_client.egg-info/
+-rw-rw-rw-   0        0        0   139484 2024-05-15 04:17:18.000000 neo_fairy_client-3.7.1.1/neo_fairy_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2024-05-15 04:17:18.000000 neo_fairy_client-3.7.1.1/neo_fairy_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 04:17:18.000000 neo_fairy_client-3.7.1.1/neo_fairy_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 04:17:18.000000 neo_fairy_client-3.7.1.1/neo_fairy_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 04:17:18.000000 neo_fairy_client-3.7.1.1/neo_fairy_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 04:17:18.691365 neo_fairy_client-3.7.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      735 2024-05-15 04:08:18.000000 neo_fairy_client-3.7.1.1/setup.py
```

### Comparing `neo-fairy-client-3.6.2.3/LICENSE` & `neo_fairy_client-3.7.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.6.2.3/PKG-INFO` & `neo_fairy_client-3.7.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-fairy-client
-Version: 3.6.2.3
+Version: 3.7.1.1
 Summary: Test & debug your Neo3 smart contracts
 Home-page: https://github.com/Hecate2/neo-fairy-client
 Author: Hecate2
 Author-email: hecate2@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neo-fairy-client-3.6.2.3/README.md` & `neo_fairy_client-3.7.1.1/README.md`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.6.2.3/neo_fairy_client/rpc/fairy_client.py` & `neo_fairy_client-3.7.1.1/neo_fairy_client/rpc/fairy_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import List, Union, Dict, Any, Callable
+from enum import Enum
 import base64
 import json
 import os
 import random
 import traceback
 import requests
 import urllib3
 
 from neo_fairy_client.utils import Hash160Str, Hash256Str, PublicKeyStr, Signer
 from neo_fairy_client.utils import Interpreter, to_list
 from neo_fairy_client.utils import ContractManagementAddress, CryptoLibAddress, GasAddress, LedgerAddress, NeoAddress, OracleAddress, PolicyAddress, RoleManagementAddress, StdLibAddress
+from neo_fairy_client.utils import NamedCurveHash
 
 from neo_fairy_client.utils import UInt160, UInt256
 from neo_fairy_client.utils import VMState
 
 RequestExceptions = (
     requests.RequestException,
     requests.ConnectionError,
@@ -426,14 +428,16 @@
                 'type': 'Map',
                 'value': [{'key': cls.parse_param(k), 'value': cls.parse_param(v)} for k, v in param.items()]
             }
         elif param is None:
             return {
                 'type': 'Any',
             }
+        elif isinstance(param, Enum):
+            return cls.parse_param(param.value)
         raise ValueError(f'Unable to handle param {param} with type {type_param}')
     
     def invokefunction_of_any_contract(self, scripthash: Hash160Str, operation: str,
                                        params: List[Union[List, str, int, dict, Hash160Str, UInt160, bytes, bytearray]] = None,
                                        signers: Union[Signer, List[Signer]] = None, relay: bool = None, do_not_raise_on_result=False,
                                        with_print=True, fairy_session: str = None) -> Any:
         fairy_session = fairy_session or self.fairy_session
@@ -598,19 +602,41 @@
 
     def set_session_fairy_wallet_with_WIF(self, wif: Union[str, List[str]], fairy_session: str = None) -> dict:
         open_wallet_result = self.meta_rpc_method("setsessionfairywalletwithwif", [fairy_session or self.fairy_session] + to_list(wif))
         if not open_wallet_result:
             raise ValueError(f'Failed to open WIF wallet {wif} with given password.')
         return open_wallet_result
 
-    def force_sign_message(self, message_base64_encoded: Union[str, bytes], fairy_session: str = None) -> bytes:
+    def force_verify_with_ecdsa(
+            self, message_base64_encoded: Union[str, bytes],
+            pubkey: Union[PublicKeyStr, str, bytes],
+            signature_base64_encoded: Union[str, bytes],
+            namedCurveHash: Union[NamedCurveHash, bytes, int] = NamedCurveHash.secp256r1SHA256) -> bool:
+        if type(message_base64_encoded) is bytes:
+            message_base64_encoded: str = base64.b64encode(message_base64_encoded).decode()
+        if type(pubkey) is PublicKeyStr:
+            pubkey: bytearray = pubkey.to_bytes()
+        pubkey: str = base64.b64encode(pubkey).decode()
+        if type(signature_base64_encoded) is bytes:
+            signature_base64_encoded: str = base64.b64encode(signature_base64_encoded).decode()
+        if type(namedCurveHash) is bytes:
+            namedCurveHash: int = namedCurveHash[0]
+        if type(namedCurveHash) is int:
+            namedCurveHash: NamedCurveHash = NamedCurveHash(namedCurveHash)
+        return self.meta_rpc_method("forceverifywithecdsa", [message_base64_encoded, pubkey, signature_base64_encoded, namedCurveHash.value], relay=False)['result']
+
+    def force_sign_message(self, message_base64_encoded: Union[str, bytes], namedCurveHash: Union[NamedCurveHash, bytes, int] = NamedCurveHash.secp256r1SHA256, fairy_session: str = None) -> bytes:
         fairy_session = fairy_session or self.fairy_session
         if type(message_base64_encoded) is bytes:
             message_base64_encoded: str = base64.b64encode(message_base64_encoded).decode()
-        return base64.b64decode(self.meta_rpc_method("forcesignmessage", [fairy_session, message_base64_encoded], relay=False)['signed'])
+        if type(namedCurveHash) is bytes:
+            namedCurveHash: int = namedCurveHash[0]
+        if type(namedCurveHash) is int:
+            namedCurveHash: NamedCurveHash = NamedCurveHash(namedCurveHash)
+        return base64.b64decode(self.meta_rpc_method("forcesignmessage", [fairy_session, message_base64_encoded, namedCurveHash.value], relay=False)['signed'])
 
     def force_sign_transaction(self, script_base64_encoded: Union[str, bytes, None] = None, fairy_session: str = None,
                                signers: List[Signer] = None, system_fee: int = 1000_0000, network_fee: int = 0,
                                valid_until_block: Union[int, None] = 0, nonce: int = 0) -> Dict[str, Any]:
         """
         Build and sign a transaction with the fairy wallet of the fairy_session,
         even if the transaction cannot be run correctly
```

### Comparing `neo-fairy-client-3.6.2.3/neo_fairy_client/utils/WitnessRule.py` & `neo_fairy_client-3.7.1.1/neo_fairy_client/utils/WitnessRule.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,41 +33,46 @@
     return {
         "type": "Or",
         "expressions": list(conditions)
     }
 
 
 def ScriptHash(scripthash: Hash160Str):
+    """ExecutingScriptHash is scripthash"""
     return {
         "type": "ScriptHash",
         "hash": scripthash.to_str()
     }
 
 
 def Group(publickey: PublicKeyStr):
+    """ExecutingScriptHash contract manifest group has publickey"""
     return {
         "type": "Group",
         "group": publickey.to_str()
     }
 
 
 def CalledByEntry():
+    """ExecutingScriptHash is entry, or called by entry"""
     return {
         "type": "CalledByEntry",
     }
 
 
 def CalledByContract(scripthash: Hash160Str):
+    """ExecutingScriptHash called by scripthash"""
     return {
         "type": "CalledByContract",
         "hash": scripthash.to_str()
     }
 
 
 def CalledByGroup(publickey: PublicKeyStr):
+    """CallingScriptHash contract manifest group has publickey"""
     return {
         "type": "CalledByGroup",
         "group": publickey.to_str()
     }
 
 
 def True_():
```

### Comparing `neo-fairy-client-3.6.2.3/neo_fairy_client/utils/interpreters.py` & `neo_fairy_client-3.7.1.1/neo_fairy_client/utils/interpreters.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.6.2.3/neo_fairy_client/utils/timers.py` & `neo_fairy_client-3.7.1.1/neo_fairy_client/utils/timers.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.6.2.3/neo_fairy_client/utils/types.py` & `neo_fairy_client-3.7.1.1/neo_fairy_client/utils/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,14 +181,17 @@
         typically
         private_key_bytes = base58.b58decode(WIF_private_key)[1:-5]
         sk = ecdsa.SigningKey.from_string(private_key_bytes, curve=ecdsa.NIST256p, hashfunc=hashlib.sha256)
         vk = sk.get_verifying_key()
         PublicKeyStr(vk.to_string('compressed').hex())
         """
         return cls(vk.to_string('compressed').hex())
+    
+    def to_bytes(self):
+        return bytearray.fromhex(self)
 
 
 class WitnessScope(Enum):
     NONE = 'None'  # no contract has your valid signature
     CalledByEntry = 'CalledByEntry'  # only the called contract has your valid signature
     Global = 'Global'  # all contracts have your valid signature
     CustomContracts = 'CustomContracts'  # only contracts of designated addresses have your valid signature
@@ -222,13 +225,18 @@
             'allowedgroups': self.allowedgroups,
             'rules': self.rules
         }
     
     def __repr__(self):
         return self.to_dict().__repr__()
 
+class NamedCurveHash(Enum):
+    secp256k1SHA256 = 22
+    secp256r1SHA256 = 23
+    secp256k1Keccak256 = 122
+    secp256r1Keccak256 = 123
 
 if __name__ == '__main__':
     print('30 days:', gen_timestamp_and_date_str_in_days(30))
     print(' 0 days:', gen_timestamp_and_date_str_in_days(0))
     print('time now:', time.time() * 1000)
     print(' 5 secs:', gen_timestamp_and_date_str_in_seconds(5))
```

### Comparing `neo-fairy-client-3.6.2.3/neo_fairy_client/websocket/fairy_websocket.py` & `neo_fairy_client-3.7.1.1/neo_fairy_client/websocket/fairy_websocket.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.6.2.3/neo_fairy_client.egg-info/PKG-INFO` & `neo_fairy_client-3.7.1.1/neo_fairy_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-fairy-client
-Version: 3.6.2.3
+Version: 3.7.1.1
 Summary: Test & debug your Neo3 smart contracts
 Home-page: https://github.com/Hecate2/neo-fairy-client
 Author: Hecate2
 Author-email: hecate2@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neo-fairy-client-3.6.2.3/neo_fairy_client.egg-info/SOURCES.txt` & `neo_fairy_client-3.7.1.1/neo_fairy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.6.2.3/setup.py` & `neo_fairy_client-3.7.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="neo-fairy-client",
-    version="3.6.2.3",
+    version="3.7.1.1",
     author="Hecate2",
     author_email="hecate2@qq.com",
     description="Test & debug your Neo3 smart contracts",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Hecate2/neo-fairy-client",
     packages=setuptools.find_packages(),
```

