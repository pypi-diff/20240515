# Comparing `tmp/martian_adapters-5.1.1.tar.gz` & `tmp/martian_adapters-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martian_adapters-5.1.1.tar", max compression
+gzip compressed data, was "martian_adapters-5.1.2.tar", max compression
```

## Comparing `martian_adapters-5.1.1.tar` & `martian_adapters-5.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    35149 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/LICENSE
--rw-r--r--   0        0        0     3553 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/README.md
--rw-r--r--   0        0        0      725 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/__init__.py
--rw-r--r--   0        0        0      305 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/__init__.py
--rw-r--r--   0        0        0     2188 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/api_key_adapter_mixin.py
--rw-r--r--   0        0        0     2125 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/base_adapter.py
--rw-r--r--   0        0        0     1226 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/chat_http_api_adapter.py
--rw-r--r--   0        0        0     7525 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/http_api_adapter_mixin.py
--rw-r--r--   0        0        0     2486 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/openai_sdk_chat_adapter.py
--rw-r--r--   0        0        0      523 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/provider_adapter_mixin.py
--rw-r--r--   0        0        0     5893 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/abstract_adapters/sdk_chat_adapter.py
--rw-r--r--   0        0        0     6154 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/adapter_factory.py
--rw-r--r--   0        0        0       59 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/concrete_adapters/__init__.py
--rw-r--r--   0        0        0     3416 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/concrete_adapters/you_com_rag_chat_adapter.py
--rw-r--r--   0        0        0     1017 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/__init__.py
--rw-r--r--   0        0        0     9231 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     3934 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2412 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2587 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     7317 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1836 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     3196 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1757 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1331 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4444 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2450 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2602 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0    11047 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0        0 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/py.typed
--rw-r--r--   0        0        0      558 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/rate_limiter.py
--rw-r--r--   0        0        0      316 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/requirements.txt
--rw-r--r--   0        0        0     7005 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/types.py
--rw-r--r--   0        0        0        0 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/utils/__init__.py
--rw-r--r--   0        0        0      263 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/utils/adapter_stream_response.py
--rw-r--r--   0        0        0     1064 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/utils/general_utils.py
--rw-r--r--   0        0        0     2492 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/utils/network_utils.py
--rw-r--r--   0        0        0     8173 2024-05-14 19:42:09.248781 martian_adapters-5.1.1/adapters/utils/openai_client_factory.py
--rw-r--r--   0        0        0     1147 2024-05-14 19:42:09.252781 martian_adapters-5.1.1/pyproject.toml
--rw-r--r--   0        0        0     4854 1970-01-01 00:00:00.000000 martian_adapters-5.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/LICENSE
+-rw-r--r--   0        0        0     3553 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/README.md
+-rw-r--r--   0        0        0      725 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/api_key_adapter_mixin.py
+-rw-r--r--   0        0        0     2125 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/base_adapter.py
+-rw-r--r--   0        0        0     1226 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/chat_http_api_adapter.py
+-rw-r--r--   0        0        0     7525 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/http_api_adapter_mixin.py
+-rw-r--r--   0        0        0     2486 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/openai_sdk_chat_adapter.py
+-rw-r--r--   0        0        0      523 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/provider_adapter_mixin.py
+-rw-r--r--   0        0        0     5915 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/sdk_chat_adapter.py
+-rw-r--r--   0        0        0     6154 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/adapter_factory.py
+-rw-r--r--   0        0        0       59 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/concrete_adapters/__init__.py
+-rw-r--r--   0        0        0     3352 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/concrete_adapters/you_com_rag_chat_adapter.py
+-rw-r--r--   0        0        0     1017 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/__init__.py
+-rw-r--r--   0        0        0     9067 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4020 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2498 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2673 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     7317 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1672 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     3032 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1593 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1167 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4280 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2536 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2438 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0    11133 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/py.typed
+-rw-r--r--   0        0        0      558 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/rate_limiter.py
+-rw-r--r--   0        0        0      316 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/requirements.txt
+-rw-r--r--   0        0        0     7067 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/types.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/utils/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/utils/adapter_stream_response.py
+-rw-r--r--   0        0        0     1064 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/utils/general_utils.py
+-rw-r--r--   0        0        0     2492 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/utils/network_utils.py
+-rw-r--r--   0        0        0     8173 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/utils/openai_client_factory.py
+-rw-r--r--   0        0        0     1147 2024-05-14 22:42:02.499739 martian_adapters-5.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4854 1970-01-01 00:00:00.000000 martian_adapters-5.1.2/PKG-INFO
```

### Comparing `martian_adapters-5.1.1/LICENSE` & `martian_adapters-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/README.md` & `martian_adapters-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/__init__.py` & `martian_adapters-5.1.2/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/abstract_adapters/api_key_adapter_mixin.py` & `martian_adapters-5.1.2/adapters/abstract_adapters/api_key_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/abstract_adapters/base_adapter.py` & `martian_adapters-5.1.2/adapters/abstract_adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/abstract_adapters/chat_http_api_adapter.py` & `martian_adapters-5.1.2/adapters/abstract_adapters/chat_http_api_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/abstract_adapters/http_api_adapter_mixin.py` & `martian_adapters-5.1.2/adapters/abstract_adapters/http_api_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/abstract_adapters/openai_sdk_chat_adapter.py` & `martian_adapters-5.1.2/adapters/abstract_adapters/openai_sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/abstract_adapters/provider_adapter_mixin.py` & `martian_adapters-5.1.2/adapters/abstract_adapters/provider_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/abstract_adapters/sdk_chat_adapter.py` & `martian_adapters-5.1.2/adapters/abstract_adapters/sdk_chat_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         self,
         llm_input: Conversation,
         **kwargs,
     ):
         params = self.get_params(llm_input, **kwargs)
 
         response = await self.get_async_client()(
-            model=self.get_model().name,
+            model=self.get_model()._get_api_path(),
             **params,
         )
 
         if params.get("stream", False):
 
             async def stream_response():
                 async with stream_generator_auto_close(response):
