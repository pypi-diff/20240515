# Comparing `tmp/martian_adapters-5.1.2.tar.gz` & `tmp/martian_adapters-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martian_adapters-5.1.2.tar", max compression
+gzip compressed data, was "martian_adapters-5.1.3.tar", max compression
```

## Comparing `martian_adapters-5.1.2.tar` & `martian_adapters-5.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    35149 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/LICENSE
--rw-r--r--   0        0        0     3553 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/README.md
--rw-r--r--   0        0        0      725 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/__init__.py
--rw-r--r--   0        0        0      305 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/__init__.py
--rw-r--r--   0        0        0     2188 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/api_key_adapter_mixin.py
--rw-r--r--   0        0        0     2125 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/base_adapter.py
--rw-r--r--   0        0        0     1226 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/chat_http_api_adapter.py
--rw-r--r--   0        0        0     7525 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/http_api_adapter_mixin.py
--rw-r--r--   0        0        0     2486 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/openai_sdk_chat_adapter.py
--rw-r--r--   0        0        0      523 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/provider_adapter_mixin.py
--rw-r--r--   0        0        0     5915 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/abstract_adapters/sdk_chat_adapter.py
--rw-r--r--   0        0        0     6154 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/adapter_factory.py
--rw-r--r--   0        0        0       59 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/concrete_adapters/__init__.py
--rw-r--r--   0        0        0     3352 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/concrete_adapters/you_com_rag_chat_adapter.py
--rw-r--r--   0        0        0     1017 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/__init__.py
--rw-r--r--   0        0        0     9067 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4020 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2498 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2673 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     7317 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1672 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     3032 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1593 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1167 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4280 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2536 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2438 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0    11133 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0        0 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/py.typed
--rw-r--r--   0        0        0      558 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/rate_limiter.py
--rw-r--r--   0        0        0      316 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/requirements.txt
--rw-r--r--   0        0        0     7067 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/types.py
--rw-r--r--   0        0        0        0 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/utils/__init__.py
--rw-r--r--   0        0        0      263 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/utils/adapter_stream_response.py
--rw-r--r--   0        0        0     1064 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/utils/general_utils.py
--rw-r--r--   0        0        0     2492 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/utils/network_utils.py
--rw-r--r--   0        0        0     8173 2024-05-14 22:42:02.495739 martian_adapters-5.1.2/adapters/utils/openai_client_factory.py
--rw-r--r--   0        0        0     1147 2024-05-14 22:42:02.499739 martian_adapters-5.1.2/pyproject.toml
--rw-r--r--   0        0        0     4854 1970-01-01 00:00:00.000000 martian_adapters-5.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/LICENSE
+-rw-r--r--   0        0        0     3553 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/README.md
+-rw-r--r--   0        0        0      725 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/abstract_adapters/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/abstract_adapters/api_key_adapter_mixin.py
+-rw-r--r--   0        0        0     2125 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/abstract_adapters/base_adapter.py
+-rw-r--r--   0        0        0     1226 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/abstract_adapters/chat_http_api_adapter.py
+-rw-r--r--   0        0        0     7525 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/abstract_adapters/http_api_adapter_mixin.py
+-rw-r--r--   0        0        0     2486 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/abstract_adapters/openai_sdk_chat_adapter.py
+-rw-r--r--   0        0        0      523 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/abstract_adapters/provider_adapter_mixin.py
+-rw-r--r--   0        0        0     5915 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/abstract_adapters/sdk_chat_adapter.py
+-rw-r--r--   0        0        0     6154 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/adapter_factory.py
+-rw-r--r--   0        0        0       59 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/concrete_adapters/__init__.py
+-rw-r--r--   0        0        0     3352 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/concrete_adapters/you_com_rag_chat_adapter.py
+-rw-r--r--   0        0        0     1017 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/provider_adapters/__init__.py
+-rw-r--r--   0        0        0     9067 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4020 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2498 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     3116 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     7317 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1672 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     3032 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1593 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1167 2024-05-15 00:11:53.097123 martian_adapters-5.1.3/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4280 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2536 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2438 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0    11133 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/py.typed
+-rw-r--r--   0        0        0      558 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/rate_limiter.py
+-rw-r--r--   0        0        0      316 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/requirements.txt
+-rw-r--r--   0        0        0     7067 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/types.py
+-rw-r--r--   0        0        0        0 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/utils/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/utils/adapter_stream_response.py
+-rw-r--r--   0        0        0     1064 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/utils/general_utils.py
+-rw-r--r--   0        0        0     2492 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/utils/network_utils.py
+-rw-r--r--   0        0        0     8173 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/adapters/utils/openai_client_factory.py
+-rw-r--r--   0        0        0     1147 2024-05-15 00:11:53.101123 martian_adapters-5.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4854 1970-01-01 00:00:00.000000 martian_adapters-5.1.3/PKG-INFO
```

### Comparing `martian_adapters-5.1.2/LICENSE` & `martian_adapters-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/README.md` & `martian_adapters-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/__init__.py` & `martian_adapters-5.1.3/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/abstract_adapters/api_key_adapter_mixin.py` & `martian_adapters-5.1.3/adapters/abstract_adapters/api_key_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/abstract_adapters/base_adapter.py` & `martian_adapters-5.1.3/adapters/abstract_adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/abstract_adapters/chat_http_api_adapter.py` & `martian_adapters-5.1.3/adapters/abstract_adapters/chat_http_api_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/abstract_adapters/http_api_adapter_mixin.py` & `martian_adapters-5.1.3/adapters/abstract_adapters/http_api_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/abstract_adapters/openai_sdk_chat_adapter.py` & `martian_adapters-5.1.3/adapters/abstract_adapters/openai_sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/abstract_adapters/provider_adapter_mixin.py` & `martian_adapters-5.1.3/adapters/abstract_adapters/provider_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/abstract_adapters/sdk_chat_adapter.py` & `martian_adapters-5.1.3/adapters/abstract_adapters/sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/adapter_factory.py` & `martian_adapters-5.1.3/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/concrete_adapters/you_com_rag_chat_adapter.py` & `martian_adapters-5.1.3/adapters/concrete_adapters/you_com_rag_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/__init__.py` & `martian_adapters-5.1.3/adapters/provider_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 from typing import Pattern
 
