# Comparing `tmp/langchain_mistralai-0.1.6.tar.gz` & `tmp/langchain_mistralai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_mistralai-0.1.6.tar", max compression
+gzip compressed data, was "langchain_mistralai-0.1.7.tar", max compression
```

## Comparing `langchain_mistralai-0.1.6.tar` & `langchain_mistralai-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-05-02 18:13:03.707168 langchain_mistralai-0.1.6/LICENSE
--rw-r--r--   0        0        0     1336 2024-05-02 18:13:03.707168 langchain_mistralai-0.1.6/README.md
--rw-r--r--   0        0        0      173 2024-05-02 18:13:03.707168 langchain_mistralai-0.1.6/langchain_mistralai/__init__.py
--rw-r--r--   0        0        0    29734 2024-05-02 18:13:03.711168 langchain_mistralai-0.1.6/langchain_mistralai/chat_models.py
--rw-r--r--   0        0        0     7310 2024-05-02 18:13:03.711168 langchain_mistralai-0.1.6/langchain_mistralai/embeddings.py
--rw-r--r--   0        0        0        0 2024-05-02 18:13:03.711168 langchain_mistralai-0.1.6/langchain_mistralai/py.typed
--rw-r--r--   0        0        0     2391 2024-05-02 18:13:03.711168 langchain_mistralai-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-15 21:30:11.773748 langchain_mistralai-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1336 2024-05-15 21:30:11.773748 langchain_mistralai-0.1.7/README.md
+-rw-r--r--   0        0        0      173 2024-05-15 21:30:11.773748 langchain_mistralai-0.1.7/langchain_mistralai/__init__.py
+-rw-r--r--   0        0        0    29734 2024-05-15 21:30:11.773748 langchain_mistralai-0.1.7/langchain_mistralai/chat_models.py
+-rw-r--r--   0        0        0     7310 2024-05-15 21:30:11.773748 langchain_mistralai-0.1.7/langchain_mistralai/embeddings.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:30:11.773748 langchain_mistralai-0.1.7/langchain_mistralai/py.typed
+-rw-r--r--   0        0        0     2401 2024-05-15 21:30:11.773748 langchain_mistralai-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.7/PKG-INFO
```

### Comparing `langchain_mistralai-0.1.6/LICENSE` & `langchain_mistralai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.6/README.md` & `langchain_mistralai-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.6/langchain_mistralai/chat_models.py` & `langchain_mistralai-0.1.7/langchain_mistralai/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.6/langchain_mistralai/embeddings.py` & `langchain_mistralai-0.1.7/langchain_mistralai/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.6/pyproject.toml` & `langchain_mistralai-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-mistralai"
-version = "0.1.6"
+version = "0.1.7"
 description = "An integration package connecting Mistral and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/mistralai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.46"
-tokenizers = "^0.15.1"
+langchain-core = ">=0.1.46,<0.3"
+tokenizers = ">=0.15.1,<1"
 httpx = ">=0.25.2,<1"
 httpx-sse = ">=0.3.1,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `langchain_mistralai-0.1.6/PKG-INFO` & `langchain_mistralai-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: langchain-mistralai
-Version: 0.1.6
+Version: 0.1.7
 Summary: An integration package connecting Mistral and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.25.2,<1)
 Requires-Dist: httpx-sse (>=0.3.1,<1)
-Requires-Dist: langchain-core (>=0.1.46,<0.2.0)
-Requires-Dist: tokenizers (>=0.15.1,<0.16.0)
+Requires-Dist: langchain-core (>=0.1.46,<0.3)
+Requires-Dist: tokenizers (>=0.15.1,<1)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/mistralai
 Description-Content-Type: text/markdown
 
 # langchain-mistralai
 
 This package contains the LangChain integrations for [MistralAI](https://docs.mistral.ai) through their [mistralai](https://pypi.org/project/mistralai/) SDK.
```

