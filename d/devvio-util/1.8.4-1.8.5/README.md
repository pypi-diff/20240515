# Comparing `tmp/devvio_util-1.8.4.tar.gz` & `tmp/devvio_util-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.8.4.tar", last modified: Wed May  8 17:56:04 2024, max compression
+gzip compressed data, was "devvio_util-1.8.5.tar", last modified: Wed May 15 14:13:37 2024, max compression
```

## Comparing `devvio_util-1.8.4.tar` & `devvio_util-1.8.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:56:04.374831 devvio_util-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-08 17:56:04.374831 devvio_util-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:55:58.000000 devvio_util-1.8.4/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:56:04.370830 devvio_util-1.8.4/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:56:04.370830 devvio_util-1.8.4/devvio_util/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/exceptions/auth_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/exceptions/controller_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/exceptions/db_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/exceptions/devv_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/exceptions/validation_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:56:04.374831 devvio_util-1.8.4/devvio_util/inn_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/inn_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/inn_sdk/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/inn_sdk/dfe_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    40617 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/inn_sdk/inn_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/inn_sdk/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/inn_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/lib_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:56:04.374831 devvio_util-1.8.4/devvio_util/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/address.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/atomic_transaction_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/chainstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/devv_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/devv_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/final_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/smart_coin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    15822 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/primitives/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    18364 2024-05-08 17:55:58.000000 devvio_util-1.8.4/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:56:04.374831 devvio_util-1.8.4/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-08 17:56:04.000000 devvio_util-1.8.4/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-08 17:56:04.000000 devvio_util-1.8.4/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:56:04.000000 devvio_util-1.8.4/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:56:04.000000 devvio_util-1.8.4/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 17:56:04.000000 devvio_util-1.8.4/devvio_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 17:56:04.000000 devvio_util-1.8.4/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-08 17:56:04.378831 devvio_util-1.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-08 17:55:58.000000 devvio_util-1.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:13:37.076790 devvio_util-1.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-15 14:13:37.076790 devvio_util-1.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:13:22.000000 devvio_util-1.8.5/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:13:37.068790 devvio_util-1.8.5/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:13:37.072790 devvio_util-1.8.5/devvio_util/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/exceptions/auth_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/exceptions/controller_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/exceptions/db_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/exceptions/devv_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/exceptions/validation_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:13:37.072790 devvio_util-1.8.5/devvio_util/inn_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/inn_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/inn_sdk/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/inn_sdk/dfe_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40617 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/inn_sdk/inn_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/inn_sdk/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/inn_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/lib_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:13:37.076790 devvio_util-1.8.5/devvio_util/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/atomic_transaction_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/chainstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/devv_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/devv_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/final_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/smart_coin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15822 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/primitives/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18364 2024-05-15 14:13:22.000000 devvio_util-1.8.5/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:13:37.076790 devvio_util-1.8.5/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-15 14:13:37.000000 devvio_util-1.8.5/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-15 14:13:37.000000 devvio_util-1.8.5/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:13:37.000000 devvio_util-1.8.5/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:13:36.000000 devvio_util-1.8.5/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 14:13:37.000000 devvio_util-1.8.5/devvio_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 14:13:37.000000 devvio_util-1.8.5/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 14:13:37.076790 devvio_util-1.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-15 14:13:22.000000 devvio_util-1.8.5/setup.py
```

### Comparing `devvio_util-1.8.4/devvio_util/config.py` & `devvio_util-1.8.5/devvio_util/config.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/decorators.py` & `devvio_util-1.8.5/devvio_util/decorators.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/exceptions/__init__.py` & `devvio_util-1.8.5/devvio_util/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/exceptions/devv_error.py` & `devvio_util-1.8.5/devvio_util/exceptions/devv_error.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/exceptions/validation_exceptions.py` & `devvio_util-1.8.5/devvio_util/exceptions/validation_exceptions.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/inn_sdk/base_client.py` & `devvio_util-1.8.5/devvio_util/inn_sdk/base_client.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/inn_sdk/dfe_client.py` & `devvio_util-1.8.5/devvio_util/inn_sdk/dfe_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -267,7 +267,27 @@
             "username": username,
             "hashed_uuid": hashed_uuid,
         }
         if other_fields:
             body.update(other_fields)
         url = "/ll/v1/admin/badges/get"
         return self._send_post_request(url, body)
+
+    def delete_badge(self, username: str, hashed_uuid: str, other_fields: dict = None):
+        body = {
+            "username": username,
+            "hashed_uuid": hashed_uuid,
+        }
+        if other_fields:
+            body.update(other_fields)
+        url = "/ll/v1/admin/badges/delete"
+        return self._send_post_request(url, body)
+
+    def update_badge(self, username: str, hashed_uuid: str, other_fields: dict = None):
+        body = {
+            "username": username,
+            "hashed_uuid": hashed_uuid,
+        }
+        if other_fields:
+            body.update(other_fields)
+        url = "/ll/v1/admin/badges/update"
+        return self._send_post_request(url, body)
```

### Comparing `devvio_util-1.8.4/devvio_util/inn_sdk/inn_client.py` & `devvio_util-1.8.5/devvio_util/inn_sdk/inn_client.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/inn_sdk/utils.py` & `devvio_util-1.8.5/devvio_util/inn_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/lib_creds.py` & `devvio_util-1.8.5/devvio_util/lib_creds.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/logging.py` & `devvio_util-1.8.5/devvio_util/logging.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/address.py` & `devvio_util-1.8.5/devvio_util/primitives/address.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/chainstate.py` & `devvio_util-1.8.5/devvio_util/primitives/chainstate.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/devv_constants.py` & `devvio_util-1.8.5/devvio_util/primitives/devv_constants.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/devv_sign.py` & `devvio_util-1.8.5/devvio_util/primitives/devv_sign.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/final_block.py` & `devvio_util-1.8.5/devvio_util/primitives/final_block.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/payload.py` & `devvio_util-1.8.5/devvio_util/primitives/payload.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/signature.py` & `devvio_util-1.8.5/devvio_util/primitives/signature.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/smart_coin.py` & `devvio_util-1.8.5/devvio_util/primitives/smart_coin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/summary.py` & `devvio_util-1.8.5/devvio_util/primitives/summary.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/transaction.py` & `devvio_util-1.8.5/devvio_util/primitives/transaction.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/transfer.py` & `devvio_util-1.8.5/devvio_util/primitives/transfer.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/utils.py` & `devvio_util-1.8.5/devvio_util/primitives/utils.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/primitives/validation.py` & `devvio_util-1.8.5/devvio_util/primitives/validation.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util/psql_mixin.py` & `devvio_util-1.8.5/devvio_util/psql_mixin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/devvio_util.egg-info/SOURCES.txt` & `devvio_util-1.8.5/devvio_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devvio_util-1.8.4/setup.py` & `devvio_util-1.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup
-VERSION = 'v1.8.4'
+VERSION = 'v1.8.5'
 
 setup(name='devvio_util',
       version=VERSION,
       long_description=open('README.txt').read(),
       long_description_content_type='text/markdown',
       description='Utility to be used inside Devvio projects',
       author='Devvio Team',
```

