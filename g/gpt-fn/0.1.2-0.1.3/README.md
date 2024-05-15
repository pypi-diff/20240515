# Comparing `tmp/gpt_fn-0.1.2.tar.gz` & `tmp/gpt_fn-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_fn-0.1.2.tar", max compression
+gzip compressed data, was "gpt_fn-0.1.3.tar", max compression
```

## Comparing `gpt_fn-0.1.2.tar` & `gpt_fn-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,62 @@
--rw-r--r--   0        0        0     1066 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/LICENSE
--rw-r--r--   0        0        0     4102 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/README.md
--rw-r--r--   0        0        0      919 2024-01-03 07:50:57.344785 gpt_fn-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/__init__.py
--rw-r--r--   0        0        0     1204 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/ai_function.py
--rw-r--r--   0        0        0    11156 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/completion.py
--rw-r--r--   0        0        0      537 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/conftest.py
--rw-r--r--   0        0        0      508 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/exceptions.py
--rw-r--r--   0        0        0      883 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/prompt.py
--rw-r--r--   0        0        0        0 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/py.typed
--rw-r--r--   0        0        0        0 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/__init__.py
--rw-r--r--   0        0        0    60847 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
--rw-r--r--   0        0        0     9435 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/__snapshots__/test_completion.ambr
--rw-r--r--   0        0        0      713 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
--rw-r--r--   0        0        0    35500 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_ai_fn_max_token.yaml
--rw-r--r--   0        0        0     7529 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fabnocci.yaml
--rw-r--r--   0        0        0     8726 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fake_hero.yaml
--rw-r--r--   0        0        0    71613 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fn_max_token.yaml
--rw-r--r--   0        0        0     9556 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion.yaml
--rw-r--r--   0        0        0    18935 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion.yaml
--rw-r--r--   0        0        0     8156 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion.yaml
--rw-r--r--   0        0        0     9533 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion.yaml
--rw-r--r--   0        0        0     5937 2024-01-03 07:50:38.896829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete.yaml
--rw-r--r--   0        0        0     7889 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_function_completion.yaml
--rw-r--r--   0        0        0     3786 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens.yaml
--rw-r--r--   0        0        0     3842 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function.yaml
--rw-r--r--   0        0        0     8607 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion.yaml
--rw-r--r--   0        0        0     7258 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens.yaml
--rw-r--r--   0        0        0     1499 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/tests/test_ai_function.py
--rw-r--r--   0        0        0     5923 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/tests/test_completion.py
--rw-r--r--   0        0        0     1557 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/tests/test_prompt.py
--rw-r--r--   0        0        0        0 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/utils/__init__.py
--rw-r--r--   0        0        0     1951 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/utils/pydantic_parser.py
--rw-r--r--   0        0        0     3827 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/utils/signature.py
--rw-r--r--   0        0        0        0 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/utils/tests/__init__.py
--rw-r--r--   0        0        0     7891 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/utils/tests/__snapshots__/test_json_decode.ambr
--rw-r--r--   0        0        0     5913 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
--rw-r--r--   0        0        0    15635 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
--rw-r--r--   0        0        0    15595 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/utils/tests/cassettes/test_pydantic_parser/test_pydantic_parser_with_prompt[email.txt-Email].yaml
--rw-r--r--   0        0        0     2186 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt
--rw-r--r--   0        0        0     3011 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/utils/tests/test_pydantic_parser.py
--rw-r--r--   0        0        0     2890 2024-01-03 07:50:38.900829 gpt_fn-0.1.2/src/gpt_fn/utils/tests/test_signature.py
--rw-r--r--   0        0        0     4625 1970-01-01 00:00:00.000000 gpt_fn-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4102 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/README.md
+-rw-r--r--   0        0        0      919 2024-05-14 13:10:22.022763 gpt_fn-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/src/gpt_fn/__init__.py
+-rw-r--r--   0        0        0     1204 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/src/gpt_fn/ai_function.py
+-rw-r--r--   0        0        0    14148 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/src/gpt_fn/completion.py
+-rw-r--r--   0        0        0      537 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/src/gpt_fn/conftest.py
+-rw-r--r--   0        0        0      508 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/src/gpt_fn/exceptions.py
+-rw-r--r--   0        0        0      883 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/src/gpt_fn/prompt.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/src/gpt_fn/py.typed
+-rw-r--r--   0        0        0        0 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/src/gpt_fn/tests/__init__.py
+-rw-r--r--   0        0        0    60815 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
+-rw-r--r--   0        0        0    32594 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/src/gpt_fn/tests/__snapshots__/test_completion.ambr
+-rw-r--r--   0        0        0      713 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
+-rw-r--r--   0        0        0    13985 2024-05-14 13:10:03.446678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fabnocci.yaml
+-rw-r--r--   0        0        0    16272 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fake_hero.yaml
+-rw-r--r--   0        0        0   142193 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fn_max_token.yaml
+-rw-r--r--   0        0        0     2930 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     2866 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3144 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[OpenAI API].yaml
+-rw-r--r--   0        0        0     3156 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3254 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3846 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[OpenAI API].yaml
+-rw-r--r--   0        0        0     3675 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3687 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     4685 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[OpenAI API].yaml
+-rw-r--r--   0        0        0     2921 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     2849 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3125 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[OpenAI API].yaml
+-rw-r--r--   0        0        0     2812 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     2812 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3021 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[OpenAI API].yaml
+-rw-r--r--   0        0        0     3145 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3243 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3835 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[OpenAI API].yaml
+-rw-r--r--   0        0        0     3261 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3289 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3496 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[OpenAI API].yaml
+-rw-r--r--   0        0        0     3352 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3450 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3530 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[OpenAI API].yaml
+-rw-r--r--   0        0        0     3628 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3676 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     4252 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[OpenAI API].yaml
+-rw-r--r--   0        0        0     3181 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3312 2024-05-14 13:10:03.450678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3894 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[OpenAI API].yaml
+-rw-r--r--   0        0        0     1499 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/tests/test_ai_function.py
+-rw-r--r--   0        0        0    14371 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/tests/test_completion.py
+-rw-r--r--   0        0        0     1557 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/utils/__init__.py
+-rw-r--r--   0        0        0     1951 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/utils/pydantic_parser.py
+-rw-r--r--   0        0        0     3827 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/utils/signature.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/utils/tests/__init__.py
+-rw-r--r--   0        0        0     7891 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/utils/tests/__snapshots__/test_json_decode.ambr
+-rw-r--r--   0        0        0     6264 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
+-rw-r--r--   0        0        0    15635 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
+-rw-r--r--   0        0        0     8147 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/utils/tests/cassettes/test_pydantic_parser/test_pydantic_parser_with_prompt[email.txt-Email].yaml
+-rw-r--r--   0        0        0     2186 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt
+-rw-r--r--   0        0        0     3011 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/utils/tests/test_pydantic_parser.py
+-rw-r--r--   0        0        0     2890 2024-05-14 13:10:03.454678 gpt_fn-0.1.3/src/gpt_fn/utils/tests/test_signature.py
+-rw-r--r--   0        0        0     4625 1970-01-01 00:00:00.000000 gpt_fn-0.1.3/PKG-INFO
```

### Comparing `gpt_fn-0.1.2/LICENSE` & `gpt_fn-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/README.md` & `gpt_fn-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/pyproject.toml` & `gpt_fn-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-fn"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gpt_fn", from = "src" }]
 include = ["fn/py.typed"]
 
 [tool.poetry.dependencies]
```

### Comparing `gpt_fn-0.1.2/src/gpt_fn/ai_function.py` & `gpt_fn-0.1.3/src/gpt_fn/ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/src/gpt_fn/completion.py` & `gpt_fn-0.1.3/src/gpt_fn/completion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from datetime import datetime
 from typing import Any, Callable, Type, TypedDict, TypeVar
 
 import fuzzy_json
 import openai
 import pydantic
 from openai import AsyncAzureOpenAI, AsyncOpenAI, AzureOpenAI, OpenAI
 
@@ -20,60 +21,79 @@
 class FunctionMessage(Message):
     name: str
 
 
 class APISettings(pydantic.BaseModel):
     api_key: str = pydantic.Field(default_factory=lambda: openai.api_key)
     api_base: str = pydantic.Field(default_factory=lambda: openai.azure_endpoint)
-    api_type: str = pydantic.Field(default_factory=lambda: openai.api_type)
-    api_version: str | None = pydantic.Field(default_factory=lambda: openai.api_version)
+    api_version: str = pydantic.Field(default_factory=lambda: openai.api_version)
 
-
-def get_api_type() -> str:
-    if os.environ.get("OPENAI_API_KEY"):
-        return "open_ai"
-    elif os.environ.get("AZURE_API_KEY"):
-        return "azure"
-    else:
-        raise ValueError("No api key found in environment variables")
+    @staticmethod
+    def infer_api_type() -> str:
+        """
+        Infers the API type based on environment variables and sets the api_type attribute accordingly.
+
+        Raises:
+            ValueError: If the API type cannot be determined.
+        """
+        if os.environ.get("OPENAI_API_KEY"):
+            return "open_ai"
+        elif os.environ.get("AZURE_OPENAI_API_KEY"):
+            return "azure"
+        else:
+            raise ValueError("API type could not be inferred from environment variables.")
+
+    api_type: str = pydantic.Field(default_factory=infer_api_type)
+
+    def check_functions_required(self) -> bool:
+        if self.api_version is None:
+            assert self.api_type != "azure", "api_version is required for azure"
+            return False
+        if self.api_type == "azure" and datetime.strptime(str(self.api_version)[:10], "%Y-%m-%d") >= datetime(2023, 12, 1):
+            return False
+        return True
 
 
 def get_sync_client(model: str, api_settings: APISettings = APISettings()) -> OpenAI:
-    if api_settings.api_type is None:
-        api_settings.api_type = get_api_type()
-
     if api_settings.api_type == "open_ai":
         return OpenAI(api_key=api_settings.api_key)
     elif api_settings.api_type == "azure":
         return AzureOpenAI(
             azure_endpoint=api_settings.api_base,
             api_key=api_settings.api_key,
             api_version=api_settings.api_version,
             azure_deployment=model,
         )
 
     raise ValueError(f"Unknown api_type {api_settings.api_type}")
 
 
 def get_async_client(model: str, api_settings: APISettings = APISettings()) -> AsyncOpenAI:
-    if api_settings.api_type is None:
-        api_settings.api_type = get_api_type()
-
     if api_settings.api_type == "open_ai":
         return AsyncOpenAI(api_key=api_settings.api_key)
     elif api_settings.api_type == "azure":
         return AsyncAzureOpenAI(
             azure_endpoint=api_settings.api_base,
             api_key=api_settings.api_key,
             api_version=api_settings.api_version,
             azure_deployment=model,
         )
     raise ValueError(f"Unknown api_type {api_settings.api_type}")
 
 
+"""
+The currently applied Azure OpenAI API version is 2023-07-01-preview,
+which is about to expire on July, 1,
+and the parameters `functions` and `function_call` have been deprecated for the OpenAI API
+and since the 2023-12-01-preview version for the Azure OpenAI API version.
+Therefore, the Azure OpenAI API version should be upgraded to either 2023-10-01-preview or versions later than and excluding 2023-12-01-preview.
+The parameters should also be updated to `tools` and `tool_choice` for OpenAI API and Azure OpenAI API with version starting from 2023-12-01-preview.
+"""
+
+
 def function_completion(
     messages: list[Message],
     max_tokens: int | None = None,
     model: str = "gpt-3.5-turbo-0613",
     temperature: float = 1.0,
     top_p: float = 1.0,
     frequency_penalty: float = 0.0,
@@ -91,32 +111,41 @@
         model=model,
         temperature=temperature,
         top_p=top_p,
         frequency_penalty=frequency_penalty,
         presence_penalty=presence_penalty,
         user=user,
         stop=stop or None,
-        functions=[signature.FunctionSignature(f).schema() for f in functions],
-        function_call=function_call,
     )
-
     client: OpenAI = get_sync_client(model, api_settings)
 
+    functions_are_required = api_settings.check_functions_required()
+
+    kwargs_ = dict(tools=[{"type": "function", "function": signature.FunctionSignature(f).schema()} for f in functions], tool_choice={"type": "function", "function": function_call} if type(function_call) != str else function_call)
+
+    if functions_are_required:
+        kwargs_ = dict(functions=[signature.FunctionSignature(f).schema() for f in functions], function_call=function_call)
+
+    kwargs.update(kwargs_)
+
     if max_tokens is not None:
         kwargs.update(max_tokens=max_tokens)
 
     response = client.chat.completions.create(**kwargs)
 
     output = response.choices[0]
     message = output.message
     finish_reason = output.finish_reason
 
-    if message.function_call is not None and finish_reason in ["stop", "function_call"]:
+    if functions_are_required and message.function_call is not None and finish_reason in ["stop", "function_call"]:
         return message.function_call
 
+    elif message.tool_calls is not None and finish_reason in ["stop", "tool_calls"]:
+        return message.tool_calls[0].function
+
     raise CompletionIncompleteError(
         f"Incomplete response. Max tokens: {max_tokens}, Finish reason: {finish_reason} Message:{message.content}",
         response=response,
         request=kwargs,
     )
 
 
@@ -141,31 +170,40 @@
         model=model,
         temperature=temperature,
         top_p=top_p,
         frequency_penalty=frequency_penalty,
         presence_penalty=presence_penalty,
         user=user,
         stop=stop or None,
-        functions=[signature.FunctionSignature(f).schema() for f in functions],
-        function_call=function_call,
     )
-
     client: AsyncOpenAI = get_async_client(model, api_settings)
 
+    functions_are_required = api_settings.check_functions_required()
+
+    kwargs_ = dict(tools=[{"type": "function", "function": signature.FunctionSignature(f).schema()} for f in functions], tool_choice={"type": "function", "function": function_call} if type(function_call) != str else function_call)
+
+    if functions_are_required:
+        kwargs_ = dict(functions=[signature.FunctionSignature(f).schema() for f in functions], function_call=function_call)
+
+    kwargs.update(kwargs_)
+
     if max_tokens is not None:
         kwargs.update(max_tokens=max_tokens)
 
     response = await client.chat.completions.create(**kwargs)
     output = response.choices[0]
     message = output.message
     finish_reason = output.finish_reason
 
-    if message.function_call is not None and finish_reason in ["stop", "function_call"]:
+    if functions_are_required and message.function_call is not None and finish_reason in ["stop", "function_call"]:
         return message.function_call
 
+    elif message.tool_calls is not None and finish_reason in ["stop", "tool_calls"]:
+        return message.tool_calls[0].function
+
     raise CompletionIncompleteError(
         f"Incomplete response. Max tokens: {max_tokens}, Finish reason: {finish_reason} Message:{message.content}",
         response=response,
         request=kwargs,
     )
 
 
