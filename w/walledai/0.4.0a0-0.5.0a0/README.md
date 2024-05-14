# Comparing `tmp/walledai-0.4.0a0.tar.gz` & `tmp/walledai-0.5.0a0.tar.gz`

## Comparing `walledai-0.4.0a0.tar` & `walledai-0.5.0a0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/__init__.py
--rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_base_client.py
--rw-r--r--   0        0        0    14794 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_constants.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_qs.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_resource.py
--rw-r--r--   0        0        0    28391 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_response.py
--rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_streaming.py
--rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_types.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_utils/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/lib/.keep
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/resources/__init__.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/resources/moderation.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/types/__init__.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walled_ai/types/moderation_create_params.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.4.0a0/src/walledai/lib/.keep
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 walledai-0.4.0a0/.gitignore
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 walledai-0.4.0a0/LICENSE
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 walledai-0.4.0a0/pyproject.toml
--rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 walledai-0.4.0a0/PKG-INFO
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walled_ai/lib/.keep
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/__init__.py
+-rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_base_client.py
+-rw-r--r--   0        0        0    14792 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_constants.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_qs.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_resource.py
+-rw-r--r--   0        0        0    28387 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_response.py
+-rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_streaming.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_types.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_utils/__init__.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/lib/.keep
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/resources/__init__.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/resources/moderation.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/types/__init__.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 walledai-0.5.0a0/src/walledai/types/moderation_create_params.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 walledai-0.5.0a0/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 walledai-0.5.0a0/LICENSE
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 walledai-0.5.0a0/pyproject.toml
+-rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 walledai-0.5.0a0/PKG-INFO
```

### Comparing `walledai-0.4.0a0/src/walled_ai/__init__.py` & `walledai-0.5.0a0/src/walledai/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from . import types
 from ._types import NOT_GIVEN, NoneType, NotGiven, Transport, ProxiesTypes
 from ._utils import file_from_path
 from ._client import (
     Client,
     Stream,
     Timeout,
-    WalledAI,
+    Walledai,
     Transport,
     AsyncClient,
     AsyncStream,
-    AsyncWalledAI,
+    AsyncWalledai,
     RequestOptions,
 )
 from ._models import BaseModel
 from ._version import __title__, __version__
 from ._response import APIResponse as APIResponse, AsyncAPIResponse as AsyncAPIResponse
 from ._constants import DEFAULT_TIMEOUT, DEFAULT_MAX_RETRIES, DEFAULT_CONNECTION_LIMITS
 from ._exceptions import (
     APIError,
     ConflictError,
     NotFoundError,
-    WalledAIError,
+    WalledaiError,
     APIStatusError,
     RateLimitError,
     APITimeoutError,
     BadRequestError,
     APIConnectionError,
     AuthenticationError,
     InternalServerError,
@@ -42,15 +42,15 @@
     "__version__",
     "__title__",
     "NoneType",
     "Transport",
     "ProxiesTypes",
     "NotGiven",
     "NOT_GIVEN",
-    "WalledAIError",
+    "WalledaiError",
     "APIError",
     "APIStatusError",
     "APITimeoutError",
     "APIConnectionError",
     "APIResponseValidationError",
     "BadRequestError",
     "AuthenticationError",
@@ -62,32 +62,32 @@
     "InternalServerError",
     "Timeout",
     "RequestOptions",
     "Client",
     "AsyncClient",
     "Stream",
     "AsyncStream",
-    "WalledAI",
-    "AsyncWalledAI",
+    "Walledai",
+    "AsyncWalledai",
     "file_from_path",
     "BaseModel",
     "DEFAULT_TIMEOUT",
     "DEFAULT_MAX_RETRIES",
     "DEFAULT_CONNECTION_LIMITS",
     "DefaultHttpxClient",
     "DefaultAsyncHttpxClient",
 ]
 
 _setup_logging()
 
 # Update the __module__ attribute for exported symbols so that
 # error messages point to this module instead of the module
 # it was originally defined in, e.g.
