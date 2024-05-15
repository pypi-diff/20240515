# Comparing `tmp/langchain_groq-0.1.3.tar.gz` & `tmp/langchain_groq-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_groq-0.1.3.tar", max compression
+gzip compressed data, was "langchain_groq-0.1.4.tar", max compression
```

## Comparing `langchain_groq-0.1.3.tar` & `langchain_groq-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2024-04-24 16:50:37.274592 langchain_groq-0.1.3/LICENSE
--rw-r--r--   0        0        0     1986 2024-04-24 16:50:37.274592 langchain_groq-0.1.3/README.md
--rw-r--r--   0        0        0       72 2024-04-24 16:50:37.274592 langchain_groq-0.1.3/langchain_groq/__init__.py
--rw-r--r--   0        0        0    39920 2024-04-24 16:50:37.274592 langchain_groq-0.1.3/langchain_groq/chat_models.py
--rw-r--r--   0        0        0        0 2024-04-24 16:50:37.274592 langchain_groq-0.1.3/langchain_groq/py.typed
--rw-r--r--   0        0        0     2628 2024-04-24 16:50:37.274592 langchain_groq-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2793 1970-01-01 00:00:00.000000 langchain_groq-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-15 21:29:59.140623 langchain_groq-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1986 2024-05-15 21:29:59.140623 langchain_groq-0.1.4/README.md
+-rw-r--r--   0        0        0       72 2024-05-15 21:29:59.140623 langchain_groq-0.1.4/langchain_groq/__init__.py
+-rw-r--r--   0        0        0    40250 2024-05-15 21:29:59.140623 langchain_groq-0.1.4/langchain_groq/chat_models.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:29:59.140623 langchain_groq-0.1.4/langchain_groq/py.typed
+-rw-r--r--   0        0        0     2639 2024-05-15 21:29:59.140623 langchain_groq-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 langchain_groq-0.1.4/PKG-INFO
```

### Comparing `langchain_groq-0.1.3/LICENSE` & `langchain_groq-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_groq-0.1.3/README.md` & `langchain_groq-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `langchain_groq-0.1.3/langchain_groq/chat_models.py` & `langchain_groq-0.1.4/langchain_groq/chat_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     Tuple,
     Type,
     TypedDict,
     Union,
     cast,
 )
 
-from langchain_core._api import beta
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import (
     BaseChatModel,
@@ -123,14 +122,17 @@
     """Maximum number of tokens to generate."""
     default_headers: Union[Mapping[str, str], None] = None
     default_query: Union[Mapping[str, object], None] = None
     # Configure a custom httpx client. See the
     # [httpx documentation](https://www.python-httpx.org/api/#client) for more details.
     http_client: Union[Any, None] = None
     """Optional httpx.Client."""
+    http_async_client: Union[Any, None] = None
+    """Optional httpx.AsyncClient. Only used for async invocations. Must specify
+        http_client as well if you'd like a custom client for sync invocations."""
 
     class Config:
         """Configuration for this pydantic object."""
 
         allow_population_by_field_name = True
 
     @root_validator(pre=True)
@@ -179,25 +181,28 @@
         client_params = {
             "api_key": values["groq_api_key"].get_secret_value(),
             "base_url": values["groq_api_base"],
             "timeout": values["request_timeout"],
             "max_retries": values["max_retries"],
             "default_headers": values["default_headers"],
             "default_query": values["default_query"],
-            "http_client": values["http_client"],
         }
 
         try:
             import groq
 
+            sync_specific = {"http_client": values["http_client"]}
             if not values.get("client"):
-                values["client"] = groq.Groq(**client_params).chat.completions
+                values["client"] = groq.Groq(
+                    **client_params, **sync_specific
+                ).chat.completions
             if not values.get("async_client"):
+                async_specific = {"http_client": values["http_async_client"]}
                 values["async_client"] = groq.AsyncGroq(
-                    **client_params
+                    **client_params, **async_specific
                 ).chat.completions
         except ImportError:
             raise ImportError(
                 "Could not import groq python package. "
                 "Please install it with `pip install groq`."
             )
         return values
@@ -591,15 +596,14 @@
                     "type": "function",
                     "function": {"name": tool_name},
                 }
 
             kwargs["tool_choice"] = tool_choice
         return super().bind(tools=formatted_tools, **kwargs)
 
-    @beta()
     def with_structured_output(
         self,
         schema: Optional[Union[Dict, Type[BaseModel]]] = None,
         *,
         method: Literal["function_calling", "json_mode"] = "function_calling",
         include_raw: bool = False,
         **kwargs: Any,
```

### Comparing `langchain_groq-0.1.3/pyproject.toml` & `langchain_groq-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-groq"
-version = "0.1.3"
+version = "0.1.4"
 description = "An integration package connecting Groq and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/groq"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.45"
+langchain-core = ">=0.1.45,<0.3"
 groq = ">=0.4.1,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
@@ -50,15 +50,15 @@
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
 langchain-core = { path = "../../core", develop = true }
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
   "W", # Warnings
 ]
```

### Comparing `langchain_groq-0.1.3/PKG-INFO` & `langchain_groq-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-groq
-Version: 0.1.3
+Version: 0.1.4
 Summary: An integration package connecting Groq and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: groq (>=0.4.1,<1)
-Requires-Dist: langchain-core (>=0.1.45,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.45,<0.3)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/groq
 Description-Content-Type: text/markdown
 
 # langchain-groq
 
 ## Welcome to Groq! 🚀
```

