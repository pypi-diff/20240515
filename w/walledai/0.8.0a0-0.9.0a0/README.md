# Comparing `tmp/walledai-0.8.0a0.tar.gz` & `tmp/walledai-0.9.0a0.tar.gz`

## Comparing `walledai-0.8.0a0.tar` & `walledai-0.9.0a0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walled_ai/lib/.keep
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/__init__.py
--rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_base_client.py
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_constants.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_qs.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_resource.py
--rw-r--r--   0        0        0    28387 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_response.py
--rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_streaming.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_types.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/__init__.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/lib/.keep
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/resources/__init__.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/resources/moderation.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/types/__init__.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/types/moderation_create_params.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 walledai-0.8.0a0/.gitignore
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 walledai-0.8.0a0/LICENSE
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 walledai-0.8.0a0/pyproject.toml
--rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 walledai-0.8.0a0/PKG-INFO
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walled_ai/lib/.keep
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/__init__.py
+-rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_base_client.py
+-rw-r--r--   0        0        0    15282 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_constants.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_qs.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_resource.py
+-rw-r--r--   0        0        0    28387 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_response.py
+-rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_streaming.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_types.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_utils/__init__.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/lib/.keep
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/resources/__init__.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/resources/moderation.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/types/__init__.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 walledai-0.9.0a0/src/walledai/types/moderation_create_params.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 walledai-0.9.0a0/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 walledai-0.9.0a0/LICENSE
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 walledai-0.9.0a0/pyproject.toml
+-rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 walledai-0.9.0a0/PKG-INFO
```

### Comparing `walledai-0.8.0a0/src/walledai/__init__.py` & `walledai-0.9.0a0/src/walledai/__init__.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_base_client.py` & `walledai-0.9.0a0/src/walledai/_base_client.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_client.py` & `walledai-0.9.0a0/src/walledai/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,20 @@
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
     @override
+    def auth_headers(self) -> dict[str, str]:
+        bearer_token = self.bearer_token
+        return {"Authorization": f"Bearer {bearer_token}"}
+
+    @property
+    @override
     def default_headers(self) -> dict[str, str | Omit]:
         return {
             **super().default_headers,
             "X-Stainless-Async": "false",
             **self._custom_headers,
         }
 
@@ -273,14 +279,20 @@
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
     @override
+    def auth_headers(self) -> dict[str, str]:
+        bearer_token = self.bearer_token
+        return {"Authorization": f"Bearer {bearer_token}"}
+
+    @property
+    @override
     def default_headers(self) -> dict[str, str | Omit]:
         return {
             **super().default_headers,
             "X-Stainless-Async": f"async:{get_async_library()}",
             **self._custom_headers,
         }