@@ -178,48 +216,62 @@
     top_p: float = 1.0,
     frequency_penalty: float = 0.0,
     presence_penalty: float = 0.0,
     user: str = "",
     auto_repair: bool = True,
     api_settings: APISettings = APISettings(),
 ) -> T:
-    function_call = {"name": "structural_response"}
+
     kwargs: dict[str, Any] = dict(
         messages=messages,
         model=model,
         temperature=temperature,
         top_p=top_p,
         frequency_penalty=frequency_penalty,
         presence_penalty=presence_penalty,
         user=user,
-        functions=[
-            function_call
-            | {
-                "description": "Response to user in a structural way.",
-                "parameters": structure.schema(),
-            }
-        ],
-        function_call=function_call,
     )
-
     client: OpenAI = get_sync_client(model, api_settings)
 
+    functions_are_required = api_settings.check_functions_required()
+
+    function_call = {"name": "structural_response"}
+    function = function_call | {
+        "description": "Response to user in a structural way.",
+        "parameters": structure.schema(),
+    }
+
+    kwargs_ = dict(
+        tools=[{"type": "function", "function": function}],
+        tool_choice={"type": "function", "function": function_call},
+    )
+
+    if functions_are_required:
+        kwargs_ = dict(
+            functions=[function],
+            function_call=function_call,
+        )
+    kwargs.update(kwargs_)
+
     if max_tokens is not None:
         kwargs.update(max_tokens=max_tokens)
 
     response = client.chat.completions.create(**kwargs)
 
     output = response.choices[0]
     message = output.message
     finish_reason = output.finish_reason
 
-    if message.function_call is not None and finish_reason == "stop":
-        args = message.function_call.arguments
-        parsed_json = fuzzy_json.loads(args, auto_repair)
+    if finish_reason == "stop":
+        if functions_are_required and message.function_call is not None:
+            args = message.function_call.arguments
+        elif message.tool_calls is not None:
+            args = message.tool_calls[0].function.arguments
 
+        parsed_json = fuzzy_json.loads(args, auto_repair)
         return pydantic.parse_obj_as(structure, parsed_json)
 
     raise CompletionIncompleteError(
         f"Incomplete response. Max tokens: {max_tokens}, Finish reason: {finish_reason} Message:{message.content}",
         response=response,
         request=kwargs,
     )
@@ -234,48 +286,62 @@
     top_p: float = 1.0,
     frequency_penalty: float = 0.0,
     presence_penalty: float = 0.0,
     user: str = "",
     auto_repair: bool = True,
     api_settings: APISettings = APISettings(),
 ) -> T:
-    function_call = {"name": "structural_response"}
+
     kwargs: dict[str, Any] = dict(
         messages=messages,
         model=model,
         temperature=temperature,
         top_p=top_p,
         frequency_penalty=frequency_penalty,
         presence_penalty=presence_penalty,
         user=user,
-        functions=[
-            function_call
-            | {
-                "description": "Response to user in a structural way.",
-                "parameters": structure.schema(),
-            }
-        ],
-        function_call=function_call,
     )
-
     client: AsyncOpenAI = get_async_client(model, api_settings)
 
+    functions_are_required = api_settings.check_functions_required()
+
+    function_call = {"name": "structural_response"}
+    function = function_call | {
+        "description": "Response to user in a structural way.",
+        "parameters": structure.schema(),
+    }
+
+    kwargs_ = dict(
+        tools=[{"type": "function", "function": function}],
+        tool_choice={"type": "function", "function": function_call},
+    )
+
+    if functions_are_required:
+        kwargs_ = dict(
+            functions=[function],
+            function_call=function_call,
+        )
+    kwargs.update(kwargs_)
+
     if max_tokens is not None:
         kwargs.update(max_tokens=max_tokens)
 
     response = await client.chat.completions.create(**kwargs)
 
     output = response.choices[0]
     message = output.message
     finish_reason = output.finish_reason
 
-    if message.function_call is not None and finish_reason == "stop":
-        args = message.function_call.arguments
-        parsed_json = fuzzy_json.loads(args, auto_repair)
+    if finish_reason == "stop":
+        if functions_are_required and message.function_call is not None:
+            args = message.function_call.arguments
+        elif message.tool_calls is not None:
+            args = message.tool_calls[0].function.arguments
 
+        parsed_json = fuzzy_json.loads(args, auto_repair)
         return pydantic.parse_obj_as(structure, parsed_json)
 
     raise CompletionIncompleteError(
         f"Incomplete response. Max tokens: {max_tokens}, Finish reason: {finish_reason} Message:{message.content}",
         response=response,
         request=kwargs,
     )
@@ -289,14 +355,15 @@
     top_p: float = 1.0,
     frequency_penalty: float = 0.0,
     presence_penalty: float = 0.0,
     stop: list[str] = [],
     user: str = "",
     api_settings: APISettings = APISettings(),
 ) -> str:
+
     kwargs: dict[str, Any] = dict(
         messages=messages,
         model=model,
         temperature=temperature,
         top_p=top_p,
         frequency_penalty=frequency_penalty,
         presence_penalty=presence_penalty,
@@ -332,14 +399,15 @@
     top_p: float = 1.0,
     frequency_penalty: float = 0.0,
     presence_penalty: float = 0.0,
     stop: list[str] = [],
     user: str = "",
     api_settings: APISettings = APISettings(),
 ) -> str:
+
     kwargs: dict[str, Any] = dict(
         messages=messages,
         model=model,
         temperature=temperature,
         top_p=top_p,
         frequency_penalty=frequency_penalty,
         presence_penalty=presence_penalty,
```

### Comparing `gpt_fn-0.1.2/src/gpt_fn/prompt.py` & `gpt_fn-0.1.3/src/gpt_fn/prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr` & `gpt_fn-0.1.3/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # serializer version: 1
 # name: test_ai_fabnocci
   55
 # ---
 # name: test_ai_fake_hero
   list([
-    Hero(name='Hero 1', age=25),
-    Hero(name='Hero 2', age=30),
-    Hero(name='Hero 3', age=35),
-    Hero(name='Hero 4', age=40),
-    Hero(name='Hero 5', age=45),
+    Hero(name='Fake Hero 1', age=25),
+    Hero(name='Fake Hero 2', age=30),
+    Hero(name='Fake Hero 3', age=28),
+    Hero(name='Fake Hero 4', age=27),
+    Hero(name='Fake Hero 5', age=29),
   ])
 # ---
 # name: test_ai_fn_max_token[context]
-  BadRequestError('Error code: 400 - {\'error\': {\'message\': "This model\'s maximum context length is 4097 tokens. However, your messages resulted in 5210 tokens. Please reduce the length of the messages.", \'type\': \'invalid_request_error\', \'param\': \'messages\', \'code\': \'context_length_exceeded\'}}')
+  BadRequestError('Error code: 400 - {\'error\': {\'message\': "Sorry! We\'ve encountered an issue with repetitive patterns in your prompt. Please try again with a different prompt.", \'type\': \'invalid_prompt\', \'param\': \'prompt\', \'code\': None}}')
 # ---
 # name: test_ai_fn_max_token[exconly]
   "gpt_fn.exceptions.AiFnError: generate_hashtags('hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello hello')"
 # ---
 # name: test_ai_fn_max_token[vars(exc)]
   dict({
     'fn_locals': dict({
```

### Comparing `gpt_fn-0.1.2/src/gpt_fn/tests/__snapshots__/test_prompt.ambr` & `gpt_fn-0.1.3/src/gpt_fn/tests/__snapshots__/test_prompt.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fn_max_token.yaml` & `gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fn_max_token.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -391,86 +391,1025 @@
       hello hello hello hello hello hello hello hello hello hello hello hello hello
       hello hello hello hello hello hello hello hello hello hello hello hello hello
       hello hello hello hello hello hello hello hello hello hello hello hello hello
       hello hello hello hello hello hello hello hello hello hello hello hello hello
       hello hello hello hello hello hello hello hello hello hello hello hello hello
       hello hello hello hello hello hello hello hello hello hello hello hello hello
       hello hello hello hello hello hello hello hello hello hello hello hello hello
-      hello hello hello hello hello hello hello hello'')"}], "model": "gpt-3.5-turbo",
-      "temperature": 0.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
-      0.0, "user": "", "stop": null}'
+      hello hello hello hello hello hello hello hello'')"}], "model": "gpt35", "frequency_penalty":
+      0.0, "presence_penalty": 0.0, "stop": null, "temperature": 0.0, "top_p": 1.0,
+      "user": ""}'
     headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
+      accept:
+      - application/json
+      accept-encoding:
       - gzip, deflate
-      Connection:
+      connection:
       - keep-alive
+      content-length:
+      - '31051'
+      content-type:
+      - application/json
+      host:
+      - gstudio.openai.azure.com
+      user-agent:
+      - AzureOpenAI/Python 1.9.0
+      x-stainless-arch:
+      - x64
+      x-stainless-async:
+      - 'false'
+      x-stainless-lang:
+      - python
+      x-stainless-os:
+      - Linux
+      x-stainless-package-version:
+      - 1.9.0
+      x-stainless-runtime:
+      - CPython
+      x-stainless-runtime-version:
+      - 3.10.14
+    method: POST
+    uri: https://gstudio.openai.azure.com/openai/deployments/gpt35/chat/completions?api-version=2023-07-01-preview
+  response:
+    content: "{\n  \"error\": {\n    \"message\": \"Sorry! We've encountered an issue
+      with repetitive patterns in your prompt. Please try again with a different prompt.\",\n
+      \   \"type\": \"invalid_request_error\",\n    \"param\": \"prompt\",\n    \"code\":
+      \"invalid_prompt\"\n  }\n}\n"
+    headers:
       Content-Length:
-      - '31059'
+      - '245'
+      Content-Type:
+      - application/json
+      Date:
+      - Thu, 09 May 2024 10:07:18 GMT
+      Strict-Transport-Security:
+      - max-age=31536000; includeSubDomains; preload
+      access-control-allow-origin:
+      - '*'
+      apim-request-id:
+      - 1249216d-0e54-4d4c-9942-67b9c59e8f3c
+      azureml-model-session:
+      - turbo-0613-07015ca4
+      ms-azureml-model-error-reason:
+      - model_error
+      ms-azureml-model-error-statuscode:
+      - '400'
+      x-content-type-options:
+      - nosniff
+      x-ms-client-request-id:
+      - 1249216d-0e54-4d4c-9942-67b9c59e8f3c
+      x-ms-rai-invoked:
+      - 'true'
+      x-ms-region:
+      - East US
+      x-ratelimit-remaining-requests:
+      - '237'
+      x-ratelimit-remaining-tokens:
+      - '239952'
+      x-request-id:
+      - dbbf34c7-b18d-449b-bac1-10bb8213ec36
+    http_version: HTTP/1.1
+    status_code: 400
+- request:
+    body: '{"messages": [{"role": "system", "content": "You are now the following
+      python function:\n```\n# generate social media hashtags from text.\ndef generate_hashtags(text:
+      str):\n```\nOnly respond with your `return` value.\n- The output should be formatted
+      as a JSON instance that conforms to the JSON schema below.\n\n- As an example,
+      for the schema {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\":
+      \"a list of strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
+      \"required\": [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted
+      instance of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}}
+      is not well-formatted.\n\n- Here is the output schema:\n```\n{\"properties\":
+      {\"ret\": {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
+      \"required\": [\"ret\"]}\n```"}, {"role": "user", "content": "generate_hashtags(''hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello'')"}], "model": "gpt35", "frequency_penalty":
+      0.0, "presence_penalty": 0.0, "stop": null, "temperature": 0.0, "top_p": 1.0,
+      "user": ""}'
+    headers:
+      accept:
+      - application/json
+      accept-encoding:
+      - gzip, deflate
+      connection:
+      - keep-alive
+      content-length:
+      - '31051'
+      content-type:
+      - application/json
+      host:
+      - gstudio.openai.azure.com
+      user-agent:
+      - AzureOpenAI/Python 1.9.0
+      x-stainless-arch:
+      - x64
+      x-stainless-async:
+      - 'false'
+      x-stainless-lang:
+      - python
+      x-stainless-os:
+      - Linux
+      x-stainless-package-version:
+      - 1.9.0
+      x-stainless-runtime:
+      - CPython
+      x-stainless-runtime-version:
+      - 3.10.14
+    method: POST
+    uri: https://gstudio.openai.azure.com/openai/deployments/gpt35/chat/completions?api-version=2023-12-01-preview
+  response:
+    content: "{\n  \"error\": {\n    \"message\": \"Sorry! We've encountered an issue
+      with repetitive patterns in your prompt. Please try again with a different prompt.\",\n
+      \   \"type\": \"invalid_request_error\",\n    \"param\": \"prompt\",\n    \"code\":
+      \"invalid_prompt\"\n  }\n}\n"
+    headers:
+      Content-Length:
+      - '245'
       Content-Type:
       - application/json