-# walled_ai._exceptions.NotFoundError -> walled_ai.NotFoundError
+# walledai._exceptions.NotFoundError -> walledai.NotFoundError
 __locals = locals()
 for __name in __all__:
     if not __name.startswith("__"):
         try:
-            __locals[__name].__module__ = "walled_ai"
+            __locals[__name].__module__ = "walledai"
         except (TypeError, AttributeError):
             # Some of our exported symbols are builtins which we can't set attributes for.
             pass
```

### Comparing `walledai-0.4.0a0/src/walled_ai/_base_client.py` & `walledai-0.5.0a0/src/walledai/_base_client.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/src/walled_ai/_client.py` & `walledai-0.5.0a0/src/walledai/_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,38 +21,38 @@
 )
 from ._utils import (
     is_given,
     get_async_library,
 )
 from ._version import __version__
 from ._streaming import Stream as Stream, AsyncStream as AsyncStream
-from ._exceptions import WalledAIError, APIStatusError
+from ._exceptions import WalledaiError, APIStatusError
 from ._base_client import (
     DEFAULT_MAX_RETRIES,
     SyncAPIClient,
     AsyncAPIClient,
 )
 
 __all__ = [
     "Timeout",
     "Transport",
     "ProxiesTypes",
     "RequestOptions",
     "resources",
-    "WalledAI",
-    "AsyncWalledAI",
+    "Walledai",
+    "AsyncWalledai",
     "Client",
     "AsyncClient",
 ]
 
 
-class WalledAI(SyncAPIClient):
+class Walledai(SyncAPIClient):
     moderation: resources.ModerationResource
