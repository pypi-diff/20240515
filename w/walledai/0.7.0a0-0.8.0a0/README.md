# Comparing `tmp/walledai-0.7.0a0.tar.gz` & `tmp/walledai-0.8.0a0.tar.gz`

## Comparing `walledai-0.7.0a0.tar` & `walledai-0.8.0a0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walled_ai/lib/.keep
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/__init__.py
--rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_base_client.py
--rw-r--r--   0        0        0    14792 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_constants.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_qs.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_resource.py
--rw-r--r--   0        0        0    28387 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_response.py
--rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_streaming.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_types.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/__init__.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/lib/.keep
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/resources/__init__.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/resources/moderation.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/types/__init__.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 walledai-0.7.0a0/src/walledai/types/moderation_create_params.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 walledai-0.7.0a0/.gitignore
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 walledai-0.7.0a0/LICENSE
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 walledai-0.7.0a0/pyproject.toml
--rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 walledai-0.7.0a0/PKG-INFO
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walled_ai/lib/.keep
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/__init__.py
+-rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_base_client.py
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_constants.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_qs.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_resource.py
+-rw-r--r--   0        0        0    28387 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_response.py
+-rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_streaming.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_types.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/__init__.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/lib/.keep
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/resources/__init__.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/resources/moderation.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/types/__init__.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 walledai-0.8.0a0/src/walledai/types/moderation_create_params.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 walledai-0.8.0a0/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 walledai-0.8.0a0/LICENSE
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 walledai-0.8.0a0/pyproject.toml
+-rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 walledai-0.8.0a0/PKG-INFO
```

### Comparing `walledai-0.7.0a0/src/walledai/__init__.py` & `walledai-0.8.0a0/src/walledai/__init__.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_base_client.py` & `walledai-0.8.0a0/src/walledai/_base_client.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_client.py` & `walledai-0.8.0a0/src/walledai/_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,20 +47,20 @@
 
 class Walledai(SyncAPIClient):
     moderation: resources.ModerationResource
     with_raw_response: WalledaiWithRawResponse
     with_streaming_response: WalledaiWithStreamedResponse
 
     # client options