-      User-Agent:
-      - OpenAI/v1 PythonBindings/0.27.8
-      X-OpenAI-Client-User-Agent:
-      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
-        "3.11.5", "platform": "macOS-14.0-arm64-arm-64bit", "publisher": "openai",
-        "uname": "Darwin 23.0.0 Darwin Kernel Version 23.0.0: Fri Sep 15 14:41:34
-        PDT 2023; root:xnu-10002.1.13~1/RELEASE_ARM64_T8103 arm64 arm"}'
+      Date:
+      - Thu, 09 May 2024 10:08:07 GMT
+      Strict-Transport-Security:
+      - max-age=31536000; includeSubDomains; preload
+      access-control-allow-origin:
+      - '*'
+      apim-request-id:
+      - 1c78953f-23c0-46fd-b581-3ca6003eb018
+      azureml-model-session:
+      - turbo-0613-30580e30
+      ms-azureml-model-error-reason:
+      - model_error
+      ms-azureml-model-error-statuscode:
+      - '400'
+      x-content-type-options:
+      - nosniff
+      x-ms-client-request-id:
+      - 1c78953f-23c0-46fd-b581-3ca6003eb018
+      x-ms-rai-invoked:
+      - 'true'
+      x-ms-region:
+      - East US
+      x-ratelimit-remaining-requests:
+      - '237'
+      x-ratelimit-remaining-tokens:
+      - '239904'
+      x-request-id:
+      - 10d3faec-e63c-4ed8-9de5-9ee05ca8e246
+    http_version: HTTP/1.1
+    status_code: 400
+- request:
+    body: '{"messages": [{"role": "system", "content": "You are now the following
+      python function:\n```\n# generate social media hashtags from text.\ndef generate_hashtags(text:
+      str):\n```\nOnly respond with your `return` value.\n- The output should be formatted
+      as a JSON instance that conforms to the JSON schema below.\n\n- As an example,
+      for the schema {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\":
+      \"a list of strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
+      \"required\": [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted
+      instance of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}}
+      is not well-formatted.\n\n- Here is the output schema:\n```\n{\"properties\":
+      {\"ret\": {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
+      \"required\": [\"ret\"]}\n```"}, {"role": "user", "content": "generate_hashtags(''hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello hello hello hello hello hello
+      hello hello hello hello hello hello hello hello'')"}], "model": "gpt35", "frequency_penalty":
+      0.0, "presence_penalty": 0.0, "stop": null, "temperature": 0.0, "top_p": 1.0,
+      "user": ""}'
+    headers:
+      accept:
+      - application/json
+      accept-encoding:
+      - gzip, deflate
+      connection:
+      - keep-alive
+      content-length:
+      - '31051'
+      content-type:
+      - application/json
+      host:
+      - api.openai.com
+      user-agent:
+      - OpenAI/Python 1.9.0
+      x-stainless-arch:
+      - x64
+      x-stainless-async:
+      - 'false'
+      x-stainless-lang:
+      - python
+      x-stainless-os:
+      - Linux
+      x-stainless-package-version:
+      - 1.9.0
+      x-stainless-runtime:
+      - CPython
+      x-stainless-runtime-version:
+      - 3.10.14
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    body:
-      string: "{\n  \"error\": {\n    \"message\": \"This model's maximum context
-        length is 4097 tokens. However, your messages resulted in 5210 tokens. Please
-        reduce the length of the messages.\",\n    \"type\": \"invalid_request_error\",\n
-        \   \"param\": \"messages\",\n    \"code\": \"context_length_exceeded\"\n
-        \ }\n}\n"
+    content: "{\n    \"error\": {\n        \"message\": \"The model `gpt35` does not
+      exist or you do not have access to it.\",\n        \"type\": \"invalid_request_error\",\n
+      \       \"param\": null,\n        \"code\": \"model_not_found\"\n    }\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 818150f5ab944a69-TPE
+      - 8810e49b4bba4a33-TPE
       Connection:
       - keep-alive
-      Content-Length:
-      - '281'
+      Content-Encoding:
+      - gzip
       Content-Type:
-      - application/json
+      - application/json; charset=utf-8
       Date:
-      - Wed, 18 Oct 2023 14:01:58 GMT
+      - Thu, 09 May 2024 10:09:16 GMT
       Server:
       - cloudflare
-      access-control-allow-origin:
-      - '*'
+      Set-Cookie:
+      - __cf_bm=kVMxn6kAC37StYWw9UhVr7Q17NvJUhNCyZs4EVZTsmA-1715249356-1.0.1.1-WAnOenJyN3SOGniTD1EJQOzS5l9bw5zBxgybqJWON7hKWHUtUWYvxUJwt.4alvUvgEmU0uBGsjO.jG8KMeXOpQ;
+        path=/; expires=Thu, 09-May-24 10:39:16 GMT; domain=.api.openai.com; HttpOnly;
+        Secure; SameSite=None
+      - _cfuvid=39fS5aJdTPMF49PeBXcmEJ54dtpbatTP15hBc033kcA-1715249356299-0.0.1.1-604800000;
+        path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
+      Transfer-Encoding:
+      - chunked
       alt-svc:
       - h3=":443"; ma=86400
-      openai-processing-ms:
-      - '18'
-      openai-version:
-      - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
-      x-ratelimit-limit-requests:
-      - '3500'
-      x-ratelimit-limit-tokens:
-      - '90000'
-      x-ratelimit-remaining-requests:
-      - '3499'
-      x-ratelimit-remaining-tokens:
-      - '82306'
-      x-ratelimit-reset-requests:
-      - 17ms
-      x-ratelimit-reset-tokens:
-      - 5.128s
+      vary:
+      - Origin
       x-request-id:
-      - 859ec7f82955d466004b7b764343cb31
-    status:
-      code: 400
-      message: Bad Request
+      - req_b347a4a23ed49b71bdcf91cb9db96b6f
+    http_version: HTTP/1.1
+    status_code: 404
 - request:
     body: '{"messages": [{"role": "system", "content": "You are now the following
       python function:\n```\n# generate social media hashtags from text.\ndef generate_hashtags(text:
       str):\n```\nOnly respond with your `return` value.\n- The output should be formatted
       as a JSON instance that conforms to the JSON schema below.\n\n- As an example,
       for the schema {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\":
       \"a list of strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
@@ -876,83 +1815,75 @@
       content-length:
       - '31059'
       content-type:
       - application/json
       host:
       - api.openai.com
       user-agent:
-      - OpenAI/Python 1.5.0
+      - OpenAI/Python 1.9.0
       x-stainless-arch:
       - x64
       x-stainless-async:
       - 'false'
       x-stainless-lang:
       - python
       x-stainless-os:
-      - MacOS
+      - Linux
       x-stainless-package-version:
-      - 1.5.0
+      - 1.9.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
-      - 3.10.13
+      - 3.10.14
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"error\": {\n    \"message\": \"This model's maximum context length
-      is 4097 tokens. However, your messages resulted in 5210 tokens. Please reduce
-      the length of the messages.\",\n    \"type\": \"invalid_request_error\",\n    \"param\":
-      \"messages\",\n    \"code\": \"context_length_exceeded\"\n  }\n}\n"
+    content: "{\n  \"error\": {\n    \"message\": \"Sorry! We've encountered an issue
+      with repetitive patterns in your prompt. Please try again with a different prompt.\",\n
+      \   \"type\": \"invalid_prompt\",\n    \"param\": \"prompt\",\n    \"code\":
+      null\n  }\n}"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 837ddf57bfe44a22-TPE
+      - 8810e55a3a754a8d-TPE
       Connection:
       - keep-alive
       Content-Length:
-      - '281'
+      - '225'
       Content-Type:
       - application/json
       Date:
-      - Tue, 19 Dec 2023 07:18:35 GMT
+      - Thu, 09 May 2024 10:09:47 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=JQXQkHX15yAA3Q2Jh3qQkoYIzf5.gqz5U5y3bahjLgc-1702970315-1-AVps+RvmMRW/7NiY7AHMhwLPiK+Cs5i57kQTEHYzosVlR+koIVDn7n0XV3zbIC7YSe7yel2+9KEpoIDRDh5CWsw=;
-        path=/; expires=Tue, 19-Dec-23 07:48:35 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=FXfG.w9Oc3ktqOtN4kTsYVZeRfb0qFxmRHBs3V8uzUw-1715249387-1.0.1.1-CMt30Z25JNfL5HtsGCLvs5YD9NO4ULXmVx9M_vUP.nA6j4Zu2hsAojIKt1nC.wDil8oOtWtxeCfU1duU.h9Anw;
+        path=/; expires=Thu, 09-May-24 10:39:47 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=EMo.Gh3lYbEhHS7S8aiXAN28Vv3AsR_rx9dg8PHXDxU-1702970315864-0-604800000;
+      - _cfuvid=tVOyfg.Vhhj5nSSgBbwbuZrqNQ6bxjVuJdJRavhaWh0-1715249387226-0.0.1.1-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
-      access-control-allow-origin:
-      - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-processing-ms:
-      - '32'
+      - '257'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
-      - '10000'
+      - '5000'
       x-ratelimit-limit-tokens:
-      - '2000000'
-      x-ratelimit-limit-tokens_usage_based:
-      - '2000000'
+      - '160000'
       x-ratelimit-remaining-requests:
-      - '9999'
+      - '4999'
       x-ratelimit-remaining-tokens:
-      - '1992306'
-      x-ratelimit-remaining-tokens_usage_based:
-      - '1992306'
+      - '152307'
       x-ratelimit-reset-requests:
-      - 6ms
+      - 12ms
       x-ratelimit-reset-tokens:
-      - 230ms
-      x-ratelimit-reset-tokens_usage_based:
-      - 230ms
+      - 2.884s
       x-request-id:
-      - 20f05f3a98300030c8e3f311d92ae656
+      - req_829ed72ba05891364b681b22eb083d71
     http_version: HTTP/1.1
     status_code: 400
 version: 1
```

### Comparing `gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion.yaml` & `gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fake_hero.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,524 +1,376 @@
 interactions:
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "I want to book a flight to London."}], "model":
-      "gpt-3.5-turbo-0613", "temperature": 1.0, "top_p": 1.0, "frequency_penalty":
-      0.0, "presence_penalty": 0.0, "user": "", "stop": null, "functions": [{"name":
-      "book_a_flight", "description": "", "parameters": {"type": "object", "required":
-      ["date", "destination"], "properties": {"date": {"title": "Date", "type": "string"},
-      "destination": {"title": "Destination", "type": "string"}, "origin": {"title":
-      "Origin", "default": "London", "type": "string"}}, "definitions": {}}}], "function_call":
-      "auto"}'
-    headers:
-      Content-Type:
-      - application/json
-      User-Agent:
-      - OpenAI/v1 PythonBindings/0.27.8
-      X-OpenAI-Client-User-Agent:
-      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
-        "3.11.4", "platform": "macOS-13.4.1-arm64-arm-64bit", "publisher": "openai",
-        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Thu Jun  8 22:22:19
-        PDT 2023; root:xnu-8796.121.3~7/RELEASE_ARM64_T8103 arm64 arm"}'
-    method: post
-    uri: https://api.openai.com/v1/chat/completions
-  response:
-    body:
-      string: "{\n  \"id\": \"chatcmpl-7i3U58wuJlTHqt9lc7pJEP04ec0rY\",\n  \"object\":
-        \"chat.completion\",\n  \"created\": 1690734181,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
-        \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-        \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n
-        \         \"name\": \"book_a_flight\",\n          \"arguments\": \"{\\n  \\\"date\\\":
-        \\\"2022-10-15\\\",\\n  \\\"destination\\\": \\\"London\\\"\\n}\"\n        }\n
-        \     },\n      \"finish_reason\": \"function_call\"\n    }\n  ],\n  \"usage\":
-        {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 28,\n    \"total_tokens\":
-        95\n  }\n}\n"
-    headers:
-      Access-Control-Allow-Origin:
-      - '*'
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-RAY:
-      - 7eeef199ca246b62-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - gzip
-      Content-Type:
-      - application/json
-      Date:
-      - Sun, 30 Jul 2023 16:23:02 GMT
-      Server:
-      - cloudflare
-      Transfer-Encoding:
-      - chunked
-      alt-svc:
-      - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
-      openai-processing-ms:
-      - '999'
-      openai-version:
-      - '2020-10-01'
-      strict-transport-security:
-      - max-age=15724800; includeSubDomains
-      x-ratelimit-limit-requests:
-      - '3500'
-      x-ratelimit-limit-tokens:
-      - '90000'
-      x-ratelimit-remaining-requests:
-      - '3499'
-      x-ratelimit-remaining-tokens:
-      - '89965'
-      x-ratelimit-reset-requests:
-      - 17ms
-      x-ratelimit-reset-tokens:
-      - 22ms
-      x-request-id:
-      - 6f842b696f3e642e2702be6aa7709277
-    status:
-      code: 200
-      message: OK
-    url: https://api.openai.com/v1/chat/completions
-- request:
-    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "I want to book a flight to London."}], "model":
-      "gpt-3.5-turbo-0613", "frequency_penalty": 0.0, "function_call": "auto", "functions":
-      [{"name": "book_a_flight", "description": "", "parameters": {"type": "object",
-      "required": ["date", "destination"], "properties": {"date": {"title": "Date",
-      "type": "string"}, "destination": {"title": "Destination", "type": "string"},
-      "origin": {"title": "Origin", "default": "London", "type": "string"}}, "definitions":
-      {}}}], "presence_penalty": 0.0, "stop": null, "temperature": 1.0, "top_p": 1.0,
-      "user": ""}'
+    body: '{"messages": [{"role": "system", "content": "You are now the following
+      python function:\n```\n# generate fake hero.\ndef fake_hero(n: int):\n```\nOnly
+      respond with your `return` value.\n- The output should be formatted as a JSON
+      instance that conforms to the JSON schema below.\n\n- As an example, for the
+      schema {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a
+      list of strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
+      \"required\": [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted
+      instance of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}}
+      is not well-formatted.\n\n- Here is the output schema:\n```\n{\"properties\":
+      {\"ret\": {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"$ref\": \"#/definitions/Hero\"}}},
+      \"required\": [\"ret\"], \"definitions\": {\"Hero\": {\"title\": \"Hero\", \"description\":
+      \"Hero model.\", \"type\": \"object\", \"properties\": {\"name\": {\"title\":
+      \"Name\", \"type\": \"string\"}, \"age\": {\"title\": \"Age\", \"type\": \"integer\"}},
+      \"required\": [\"name\", \"age\"]}}}\n```"}, {"role": "user", "content": "fake_hero(5)"}],
+      "model": "gpt35", "frequency_penalty": 0.0, "presence_penalty": 0.0, "stop":
+      null, "temperature": 0.0, "top_p": 1.0, "user": ""}'
     headers:
       accept:
       - application/json
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '652'
+      - '1286'
       content-type:
       - application/json
       host:
-      - api.openai.com
+      - gstudio.openai.azure.com
       user-agent:
-      - OpenAI/Python 1.3.9
+      - AzureOpenAI/Python 1.9.0
       x-stainless-arch:
       - x64
       x-stainless-async:
       - 'false'
       x-stainless-lang:
       - python
       x-stainless-os:
-      - MacOS
+      - Linux
       x-stainless-package-version:
-      - 1.3.9
+      - 1.9.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
-      - 3.10.13
+      - 3.10.14
     method: POST
-    uri: https://api.openai.com/v1/chat/completions
+    uri: https://gstudio.openai.azure.com/openai/deployments/gpt35/chat/completions?api-version=2023-07-01-preview
   response:
-    content: "{\n  \"id\": \"chatcmpl-8X3Rsmcy0L2gagpLgTxSEXCf3B5nu\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1702888772,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
-      \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n          \"name\":
-      \"book_a_flight\",\n          \"arguments\": \"{\\n  \\\"date\\\": \\\"2022-08-15\\\",\\n
-      \ \\\"destination\\\": \\\"London\\\"\\n}\"\n        }\n      },\n      \"logprobs\":
-      null,\n      \"finish_reason\": \"function_call\"\n    }\n  ],\n  \"usage\":
-      {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 28,\n    \"total_tokens\":
-      95\n  },\n  \"system_fingerprint\": null\n}\n"
+    content: '{"choices":[{"content_filter_results":{"hate":{"filtered":false,"severity":"safe"},"self_harm":{"filtered":false,"severity":"safe"},"sexual":{"filtered":false,"severity":"safe"},"violence":{"filtered":false,"severity":"safe"}},"finish_reason":"stop","index":0,"message":{"content":"{\"ret\":
+      [{\"name\": \"Hero 1\", \"age\": 25}, {\"name\": \"Hero 2\", \"age\": 30}, {\"name\":
+      \"Hero 3\", \"age\": 35}, {\"name\": \"Hero 4\", \"age\": 40}, {\"name\": \"Hero
+      5\", \"age\": 45}]}","role":"assistant"}}],"created":1715249236,"id":"chatcmpl-9MuyCeT79BYaOt9h13lbBaX5F4dA0","model":"gpt-35-turbo-16k","object":"chat.completion","prompt_filter_results":[{"prompt_index":0,"content_filter_results":{"hate":{"filtered":false,"severity":"safe"},"self_harm":{"filtered":false,"severity":"safe"},"sexual":{"filtered":false,"severity":"safe"},"violence":{"filtered":false,"severity":"safe"}}}],"system_fingerprint":null,"usage":{"completion_tokens":74,"prompt_tokens":279,"total_tokens":353}}
+
+      '
     headers:
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-RAY:
-      - 8376188cd94d4a1b-TPE
       Cache-Control:
       - no-cache, must-revalidate
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - gzip
+      Content-Length:
+      - '981'
       Content-Type:
       - application/json
       Date:
-      - Mon, 18 Dec 2023 08:39:34 GMT
-      Server:
-      - cloudflare
-      Set-Cookie:
-      - __cf_bm=iPTutriSl5GS45eJkm4U4m2ed29aN8r7nfzNne3sqGQ-1702888774-1-AWKgTDQO1BU6nzpRepVdtSKD5YjJf8+iFWOeoCu2KSgDGhyn3sFfBYHCqI/PNNGtLMeqRkkarWGtJ4xsRaXBvp0=;
-        path=/; expires=Mon, 18-Dec-23 09:09:34 GMT; domain=.api.openai.com; HttpOnly;
-        Secure; SameSite=None
-      - _cfuvid=zlrepFeDp56HCK4GjixNH1X5I2IdsgsD8mSAoTKwneU-1702888774226-0-604800000;
-        path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
-      Transfer-Encoding:
-      - chunked
+      - Thu, 09 May 2024 10:07:17 GMT
+      Strict-Transport-Security:
+      - max-age=31536000; includeSubDomains; preload
       access-control-allow-origin:
       - '*'
-      alt-svc:
-      - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
-      openai-processing-ms:
-      - '1105'
-      openai-version:
-      - '2020-10-01'
-      strict-transport-security:
-      - max-age=15724800; includeSubDomains
-      x-ratelimit-limit-requests:
-      - '10000'
-      x-ratelimit-limit-tokens:
-      - '2000000'
-      x-ratelimit-limit-tokens_usage_based:
-      - '2000000'
+      apim-request-id:
+      - 3dfd3289-df2f-4d5f-9732-92bba3065800
+      azureml-model-session:
+      - turbo-0613-16a13266
+      x-accel-buffering:
+      - 'no'
+      x-content-type-options:
+      - nosniff
+      x-ms-client-request-id:
+      - 3dfd3289-df2f-4d5f-9732-92bba3065800
+      x-ms-rai-invoked:
+      - 'true'
+      x-ms-region:
+      - East US
       x-ratelimit-remaining-requests:
-      - '9999'
+      - '238'
       x-ratelimit-remaining-tokens:
-      - '1999965'
-      x-ratelimit-remaining-tokens_usage_based:
-      - '1999965'
-      x-ratelimit-reset-requests:
-      - 6ms
-      x-ratelimit-reset-tokens:
-      - 1ms
-      x-ratelimit-reset-tokens_usage_based:
-      - 1ms
+      - '239968'
       x-request-id:
-      - 17dc404ace9dbeefba35940532bfeced
+      - 556593c2-5631-424b-a4f7-2fd5a3cfeb2c
     http_version: HTTP/1.1
     status_code: 200
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "I want to book a flight to London."}], "model":
-      "gpt-3.5-turbo-0613", "frequency_penalty": 0.0, "function_call": "auto", "functions":
-      [{"name": "book_a_flight", "description": "", "parameters": {"type": "object",
-      "required": ["date", "destination"], "properties": {"date": {"title": "Date",
-      "type": "string"}, "destination": {"title": "Destination", "type": "string"},
-      "origin": {"title": "Origin", "default": "London", "type": "string"}}, "definitions":
-      {}}}], "presence_penalty": 0.0, "stop": null, "temperature": 1.0, "top_p": 1.0,
-      "user": ""}'
+    body: '{"messages": [{"role": "system", "content": "You are now the following
+      python function:\n```\n# generate fake hero.\ndef fake_hero(n: int):\n```\nOnly
+      respond with your `return` value.\n- The output should be formatted as a JSON
+      instance that conforms to the JSON schema below.\n\n- As an example, for the
+      schema {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a
+      list of strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
+      \"required\": [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted
+      instance of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}}
+      is not well-formatted.\n\n- Here is the output schema:\n```\n{\"properties\":
+      {\"ret\": {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"$ref\": \"#/definitions/Hero\"}}},
+      \"required\": [\"ret\"], \"definitions\": {\"Hero\": {\"title\": \"Hero\", \"description\":
+      \"Hero model.\", \"type\": \"object\", \"properties\": {\"name\": {\"title\":
+      \"Name\", \"type\": \"string\"}, \"age\": {\"title\": \"Age\", \"type\": \"integer\"}},
+      \"required\": [\"name\", \"age\"]}}}\n```"}, {"role": "user", "content": "fake_hero(5)"}],
+      "model": "gpt35", "frequency_penalty": 0.0, "presence_penalty": 0.0, "stop":
+      null, "temperature": 0.0, "top_p": 1.0, "user": ""}'
     headers:
       accept:
       - application/json
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '652'
+      - '1286'
       content-type:
       - application/json
       host:
-      - api.openai.com
+      - gstudio.openai.azure.com
       user-agent:
-      - OpenAI/Python 1.3.9
+      - AzureOpenAI/Python 1.9.0
       x-stainless-arch:
       - x64
       x-stainless-async:
       - 'false'
       x-stainless-lang:
       - python
       x-stainless-os:
-      - MacOS
+      - Linux
       x-stainless-package-version:
-      - 1.3.9
+      - 1.9.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
-      - 3.10.13
+      - 3.10.14
     method: POST
-    uri: https://api.openai.com/v1/chat/completions
+    uri: https://gstudio.openai.azure.com/openai/deployments/gpt35/chat/completions?api-version=2023-12-01-preview
   response:
-    content: "{\n  \"id\": \"chatcmpl-8X3Utn99nPRoGoJpfi2jedsDZZoCs\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1702888959,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
-      \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n          \"name\":
-      \"book_a_flight\",\n          \"arguments\": \"{\\n  \\\"date\\\": \\\"2022-07-15\\\",\\n
-      \ \\\"destination\\\": \\\"London\\\"\\n}\"\n        }\n      },\n      \"logprobs\":
-      null,\n      \"finish_reason\": \"function_call\"\n    }\n  ],\n  \"usage\":
-      {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 28,\n    \"total_tokens\":
-      95\n  },\n  \"system_fingerprint\": null\n}\n"
+    content: '{"choices":[{"content_filter_results":{"hate":{"filtered":false,"severity":"safe"},"self_harm":{"filtered":false,"severity":"safe"},"sexual":{"filtered":false,"severity":"safe"},"violence":{"filtered":false,"severity":"safe"}},"finish_reason":"stop","index":0,"message":{"content":"{\"ret\":
+      [{\"name\": \"Hero 1\", \"age\": 25}, {\"name\": \"Hero 2\", \"age\": 30}, {\"name\":
+      \"Hero 3\", \"age\": 35}, {\"name\": \"Hero 4\", \"age\": 40}, {\"name\": \"Hero
+      5\", \"age\": 45}]}","role":"assistant"}}],"created":1715249285,"id":"chatcmpl-9Muyz3RbRO78G2fzWHdCZH8pexfNh","model":"gpt-35-turbo-16k","object":"chat.completion","prompt_filter_results":[{"prompt_index":0,"content_filter_results":{"hate":{"filtered":false,"severity":"safe"},"self_harm":{"filtered":false,"severity":"safe"},"sexual":{"filtered":false,"severity":"safe"},"violence":{"filtered":false,"severity":"safe"}}}],"system_fingerprint":null,"usage":{"completion_tokens":74,"prompt_tokens":279,"total_tokens":353}}
+
+      '
     headers:
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-RAY:
-      - 83761d186ff84a7e-TPE
       Cache-Control:
       - no-cache, must-revalidate
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - gzip
+      Content-Length:
+      - '981'
       Content-Type:
       - application/json
       Date:
-      - Mon, 18 Dec 2023 08:42:40 GMT
-      Server:
-      - cloudflare
-      Set-Cookie:
-      - __cf_bm=OxTkn35Z8EEqkRsOoF.6NC.e4Z2rmIUGFOXhpjo4cyw-1702888960-1-Afz176VG8lZj/62Gu4ywkq3279RMzcwdlG/m400HnMfUgfyRwJAdiMcG5/qhCtWAGlqX1LLfw+/XCiBfMaPiCCs=;
-        path=/; expires=Mon, 18-Dec-23 09:12:40 GMT; domain=.api.openai.com; HttpOnly;
-        Secure; SameSite=None
-      - _cfuvid=g6oV6X7LLCFm_.0sxr13uOZtZ6xmDfJV_fE7gV3IrPI-1702888960408-0-604800000;
-        path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
-      Transfer-Encoding:
-      - chunked
+      - Thu, 09 May 2024 10:08:06 GMT
+      Strict-Transport-Security:
+      - max-age=31536000; includeSubDomains; preload
       access-control-allow-origin:
       - '*'
-      alt-svc:
-      - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
-      openai-processing-ms:
-      - '1117'
-      openai-version:
-      - '2020-10-01'
-      strict-transport-security:
-      - max-age=15724800; includeSubDomains
-      x-ratelimit-limit-requests:
-      - '10000'
-      x-ratelimit-limit-tokens:
-      - '2000000'
-      x-ratelimit-limit-tokens_usage_based:
-      - '2000000'
+      apim-request-id:
+      - 71a9ceac-aa01-45eb-b9d6-4e13a92296a3
+      azureml-model-session:
+      - turbo-0613-27f31441
+      x-accel-buffering:
+      - 'no'
+      x-content-type-options:
+      - nosniff
+      x-ms-client-request-id:
+      - 71a9ceac-aa01-45eb-b9d6-4e13a92296a3
+      x-ms-rai-invoked:
+      - 'true'
+      x-ms-region:
+      - East US
       x-ratelimit-remaining-requests:
-      - '9999'
+      - '238'
       x-ratelimit-remaining-tokens:
-      - '1999965'
-      x-ratelimit-remaining-tokens_usage_based:
-      - '1999965'
-      x-ratelimit-reset-requests:
-      - 6ms
-      x-ratelimit-reset-tokens:
-      - 1ms
-      x-ratelimit-reset-tokens_usage_based:
-      - 1ms
+      - '239920'
       x-request-id:
-      - f2baa8c34e422b1aa7d0926c647dfe21
+      - 5fac9305-b66a-4aba-bd82-f677b4269ae7
     http_version: HTTP/1.1
     status_code: 200
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "I want to book a flight to London."}], "model":
-      "gpt-3.5-turbo-0613", "frequency_penalty": 0.0, "function_call": "auto", "functions":
-      [{"name": "book_a_flight", "description": "", "parameters": {"type": "object",
-      "required": ["date", "destination"], "properties": {"date": {"title": "Date",
-      "type": "string"}, "destination": {"title": "Destination", "type": "string"},
-      "origin": {"title": "Origin", "default": "London", "type": "string"}}, "definitions":
-      {}}}], "presence_penalty": 0.0, "stop": null, "temperature": 1.0, "top_p": 1.0,
-      "user": ""}'
+    body: '{"messages": [{"role": "system", "content": "You are now the following
+      python function:\n```\n# generate fake hero.\ndef fake_hero(n: int):\n```\nOnly
+      respond with your `return` value.\n- The output should be formatted as a JSON
+      instance that conforms to the JSON schema below.\n\n- As an example, for the
+      schema {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a
+      list of strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
+      \"required\": [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted
+      instance of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}}
+      is not well-formatted.\n\n- Here is the output schema:\n```\n{\"properties\":
+      {\"ret\": {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"$ref\": \"#/definitions/Hero\"}}},
+      \"required\": [\"ret\"], \"definitions\": {\"Hero\": {\"title\": \"Hero\", \"description\":
+      \"Hero model.\", \"type\": \"object\", \"properties\": {\"name\": {\"title\":
+      \"Name\", \"type\": \"string\"}, \"age\": {\"title\": \"Age\", \"type\": \"integer\"}},
+      \"required\": [\"name\", \"age\"]}}}\n```"}, {"role": "user", "content": "fake_hero(5)"}],
+      "model": "gpt35", "frequency_penalty": 0.0, "presence_penalty": 0.0, "stop":
+      null, "temperature": 0.0, "top_p": 1.0, "user": ""}'
     headers:
       accept:
       - application/json
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '652'
+      - '1286'
       content-type:
       - application/json
       host:
       - api.openai.com
       user-agent:
-      - AsyncOpenAI/Python 1.3.9
+      - OpenAI/Python 1.9.0
       x-stainless-arch:
       - x64
       x-stainless-async:
-      - async:asyncio
+      - 'false'
       x-stainless-lang:
       - python
       x-stainless-os:
-      - MacOS
+      - Linux
       x-stainless-package-version:
-      - 1.3.9
+      - 1.9.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
-      - 3.10.13
+      - 3.10.14
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"id\": \"chatcmpl-8X3VRLvY2YJeZ1NAj1WCkVKvMw7mE\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1702888993,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
-      \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n          \"name\":
-      \"book_a_flight\",\n          \"arguments\": \"{\\n  \\\"date\\\": \\\"2021-08-15\\\",\\n
-      \ \\\"destination\\\": \\\"London\\\"\\n}\"\n        }\n      },\n      \"logprobs\":
-      null,\n      \"finish_reason\": \"function_call\"\n    }\n  ],\n  \"usage\":
-      {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 28,\n    \"total_tokens\":
-      95\n  },\n  \"system_fingerprint\": null\n}\n"
+    content: "{\n    \"error\": {\n        \"message\": \"The model `gpt35` does not
+      exist or you do not have access to it.\",\n        \"type\": \"invalid_request_error\",\n
+      \       \"param\": null,\n        \"code\": \"model_not_found\"\n    }\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 83761ded0de16a86-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
+      - 8810e497ecde4a1c-TPE
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
-      - application/json
+      - application/json; charset=utf-8
       Date:
