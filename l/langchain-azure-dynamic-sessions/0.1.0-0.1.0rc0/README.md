# Comparing `tmp/langchain_azure_dynamic_sessions-0.1.0.tar.gz` & `tmp/langchain_azure_dynamic_sessions-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_azure_dynamic_sessions-0.1.0.tar", max compression
+gzip compressed data, was "langchain_azure_dynamic_sessions-0.1.0rc0.tar", max compression
```

## Comparing `langchain_azure_dynamic_sessions-0.1.0.tar` & `langchain_azure_dynamic_sessions-0.1.0rc0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-05-15 21:29:37.063376 langchain_azure_dynamic_sessions-0.1.0/LICENSE
--rw-r--r--   0        0        0     1295 2024-05-15 21:29:37.063376 langchain_azure_dynamic_sessions-0.1.0/README.md
--rw-r--r--   0        0        0      128 2024-05-15 21:29:37.063376 langchain_azure_dynamic_sessions-0.1.0/langchain_azure_dynamic_sessions/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 21:29:37.063376 langchain_azure_dynamic_sessions-0.1.0/langchain_azure_dynamic_sessions/py.typed
--rw-r--r--   0        0        0      128 2024-05-15 21:29:37.063376 langchain_azure_dynamic_sessions-0.1.0/langchain_azure_dynamic_sessions/tools/__init__.py
--rw-r--r--   0        0        0     9222 2024-05-15 21:29:37.063376 langchain_azure_dynamic_sessions-0.1.0/langchain_azure_dynamic_sessions/tools/sessions.py
--rw-r--r--   0        0        0     2819 2024-05-15 21:29:37.063376 langchain_azure_dynamic_sessions-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 langchain_azure_dynamic_sessions-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-09 21:41:23.712012 langchain_azure_dynamic_sessions-0.1.0rc0/LICENSE
+-rw-r--r--   0        0        0     1295 2024-05-09 21:41:23.712012 langchain_azure_dynamic_sessions-0.1.0rc0/README.md
+-rw-r--r--   0        0        0      128 2024-05-09 21:41:23.712012 langchain_azure_dynamic_sessions-0.1.0rc0/langchain_azure_dynamic_sessions/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 21:41:23.712012 langchain_azure_dynamic_sessions-0.1.0rc0/langchain_azure_dynamic_sessions/py.typed
+-rw-r--r--   0        0        0      128 2024-05-09 21:41:23.712012 langchain_azure_dynamic_sessions-0.1.0rc0/langchain_azure_dynamic_sessions/tools/__init__.py
+-rw-r--r--   0        0        0     9222 2024-05-09 21:41:23.712012 langchain_azure_dynamic_sessions-0.1.0rc0/langchain_azure_dynamic_sessions/tools/sessions.py
+-rw-r--r--   0        0        0     2819 2024-05-09 21:41:23.712012 langchain_azure_dynamic_sessions-0.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     2231 1970-01-01 00:00:00.000000 langchain_azure_dynamic_sessions-0.1.0rc0/PKG-INFO
```

### Comparing `langchain_azure_dynamic_sessions-0.1.0/LICENSE` & `langchain_azure_dynamic_sessions-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_azure_dynamic_sessions-0.1.0/README.md` & `langchain_azure_dynamic_sessions-0.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_azure_dynamic_sessions-0.1.0/langchain_azure_dynamic_sessions/tools/sessions.py` & `langchain_azure_dynamic_sessions-0.1.0rc0/langchain_azure_dynamic_sessions/tools/sessions.py`

 * *Files identical despite different names*

### Comparing `langchain_azure_dynamic_sessions-0.1.0/pyproject.toml` & `langchain_azure_dynamic_sessions-0.1.0rc0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "langchain-azure-dynamic-sessions"
-version = "0.1.0"
+version = "0.1.0rc0"
 description = "An integration package connecting Azure Container Apps dynamic sessions and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/azure-dynamic-sessions"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = ">=0.1.52,<0.3"
+langchain-core = "^0.1.52"
 azure-identity = "^1.16.0"
 requests = "^2.31.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
-pytest-mock = "^3.10.0"
+pytest-mock  = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
-langchain-core = { path = "../../core", develop = true }
+langchain-core = {path = "../../core", develop = true}
 python-dotenv = "^1.0.1"
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
 pytest = "^7.3.0"
@@ -48,38 +48,40 @@
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 python-dotenv = "^1.0.1"
 pytest = "^7.3.0"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
-langchain-core = { path = "../../core", develop = true }
+langchain-core = {path = "../../core", develop = true}
 types-requests = "^2.31.0.20240406"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-langchain-core = { path = "../../core", develop = true }
+langchain-core = {path = "../../core", develop = true}
 ipykernel = "^6.29.4"
-langchain-openai = { path = "../openai", develop = true }
+langchain-openai = {path = "../openai", develop = true}
 langchainhub = "^0.1.15"
 
 [tool.ruff]
 select = [
-  "E", # pycodestyle
-  "F", # pyflakes
-  "I", # isort
+  "E",  # pycodestyle
+  "F",  # pyflakes
+  "I",  # isort
 ]
 
 [tool.mypy]
 disallow_untyped_defs = "True"
 
 [tool.coverage.run]
-omit = ["tests/*"]
+omit = [
+    "tests/*",
+]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 # --strict-markers will raise errors on unknown marks.
```

### Comparing `langchain_azure_dynamic_sessions-0.1.0/PKG-INFO` & `langchain_azure_dynamic_sessions-0.1.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-azure-dynamic-sessions
-Version: 0.1.0
+Version: 0.1.0rc0
 Summary: An integration package connecting Azure Container Apps dynamic sessions and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: azure-identity (>=1.16.0,<2.0.0)
-Requires-Dist: langchain-core (>=0.1.52,<0.3)
+Requires-Dist: langchain-core (>=0.1.52,<0.2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/azure-dynamic-sessions
 Description-Content-Type: text/markdown
 
 # langchain-azure-dynamic-sessions
```