-    api_key: str
+    bearer_token: str
 
     def __init__(
         self,
         *,
-        api_key: str | None = None,
+        bearer_token: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         # Configure a custom httpx client.
         # We provide a `DefaultHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
@@ -74,23 +74,23 @@
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new synchronous walledai client instance.
 
-        This automatically infers the `api_key` argument from the `WALLEDAI_API_KEY` environment variable if it is not provided.
+        This automatically infers the `bearer_token` argument from the `WALLEDAI_API_KEY` environment variable if it is not provided.
         """
-        if api_key is None:
-            api_key = os.environ.get("WALLEDAI_API_KEY")
-        if api_key is None:
+        if bearer_token is None:
+            bearer_token = os.environ.get("WALLEDAI_API_KEY")
+        if bearer_token is None:
             raise WalledaiError(
-                "The api_key client option must be set either by passing api_key to the client or by setting the WALLEDAI_API_KEY environment variable"
+                "The bearer_token client option must be set either by passing bearer_token to the client or by setting the WALLEDAI_API_KEY environment variable"
             )
-        self.api_key = api_key
+        self.bearer_token = bearer_token
 
         if base_url is None:
             base_url = os.environ.get("WALLEDAI_BASE_URL")
         if base_url is None:
             base_url = f"http://34.143.172.165"
 
         super().__init__(
@@ -121,15 +121,15 @@
             "X-Stainless-Async": "false",
             **self._custom_headers,
         }
 
     def copy(
         self,
         *,
-        api_key: str | None = None,
+        bearer_token: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.Client | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
         default_headers: Mapping[str, str] | None = None,
         set_default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
@@ -155,15 +155,15 @@
         if default_query is not None:
             params = {**params, **default_query}
         elif set_default_query is not None:
             params = set_default_query
 
         http_client = http_client or self._client
         return self.__class__(
-            api_key=api_key or self.api_key,
+            bearer_token=bearer_token or self.bearer_token,
             base_url=base_url or self.base_url,
             timeout=self.timeout if isinstance(timeout, NotGiven) else timeout,
             http_client=http_client,
             max_retries=max_retries if is_given(max_retries) else self.max_retries,
             default_headers=headers,
             default_query=params,
             **_extra_kwargs,
@@ -209,20 +209,20 @@
 
 class AsyncWalledai(AsyncAPIClient):
     moderation: resources.AsyncModerationResource
     with_raw_response: AsyncWalledaiWithRawResponse
     with_streaming_response: AsyncWalledaiWithStreamedResponse
 
     # client options
-    api_key: str
+    bearer_token: str
 
     def __init__(
         self,
         *,
-        api_key: str | None = None,
+        bearer_token: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         # Configure a custom httpx client.
         # We provide a `DefaultAsyncHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
@@ -236,23 +236,23 @@
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new async walledai client instance.
 
-        This automatically infers the `api_key` argument from the `WALLEDAI_API_KEY` environment variable if it is not provided.
+        This automatically infers the `bearer_token` argument from the `WALLEDAI_API_KEY` environment variable if it is not provided.
         """
-        if api_key is None:
-            api_key = os.environ.get("WALLEDAI_API_KEY")
-        if api_key is None:
+        if bearer_token is None:
+            bearer_token = os.environ.get("WALLEDAI_API_KEY")
+        if bearer_token is None:
             raise WalledaiError(
-                "The api_key client option must be set either by passing api_key to the client or by setting the WALLEDAI_API_KEY environment variable"
+                "The bearer_token client option must be set either by passing bearer_token to the client or by setting the WALLEDAI_API_KEY environment variable"
             )
-        self.api_key = api_key
+        self.bearer_token = bearer_token
 
         if base_url is None:
             base_url = os.environ.get("WALLEDAI_BASE_URL")
         if base_url is None:
             base_url = f"http://34.143.172.165"
 
         super().__init__(
@@ -283,15 +283,15 @@
             "X-Stainless-Async": f"async:{get_async_library()}",
             **self._custom_headers,
         }
 
     def copy(
         self,
         *,
-        api_key: str | None = None,
+        bearer_token: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.AsyncClient | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
         default_headers: Mapping[str, str] | None = None,
         set_default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
@@ -317,15 +317,15 @@
         if default_query is not None:
             params = {**params, **default_query}
         elif set_default_query is not None:
             params = set_default_query
 
         http_client = http_client or self._client
         return self.__class__(
-            api_key=api_key or self.api_key,
+            bearer_token=bearer_token or self.bearer_token,
             base_url=base_url or self.base_url,
             timeout=self.timeout if isinstance(timeout, NotGiven) else timeout,
             http_client=http_client,
             max_retries=max_retries if is_given(max_retries) else self.max_retries,
             default_headers=headers,
             default_query=params,
             **_extra_kwargs,
```

### Comparing `walledai-0.7.0a0/src/walledai/_compat.py` & `walledai-0.8.0a0/src/walledai/_compat.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_exceptions.py` & `walledai-0.8.0a0/src/walledai/_exceptions.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_files.py` & `walledai-0.8.0a0/src/walledai/_files.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_models.py` & `walledai-0.8.0a0/src/walledai/_models.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_qs.py` & `walledai-0.8.0a0/src/walledai/_qs.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_resource.py` & `walledai-0.8.0a0/src/walledai/_resource.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_response.py` & `walledai-0.8.0a0/src/walledai/_response.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_streaming.py` & `walledai-0.8.0a0/src/walledai/_streaming.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_types.py` & `walledai-0.8.0a0/src/walledai/_types.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_utils/__init__.py` & `walledai-0.8.0a0/src/walledai/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_utils/_logs.py` & `walledai-0.8.0a0/src/walledai/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_utils/_proxy.py` & `walledai-0.8.0a0/src/walledai/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_utils/_sync.py` & `walledai-0.8.0a0/src/walledai/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_utils/_transform.py` & `walledai-0.8.0a0/src/walledai/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_utils/_typing.py` & `walledai-0.8.0a0/src/walledai/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/_utils/_utils.py` & `walledai-0.8.0a0/src/walledai/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/resources/__init__.py` & `walledai-0.8.0a0/src/walledai/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/src/walledai/resources/moderation.py` & `walledai-0.8.0a0/src/walledai/resources/moderation.py`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/LICENSE` & `walledai-0.8.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `walledai-0.7.0a0/pyproject.toml` & `walledai-0.8.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "walledai"
-version = "0.7.0-alpha"
+version = "0.8.0-alpha"
 description = "The official Python library for the walledai API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Walledai", email = "admin@walled.ai" },
 ]
 dependencies = [
```

### Comparing `walledai-0.7.0a0/PKG-INFO` & `walledai-0.8.0a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: walledai
-Version: 0.7.0a0
+Version: 0.8.0a0
 Summary: The official Python library for the walledai API
 Project-URL: Homepage, https://github.com/rajatb94/walledai-python
 Project-URL: Repository, https://github.com/rajatb94/walledai-python
 Author-email: Walledai <admin@walled.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -57,15 +57,15 @@
 
 The full API of this library can be found in [api.md](https://github.com/rajatb94/walledai-python/tree/main/api.md).
 
 ```python
 from walledai import Walledai
 
 client = Walledai(
-    api_key="My API Key",
+    bearer_token="My Bearer Token",
 )
 
 moderation_create_response = client.moderation.create(
     text="string",
 )
 ```
 
@@ -74,15 +74,15 @@
 Simply import `AsyncWalledai` instead of `Walledai` and use `await` with each API call:
 
 ```python
 import asyncio
 from walledai import AsyncWalledai
 
 client = AsyncWalledai(
-    api_key="My API Key",
+    bearer_token="My Bearer Token",
 )
 
 
 async def main() -> None:
     moderation_create_response = await client.moderation.create(
         text="string",
     )
@@ -112,15 +112,15 @@
 All errors inherit from `walledai.APIError`.
 
 ```python
 import walledai
 from walledai import Walledai
 
 client = Walledai(
-    api_key="My API Key",
+    bearer_token="My Bearer Token",
 )
 
 try:
     client.moderation.create(
         text="string",
     )
 except walledai.APIConnectionError as e:
@@ -158,15 +158,15 @@
 ```python
 from walledai import Walledai
 
 # Configure the default for all requests:
 client = Walledai(
     # default is 2
     max_retries=0,
-    api_key="My API Key",
+    bearer_token="My Bearer Token",
 )
 
 # Or, configure per-request:
 client.with_options(max_retries=5).moderation.create(
     text="string",
 )
 ```
@@ -179,21 +179,21 @@
 ```python
 from walledai import Walledai
 
 # Configure the default for all requests:
 client = Walledai(
     # 20 seconds (default is 1 minute)
     timeout=20.0,
-    api_key="My API Key",
+    bearer_token="My Bearer Token",
 )
 
 # More granular control:
 client = Walledai(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
-    api_key="My API Key",
+    bearer_token="My Bearer Token",
 )
 
 # Override per-request:
 client.with_options(timeout=5.0).moderation.create(
     text="string",
 )
 ```
@@ -230,15 +230,15 @@
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
 from walledai import Walledai
 
 client = Walledai(
-    api_key="My API Key",
+    bearer_token="My Bearer Token",
 )
 response = client.moderation.with_raw_response.create(
     text="string",
 )
 print(response.headers.get('X-My-Header'))
 
 moderation = response.parse()  # get the object that `moderation.create()` would have returned
@@ -316,15 +316,15 @@
 client = Walledai(
     # Or use the `WALLEDAI_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
     http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
     ),
-    api_key="My API Key",
+    bearer_token="My Bearer Token",
 )
 ```
 
 ### Managing HTTP resources
 
 By default the library closes underlying HTTP connections whenever the client is [garbage collected](https://docs.python.org/3/reference/datamodel.html#object.__del__). You can manually close the client using the `.close()` method if desired, or with a context manager that closes when exiting.
```