-      - Mon, 18 Dec 2023 08:43:14 GMT
+      - Thu, 09 May 2024 10:09:15 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=psEs3cRT7.IWBZoWC7WXa7q3McY1Uv5Li_IeJKl5Ztk-1702888994-1-AS6aj7JlnUqp9oajsxNnaxRAUmkJY+DwN523B//i0mNtYZ6qCveQa3SCxoH3//k/eBTAxyIEyYBgSXMZA/YcoiI=;
-        path=/; expires=Mon, 18-Dec-23 09:13:14 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=4amjYyQR4m38Yq46EVvM6HIkFaLRnR9rRSh_nruWv3E-1715249355-1.0.1.1-x1HM8mWfyR6_We.KMtVOX2sBKP5wiXI903ZwQen3CVKuzn88WXgjwQ8fH2Ci53G_Tj6HzzRcwteulco3dpgXzA;
+        path=/; expires=Thu, 09-May-24 10:39:15 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=aumQA_fW_8I41U1oR1fn806BQwOL6dR36DSPBgVfGYg-1702888994391-0-604800000;
+      - _cfuvid=VLrrYmiDLbZI0Phi6n66mWeWga.Fu5KHrUCSuDmElR4-1715249355718-0.0.1.1-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
       Transfer-Encoding:
       - chunked
-      access-control-allow-origin:
-      - '*'
       alt-svc:
       - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
-      openai-processing-ms:
-      - '1099'
-      openai-version:
-      - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
-      x-ratelimit-limit-requests:
-      - '10000'
-      x-ratelimit-limit-tokens:
-      - '2000000'
-      x-ratelimit-limit-tokens_usage_based:
-      - '2000000'
-      x-ratelimit-remaining-requests:
-      - '9999'
-      x-ratelimit-remaining-tokens:
-      - '1999965'
-      x-ratelimit-remaining-tokens_usage_based:
-      - '1999965'
-      x-ratelimit-reset-requests:
-      - 6ms
-      x-ratelimit-reset-tokens:
-      - 1ms
-      x-ratelimit-reset-tokens_usage_based:
-      - 1ms
+      vary:
+      - Origin
       x-request-id:
-      - 26a54147c78e4e609da36758ed959627
+      - req_50b1e35461e4d0facadaae863f0d074d
     http_version: HTTP/1.1
-    status_code: 200
+    status_code: 404
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "I want to book a flight to London."}], "model":
-      "gpt-3.5-turbo-0613", "frequency_penalty": 0.0, "function_call": "auto", "functions":
-      [{"name": "book_a_flight", "description": "", "parameters": {"type": "object",
-      "required": ["date", "destination"], "properties": {"date": {"title": "Date",
-      "type": "string"}, "destination": {"title": "Destination", "type": "string"},
-      "origin": {"title": "Origin", "default": "London", "type": "string"}}, "definitions":
-      {}}}], "presence_penalty": 0.0, "stop": null, "temperature": 1.0, "top_p": 1.0,
-      "user": ""}'
+    body: '{"messages": [{"role": "system", "content": "You are now the following
+      python function:\n```\n# generate fake hero.\ndef fake_hero(n: int):\n```\nOnly
+      respond with your `return` value.\n- The output should be formatted as a JSON
+      instance that conforms to the JSON schema below.\n\n- As an example, for the
+      schema {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a
+      list of strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
+      \"required\": [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted
+      instance of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}}
+      is not well-formatted.\n\n- Here is the output schema:\n```\n{\"properties\":
+      {\"ret\": {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"$ref\": \"#/definitions/Hero\"}}},
+      \"required\": [\"ret\"], \"definitions\": {\"Hero\": {\"title\": \"Hero\", \"description\":
+      \"Hero model.\", \"type\": \"object\", \"properties\": {\"name\": {\"title\":
+      \"Name\", \"type\": \"string\"}, \"age\": {\"title\": \"Age\", \"type\": \"integer\"}},
+      \"required\": [\"name\", \"age\"]}}}\n```"}, {"role": "user", "content": "fake_hero(5)"}],
+      "model": "gpt-3.5-turbo", "frequency_penalty": 0.0, "presence_penalty": 0.0,
+      "stop": null, "temperature": 0.0, "top_p": 1.0, "user": ""}'
     headers:
       accept:
       - application/json
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '652'
+      - '1294'
       content-type:
       - application/json
       host:
       - api.openai.com
       user-agent:
-      - AsyncOpenAI/Python 1.5.0
+      - OpenAI/Python 1.9.0
       x-stainless-arch:
       - x64
       x-stainless-async:
-      - async:asyncio
+      - 'false'
       x-stainless-lang:
       - python
       x-stainless-os:
-      - MacOS
+      - Linux
       x-stainless-package-version:
-      - 1.5.0
+      - 1.9.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
-      - 3.10.13
+      - 3.10.14
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"id\": \"chatcmpl-8XOf7cAm91k3cQ4ZqD1dxMRxLuMu4\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1702970317,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+    content: "{\n  \"id\": \"chatcmpl-9Mv0anVntVg30AgrRfDP6vgCGe9y3\",\n  \"object\":
+      \"chat.completion\",\n  \"created\": 1715249384,\n  \"model\": \"gpt-3.5-turbo-0125\",\n
       \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n          \"name\":
-      \"book_a_flight\",\n          \"arguments\": \"{\\n  \\\"date\\\": \\\"2022-06-15\\\",\\n
-      \ \\\"destination\\\": \\\"London\\\"\\n}\"\n        }\n      },\n      \"logprobs\":
-      null,\n      \"finish_reason\": \"function_call\"\n    }\n  ],\n  \"usage\":
-      {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 28,\n    \"total_tokens\":
-      95\n  },\n  \"system_fingerprint\": null\n}\n"
+      \"assistant\",\n        \"content\": \"{\\n    \\\"ret\\\": [\\n        {\\n
+      \           \\\"name\\\": \\\"Fake Hero 1\\\",\\n            \\\"age\\\": 25\\n
+      \       },\\n        {\\n            \\\"name\\\": \\\"Fake Hero 2\\\",\\n            \\\"age\\\":
+      30\\n        },\\n        {\\n            \\\"name\\\": \\\"Fake Hero 3\\\",\\n
+      \           \\\"age\\\": 28\\n        },\\n        {\\n            \\\"name\\\":
+      \\\"Fake Hero 4\\\",\\n            \\\"age\\\": 27\\n        },\\n        {\\n
+      \           \\\"name\\\": \\\"Fake Hero 5\\\",\\n            \\\"age\\\": 29\\n
+      \       }\\n    ]\\n}\"\n      },\n      \"logprobs\": null,\n      \"finish_reason\":
+      \"stop\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\": 279,\n    \"completion_tokens\":
+      114,\n    \"total_tokens\": 393\n  },\n  \"system_fingerprint\": null\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 837ddf652f734a91-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
+      - 8810e54bf81e826b-TPE
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Tue, 19 Dec 2023 07:18:39 GMT
+      - Thu, 09 May 2024 10:09:46 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=sjLcIvpPi7do1m.M3IKNal5iNgd1BSZsILCMk9lGH9w-1702970319-1-Acl/9bDrPVfaYBorUHtF7kcOVfRhh9OkoflOMU2gjSnIcEWNdxhhYZ/sYfaIyIBufGjKB5YwIBexxDE55B46uYo=;
-        path=/; expires=Tue, 19-Dec-23 07:48:39 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=w2BOBEcZSYwVQeZlUJvTo_.z5H2T.P9lyfawDqoi3Mg-1715249386-1.0.1.1-fC2I88Niz.UCXxSCFYhHvWzvXmEhNUA5qLxK09mV7CsXN_ao6eIVLXd4CIO7o3sGFse.q2Q_5I7qyFRApbV6hw;
+        path=/; expires=Thu, 09-May-24 10:39:46 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=KnnoCCvUiBJu4jUwfnJQpTUSDYjouBa7Mq3Fde4ALN8-1702970319041-0-604800000;
+      - _cfuvid=54fIYpydE2vsJ1Z0GmTQoOuzcSTflkmQxdsYav_YU0k-1715249386414-0.0.1.1-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
       Transfer-Encoding:
       - chunked
-      access-control-allow-origin:
-      - '*'
       alt-svc:
       - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
       openai-processing-ms:
-      - '931'
+      - '1739'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
-      - '10000'
+      - '5000'
       x-ratelimit-limit-tokens:
-      - '2000000'
-      x-ratelimit-limit-tokens_usage_based:
-      - '2000000'
+      - '160000'
       x-ratelimit-remaining-requests:
-      - '9999'
+      - '4999'
       x-ratelimit-remaining-tokens:
-      - '1999965'
-      x-ratelimit-remaining-tokens_usage_based:
-      - '1999965'
+      - '159743'
       x-ratelimit-reset-requests:
-      - 6ms
+      - 12ms
       x-ratelimit-reset-tokens:
-      - 1ms
-      x-ratelimit-reset-tokens_usage_based:
-      - 1ms
+      - 96ms
       x-request-id:
-      - 28b9552c873bb31da96d22ac598001f2
+      - req_b5b355963570a80a40bcb5bfd38d7725
     http_version: HTTP/1.1
     status_code: 200
 version: 1
```

### Comparing `gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion.yaml` & `gpt_fn-0.1.3/src/gpt_fn/utils/tests/cassettes/test_pydantic_parser/test_pydantic_parser_with_prompt[email.txt-Email].yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,203 +1,152 @@
 interactions:
 - request:
-    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "Give me a sample email."}], "model": "gpt-3.5-turbo-0613",
-      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
-      0.0, "user": "", "functions": [{"name": "structural_response", "description":
+    body: '{"messages": [{"role": "system", "content": ""}, {"role": "user", "content":
+      "Given the press release article of our company: \"RIVERTON Industries - Revolutionizing
+      the Aluminum Casting Industry for E-Bikes\n\nRIVERTON Industries is a leading
+      manufacturer and exporter of aluminum casting products for E-Bikes. Established
+      in 2022, the company has quickly gained a reputation for its innovative approach
+      to aluminum frame manufacturing. We offer one-stop solutions for customized
+      bike frames, which include designing, manufacturing, and assembly services.\n\n###
+      About RIVERTON Industries\nRIVERTON Industries is an innovative international
+      company specializing in aluminum casting products for E-Bikes. The company is
+      committed to providing innovative aluminum frames built for bicycles and modular
+      features for multiple modeling combinations. We offer ready-to-use products
+      and vehicle assembly services that meet customer satisfaction and provide specialized
+      services tailored to their requirements.\n\nRIVERTON Industries is revolutionizing
+      the aluminum casting industry for E-bikes. Our main product, the Aluminum frame
+      for E-bike, is available in three models - 001, 002, and 003 but more could
+      be customized. The one-piece-formed bike frame provides increased rigidity,
+      improving the stability and safety of the ride. The solid frame made of aluminum
+      pipeline built-in supports complex designs for electric bikes.\n\nOur one-stop
+      solution for customized bike frames has made us a popular choice among customers.
+      We offer a range of products, including the Electric bike frame, Aluminum motor
+      frames for E-bikes, Motor frames for E-bikes, and Customized Motor frames for
+      E-bikes.\n\nRIVERTON Industries exports its products to Europe and the USA.
+      Our commitment to quality has earned us a reputation for producing high-quality
+      aluminum frames that meet international standards.\n\nIn conclusion, RIVERTON
+      Industries is a company that is revolutionizing the aluminum casting industry
+      for E-bikes. Our innovative approach to manufacturing aluminum frames and one-stop
+      solutions for customized bike frames has made us a popular choice among customers.
+      If you''re looking for high-quality aluminum frames for your E-bikes, visit
+      our website at https://riverton.example.com/.\"\n"}], "model": "gpt-3.5-turbo-0613",
+      "frequency_penalty": 0.0, "presence_penalty": 0.0, "temperature": 1.0, "tool_choice":
+      {"type": "function", "function": {"name": "structural_response"}}, "tools":
+      [{"type": "function", "function": {"name": "structural_response", "description":
       "Response to user in a structural way.", "parameters": {"title": "Email", "type":
       "object", "properties": {"subject": {"title": "Subject", "description": "the
       subject of email", "type": "string"}, "body": {"title": "Body", "description":
-      "the body of email", "type": "string"}}, "required": ["subject", "body"]}}],
-      "function_call": {"name": "structural_response"}}'
-    headers:
-      Content-Type:
-      - application/json
-      User-Agent:
-      - OpenAI/v1 PythonBindings/0.27.8
-      X-OpenAI-Client-User-Agent:
-      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
-        "3.11.4", "platform": "macOS-13.4.1-arm64-arm-64bit", "publisher": "openai",
-        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Thu Jun  8 22:22:19
-        PDT 2023; root:xnu-8796.121.3~7/RELEASE_ARM64_T8103 arm64 arm"}'
-    method: post
-    uri: https://api.openai.com/v1/chat/completions
-  response:
-    content: "{\n  \"id\": \"chatcmpl-7i3UEtSi8kUoTyV8w3AbL2b39CGdO\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1690734190,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
-      \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n          \"name\":
-      \"structural_response\",\n          \"arguments\": \"{\\n  \\\"subject\\\":
-      \\\"Hello!\\\",\\n  \\\"body\\\": \\\"Dear [Recipient's Name],\\\\n\\\\nI hope
-      this email finds you well. I just wanted to reach out and say hello. It has
-      been a while since we last caught up and I wanted to see how you have been doing.\\\\n\\\\nIs
-      there a good time for us to connect and catch up? I would love to hear about
-      all the exciting things happening in your life.\\\\n\\\\nLooking forward to
-      hearing from you!\\\\n\\\\nBest regards,\\\\n[Your Name]\\\"\\n}\"\n        }\n
-      \     },\n      \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
-      82,\n    \"completion_tokens\": 111,\n    \"total_tokens\": 193\n  }\n}\n"
-    headers:
-      Access-Control-Allow-Origin:
-      - '*'
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-RAY:
-      - 7eeef1ccde834a48-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - gzip
-      Content-Type:
-      - application/json
-      Date:
-      - Sun, 30 Jul 2023 16:23:13 GMT
-      Server:
-      - cloudflare
-      Transfer-Encoding:
-      - chunked
-      alt-svc:
-      - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
-      openai-processing-ms:
-      - '3791'
-      openai-version:
-      - '2020-10-01'
-      strict-transport-security:
-      - max-age=15724800; includeSubDomains
-      x-ratelimit-limit-requests:
-      - '3500'
-      x-ratelimit-limit-tokens:
-      - '90000'
-      x-ratelimit-remaining-requests:
-      - '3499'
-      x-ratelimit-remaining-tokens:
-      - '89968'
-      x-ratelimit-reset-requests:
-      - 17ms
-      x-ratelimit-reset-tokens:
-      - 20ms
-      x-request-id:
-      - c9cafa17b1fdbf94b33a470d1d3ec6fd
-    status:
-      code: 200
-      message: OK
-    url: https://api.openai.com/v1/chat/completions
-- request:
-    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "Give me a sample email."}], "model": "gpt-3.5-turbo-0613",
-      "frequency_penalty": 0.0, "function_call": {"name": "structural_response"},
-      "functions": [{"name": "structural_response", "description": "Response to user
-      in a structural way.", "parameters": {"title": "Email", "type": "object", "properties":
-      {"subject": {"title": "Subject", "description": "the subject of email", "type":
-      "string"}, "body": {"title": "Body", "description": "the body of email", "type":
-      "string"}}, "required": ["subject", "body"]}}], "presence_penalty": 0.0, "temperature":
-      1.0, "top_p": 1.0, "user": ""}'
+      "the body of email", "type": "string"}}, "required": ["subject", "body"]}}}],
+      "top_p": 1.0, "user": ""}'
     headers:
       accept:
       - application/json
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '687'
+      - '2900'
       content-type:
       - application/json
       host:
       - api.openai.com
       user-agent:
-      - AsyncOpenAI/Python 1.5.0
+      - OpenAI/Python 1.9.0
       x-stainless-arch:
       - x64
       x-stainless-async:
-      - async:asyncio
+      - 'false'
       x-stainless-lang:
       - python
       x-stainless-os:
-      - MacOS
+      - Linux
       x-stainless-package-version:
-      - 1.5.0
+      - 1.9.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
-      - 3.10.13
+      - 3.10.14
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"id\": \"chatcmpl-8XOfJERyRd8QeOGumycg9iJdqEgMk\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1702970329,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+    content: "{\n  \"id\": \"chatcmpl-9OLY7Q1ARHFGj8GQhOIKZZz6t5XfZ\",\n  \"object\":
+      \"chat.completion\",\n  \"created\": 1715589735,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
       \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n          \"name\":
-      \"structural_response\",\n          \"arguments\": \"{\\n  \\\"subject\\\":
-      \\\"Sample Email\\\",\\n  \\\"body\\\": \\\"Dear [Recipient's Name],\\\\n\\\\nI
-      hope this email finds you well. I am reaching out to discuss [Subject of Discussion].\\\\n\\\\n[Provide
-      a brief introduction and purpose of the email].\\\\n\\\\n[Include relevant details,
-      information, or requests].\\\\n\\\\n[Offer assistance or provide next steps].\\\\n\\\\nPlease
-      let me know if you have any questions or require further clarification. I look
-      forward to your response.\\\\n\\\\nThank you and best regards,\\\\n[Your Name]\\\\n[Your
-      Contact Information]\\\"\\n}\"\n        }\n      },\n      \"logprobs\": null,\n
-      \     \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
-      82,\n    \"completion_tokens\": 124,\n    \"total_tokens\": 206\n  },\n  \"system_fingerprint\":
+      \"assistant\",\n        \"content\": null,\n        \"tool_calls\": [\n          {\n
+      \           \"id\": \"call_TCw6JzqLIrFsAtnHKVpTMGeG\",\n            \"type\":
+      \"function\",\n            \"function\": {\n              \"name\": \"structural_response\",\n
+      \             \"arguments\": \"{\\n  \\\"subject\\\": \\\"RIVERTON Industries
+      - Revolutionizing the Aluminum Casting Industry for E-Bikes\\\",\\n  \\\"body\\\":
+      \\\"Dear [Recipient],\\\\n\\\\nI am excited to share with you the press release
+      article about RIVERTON Industries, a leading manufacturer and exporter of aluminum
+      casting products for E-Bikes. Established in 2022, RIVERTON Industries has quickly
+      gained a reputation for its innovative approach to aluminum frame manufacturing.\\\\n\\\\nRIVERTON
+      Industries offers one-stop solutions for customized bike frames, which include
+      designing, manufacturing, and assembly services. Our commitment to providing
+      innovative aluminum frames built for bicycles and modular features for multiple
+      modeling combinations sets us apart from the competition.\\\\n\\\\nOur main
+      product, the Aluminum frame for E-bike, is available in three models - 001,
+      002, and 003, but more can be customized according to customers' requirements.
+      The one-piece-formed bike frame provides increased rigidity, improving the stability
+      and safety of the ride. The solid frame made of aluminum pipeline built-in supports
+      complex designs for electric bikes.\\\\n\\\\nAs a popular choice among customers,
+      we offer a range of products, including the Electric bike frame, Aluminum motor
+      frames for E-bikes, Motor frames for E-bikes, and Customized Motor frames for
+      E-bikes. Our one-stop solution for customized bike frames ensures customer satisfaction
+      and specialized services tailored to their requirements.\\\\n\\\\nRIVERTON Industries
+      exports its products to Europe and the USA, with a reputation for producing
+      high-quality aluminum frames that meet international standards. If you're looking
+      for high-quality aluminum frames for your E-bikes, I invite you to visit our
+      website at https://riverton.example.com/.\\\\n\\\\nThank you,\\\\n[Your Name]\\\\nRIVERTON
+      Industries\\\"\\n}\"\n            }\n          }\n        ]\n      },\n      \"logprobs\":
+      null,\n      \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
+      480,\n    \"completion_tokens\": 364,\n    \"total_tokens\": 844\n  },\n  \"system_fingerprint\":
       null\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 837ddfaad9bb4a82-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
+      - 88315aa78c9fa9b3-TPE
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Tue, 19 Dec 2023 07:18:53 GMT
+      - Mon, 13 May 2024 08:42:20 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=dEoCNQG1FBUqJd4j2Gcwt8gPVx3LmcdtPVHz3ULkDek-1702970333-1-AbzdNlq/v1lxXerenXTT2A05ckyMV6oSyS2ullPHc8ML/IVhVI6mH044fvC7n41stqrwHOKn3bxReLHz6SrHL2g=;
-        path=/; expires=Tue, 19-Dec-23 07:48:53 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=zU9NO7lokl0LyLi0ZsKDlGl_umdtE37OAnFJ_DvmEDY-1715589740-1.0.1.1-DyciOvPjZjEHPp0pdrJUup2_VOfzbv8qJI.l_LkxaeUocuuu7awdLGDSJLP_Pab0IDwWHnm5cy56n5.i3oagUA;
+        path=/; expires=Mon, 13-May-24 09:12:20 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=L0AYlaUsv2UoqT9b4NJ263.QvWqNahFAA5MOywxKXNU-1702970333051-0-604800000;
+      - _cfuvid=R5_G.w7HIXujwzILJ3g.LsjK5nWYUDubVIYSrZYVRE0-1715589740162-0.0.1.1-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
       Transfer-Encoding:
       - chunked
-      access-control-allow-origin:
-      - '*'
       alt-svc:
       - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
       openai-processing-ms:
-      - '3784'
+      - '4091'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
-      - '10000'
+      - '5000'
       x-ratelimit-limit-tokens:
-      - '2000000'
-      x-ratelimit-limit-tokens_usage_based:
-      - '2000000'
+      - '160000'
       x-ratelimit-remaining-requests:
-      - '9999'
+      - '4999'
       x-ratelimit-remaining-tokens:
-      - '1999969'
-      x-ratelimit-remaining-tokens_usage_based:
-      - '1999969'
+      - '159435'
       x-ratelimit-reset-requests:
-      - 6ms
+      - 12ms
       x-ratelimit-reset-tokens:
-      - 0s
-      x-ratelimit-reset-tokens_usage_based:
-      - 0s
+      - 211ms
       x-request-id:
-      - 3b534e65bee32ebf5c080270bfc7e2b4
+      - req_f78ef753b66c08c74627805222db5b95
     http_version: HTTP/1.1
     status_code: 200
 version: 1
```

### Comparing `gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete.yaml` & `gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[OpenAI API].yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,195 +1,102 @@
 interactions:
 - request:
     body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
-      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
-      0.0, "user": "", "stop": null, "max_tokens": 1}'
-    headers:
-      accept:
-      - application/json
-      accept-encoding:
-      - gzip, deflate
-      connection:
-      - keep-alive
-      content-Length:
-      - '283'
-      content-Type:
-      - application/json
-      host:
-      - api.openai.com
-      user-agent:
-      - OpenAI/Python 1.5.0
-      x-stainless-arch:
-      - x64
-      x-stainless-async:
-      - 'false'
-      x-stainless-lang:
-      - python
-      x-stainless-os:
-      - MacOS
-      x-stainless-package-version:
-      - 1.5.0
-      x-stainless-runtime:
-      - CPython
-      x-stainless-runtime-version:
-      - 3.10.13
-    method: POST
-    uri: https://api.openai.com/v1/chat/completions
-  response:
-    content: "{\n  \"id\": \"chatcmpl-7i3UPS1ZGAuO30Rqrcp4oI1Tuomtv\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1690734201,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
-      \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": \"Hello\"\n      },\n      \"finish_reason\":
-      \"length\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\": 23,\n    \"completion_tokens\":
-      1,\n    \"total_tokens\": 24\n  }\n}\n"
-    headers:
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-RAY:
-      - 7eeef2139b4a4aa8-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - gzip
-      Content-Type:
-      - application/json
-      Date:
-      - Sun, 30 Jul 2023 16:23:21 GMT
-      Server:
-      - cloudflare
-      Transfer-Encoding:
-      - chunked
-      access-control-allow-origin:
-      - '*'
-      alt-svc:
-      - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
-      openai-processing-ms:
-      - '169'
-      openai-version:
-      - '2020-10-01'
-      strict-transport-security:
-      - max-age=15724800; includeSubDomains
-      x-ratelimit-limit-requests:
-      - '3500'
-      x-ratelimit-limit-tokens:
-      - '90000'
-      x-ratelimit-remaining-requests:
-      - '3499'
-      x-ratelimit-remaining-tokens:
-      - '89985'
-      x-ratelimit-reset-requests:
-      - 17ms
-      x-ratelimit-reset-tokens:
-      - 10ms
-      x-request-id:
-      - 037f3b4947d1950cc4b89c9c77cffbb8
-    http_version: HTTP/1.1
-    status_code: 200
-- request:
-    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "Hello, who are you?"}], "model": "gpt-3.5-turbo",
-      "frequency_penalty": 0.0, "max_tokens": 1, "presence_penalty": 0.0, "stop":
-      null, "temperature": 1.0, "top_p": 1.0, "user": ""}'
+      {"role": "user", "content": "I want to book a flight to London."}], "model":
+      "gpt-3.5-turbo-0613", "frequency_penalty": 0.0, "presence_penalty": 0.0, "stop":
+      null, "temperature": 1.0, "tool_choice": "auto", "tools": [{"type": "function",
+      "function": {"name": "book_a_flight", "description": "", "parameters": {"type":
+      "object", "required": ["date", "destination"], "properties": {"date": {"title":
+      "Date", "type": "string"}, "destination": {"title": "Destination", "type": "string"},
+      "origin": {"title": "Origin", "default": "London", "type": "string"}}, "definitions":
+      {}}}}], "top_p": 1.0, "user": ""}'
     headers:
       accept:
       - application/json
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '283'
+      - '680'
       content-type:
       - application/json
       host:
       - api.openai.com
       user-agent:
-      - OpenAI/Python 1.5.0
+      - AsyncOpenAI/Python 1.9.0
       x-stainless-arch:
       - x64
       x-stainless-async:
-      - 'false'
+      - async:asyncio
       x-stainless-lang:
       - python
       x-stainless-os:
-      - MacOS
+      - Linux
       x-stainless-package-version:
-      - 1.5.0
+      - 1.9.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
-      - 3.10.13
+      - 3.10.14
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"id\": \"chatcmpl-8XOfRJC0Fitnq1uqkhdhEYCECFt0T\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1702970337,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+    content: "{\n  \"id\": \"chatcmpl-9OLVdy1xJELLwz3d9ZSu14PKxOYDC\",\n  \"object\":
+      \"chat.completion\",\n  \"created\": 1715589581,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
       \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": \"Hello\"\n      },\n      \"logprobs\":
-      null,\n      \"finish_reason\": \"length\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
-      23,\n    \"completion_tokens\": 1,\n    \"total_tokens\": 24\n  },\n  \"system_fingerprint\":
-      null\n}\n"
+      \"assistant\",\n        \"content\": null,\n        \"tool_calls\": [\n          {\n
+      \           \"id\": \"call_4r8te63zGEJuhMXAZj02TGES\",\n            \"type\":
+      \"function\",\n            \"function\": {\n              \"name\": \"book_a_flight\",\n
+      \             \"arguments\": \"{\\n  \\\"date\\\": \\\"2022-10-15\\\",\\n  \\\"destination\\\":
+      \\\"London\\\"\\n}\"\n            }\n          }\n        ]\n      },\n      \"logprobs\":
+      null,\n      \"finish_reason\": \"tool_calls\"\n    }\n  ],\n  \"usage\": {\n
+      \   \"prompt_tokens\": 67,\n    \"completion_tokens\": 28,\n    \"total_tokens\":
+      95\n  },\n  \"system_fingerprint\": null\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 837ddfdfd8566a84-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
+      - 883156e48c8b8457-TPE
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Tue, 19 Dec 2023 07:18:57 GMT
+      - Mon, 13 May 2024 08:39:42 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=z7hMYGBZQIm78RjNCZxyI8c.BS6z.EhSVQWW3qBJrMk-1702970337-1-Ad9T5uuU2WnygqHw3AlANmj2V7LCyq4YpO6I8kxKt6PdUtkhTwonSn6IkWC3hAJIvJ36Lnqye1FrFZuNKzJHm3E=;
-        path=/; expires=Tue, 19-Dec-23 07:48:57 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=.toBW_15ERhoqEBFfJIhhHezNZllnk3_4R5OFF48zxY-1715589582-1.0.1.1-MOc4iRvZthWu5zEUj1TVBK92frVKJum6C1OiBEhFOV8qh1ozvwdOfvujedG0rEBtNgrjkPzptH.mA4y_V5POaA;
+        path=/; expires=Mon, 13-May-24 09:09:42 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=1kA49xg..7.F0WPfpp3Gz7RbuK03qIXoVvXszOfK6Hg-1702970337868-0-604800000;
+      - _cfuvid=KWNzai3G3PqQJJCi.11YdP_75_p86Ka6x3qd8rCcOHk-1715589582799-0.0.1.1-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
       Transfer-Encoding:
       - chunked
-      access-control-allow-origin:
-      - '*'
       alt-svc:
       - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
       openai-processing-ms:
