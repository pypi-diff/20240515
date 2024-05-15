# Comparing `tmp/drax_sdk-2.2.4.tar.gz` & `tmp/drax_sdk-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drax_sdk-2.2.4.tar", max compression
+gzip compressed data, was "drax_sdk-2.2.5.tar", max compression
```

## Comparing `drax_sdk-2.2.4.tar` & `drax_sdk-2.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      695 2024-05-02 08:19:05.031537 drax_sdk-2.2.4/README.md
--rw-r--r--   0        0        0        0 2024-04-23 09:08:58.311282 drax_sdk-2.2.4/drax_sdk/__init__.py
--rw-r--r--   0        0        0    10477 2024-05-02 07:53:41.565314 drax_sdk-2.2.4/drax_sdk/broker/amqp_broker.py
--rw-r--r--   0        0        0     9722 2024-04-23 19:01:05.353666 drax_sdk-2.2.4/drax_sdk/clients/drax_core_client.py
--rw-r--r--   0        0        0     8191 2024-05-02 08:15:24.927452 drax_sdk-2.2.4/drax_sdk/drax.py
--rw-r--r--   0        0        0     2632 2024-04-24 11:25:01.894264 drax_sdk-2.2.4/drax_sdk/keystore.parquet
--rw-r--r--   0        0        0     1961 2024-05-08 09:32:03.330767 drax_sdk-2.2.4/drax_sdk/model/automations.py
--rw-r--r--   0        0        0     4234 2024-04-29 17:14:04.731172 drax_sdk-2.2.4/drax_sdk/model/dto.py
--rw-r--r--   0        0        0     1479 2024-04-29 17:05:39.625330 drax_sdk-2.2.4/drax_sdk/model/dynamic.py
--rw-r--r--   0        0        0      512 2024-04-23 13:55:28.408981 drax_sdk-2.2.4/drax_sdk/model/event.py
--rw-r--r--   0        0        0     3448 2024-04-30 08:39:15.667730 drax_sdk-2.2.4/drax_sdk/model/node.py
--rw-r--r--   0        0        0      524 2024-04-23 14:04:03.872372 drax_sdk-2.2.4/drax_sdk/model/project.py
--rw-r--r--   0        0        0        0 2024-04-23 14:40:17.430746 drax_sdk-2.2.4/drax_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1643 2024-04-23 18:05:22.265455 drax_sdk-2.2.4/drax_sdk/utils/bytes_codec.py
--rw-r--r--   0        0        0     1432 2024-04-29 17:12:52.612558 drax_sdk-2.2.4/drax_sdk/utils/codec.py
--rw-r--r--   0        0        0     2468 2024-04-24 11:01:18.261896 drax_sdk-2.2.4/drax_sdk/utils/keystore.py
--rw-r--r--   0        0        0       71 2024-04-23 14:29:18.856060 drax_sdk-2.2.4/drax_sdk/utils/timestamp.py
--rw-r--r--   0        0        0      447 2024-05-08 09:32:26.954842 drax_sdk-2.2.4/pyproject.toml
--rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 drax_sdk-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0      695 2024-05-02 08:19:05.031537 drax_sdk-2.2.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 09:08:58.311282 drax_sdk-2.2.5/drax_sdk/__init__.py
+-rw-r--r--   0        0        0    10477 2024-05-02 07:53:41.565314 drax_sdk-2.2.5/drax_sdk/broker/amqp_broker.py
+-rw-r--r--   0        0        0     9722 2024-04-23 19:01:05.353666 drax_sdk-2.2.5/drax_sdk/clients/drax_core_client.py
+-rw-r--r--   0        0        0     8191 2024-05-02 08:15:24.927452 drax_sdk-2.2.5/drax_sdk/drax.py
+-rw-r--r--   0        0        0     2632 2024-04-24 11:25:01.894264 drax_sdk-2.2.5/drax_sdk/keystore.parquet
+-rw-r--r--   0        0        0     1961 2024-05-08 09:32:03.330767 drax_sdk-2.2.5/drax_sdk/model/automations.py
+-rw-r--r--   0        0        0     4234 2024-04-29 17:14:04.731172 drax_sdk-2.2.5/drax_sdk/model/dto.py
+-rw-r--r--   0        0        0     1479 2024-04-29 17:05:39.625330 drax_sdk-2.2.5/drax_sdk/model/dynamic.py
+-rw-r--r--   0        0        0      512 2024-04-23 13:55:28.408981 drax_sdk-2.2.5/drax_sdk/model/event.py
+-rw-r--r--   0        0        0     3475 2024-05-15 16:14:06.413205 drax_sdk-2.2.5/drax_sdk/model/node.py
+-rw-r--r--   0        0        0      524 2024-04-23 14:04:03.872372 drax_sdk-2.2.5/drax_sdk/model/project.py
+-rw-r--r--   0        0        0        0 2024-04-23 14:40:17.430746 drax_sdk-2.2.5/drax_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1643 2024-04-23 18:05:22.265455 drax_sdk-2.2.5/drax_sdk/utils/bytes_codec.py
+-rw-r--r--   0        0        0     1432 2024-04-29 17:12:52.612558 drax_sdk-2.2.5/drax_sdk/utils/codec.py
+-rw-r--r--   0        0        0     2468 2024-04-24 11:01:18.261896 drax_sdk-2.2.5/drax_sdk/utils/keystore.py
+-rw-r--r--   0        0        0       71 2024-04-23 14:29:18.856060 drax_sdk-2.2.5/drax_sdk/utils/timestamp.py
+-rw-r--r--   0        0        0      447 2024-05-15 16:15:37.701421 drax_sdk-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 drax_sdk-2.2.5/PKG-INFO
```

### Comparing `drax_sdk-2.2.4/README.md` & `drax_sdk-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/drax_sdk/broker/amqp_broker.py` & `drax_sdk-2.2.5/drax_sdk/broker/amqp_broker.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/drax_sdk/clients/drax_core_client.py` & `drax_sdk-2.2.5/drax_sdk/clients/drax_core_client.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/drax_sdk/drax.py` & `drax_sdk-2.2.5/drax_sdk/drax.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/drax_sdk/keystore.parquet` & `drax_sdk-2.2.5/drax_sdk/keystore.parquet`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/drax_sdk/model/automations.py` & `drax_sdk-2.2.5/drax_sdk/model/automations.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/drax_sdk/model/dto.py` & `drax_sdk-2.2.5/drax_sdk/model/dto.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/drax_sdk/model/dynamic.py` & `drax_sdk-2.2.5/drax_sdk/model/dynamic.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/drax_sdk/model/event.py` & `drax_sdk-2.2.5/drax_sdk/model/event.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/drax_sdk/model/node.py` & `drax_sdk-2.2.5/drax_sdk/model/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     )
     public_keys: List[ECDHKey] = Field(default_factory=list, alias="publicKeys")
     active: bool = False
     script: Optional[str] = None
     max_idle_time: int = Field(0, alias="maxIdleTime")
     last_check: int = Field(default=unix_timestamp(), alias="lastCheck")
     status: Optional[str] = None
+    state: State = State()
 
     def add_supported_type(self, type: str):
         self.supported_types.append(type)
 
     def add_public_key(self, public_key: bytes):
         if not any(k.key == public_key for k in self.public_keys):
             self.public_keys.append(ECDHKey(key=public_key, status=ECDHKeyType.ACTIVE))
```

### Comparing `drax_sdk-2.2.4/drax_sdk/model/project.py` & `drax_sdk-2.2.5/drax_sdk/model/project.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/drax_sdk/utils/bytes_codec.py` & `drax_sdk-2.2.5/drax_sdk/utils/bytes_codec.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/drax_sdk/utils/codec.py` & `drax_sdk-2.2.5/drax_sdk/utils/codec.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/drax_sdk/utils/keystore.py` & `drax_sdk-2.2.5/drax_sdk/utils/keystore.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.4/PKG-INFO` & `drax_sdk-2.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drax-sdk
-Version: 2.2.4
+Version: 2.2.5
 Summary: Python sdk for Drax IoT Platform
 Author: Applica Software Guru
 Author-email: info@applica.guru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