+from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
+
 from adapters.abstract_adapters.openai_sdk_chat_adapter import OpenAISDKChatAdapter
 from adapters.abstract_adapters.provider_adapter_mixin import ProviderAdapterMixin
 from adapters.types import Cost, Model
 
 PROVIDER_NAME = "fireworks"
 BASE_URL = "https://api.fireworks.ai/inference/v1"
 API_KEY_NAME = "FIREWORKS_API_KEY"
@@ -87,7 +89,15 @@
     @staticmethod
     def get_api_key_name() -> str:
         return API_KEY_NAME
 
     @staticmethod
     def get_api_key_pattern() -> Pattern:
         return API_KEY_PATTERN
+
+    def extract_stream_response(self, request, response: ChatCompletionChunk) -> str:
+        if response.choices and response.choices[0].delta.content is None:
+            # It must be the first response.
+            # Most models start with an empty string.
+            response.choices[0].delta.content = ""
+
+        return f"data: {response.model_dump_json()}\n\n"
```

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/provider_adapters/together_sdk_chat_provider_adapter.py` & `martian_adapters-5.1.3/adapters/provider_adapters/together_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/rate_limiter.py` & `martian_adapters-5.1.3/adapters/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/types.py` & `martian_adapters-5.1.3/adapters/types.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/utils/general_utils.py` & `martian_adapters-5.1.3/adapters/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/utils/network_utils.py` & `martian_adapters-5.1.3/adapters/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/adapters/utils/openai_client_factory.py` & `martian_adapters-5.1.3/adapters/utils/openai_client_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.1.2/pyproject.toml` & `martian_adapters-5.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "martian-adapters"
-version = "5.1.2"
+version = "5.1.3"
 description = "Adapters as API gateways to Different LLM Models"
 authors = ["Martian team <team@withmartian.com>"]
 readme = "README.md"
 packages = [{include = "adapters", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `martian_adapters-5.1.2/PKG-INFO` & `martian_adapters-5.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martian-adapters
-Version: 5.1.2
+Version: 5.1.3
 Summary: Adapters as API gateways to Different LLM Models
 Author: Martian team
 Author-email: team@withmartian.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
```