-      - '119'
+      - '814'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
-      - '10000'
+      - '5000'
       x-ratelimit-limit-tokens:
-      - '2000000'
-      x-ratelimit-limit-tokens_usage_based:
-      - '2000000'
+      - '160000'
       x-ratelimit-remaining-requests:
-      - '9999'
+      - '4999'
       x-ratelimit-remaining-tokens:
-      - '1999985'
-      x-ratelimit-remaining-tokens_usage_based:
-      - '1999985'
+      - '159966'
       x-ratelimit-reset-requests:
-      - 6ms
+      - 12ms
       x-ratelimit-reset-tokens:
-      - 0s
-      x-ratelimit-reset-tokens_usage_based:
-      - 0s
+      - 12ms
       x-request-id:
-      - 0777330f20831d0baae989d0e0f52fc9
+      - req_66830bf22e53daf92e43254663035e6e
     http_version: HTTP/1.1
     status_code: 200
 version: 1
```

### Comparing `gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens.yaml` & `gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[Azure 2023-12-01 API].yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,87 @@
 interactions:
 - request:
     body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "I want to book a restaurant in London."}], "model":
-      "gpt-3.5-turbo-0613", "frequency_penalty": 0.0, "function_call": "auto", "functions":
-      [{"name": "book_a_flight", "description": "", "parameters": {"type": "object",
-      "required": ["date", "destination"], "properties": {"date": {"title": "Date",
-      "type": "string"}, "destination": {"title": "Destination", "type": "string"},
-      "origin": {"title": "Origin", "default": "London", "type": "string"}}, "definitions":
-      {}}}], "max_tokens": 10, "presence_penalty": 0.0, "stop": null, "temperature":
-      1.0, "top_p": 1.0, "user": ""}'
+      {"role": "user", "content": "Give me a sample email."}], "model": "gpt35", "frequency_penalty":
+      0.0, "presence_penalty": 0.0, "temperature": 1.0, "tool_choice": {"type": "function",
+      "function": {"name": "structural_response"}}, "tools": [{"type": "function",
+      "function": {"name": "structural_response", "description": "Response to user
+      in a structural way.", "parameters": {"title": "Email", "type": "object", "properties":
+      {"subject": {"title": "Subject", "description": "the subject of email", "type":
+      "string"}, "body": {"title": "Body", "description": "the body of email", "type":
+      "string"}}, "required": ["subject", "body"]}}}], "top_p": 1.0, "user": ""}'
     headers:
       accept:
       - application/json
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '674'
+      - '736'
       content-type:
       - application/json
       host:
-      - api.openai.com
+      - gstudio.openai.azure.com
       user-agent:
-      - OpenAI/Python 1.5.0
+      - AsyncAzureOpenAI/Python 1.9.0
       x-stainless-arch:
       - x64
       x-stainless-async:
-      - 'false'
+      - async:asyncio
       x-stainless-lang:
       - python
       x-stainless-os:
-      - MacOS
+      - Linux
       x-stainless-package-version:
-      - 1.5.0
+      - 1.9.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
-      - 3.10.13
+      - 3.10.14
     method: POST
-    uri: https://api.openai.com/v1/chat/completions
+    uri: https://gstudio.openai.azure.com/openai/deployments/gpt35/chat/completions?api-version=2023-12-01-preview
   response:
-    content: "{\n  \"id\": \"chatcmpl-8XfomRHXE6SaDIUZyAJLJK1mUPIXb\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1703036264,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
-      \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": \"Sure, I can help you with that.\"\n      },\n
-      \     \"logprobs\": null,\n      \"finish_reason\": \"length\"\n    }\n  ],\n
-      \ \"usage\": {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 10,\n
-      \   \"total_tokens\": 77\n  },\n  \"system_fingerprint\": null\n}\n"
+    content: '{"choices":[{"content_filter_results":{},"finish_reason":"stop","index":0,"message":{"content":null,"role":"assistant","tool_calls":[{"function":{"arguments":"{\n  \"subject\":
+      \"Sample Email\",\n  \"body\": \"Dear [Recipient],\\n\\nI hope this email finds
+      you well. I am writing to inform you about [subject]. [Include any necessary
+      details or information].\\n\\n[If applicable, provide any additional information
+      or updates].\\n\\n[Conclude the email with a closing remark].\\n\\nThank you
+      for your attention to this matter.\\n\\nSincerely,\\n[Your Name]\"\n}","name":"structural_response"},"id":"call_PVpfCnQC4YXcbAKeZQ5xt2AW","type":"function"}]}}],"created":1715589606,"id":"chatcmpl-9OLW2wW15damM1MaAei60TpCEn75w","model":"gpt-35-turbo-16k","object":"chat.completion","prompt_filter_results":[{"prompt_index":0,"content_filter_results":{"hate":{"filtered":false,"severity":"safe"},"self_harm":{"filtered":false,"severity":"safe"},"sexual":{"filtered":false,"severity":"safe"},"violence":{"filtered":false,"severity":"safe"}}}],"system_fingerprint":null,"usage":{"completion_tokens":97,"prompt_tokens":82,"total_tokens":179}}
+
+      '
     headers:
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-RAY:
-      - 8384296da9d34a88-TPE
       Cache-Control:
       - no-cache, must-revalidate
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - gzip
+      Content-Length:
+      - '1131'
       Content-Type:
       - application/json
       Date:
-      - Wed, 20 Dec 2023 01:37:45 GMT
-      Server:
-      - cloudflare
-      Set-Cookie:
-      - __cf_bm=N1oG2Ix80V74IifmonIBtAVTnFQUsO25es4E4BR05uY-1703036265-1-AaVLigqdP5WRrglNqb05//Dse0jHLDx88jQ85dBCcyXWsu7N4TIKisO0jGGv5bd6U7XWjXCGyGkZHGuk/OxSi8Y=;
-        path=/; expires=Wed, 20-Dec-23 02:07:45 GMT; domain=.api.openai.com; HttpOnly;
-        Secure; SameSite=None
-      - _cfuvid=HdIWpL1f8Y5452edzEenmjvWnAaDw1ytpboQ5qvYGIs-1703036265340-0-604800000;
-        path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
-      Transfer-Encoding:
-      - chunked
+      - Mon, 13 May 2024 08:40:06 GMT
+      Strict-Transport-Security:
+      - max-age=31536000; includeSubDomains; preload
       access-control-allow-origin:
       - '*'
-      alt-svc:
-      - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
-      openai-processing-ms:
-      - '278'
-      openai-version:
-      - '2020-10-01'
-      strict-transport-security:
-      - max-age=15724800; includeSubDomains
-      x-ratelimit-limit-requests:
-      - '10000'
-      x-ratelimit-limit-tokens:
-      - '2000000'
-      x-ratelimit-limit-tokens_usage_based:
-      - '2000000'
+      apim-request-id:
+      - d49908f8-18fe-4447-b1d0-18cbd79230fc
+      azureml-model-session:
+      - turbo-0613-7bacf2d7
+      x-accel-buffering:
+      - 'no'
+      x-content-type-options:
+      - nosniff
+      x-ms-client-request-id:
+      - d49908f8-18fe-4447-b1d0-18cbd79230fc
+      x-ms-rai-invoked:
+      - 'true'
+      x-ms-region:
+      - East US
       x-ratelimit-remaining-requests:
-      - '9999'
+      - '237'
       x-ratelimit-remaining-tokens:
-      - '1999971'
-      x-ratelimit-remaining-tokens_usage_based:
-      - '1999971'
-      x-ratelimit-reset-requests:
-      - 6ms
-      x-ratelimit-reset-tokens:
-      - 0s
-      x-ratelimit-reset-tokens_usage_based:
-      - 0s
+      - '239820'
       x-request-id:
-      - 7993d0ee1875a21aa251b457cc55e15f
+      - 328d659c-62d9-484e-9422-9dee664c3397
     http_version: HTTP/1.1
     status_code: 200
 version: 1
```

### Comparing `gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function.yaml` & `gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[OpenAI API].yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,98 @@
 interactions:
 - request:
     body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
       {"role": "user", "content": "I want to book a restaurant in London."}], "model":
-      "gpt-3.5-turbo-0613", "frequency_penalty": 0.0, "function_call": "auto", "functions":
-      [{"name": "book_a_flight", "description": "", "parameters": {"type": "object",
-      "required": ["date", "destination"], "properties": {"date": {"title": "Date",
-      "type": "string"}, "destination": {"title": "Destination", "type": "string"},
-      "origin": {"title": "Origin", "default": "London", "type": "string"}}, "definitions":
-      {}}}], "presence_penalty": 0.0, "stop": null, "temperature": 1.0, "top_p": 1.0,
-      "user": ""}'
+      "gpt-3.5-turbo-0613", "frequency_penalty": 0.0, "max_tokens": 10, "presence_penalty":
+      0.0, "stop": null, "temperature": 1.0, "tool_choice": "auto", "tools": [{"type":
+      "function", "function": {"name": "book_a_flight", "description": "", "parameters":
+      {"type": "object", "required": ["date", "destination"], "properties": {"date":
+      {"title": "Date", "type": "string"}, "destination": {"title": "Destination",
+      "type": "string"}, "origin": {"title": "Origin", "default": "London", "type":
+      "string"}}, "definitions": {}}}}], "top_p": 1.0, "user": ""}'
     headers:
       accept:
       - application/json
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '656'
+      - '702'
       content-type:
       - application/json
       host:
       - api.openai.com
       user-agent:
-      - OpenAI/Python 1.5.0
+      - OpenAI/Python 1.9.0
       x-stainless-arch:
       - x64
       x-stainless-async:
       - 'false'
       x-stainless-lang:
       - python
       x-stainless-os:
-      - MacOS
+      - Linux
       x-stainless-package-version:
-      - 1.5.0
+      - 1.9.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
-      - 3.10.13
+      - 3.10.14
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"id\": \"chatcmpl-8Xfon9uU1deOBwaKolkBf7HCcRtUB\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1703036265,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+    content: "{\n  \"id\": \"chatcmpl-9OLViu28fBlRMyilK38VtiN5TqfUt\",\n  \"object\":
+      \"chat.completion\",\n  \"created\": 1715589586,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
       \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": \"Sure, I can help you with that. Could
-      you please provide me with the date and time for the booking?\"\n      },\n
-      \     \"logprobs\": null,\n      \"finish_reason\": \"stop\"\n    }\n  ],\n
-      \ \"usage\": {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 24,\n
-      \   \"total_tokens\": 91\n  },\n  \"system_fingerprint\": null\n}\n"
+      \"assistant\",\n        \"content\": \"Sure, I can help you with that.\"\n      },\n
+      \     \"logprobs\": null,\n      \"finish_reason\": \"length\"\n    }\n  ],\n
+      \ \"usage\": {\n    \"prompt_tokens\": 67,\n    \"completion_tokens\": 10,\n
+      \   \"total_tokens\": 77\n  },\n  \"system_fingerprint\": null\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 83842972ea046b68-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
+      - 883156fe694ca9af-TPE
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Wed, 20 Dec 2023 01:37:46 GMT
+      - Mon, 13 May 2024 08:39:46 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=VSoYO06G7ESNk0Q_cBL7IUMAATlAASCN1l7zIHNV_Dg-1703036266-1-AdrKBREK8y/+F8cXOXDfb0CohWaVEWujxpuY2AXdNSAkHkL2zd8xhFWrPJpG2MUfRdlsQNFL6PRuhsew4xpyRQs=;
-        path=/; expires=Wed, 20-Dec-23 02:07:46 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=Wl2pL2vYe5_JGbuzLGKFrQSDCzb.PsmqInwq4OGAPkk-1715589586-1.0.1.1-Ar5no0FB8rzlFsEzwn1KPoVlLnDYCpERdfLnr4zRmuiarow2YDK_WA8MojKjYl0DsithQMSTka8p91TZI6Ghgw;
+        path=/; expires=Mon, 13-May-24 09:09:46 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=3DRXTn4srkqSOV1M1lEj_7ZPbKBR1T68GAOTJZL6OWk-1703036266549-0-604800000;
+      - _cfuvid=AJVXOVJ1S29WBvw62dA5pCVGpsZjI9tU6o1Mc3x0Hc4-1715589586600-0.0.1.1-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
       Transfer-Encoding:
       - chunked
-      access-control-allow-origin:
-      - '*'
       alt-svc:
       - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
       openai-processing-ms:
-      - '642'
+      - '524'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
-      - '10000'
+      - '5000'
       x-ratelimit-limit-tokens:
-      - '2000000'
-      x-ratelimit-limit-tokens_usage_based:
-      - '2000000'
+      - '160000'
       x-ratelimit-remaining-requests:
-      - '9999'
+      - '4999'
       x-ratelimit-remaining-tokens:
-      - '1999964'
-      x-ratelimit-remaining-tokens_usage_based:
-      - '1999964'
+      - '159971'
       x-ratelimit-reset-requests:
-      - 6ms
+      - 12ms
       x-ratelimit-reset-tokens:
-      - 1ms
-      x-ratelimit-reset-tokens_usage_based:
-      - 1ms
+      - 10ms
       x-request-id:
-      - 56cfe8779b30c143f89ca5092a57756e
+      - req_5ac5e0ed507576e947973e22e9b3bbcb
     http_version: HTTP/1.1
     status_code: 200
 version: 1
```

### Comparing `gpt_fn-0.1.2/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens.yaml` & `gpt_fn-0.1.3/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[OpenAI API].yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,200 +1,112 @@
 interactions:
 - request:
     body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
       {"role": "user", "content": "Give me a sample email."}], "model": "gpt-3.5-turbo-0613",