-    with_raw_response: WalledAIWithRawResponse
-    with_streaming_response: WalledAIWithStreamedResponse
+    with_raw_response: WalledaiWithRawResponse
+    with_streaming_response: WalledaiWithStreamedResponse
 
     # client options
     api_key: str
 
     def __init__(
         self,
         *,
@@ -72,28 +72,28 @@
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
-        """Construct a new synchronous WalledAI client instance.
+        """Construct a new synchronous walledai client instance.
 
         This automatically infers the `api_key` argument from the `WALLEDAI_API_KEY` environment variable if it is not provided.
         """
         if api_key is None:
             api_key = os.environ.get("WALLEDAI_API_KEY")
         if api_key is None:
-            raise WalledAIError(
+            raise WalledaiError(
                 "The api_key client option must be set either by passing api_key to the client or by setting the WALLEDAI_API_KEY environment variable"
             )
         self.api_key = api_key
 
         if base_url is None:
-            base_url = os.environ.get("WALLED_AI_BASE_URL")
+            base_url = os.environ.get("WALLEDAI_BASE_URL")
         if base_url is None:
             base_url = f"http://34.143.172.165"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
@@ -101,16 +101,16 @@
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
         self.moderation = resources.ModerationResource(self)
-        self.with_raw_response = WalledAIWithRawResponse(self)
-        self.with_streaming_response = WalledAIWithStreamedResponse(self)
+        self.with_raw_response = WalledaiWithRawResponse(self)
+        self.with_streaming_response = WalledaiWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
@@ -203,18 +203,18 @@
             return _exceptions.RateLimitError(err_msg, response=response, body=body)
 
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
-class AsyncWalledAI(AsyncAPIClient):
+class AsyncWalledai(AsyncAPIClient):
     moderation: resources.AsyncModerationResource
-    with_raw_response: AsyncWalledAIWithRawResponse
-    with_streaming_response: AsyncWalledAIWithStreamedResponse
+    with_raw_response: AsyncWalledaiWithRawResponse
+    with_streaming_response: AsyncWalledaiWithStreamedResponse
 
     # client options
     api_key: str
 
     def __init__(
         self,
         *,
@@ -234,28 +234,28 @@
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
-        """Construct a new async WalledAI client instance.
+        """Construct a new async walledai client instance.
 
         This automatically infers the `api_key` argument from the `WALLEDAI_API_KEY` environment variable if it is not provided.
         """
         if api_key is None:
             api_key = os.environ.get("WALLEDAI_API_KEY")
         if api_key is None:
-            raise WalledAIError(
+            raise WalledaiError(
                 "The api_key client option must be set either by passing api_key to the client or by setting the WALLEDAI_API_KEY environment variable"
             )
         self.api_key = api_key
 
         if base_url is None:
-            base_url = os.environ.get("WALLED_AI_BASE_URL")
+            base_url = os.environ.get("WALLEDAI_BASE_URL")
         if base_url is None:
             base_url = f"http://34.143.172.165"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
@@ -263,16 +263,16 @@
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
         self.moderation = resources.AsyncModerationResource(self)
-        self.with_raw_response = AsyncWalledAIWithRawResponse(self)
-        self.with_streaming_response = AsyncWalledAIWithStreamedResponse(self)
+        self.with_raw_response = AsyncWalledaiWithRawResponse(self)
+        self.with_streaming_response = AsyncWalledaiWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
@@ -365,30 +365,30 @@
             return _exceptions.RateLimitError(err_msg, response=response, body=body)
 
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
-class WalledAIWithRawResponse:
-    def __init__(self, client: WalledAI) -> None:
+class WalledaiWithRawResponse:
+    def __init__(self, client: Walledai) -> None:
         self.moderation = resources.ModerationResourceWithRawResponse(client.moderation)
 
 
-class AsyncWalledAIWithRawResponse:
-    def __init__(self, client: AsyncWalledAI) -> None:
+class AsyncWalledaiWithRawResponse:
+    def __init__(self, client: AsyncWalledai) -> None:
         self.moderation = resources.AsyncModerationResourceWithRawResponse(client.moderation)
 
 
-class WalledAIWithStreamedResponse:
-    def __init__(self, client: WalledAI) -> None:
+class WalledaiWithStreamedResponse:
+    def __init__(self, client: Walledai) -> None:
         self.moderation = resources.ModerationResourceWithStreamingResponse(client.moderation)
 
 
-class AsyncWalledAIWithStreamedResponse:
-    def __init__(self, client: AsyncWalledAI) -> None:
+class AsyncWalledaiWithStreamedResponse:
+    def __init__(self, client: AsyncWalledai) -> None:
         self.moderation = resources.AsyncModerationResourceWithStreamingResponse(client.moderation)
 
 
-Client = WalledAI
+Client = Walledai
 
-AsyncClient = AsyncWalledAI
+AsyncClient = AsyncWalledai
```

### Comparing `walledai-0.4.0a0/src/walled_ai/_compat.py` & `walledai-0.5.0a0/src/walledai/_compat.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/src/walled_ai/_exceptions.py` & `walledai-0.5.0a0/src/walledai/_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     "ConflictError",
     "UnprocessableEntityError",
     "RateLimitError",
     "InternalServerError",
 ]
 
 
-class WalledAIError(Exception):
+class WalledaiError(Exception):
     pass
 
 
-class APIError(WalledAIError):
+class APIError(WalledaiError):
     message: str
     request: httpx.Request
 
     body: object | None
     """The API response body.
 
     If the API responded with a valid JSON structure then this property will be the
```

### Comparing `walledai-0.4.0a0/src/walled_ai/_files.py` & `walledai-0.5.0a0/src/walledai/_files.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/src/walled_ai/_models.py` & `walledai-0.5.0a0/src/walledai/_models.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/src/walled_ai/_qs.py` & `walledai-0.5.0a0/src/walledai/_qs.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/src/walled_ai/_response.py` & `walledai-0.5.0a0/src/walledai/_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import pydantic
 
 from ._types import NoneType
 from ._utils import is_given, extract_type_arg, is_annotated_type, extract_type_var_from_base
 from ._models import BaseModel, is_basemodel
 from ._constants import RAW_RESPONSE_HEADER, OVERRIDE_CAST_TO_HEADER
 from ._streaming import Stream, AsyncStream, is_stream_class_type, extract_stream_chunk_type
-from ._exceptions import WalledAIError, APIResponseValidationError
+from ._exceptions import WalledaiError, APIResponseValidationError
 
 if TYPE_CHECKING:
     from ._models import FinalRequestOptions
     from ._base_client import BaseClient
 
 
 P = ParamSpec("P")
@@ -199,15 +199,15 @@
             # the response class ourselves but that is something that should be supported directly in httpx
             # as it would be easy to incorrectly construct the Response object due to the multitude of arguments.
             if cast_to != httpx.Response:
                 raise ValueError(f"Subclasses of httpx.Response cannot be passed to `cast_to`")
             return cast(R, response)
 
         if inspect.isclass(origin) and not issubclass(origin, BaseModel) and issubclass(origin, pydantic.BaseModel):
-            raise TypeError("Pydantic models must subclass our base model type, e.g. `from walled_ai import BaseModel`")
+            raise TypeError("Pydantic models must subclass our base model type, e.g. `from walledai import BaseModel`")
 
         if (
             cast_to is not object
             and not origin is list
             and not origin is dict
             and not origin is Union
             and not issubclass(origin, BaseModel)
@@ -267,15 +267,15 @@
 
         For lower-level control, see `.read()`, `.json()`, `.iter_bytes()`.
 
         You can customise the type that the response is parsed into through
         the `to` argument, e.g.
 
         ```py
-        from walled_ai import BaseModel
+        from walledai import BaseModel
 
 
         class MyModel(BaseModel):
             foo: str
 
 
         obj = response.parse(to=MyModel)
@@ -371,15 +371,15 @@
 
         For lower-level control, see `.read()`, `.json()`, `.iter_bytes()`.
 
         You can customise the type that the response is parsed into through
         the `to` argument, e.g.
 
         ```py
-        from walled_ai import BaseModel
+        from walledai import BaseModel
 
 
         class MyModel(BaseModel):
             foo: str
 
 
         obj = response.parse(to=MyModel)
@@ -542,19 +542,19 @@
             async for data in self.iter_bytes(chunk_size):
                 await f.write(data)
 
 
 class MissingStreamClassError(TypeError):
     def __init__(self) -> None:
         super().__init__(
-            "The `stream` argument was set to `True` but the `stream_cls` argument was not given. See `walled_ai._streaming` for reference",
+            "The `stream` argument was set to `True` but the `stream_cls` argument was not given. See `walledai._streaming` for reference",
         )
 
 
-class StreamAlreadyConsumed(WalledAIError):
+class StreamAlreadyConsumed(WalledaiError):
     """
     Attempted to read or stream content, but the content has already
     been streamed.
 
     This can happen if you use a method like `.iter_lines()` and then attempt
     to read th entire response body afterwards, e.g.
```

### Comparing `walledai-0.4.0a0/src/walled_ai/_streaming.py` & `walledai-0.5.0a0/src/walledai/_streaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing_extensions import Self, Protocol, TypeGuard, override, get_origin, runtime_checkable
 
 import httpx
 
 from ._utils import extract_type_var_from_base
 
 if TYPE_CHECKING:
-    from ._client import WalledAI, AsyncWalledAI
+    from ._client import Walledai, AsyncWalledai
 
 
 _T = TypeVar("_T")
 
 
 class Stream(Generic[_T]):
     """Provides the core interface to iterate over a synchronous stream response."""
@@ -26,15 +26,15 @@
     _decoder: SSEBytesDecoder
 
     def __init__(
         self,
         *,
         cast_to: type[_T],
         response: httpx.Response,
-        client: WalledAI,
+        client: Walledai,
     ) -> None:
         self.response = response
         self._cast_to = cast_to
         self._client = client
         self._decoder = client._make_sse_decoder()
         self._iterator = self.__stream__()
 
@@ -89,15 +89,15 @@
     _decoder: SSEDecoder | SSEBytesDecoder
 
     def __init__(
         self,
         *,
         cast_to: type[_T],
         response: httpx.Response,
-        client: AsyncWalledAI,
+        client: AsyncWalledai,
     ) -> None:
         self.response = response
         self._cast_to = cast_to
         self._client = client
         self._decoder = client._make_sse_decoder()
         self._iterator = self.__stream__()
```

### Comparing `walledai-0.4.0a0/src/walled_ai/_types.py` & `walledai-0.5.0a0/src/walledai/_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 # method that uses `ResponseT` which would lead to an unacceptable
 # amount of code duplication and make it unreadable. See _base_client.py
 # for example usage.
 #
 # This unfortunately means that you will either have
 # to import this type and pass it explicitly:
 #
-# from walled_ai import NoneType
+# from walledai import NoneType
 # client.get('/foo', cast_to=NoneType)
 #
 # or build it yourself:
 #
 # client.get('/foo', cast_to=type(None))
 if TYPE_CHECKING:
     NoneType: Type[None]
```

### Comparing `walledai-0.4.0a0/src/walled_ai/_utils/__init__.py` & `walledai-0.5.0a0/src/walledai/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/src/walled_ai/_utils/_proxy.py` & `walledai-0.5.0a0/src/walledai/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/src/walled_ai/_utils/_sync.py` & `walledai-0.5.0a0/src/walledai/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/src/walled_ai/_utils/_transform.py` & `walledai-0.5.0a0/src/walledai/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/src/walled_ai/_utils/_typing.py` & `walledai-0.5.0a0/src/walledai/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/src/walled_ai/_utils/_utils.py` & `walledai-0.5.0a0/src/walledai/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/src/walled_ai/resources/__init__.py` & `walledai-0.5.0a0/src/walledai/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/src/walled_ai/resources/moderation.py` & `walledai-0.5.0a0/src/walledai/resources/moderation.py`

 * *Files identical despite different names*

### Comparing `walledai-0.4.0a0/LICENSE` & `walledai-0.5.0a0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2024 Walled AI
+   Copyright 2024 Walledai
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `walledai-0.4.0a0/pyproject.toml` & `walledai-0.5.0a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "walledai"
-version = "0.4.0-alpha"
-description = "The official Python library for the WalledAI API"
+version = "0.5.0-alpha"
+description = "The official Python library for the walledai API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
-{ name = "Walled AI", email = "admin@walledai.com" },
+{ name = "Walledai", email = "admin@walled.ai" },
 ]
 dependencies = [
     "httpx>=0.23.0, <1",
     "pydantic>=1.9.0, <3",
     "typing-extensions>=4.7, <5",
     "anyio>=3.5.0, <5",
     "distro>=1.7.0, <2",
@@ -80,28 +80,28 @@
 "fix:ruff" = "ruff --fix ."
 
 typecheck = { chain = [
   "typecheck:pyright",
   "typecheck:mypy"
 ]}
 "typecheck:pyright" = "pyright"
-"typecheck:verify-types" = "pyright --verifytypes walled_ai --ignoreexternal"
+"typecheck:verify-types" = "pyright --verifytypes walledai --ignoreexternal"
 "typecheck:mypy" = "mypy ."
 
 [build-system]
 requires = ["hatchling", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = [
   "src/*"
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/walled_ai"]
+packages = ["src/walledai"]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 
@@ -183,14 +183,14 @@
 "functools.lru_cache".msg = "This function does not retain type information for the wrapped function's arguments; The `lru_cache` function from `_utils` should be used instead"
 
 [tool.ruff.lint.isort]
 length-sort = true
 length-sort-straight = true
 combine-as-imports = true
 extra-standard-library = ["typing_extensions"]
-known-first-party = ["walled_ai", "tests"]
+known-first-party = ["walledai", "tests"]
 
 [tool.ruff.per-file-ignores]
 "bin/**.py" = ["T201", "T203"]
 "scripts/**.py" = ["T201", "T203"]
 "tests/**.py" = ["T201", "T203"]
 "examples/**.py" = ["T201", "T203"]
```

### Comparing `walledai-0.4.0a0/PKG-INFO` & `walledai-0.5.0a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: walledai
-Version: 0.4.0a0
-Summary: The official Python library for the WalledAI API
+Version: 0.5.0a0
+Summary: The official Python library for the walledai API
 Project-URL: Homepage, https://github.com/rajatb94/walledai-python
 Project-URL: Repository, https://github.com/rajatb94/walledai-python
-Author-email: Walled AI <admin@walledai.com>
+Author-email: Walledai <admin@walled.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
@@ -28,19 +28,19 @@
 Requires-Dist: distro<2,>=1.7.0
 Requires-Dist: httpx<1,>=0.23.0
 Requires-Dist: pydantic<3,>=1.9.0
 Requires-Dist: sniffio
 Requires-Dist: typing-extensions<5,>=4.7
 Description-Content-Type: text/markdown
 
-# Walled AI Python API library
+# WalledAI API library
 
 [![PyPI version](https://img.shields.io/pypi/v/walledai.svg)](https://pypi.org/project/walledai/)
 
-The Walled AI Python library provides convenient access to the Walled AI REST API from any Python 3.7+
+The WalledAI library provides convenient access to the Walledai REST API from any Python 3.7+
 application. The library includes type definitions for all request params and response fields,
 and offers both synchronous and asynchronous clients powered by [httpx](https://github.com/encode/httpx).
 
 It is generated with [Stainless](https://www.stainlessapi.com/).
 
 ## Documentation
 
@@ -54,34 +54,34 @@
 ```
 
 ## Usage
 
 The full API of this library can be found in [api.md](https://github.com/rajatb94/walledai-python/tree/main/api.md).
 
 ```python
-from walled_ai import WalledAI
+from walledai import Walledai
 
-client = WalledAI(
+client = Walledai(
     api_key="My API Key",
 )
 
 moderation_create_response = client.moderation.create(
     text="string",
 )
 ```
 
 ## Async usage
 
-Simply import `AsyncWalledAI` instead of `WalledAI` and use `await` with each API call:
+Simply import `AsyncWalledai` instead of `Walledai` and use `await` with each API call:
 
 ```python
 import asyncio
-from walled_ai import AsyncWalledAI
+from walledai import AsyncWalledai
 
-client = AsyncWalledAI(
+client = AsyncWalledai(
     api_key="My API Key",
 )
 
 
 async def main() -> None:
     moderation_create_response = await client.moderation.create(
         text="string",
@@ -100,39 +100,39 @@
 - Serializing back into JSON, `model.to_json()`
 - Converting to a dictionary, `model.to_dict()`
 
 Typed requests and responses provide autocomplete and documentation within your editor. If you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `basic`.
 
 ## Handling errors
 
-When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `walled_ai.APIConnectionError` is raised.
+When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `walledai.APIConnectionError` is raised.
 
 When the API returns a non-success status code (that is, 4xx or 5xx
-response), a subclass of `walled_ai.APIStatusError` is raised, containing `status_code` and `response` properties.
+response), a subclass of `walledai.APIStatusError` is raised, containing `status_code` and `response` properties.
 
-All errors inherit from `walled_ai.APIError`.
+All errors inherit from `walledai.APIError`.
 
 ```python
-import walled_ai
-from walled_ai import WalledAI
+import walledai
+from walledai import Walledai
 
-client = WalledAI(
+client = Walledai(
     api_key="My API Key",
 )
 
 try:
     client.moderation.create(
         text="string",
     )
-except walled_ai.APIConnectionError as e:
+except walledai.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
-except walled_ai.RateLimitError as e:
+except walledai.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
-except walled_ai.APIStatusError as e:
+except walledai.APIStatusError as e:
     print("Another non-200-range status code was received")
     print(e.status_code)
     print(e.response)
 ```
 
 Error codes are as followed:
 
@@ -152,18 +152,18 @@
 Certain errors are automatically retried 2 times by default, with a short exponential backoff.
 Connection errors (for example, due to a network connectivity problem), 408 Request Timeout, 409 Conflict,
 429 Rate Limit, and >=500 Internal errors are all retried by default.
 
 You can use the `max_retries` option to configure or disable retry settings:
 
 ```python
-from walled_ai import WalledAI
+from walledai import Walledai
 
 # Configure the default for all requests:
-client = WalledAI(
+client = Walledai(
     # default is 2
     max_retries=0,
     api_key="My API Key",
 )
 
 # Or, configure per-request:
 client.with_options(max_retries=5).moderation.create(
@@ -173,25 +173,25 @@
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration) object:
 
 ```python
-from walled_ai import WalledAI
+from walledai import Walledai
 
 # Configure the default for all requests:
-client = WalledAI(
+client = Walledai(
     # 20 seconds (default is 1 minute)
     timeout=20.0,
     api_key="My API Key",
 )
 
 # More granular control:
-client = WalledAI(
+client = Walledai(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
     api_key="My API Key",
 )
 
 # Override per-request:
 client.with_options(timeout=5.0).moderation.create(
     text="string",
@@ -204,18 +204,18 @@
 
 ## Advanced
 
 ### Logging
 
 We use the standard library [`logging`](https://docs.python.org/3/library/logging.html) module.
 
-You can enable logging by setting the environment variable `WALLED_AI_LOG` to `debug`.
+You can enable logging by setting the environment variable `WALLEDAI_LOG` to `debug`.
 
 ```shell
-$ export WALLED_AI_LOG=debug
+$ export WALLEDAI_LOG=debug
 ```
 
 ### How to tell whether `None` means `null` or missing
 
 In an API response, a field may be explicitly `null`, or missing entirely; in either case, its value is `None` in this library. You can differentiate the two cases with `.model_fields_set`:
 
 ```py
@@ -227,31 +227,31 @@
 ```
 
 ### Accessing raw response data (e.g. headers)
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
-from walled_ai import WalledAI
+from walledai import Walledai
 
-client = WalledAI(
+client = Walledai(
     api_key="My API Key",
 )
 response = client.moderation.with_raw_response.create(
     text="string",
 )
 print(response.headers.get('X-My-Header'))
 
 moderation = response.parse()  # get the object that `moderation.create()` would have returned
 print(moderation)
 ```
 
-These methods return an [`APIResponse`](https://github.com/rajatb94/walledai-python/tree/main/src/walled_ai/_response.py) object.
+These methods return an [`APIResponse`](https://github.com/rajatb94/walledai-python/tree/main/src/walledai/_response.py) object.
 
-The async client returns an [`AsyncAPIResponse`](https://github.com/rajatb94/walledai-python/tree/main/src/walled_ai/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
+The async client returns an [`AsyncAPIResponse`](https://github.com/rajatb94/walledai-python/tree/main/src/walledai/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
 
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
@@ -307,18 +307,18 @@
 You can directly override the [httpx client](https://www.python-httpx.org/api/#client) to customize it for your use case, including:
 
 - Support for proxies
 - Custom transports
 - Additional [advanced](https://www.python-httpx.org/advanced/#client-instances) functionality
 
 ```python
-from walled_ai import WalledAI, DefaultHttpxClient
+from walledai import Walledai, DefaultHttpxClient
 
-client = WalledAI(
-    # Or use the `WALLED_AI_BASE_URL` env var
+client = Walledai(
+    # Or use the `WALLEDAI_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
     http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
     ),
     api_key="My API Key",
 )
```