```

### Comparing `walledai-0.8.0a0/src/walledai/_compat.py` & `walledai-0.9.0a0/src/walledai/_compat.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_exceptions.py` & `walledai-0.9.0a0/src/walledai/_exceptions.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_files.py` & `walledai-0.9.0a0/src/walledai/_files.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_models.py` & `walledai-0.9.0a0/src/walledai/_models.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_qs.py` & `walledai-0.9.0a0/src/walledai/_qs.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_resource.py` & `walledai-0.9.0a0/src/walledai/_resource.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_response.py` & `walledai-0.9.0a0/src/walledai/_response.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_streaming.py` & `walledai-0.9.0a0/src/walledai/_streaming.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_types.py` & `walledai-0.9.0a0/src/walledai/_types.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_utils/__init__.py` & `walledai-0.9.0a0/src/walledai/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_utils/_logs.py` & `walledai-0.9.0a0/src/walledai/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_utils/_proxy.py` & `walledai-0.9.0a0/src/walledai/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_utils/_sync.py` & `walledai-0.9.0a0/src/walledai/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_utils/_transform.py` & `walledai-0.9.0a0/src/walledai/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_utils/_typing.py` & `walledai-0.9.0a0/src/walledai/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/_utils/_utils.py` & `walledai-0.9.0a0/src/walledai/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/resources/__init__.py` & `walledai-0.9.0a0/src/walledai/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/src/walledai/resources/moderation.py` & `walledai-0.9.0a0/src/walledai/resources/moderation.py`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/LICENSE` & `walledai-0.9.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `walledai-0.8.0a0/pyproject.toml` & `walledai-0.9.0a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "walledai"
-version = "0.8.0-alpha"
+version = "0.9.0-alpha"
 description = "The official Python library for the walledai API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Walledai", email = "admin@walled.ai" },
 ]
 dependencies = [
```

### Comparing `walledai-0.8.0a0/PKG-INFO` & `walledai-0.9.0a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: walledai
-Version: 0.8.0a0
+Version: 0.9.0a0
 Summary: The official Python library for the walledai API
 Project-URL: Homepage, https://github.com/rajatb94/walledai-python
 Project-URL: Repository, https://github.com/rajatb94/walledai-python
 Author-email: Walledai <admin@walled.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -56,34 +56,35 @@
 ## Usage
 
 The full API of this library can be found in [api.md](https://github.com/rajatb94/walledai-python/tree/main/api.md).
 
 ```python
 from walledai import Walledai
 
-client = Walledai(
-    bearer_token="My Bearer Token",
-)
+client = Walledai()
 
 moderation_create_response = client.moderation.create(
     text="string",
 )
 ```
 
+While you can provide a `bearer_token` keyword argument,
+we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
+to add `WALLEDAI_API_KEY="My Bearer Token"` to your `.env` file
+so that your Bearer Token is not stored in source control.
+
 ## Async usage
 
 Simply import `AsyncWalledai` instead of `Walledai` and use `await` with each API call:
 
 ```python
 import asyncio
 from walledai import AsyncWalledai
 
-client = AsyncWalledai(
-    bearer_token="My Bearer Token",
-)
+client = AsyncWalledai()
 
 
 async def main() -> None:
     moderation_create_response = await client.moderation.create(
         text="string",
     )
 
@@ -111,17 +112,15 @@
 
 All errors inherit from `walledai.APIError`.
 
 ```python
 import walledai
 from walledai import Walledai
 
-client = Walledai(
-    bearer_token="My Bearer Token",
-)
+client = Walledai()
 
 try:
     client.moderation.create(
         text="string",
     )
 except walledai.APIConnectionError as e:
     print("The server could not be reached")
@@ -158,15 +157,14 @@
 ```python
 from walledai import Walledai
 
 # Configure the default for all requests:
 client = Walledai(
     # default is 2
     max_retries=0,
-    bearer_token="My Bearer Token",
 )
 
 # Or, configure per-request:
 client.with_options(max_retries=5).moderation.create(
     text="string",
 )
 ```
@@ -179,21 +177,19 @@
 ```python
 from walledai import Walledai
 
 # Configure the default for all requests:
 client = Walledai(
     # 20 seconds (default is 1 minute)
     timeout=20.0,
-    bearer_token="My Bearer Token",
 )
 
 # More granular control:
 client = Walledai(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
-    bearer_token="My Bearer Token",
 )
 
 # Override per-request:
 client.with_options(timeout=5.0).moderation.create(
     text="string",
 )
 ```
@@ -229,17 +225,15 @@
 ### Accessing raw response data (e.g. headers)
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
 from walledai import Walledai
 
-client = Walledai(
-    bearer_token="My Bearer Token",
-)
+client = Walledai()
 response = client.moderation.with_raw_response.create(
     text="string",
 )
 print(response.headers.get('X-My-Header'))
 
 moderation = response.parse()  # get the object that `moderation.create()` would have returned
 print(moderation)
@@ -316,15 +310,14 @@
 client = Walledai(
     # Or use the `WALLEDAI_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
     http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
     ),
-    bearer_token="My Bearer Token",
 )
 ```
 
 ### Managing HTTP resources
 
 By default the library closes underlying HTTP connections whenever the client is [garbage collected](https://docs.python.org/3/reference/datamodel.html#object.__del__). You can manually close the client using the `.close()` method if desired, or with a context manager that closes when exiting.
```