-      "temperature": 1.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty":
-      0.0, "user": "", "functions": [{"name": "structural_response", "description":
+      "frequency_penalty": 0.0, "presence_penalty": 0.0, "temperature": 1.0, "tool_choice":
+      {"type": "function", "function": {"name": "structural_response"}}, "tools":
+      [{"type": "function", "function": {"name": "structural_response", "description":
       "Response to user in a structural way.", "parameters": {"title": "Email", "type":
       "object", "properties": {"subject": {"title": "Subject", "description": "the
       subject of email", "type": "string"}, "body": {"title": "Body", "description":
-      "the body of email", "type": "string"}}, "required": ["subject", "body"]}}],
-      "function_call": {"name": "structural_response"}, "max_tokens": 10}'
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      Content-Length:
-      - '705'
-      Content-Type:
-      - application/json
-      User-Agent:
-      - OpenAI/v1 PythonBindings/0.27.8
-      X-OpenAI-Client-User-Agent:
-      - '{"bindings_version": "0.27.8", "httplib": "requests", "lang": "python", "lang_version":
-        "3.11.4", "platform": "macOS-13.4.1-arm64-arm-64bit", "publisher": "openai",
-        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Thu Jun  8 22:22:19
-        PDT 2023; root:xnu-8796.121.3~7/RELEASE_ARM64_T8103 arm64 arm"}'
-    method: POST
-    uri: https://api.openai.com/v1/chat/completions
-  response:
-    body:
-      string: "{\n  \"id\": \"chatcmpl-7i3UKvREvsnQqPtjETLD4eXfCl4M4\",\n  \"object\":
-        \"chat.completion\",\n  \"created\": 1690734196,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
-        \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-        \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n
-        \         \"name\": \"structural_response\",\n          \"arguments\": \"{\\n
-        \ \\\"subject\\\": \\\"Invitation to attend\"\n        }\n      },\n      \"finish_reason\":
-        \"length\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\": 82,\n    \"completion_tokens\":
-        10,\n    \"total_tokens\": 92\n  }\n}\n"
-    headers:
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-RAY:
-      - 7eeef1e85e066a87-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - gzip
-      Content-Type:
-      - application/json
-      Date:
-      - Sun, 30 Jul 2023 16:23:16 GMT
-      Server:
-      - cloudflare
-      Transfer-Encoding:
-      - chunked
-      access-control-allow-origin:
-      - '*'
-      alt-svc:
-      - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
-      openai-processing-ms:
-      - '512'
-      openai-version:
-      - '2020-10-01'
-      strict-transport-security:
-      - max-age=15724800; includeSubDomains
-      x-ratelimit-limit-requests:
-      - '3500'
-      x-ratelimit-limit-tokens:
-      - '90000'
-      x-ratelimit-remaining-requests:
-      - '3499'
-      x-ratelimit-remaining-tokens:
-      - '89974'
-      x-ratelimit-reset-requests:
-      - 17ms
-      x-ratelimit-reset-tokens:
-      - 16ms
-      x-request-id:
-      - 5f2d2cac851db7bff168741127ae5ce4
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"messages": [{"role": "system", "content": "You are a helpful assistant."},
-      {"role": "user", "content": "Give me a sample email."}], "model": "gpt-3.5-turbo-0613",
-      "frequency_penalty": 0.0, "function_call": {"name": "structural_response"},
-      "functions": [{"name": "structural_response", "description": "Response to user
-      in a structural way.", "parameters": {"title": "Email", "type": "object", "properties":
-      {"subject": {"title": "Subject", "description": "the subject of email", "type":
-      "string"}, "body": {"title": "Body", "description": "the body of email", "type":
-      "string"}}, "required": ["subject", "body"]}}], "max_tokens": 10, "presence_penalty":
-      0.0, "temperature": 1.0, "top_p": 1.0, "user": ""}'
+      "the body of email", "type": "string"}}, "required": ["subject", "body"]}}}],
+      "top_p": 1.0, "user": ""}'
     headers:
       accept:
       - application/json
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
-      - '705'
+      - '749'
       content-type:
       - application/json
       host:
       - api.openai.com
       user-agent:
-      - OpenAI/Python 1.5.0
+      - AsyncOpenAI/Python 1.9.0
       x-stainless-arch:
       - x64
       x-stainless-async:
-      - 'false'
+      - async:asyncio
       x-stainless-lang:
       - python
       x-stainless-os:
-      - MacOS
+      - Linux
       x-stainless-package-version:
-      - 1.5.0
+      - 1.9.0
       x-stainless-runtime:
       - CPython
       x-stainless-runtime-version:
-      - 3.10.13
+      - 3.10.14
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
-    content: "{\n  \"id\": \"chatcmpl-8XOfNxHhCORGJiNKFSdDrGk7Q54XN\",\n  \"object\":
-      \"chat.completion\",\n  \"created\": 1702970333,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
+    content: "{\n  \"id\": \"chatcmpl-9OLVwZnvHD6NyZpwyZ6pzekyZ6J8n\",\n  \"object\":
+      \"chat.completion\",\n  \"created\": 1715589600,\n  \"model\": \"gpt-3.5-turbo-0613\",\n
       \ \"choices\": [\n    {\n      \"index\": 0,\n      \"message\": {\n        \"role\":
-      \"assistant\",\n        \"content\": null,\n        \"function_call\": {\n          \"name\":
-      \"structural_response\",\n          \"arguments\": \"{\\n  \\\"subject\\\":
-      \\\"Sample Email\\\",\\n \"\n        }\n      },\n      \"logprobs\": null,\n
-      \     \"finish_reason\": \"length\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
-      82,\n    \"completion_tokens\": 10,\n    \"total_tokens\": 92\n  },\n  \"system_fingerprint\":
+      \"assistant\",\n        \"content\": null,\n        \"tool_calls\": [\n          {\n
+      \           \"id\": \"call_nkxgakv1vSNbIDTV3VfmoJCA\",\n            \"type\":
+      \"function\",\n            \"function\": {\n              \"name\": \"structural_response\",\n
+      \             \"arguments\": \"{\\n  \\\"subject\\\": \\\"Meeting Request\\\",\\n
+      \ \\\"body\\\": \\\"Dear [Recipient's Name],\\\\n\\\\nI hope this email finds
+      you well. I am writing to request a meeting with you to discuss [subject/topic].
+      As we continue to work on [project/initiative], it would be beneficial to have
+      your insights and input.\\\\n\\\\nI have checked your availability on the calendar
+      and suggest the following meeting options:\\\\n\\\\nOption 1:\\\\nDate: [Date]\\\\nTime:
+      [Time]\\\\nLocation: [Location]\\\\n\\\\nOption 2:\\\\nDate: [Date]\\\\nTime:
+      [Time]\\\\nLocation: [Location]\\\\n\\\\nPlease let me know which option works
+      best for you, or if you have any alternative suggestions. I look forward to
+      meeting with you and furthering our collaboration.\\\\n\\\\nBest regards,\\\\n[Your
+      Name]\\\"\\n}\"\n            }\n          }\n        ]\n      },\n      \"logprobs\":
+      null,\n      \"finish_reason\": \"stop\"\n    }\n  ],\n  \"usage\": {\n    \"prompt_tokens\":
+      82,\n    \"completion_tokens\": 178,\n    \"total_tokens\": 260\n  },\n  \"system_fingerprint\":
       null\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 837ddfc64a154a52-TPE
-      Cache-Control:
-      - no-cache, must-revalidate
+      - 8831575528f34aa8-TPE
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Tue, 19 Dec 2023 07:18:54 GMT
+      - Mon, 13 May 2024 08:40:02 GMT
       Server:
       - cloudflare
       Set-Cookie:
-      - __cf_bm=.S9lKZEtSMn5oSOFmmuPb9.S4FDFXk0PKYs6heH0Slg-1702970334-1-AWZK3n/eHh6InxOmvbFy8FxaoyXrZCyrQBM0q1dGyXLieUV3PKSqcfC2QiwRBm2RVRzu7B/9s2hKcAJFkP2bmbE=;
-        path=/; expires=Tue, 19-Dec-23 07:48:54 GMT; domain=.api.openai.com; HttpOnly;
+      - __cf_bm=Wsy2u6OAcvRmIaFo.go.vu2fcXHb2vYtMF._V7cA5Qo-1715589602-1.0.1.1-yWx0D1IlGN1pvST3iDpAFVo4iBtA1gobfrMOUxoanx7j4OlcnTZkcPhtMZCwaIrOLJhGyan6PQWm9WAGaBEsGQ;
+        path=/; expires=Mon, 13-May-24 09:10:02 GMT; domain=.api.openai.com; HttpOnly;
         Secure; SameSite=None
-      - _cfuvid=r2Lrnmh1CChvvJ5AgJqDRuY8HXgHWXufBbnYaLcVHwI-1702970334145-0-604800000;
+      - _cfuvid=mJL.efAEyNJHB5CDiARjCTDt86.iabGvd5aK6Cp6jZM-1715589602508-0.0.1.1-604800000;
         path=/; domain=.api.openai.com; HttpOnly; Secure; SameSite=None
       Transfer-Encoding:
       - chunked
-      access-control-allow-origin:
-      - '*'
       alt-svc:
       - h3=":443"; ma=86400
-      openai-model:
-      - gpt-3.5-turbo-0613
       openai-processing-ms:
-      - '481'
+      - '2110'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
-      - '10000'
+      - '5000'
       x-ratelimit-limit-tokens:
-      - '2000000'
-      x-ratelimit-limit-tokens_usage_based:
-      - '2000000'
+      - '160000'
       x-ratelimit-remaining-requests:
-      - '9999'
+      - '4999'
       x-ratelimit-remaining-tokens:
-      - '1999975'
-      x-ratelimit-remaining-tokens_usage_based:
-      - '1999975'
+      - '159969'
       x-ratelimit-reset-requests:
-      - 6ms
+      - 12ms
       x-ratelimit-reset-tokens:
-      - 0s
-      x-ratelimit-reset-tokens_usage_based:
-      - 0s
+      - 11ms
       x-request-id:
-      - 7d185641ae306c52c0d977113cb07c61
+      - req_6d0947a8176656b6383912c8beb7e977
     http_version: HTTP/1.1
     status_code: 200
 version: 1
```

### Comparing `gpt_fn-0.1.2/src/gpt_fn/tests/test_ai_function.py` & `gpt_fn-0.1.3/src/gpt_fn/tests/test_ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/src/gpt_fn/tests/test_prompt.py` & `gpt_fn-0.1.3/src/gpt_fn/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/src/gpt_fn/utils/pydantic_parser.py` & `gpt_fn-0.1.3/src/gpt_fn/utils/pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/src/gpt_fn/utils/signature.py` & `gpt_fn-0.1.3/src/gpt_fn/utils/signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/src/gpt_fn/utils/tests/__snapshots__/test_json_decode.ambr` & `gpt_fn-0.1.3/src/gpt_fn/utils/tests/__snapshots__/test_json_decode.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr` & `gpt_fn-0.1.3/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   ```
   '''
 # ---
 # name: test_pydantic_parser_parse
   Email(subject='Revolutionizing the E-Bike Industry with Innovative Aluminum Frames', body='Dear valued client,\n\nWe are excited to share with you the latest news from JIN-JI International Co., Ltd. We have revolutionized the E-Bike industry with our innovative aluminum frames for SPACIOUS Industrial Co., Ltd. in Taiwan. Our commitment to innovation and customer satisfaction has positioned us as a key player in the market.\n\nCEO Xiao Ming, Chen, emphasizes, "We provide the best quality products," reflecting our dedication to excellence.\n\nTo learn more about our revolutionary aluminum frames and how they offer increased rigidity, stability, and safety for riders, we invite you to visit our website at https://jinji.en.taiwantrade.com/. We believe that our innovative designs will support complex structures for electric bikes, ensuring a confident and secure riding experience.\n\nThank you for your continued support, and we look forward to bringing you more groundbreaking developments in the future.\n\nBest regards,\n[Your Name]\nJIN-JI International Co., Ltd.')
 # ---
 # name: test_pydantic_parser_with_prompt[email.txt-Email][gpt response]
-  Email(subject='Press Release: RIVERTON Industries - Revolutionizing the Aluminum Casting Industry for E-Bikes', body='Dear [Recipient],\n\nWe are pleased to announce that RIVERTON Industries is revolutionizing the aluminum casting industry for E-Bikes. Our innovative approach to manufacturing aluminum frames and one-stop solutions for customized bike frames has made us a popular choice among customers.\n\nAbout RIVERTON Industries:\nRIVERTON Industries is an innovative international company specializing in aluminum casting products for E-Bikes. We offer one-stop solutions for customized bike frames, which include designing, manufacturing, and assembly services. Our commitment to quality has earned us a reputation for producing high-quality aluminum frames that meet international standards.\n\nKey Products:\n- Aluminum frame for E-bike: Available in three models - 001, 002, and 003, but more can be customized. The one-piece-formed bike frame provides increased rigidity, improving the stability and safety of the ride.\n- Electric bike frame\n- Aluminum motor frames for E-bikes\n- Motor frames for E-bikes\n- Customized Motor frames for E-bikes\n\nExport Market:\nRIVERTON Industries exports its products to Europe and the USA.\n\nFor more information or to inquire about our products, please visit our website at [Website URL].\n\nThank you for your attention.\n\nSincerely,\n[Your Name]\n[Your Title]\nRIVERTON Industries')
+  Email(subject='RIVERTON Industries - Revolutionizing the Aluminum Casting Industry for E-Bikes', body="Dear [Recipient],\n\nI am excited to share with you the press release article about RIVERTON Industries, a leading manufacturer and exporter of aluminum casting products for E-Bikes. Established in 2022, RIVERTON Industries has quickly gained a reputation for its innovative approach to aluminum frame manufacturing.\n\nRIVERTON Industries offers one-stop solutions for customized bike frames, which include designing, manufacturing, and assembly services. Our commitment to providing innovative aluminum frames built for bicycles and modular features for multiple modeling combinations sets us apart from the competition.\n\nOur main product, the Aluminum frame for E-bike, is available in three models - 001, 002, and 003, but more can be customized according to customers' requirements. The one-piece-formed bike frame provides increased rigidity, improving the stability and safety of the ride. The solid frame made of aluminum pipeline built-in supports complex designs for electric bikes.\n\nAs a popular choice among customers, we offer a range of products, including the Electric bike frame, Aluminum motor frames for E-bikes, Motor frames for E-bikes, and Customized Motor frames for E-bikes. Our one-stop solution for customized bike frames ensures customer satisfaction and specialized services tailored to their requirements.\n\nRIVERTON Industries exports its products to Europe and the USA, with a reputation for producing high-quality aluminum frames that meet international standards. If you're looking for high-quality aluminum frames for your E-bikes, I invite you to visit our website at https://riverton.example.com/.\n\nThank you,\n[Your Name]\nRIVERTON Industries")
 # ---
 # name: test_pydantic_parser_with_prompt[email.txt-Email][instructoin]
   '''
   Given the press release article of our company: "RIVERTON Industries - Revolutionizing the Aluminum Casting Industry for E-Bikes
   
   RIVERTON Industries is a leading manufacturer and exporter of aluminum casting products for E-Bikes. Established in 2022, the company has quickly gained a reputation for its innovative approach to aluminum frame manufacturing. We offer one-stop solutions for customized bike frames, which include designing, manufacturing, and assembly services.
```

### Comparing `gpt_fn-0.1.2/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr` & `gpt_fn-0.1.3/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt` & `gpt_fn-0.1.3/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/src/gpt_fn/utils/tests/test_pydantic_parser.py` & `gpt_fn-0.1.3/src/gpt_fn/utils/tests/test_pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/src/gpt_fn/utils/tests/test_signature.py` & `gpt_fn-0.1.3/src/gpt_fn/utils/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.2/PKG-INFO` & `gpt_fn-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-fn
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