@@ -158,15 +158,15 @@
         self,
         llm_input: Conversation,
         **kwargs,
     ):
         params = self.get_params(llm_input, **kwargs)
 
         response = self.get_sync_client()(
-            model=self.get_model().name,
+            model=self.get_model()._get_api_path(),
             **params,
         )
 
         if params.get("stream", False):
 
             def stream_response():
                 try:
```

### Comparing `martian_adapters-5.1.1/adapters/adapter_factory.py` & `martian_adapters-5.1.2/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/concrete_adapters/you_com_rag_chat_adapter.py` & `martian_adapters-5.1.2/adapters/concrete_adapters/you_com_rag_chat_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,14 @@
     def get_api_key_name() -> str:
         return YOU_COM_RAG_API_KEY_NAME
 
     @staticmethod
     def get_api_key_pattern() -> Pattern:
         return API_KEY_PATTERN
 
-    def get_model_name(self) -> str:
-        return MODEL_NAME
-
     def get_model(self) -> Model:
         return YOU_COM_MODEL
 
     def _get_headers(self) -> Dict[str, str]:
         """returns the headers that are sent on each api call to the vendor
 
         Returns:
```

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/__init__.py` & `martian_adapters-5.1.2/adapters/provider_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,19 +139,14 @@
         self._sync_client = Anthropic(
             api_key=self.get_api_key(),
         )
         self._async_client = AsyncAnthropic(
             api_key=self.get_api_key(),
         )
 
-    def get_model_name(self) -> str:
-        if self._current_model is None:
-            raise ValueError("Model not set")
-        return self._current_model.name
-
     def get_async_client(self):
         return self._async_client.messages.create
 
     def get_sync_client(self):
         return self._sync_client.messages.create
 
     def adjust_temperature(self, temperature: float) -> float:
```

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 API_KEY_PATTERN = re.compile(r".*")
 
 
 class AnyscaleModel(Model):
     supports_streaming: bool = True
     provider_name: str = PROVIDER_NAME
 
+    def _get_api_path(self) -> str:
+        return f"{self.vendor_name}/{self.name}"
+
 
 MODELS = [
     AnyscaleModel(
         name="gemma-7b-it",
         cost=Cost(prompt=0.15e-6, completion=0.15e-6),
         context_length=8192,
         vendor_name="google",
```

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 API_KEY_PATTERN = re.compile(r".*")
 
 
 class DeepInfraModel(Model):
     supports_streaming: bool = True
     provider_name: str = PROVIDER_NAME
 
+    def _get_api_path(self) -> str:
+        return f"{self.vendor_name}/{self.name}"
+
 
 MODELS = [
     DeepInfraModel(
         name="gemma-1.1-7b-it",
         cost=Cost(prompt=0.07e-6, completion=0.07e-6),
         context_length=8192,
         vendor_name="google",
```

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 API_KEY_PATTERN = re.compile(r".*")
 
 
 class FireworksModel(Model):
     supports_streaming: bool = True
     provider_name: str = PROVIDER_NAME
 
+    def _get_api_path(self) -> str:
+        return f"{self.vendor_name}/{self.name}"
+
 
 MODELS = [
     FireworksModel(
         name="gemma-7b-it",
         cost=Cost(prompt=0.20e-6, completion=0.20e-6),
         context_length=8192,
         vendor_name="accounts/fireworks/models",
```

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,12 +60,7 @@
     @staticmethod
     def get_api_key_name() -> str:
         return API_KEY_NAME
 
     @staticmethod
     def get_api_key_pattern() -> Pattern:
         return API_KEY_PATTERN
-
-    def get_model_name(self) -> str:
-        if self._current_model is None:
-            raise ValueError("Model not set")
-        return self._current_model.name
```

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -86,19 +86,14 @@
 
     def _set_current_model(self, model: Model) -> None:
         super()._set_current_model(model)
 
         self._sync_client.base_url = URL(self._current_model.base_url)
         self._async_client.base_url = URL(self._current_model.base_url)
 
-    def get_model_name(self) -> str:
-        if self._current_model is None:
-            raise ValueError("Model not set")
-        return self._current_model.name
-
     def extract_stream_response(self, request, response: ChatCompletionChunk) -> str:
         # It must be the last response from Lepton that is empty.
         if not response.choices:
             response.choices = [
                 Choice(
                     delta=ChoiceDelta(),
                     finish_reason="stop",
```

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,12 +55,7 @@
     @staticmethod
     def get_api_key_name() -> str:
         return API_KEY_NAME
 
     @staticmethod
     def get_api_key_pattern() -> Pattern:
         return API_KEY_PATTERN
-
-    def get_model_name(self) -> str:
-        if self._current_model is None:
-            raise ValueError("Model not set")
-        return self._current_model.name
```

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,12 +42,7 @@
     @staticmethod
     def get_api_key_name() -> str:
         return API_KEY_NAME
 
     @staticmethod
     def get_api_key_pattern() -> Pattern:
         return API_KEY_PATTERN
-
-    def get_model_name(self) -> str:
-        if self._current_model is None:
-            raise ValueError("Model not set")
-        return self._current_model.name
```

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,12 +146,7 @@
     @staticmethod
     def get_api_key_name() -> str:
         return API_KEY_NAME
 
     @staticmethod
     def get_api_key_pattern() -> Pattern:
         return API_KEY_PATTERN
-
-    def get_model_name(self) -> str:
-        if self._current_model is None:
-            raise ValueError("Model not set")
-        return self._current_model.name
```

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 API_KEY_PATTERN = re.compile(r".*")
 
 
 class OpenRouterModel(Model):
     supports_streaming: bool = True
     provider_name: str = PROVIDER_NAME
 
+    def _get_api_path(self) -> str:
+        return f"{self.vendor_name}/{self.name}"
+
 
 MODELS = [
     OpenRouterModel(
         name="dbrx-instruct",
         cost=Cost(prompt=0.60e-6, completion=0.60e-6),
         context_length=32_768,
         vendor_name="databricks",
```

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -82,12 +82,7 @@
     @staticmethod
     def get_api_key_name() -> str:
         return API_KEY_NAME
 
     @staticmethod
     def get_api_key_pattern() -> Pattern:
         return API_KEY_PATTERN
-
-    def get_model_name(self) -> str:
-        if self._current_model is None:
-            raise ValueError("Model not set")
-        return self._current_model.name
```

### Comparing `martian_adapters-5.1.1/adapters/provider_adapters/together_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.2/adapters/provider_adapters/together_sdk_chat_provider_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
 
 class TogetherModel(Model):
     supports_streaming: bool = True
     supports_json_content: bool = True
     provider_name: str = PROVIDER_NAME
 
+    def _get_api_path(self) -> str:
+        return f"{self.vendor_name}/{self.name}"
+
 
 MODELS = [
     TogetherModel(
         name="Yi-34B-Chat",
         cost=Cost(prompt=0.8e-6, completion=0.8e-6),
         context_length=4096,
         vendor_name="zero-one-ai",
```

### Comparing `martian_adapters-5.1.1/adapters/rate_limiter.py` & `martian_adapters-5.1.2/adapters/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/types.py` & `martian_adapters-5.1.2/adapters/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,17 @@
     supports_json_output: bool = False
     supports_json_content: bool = False
     completion_length: Optional[int] = None
 
     def get_path(self) -> str:
         return f"{self.provider_name}/{self.vendor_name}/{self.name}"
 
+    def _get_api_path(self) -> str:
+        return self.name
+
 
 class Conversation(BaseModel):
     turns: List[
         Union[Turn, FunctionOutputTurn, ToolOutputTurn, ToolsCallTurn, ContentTurn]
     ]
 
     def __init__(
```

### Comparing `martian_adapters-5.1.1/adapters/utils/general_utils.py` & `martian_adapters-5.1.2/adapters/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/utils/network_utils.py` & `martian_adapters-5.1.2/adapters/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/adapters/utils/openai_client_factory.py` & `martian_adapters-5.1.2/adapters/utils/openai_client_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.1/pyproject.toml` & `martian_adapters-5.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "martian-adapters"
-version = "5.1.1"
+version = "5.1.2"
 description = "Adapters as API gateways to Different LLM Models"
 authors = ["Martian team <team@withmartian.com>"]
 readme = "README.md"
 packages = [{include = "adapters", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `martian_adapters-5.1.1/PKG-INFO` & `martian_adapters-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martian-adapters
-Version: 5.1.1
+Version: 5.1.2
 Summary: Adapters as API gateways to Different LLM Models
 Author: Martian team
 Author-email: team@withmartian.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
```

