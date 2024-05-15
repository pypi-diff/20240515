# Comparing `tmp/arthub_api-1.9.0.tar.gz` & `tmp/arthub_api-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.9.0.tar", last modified: Fri Apr 26 07:43:12 2024, max compression
+gzip compressed data, was "arthub_api-1.9.1.tar", last modified: Wed May 15 14:23:48 2024, max compression
```

## Comparing `arthub_api-1.9.0.tar` & `arthub_api-1.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 07:43:12.947695 arthub_api-1.9.0/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.9.0/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2024-04-26 07:43:12.947695 arthub_api-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.9.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 07:43:12.920568 arthub_api-1.9.0/arthub_api/
--rw-rw-rw-   0        0        0      675 2023-07-25 13:45:45.000000 arthub_api-1.9.0/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     3049 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2024-04-26 07:41:47.000000 arthub_api-1.9.0/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.9.0/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0      128 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      501 2023-07-25 13:45:45.000000 arthub_api-1.9.0/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    43536 2023-07-25 13:45:45.000000 arthub_api-1.9.0/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0     2072 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/blade_api_instance.py
--rw-rw-rw-   0        0        0    28990 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.9.0/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1443 2023-07-25 13:45:45.000000 arthub_api-1.9.0/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.9.0/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1465 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/models.py
--rw-rw-rw-   0        0        0    47472 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    46992 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/storage.py
--rw-rw-rw-   0        0        0    10006 2024-04-26 07:41:26.000000 arthub_api-1.9.0/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:43:12.935168 arthub_api-1.9.0/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2024-04-26 07:43:12.000000 arthub_api-1.9.0/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2024-04-26 07:43:12.000000 arthub_api-1.9.0/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 07:43:12.000000 arthub_api-1.9.0/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-26 07:43:12.000000 arthub_api-1.9.0/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-14 07:53:40.000000 arthub_api-1.9.0/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      185 2024-04-26 07:43:12.000000 arthub_api-1.9.0/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 07:43:12.000000 arthub_api-1.9.0/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.9.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 07:43:12.947695 arthub_api-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0     3157 2024-04-26 07:41:26.000000 arthub_api-1.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:43:12.944145 arthub_api-1.9.0/tests/
--rw-rw-rw-   0        0        0      176 2023-07-25 13:45:45.000000 arthub_api-1.9.0/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.9.0/tests/_utils.py
--rw-rw-rw-   0        0        0      866 2024-04-26 07:41:26.000000 arthub_api-1.9.0/tests/conftest.py
--rw-rw-rw-   0        0        0     7139 2024-04-26 07:41:26.000000 arthub_api-1.9.0/tests/test_open_api.py
--rw-rw-rw-   0        0        0     3471 2024-04-26 07:41:26.000000 arthub_api-1.9.0/tests/test_storage.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:48.897526 arthub_api-1.9.1/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.9.1/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2024-05-15 14:23:48.891542 arthub_api-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:48.811207 arthub_api-1.9.1/arthub_api/
+-rw-rw-rw-   0        0        0      675 2023-07-25 13:45:45.000000 arthub_api-1.9.1/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     3049 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2024-05-15 14:23:08.000000 arthub_api-1.9.1/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.9.1/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0      128 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      501 2023-07-25 13:45:45.000000 arthub_api-1.9.1/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    43536 2023-07-25 13:45:45.000000 arthub_api-1.9.1/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     2072 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    28990 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.9.1/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1443 2023-07-25 13:45:45.000000 arthub_api-1.9.1/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.9.1/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1465 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/models.py
+-rw-rw-rw-   0        0        0    47584 2024-05-15 14:20:21.000000 arthub_api-1.9.1/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    46992 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/storage.py
+-rw-rw-rw-   0        0        0    10006 2024-04-26 07:41:26.000000 arthub_api-1.9.1/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:48.821181 arthub_api-1.9.1/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2024-05-15 14:23:47.000000 arthub_api-1.9.1/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2024-05-15 14:23:48.000000 arthub_api-1.9.1/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:23:47.000000 arthub_api-1.9.1/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-15 14:23:47.000000 arthub_api-1.9.1/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-03-14 07:53:40.000000 arthub_api-1.9.1/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      185 2024-05-15 14:23:47.000000 arthub_api-1.9.1/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 14:23:47.000000 arthub_api-1.9.1/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.9.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:23:48.897526 arthub_api-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     3157 2024-04-26 07:41:26.000000 arthub_api-1.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:23:48.864614 arthub_api-1.9.1/tests/
+-rw-rw-rw-   0        0        0      176 2023-07-25 13:45:45.000000 arthub_api-1.9.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.9.1/tests/_utils.py
+-rw-rw-rw-   0        0        0      866 2024-04-26 07:41:26.000000 arthub_api-1.9.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     7139 2024-04-26 07:41:26.000000 arthub_api-1.9.1/tests/test_open_api.py
+-rw-rw-rw-   0        0        0     3471 2024-04-26 07:41:26.000000 arthub_api-1.9.1/tests/test_storage.py
```

### Comparing `arthub_api-1.9.0/LICENSE` & `arthub_api-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/PKG-INFO` & `arthub_api-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.9.0
+Version: 1.9.1
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.9.0/README.md` & `arthub_api-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/arthub_api/__init__.py` & `arthub_api-1.9.1/arthub_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/arthub_api/__main__.py` & `arthub_api-1.9.1/arthub_api/__main__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/arthub_api/_internal_utils.py` & `arthub_api-1.9.1/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/arthub_api/blade_api.py` & `arthub_api-1.9.1/arthub_api/blade_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/arthub_api/blade_api_instance.py` & `arthub_api-1.9.1/arthub_api/blade_api_instance.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/arthub_api/blade_storage.py` & `arthub_api-1.9.1/arthub_api/blade_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/arthub_api/config.py` & `arthub_api-1.9.1/arthub_api/config.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/arthub_api/exception.py` & `arthub_api-1.9.1/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/arthub_api/models.py` & `arthub_api-1.9.1/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/arthub_api/open_api.py` & `arthub_api-1.9.1/arthub_api/open_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,15 +546,18 @@
             "nounce": utils.get_random_string(8),
             "oauth_type": "password",
             "login_type": "arthub_token"
         }
 
         url = self._account_url("login")
         if not login_public_keys:
-            req_payload["verification_code"] = verification_code
+            if verification_code:
+                req_payload["verification_code"] = verification_code
+            else:
+                url = self._account_url("login-fix")
         else:
             url = self._account_url("open-secret-login")
             req_payload["ticket"] = self.generate_login_ticket(req_payload, login_public_keys)
 
         res = self._make_api_request(url, req_payload, try_login_on_expired=False)
         if res.is_succeeded():
             r = res.results.get(0)
```

### Comparing `arthub_api-1.9.0/arthub_api/storage.py` & `arthub_api-1.9.1/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/arthub_api/utils.py` & `arthub_api-1.9.1/arthub_api/utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.9.1/arthub_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.9.0
+Version: 1.9.1
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.9.0/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.9.1/arthub_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/setup.py` & `arthub_api-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/tests/conftest.py` & `arthub_api-1.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/tests/test_open_api.py` & `arthub_api-1.9.1/tests/test_open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.9.0/tests/test_storage.py` & `arthub_api-1.9.1/tests/test_storage.py`

 * *Files identical despite different names*

