# Comparing `tmp/walledai-0.6.0a0.tar.gz` & `tmp/walledai-0.7.0a0.tar.gz`

## Comparing `walledai-0.6.0a0.tar` & `walledai-0.7.0a0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walled_ai/lib/.keep
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/__init__.py
--rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_base_client.py
--rw-r--r--   0        0        0    14792 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_constants.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_qs.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_resource.py
--rw-r--r--   0        0        0    28387 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_response.py
--rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_streaming.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_types.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_utils/__init__.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/lib/.keep
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/resources/__init__.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/resources/moderation.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/types/__init__.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 walledai-0.6.0a0/src/walledai/types/moderation_create_params.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 walledai-0.6.0a0/.gitignore
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 walledai-0.6.0a0/LICENSE
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 walledai-0.6.0a0/pyproject.toml
--rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 walledai-0.6.0a0/PKG-INFO
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walled_ai/lib/.keep
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/__init__.py
+-rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_base_client.py
+-rw-r--r--   0        0        0    14792 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_constants.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_qs.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_resource.py
+-rw-r--r--   0        0        0    28387 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_response.py
+-rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_streaming.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_types.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/__init__.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/lib/.keep
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/resources/__init__.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/resources/moderation.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/types/__init__.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/types/moderation_create_params.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 walledai-0.7.0a0/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 walledai-0.7.0a0/LICENSE
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 walledai-0.7.0a0/pyproject.toml
+-rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 walledai-0.7.0a0/PKG-INFO
```

### Comparing `walledai-0.6.0a0/src/walledai/__init__.py` & `walledai-0.7.0a0/src/walledai/__init__.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_base_client.py` & `walledai-0.7.0a0/src/walledai/_base_client.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_client.py` & `walledai-0.7.0a0/src/walledai/_client.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_compat.py` & `walledai-0.7.0a0/src/walledai/_compat.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_exceptions.py` & `walledai-0.7.0a0/src/walledai/_exceptions.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_files.py` & `walledai-0.7.0a0/src/walledai/_files.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_models.py` & `walledai-0.7.0a0/src/walledai/_models.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_qs.py` & `walledai-0.7.0a0/src/walledai/_qs.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_resource.py` & `walledai-0.7.0a0/src/walledai/_resource.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_response.py` & `walledai-0.7.0a0/src/walledai/_response.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_streaming.py` & `walledai-0.7.0a0/src/walledai/_streaming.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_types.py` & `walledai-0.7.0a0/src/walledai/_types.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_utils/__init__.py` & `walledai-0.7.0a0/src/walledai/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_utils/_logs.py` & `walledai-0.7.0a0/src/walledai/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_utils/_proxy.py` & `walledai-0.7.0a0/src/walledai/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_utils/_sync.py` & `walledai-0.7.0a0/src/walledai/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_utils/_transform.py` & `walledai-0.7.0a0/src/walledai/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_utils/_typing.py` & `walledai-0.7.0a0/src/walledai/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/_utils/_utils.py` & `walledai-0.7.0a0/src/walledai/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/resources/__init__.py` & `walledai-0.7.0a0/src/walledai/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/src/walledai/resources/moderation.py` & `walledai-0.7.0a0/src/walledai/resources/moderation.py`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/LICENSE` & `walledai-0.7.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `walledai-0.6.0a0/pyproject.toml` & `walledai-0.7.0a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "walledai"
-version = "0.6.0-alpha"
+version = "0.7.0-alpha"
 description = "The official Python library for the walledai API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Walledai", email = "admin@walled.ai" },
 ]
 dependencies = [
```

### Comparing `walledai-0.6.0a0/PKG-INFO` & `walledai-0.7.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: walledai
-Version: 0.6.0a0
+Version: 0.7.0a0
 Summary: The official Python library for the walledai API
 Project-URL: Homepage, https://github.com/rajatb94/walledai-python
 Project-URL: Repository, https://github.com/rajatb94/walledai-python
 Author-email: Walledai <admin@walled.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

