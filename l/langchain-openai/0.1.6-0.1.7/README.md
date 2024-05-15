# Comparing `tmp/langchain_openai-0.1.6.tar.gz` & `tmp/langchain_openai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_openai-0.1.6.tar", max compression
+gzip compressed data, was "langchain_openai-0.1.7.tar", max compression
```

## Comparing `langchain_openai-0.1.6.tar` & `langchain_openai-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/LICENSE
--rw-r--r--   0        0        0     1627 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/README.md
--rw-r--r--   0        0        0      371 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/__init__.py
--rw-r--r--   0        0        0      176 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/chat_models/__init__.py
--rw-r--r--   0        0        0    10790 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/chat_models/azure.py
--rw-r--r--   0        0        0    47309 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/chat_models/base.py
--rw-r--r--   0        0        0      198 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/embeddings/__init__.py
--rw-r--r--   0        0        0     6567 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/embeddings/azure.py
--rw-r--r--   0        0        0    22520 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/embeddings/base.py
--rw-r--r--   0        0        0      146 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/llms/__init__.py
--rw-r--r--   0        0        0     8354 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/llms/azure.py
--rw-r--r--   0        0        0    24578 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/llms/base.py
--rw-r--r--   0        0        0      229 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/output_parsers/__init__.py
--rw-r--r--   0        0        0      229 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/output_parsers/tools.py
--rw-r--r--   0        0        0        0 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/langchain_openai/py.typed
--rw-r--r--   0        0        0     2835 2024-05-03 04:15:38.303901 langchain_openai-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 langchain_openai-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1627 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/README.md
+-rw-r--r--   0        0        0      371 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/chat_models/__init__.py
+-rw-r--r--   0        0        0    10790 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/chat_models/azure.py
+-rw-r--r--   0        0        0    47309 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/chat_models/base.py
+-rw-r--r--   0        0        0      198 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/embeddings/__init__.py
+-rw-r--r--   0        0        0     6567 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/embeddings/azure.py
+-rw-r--r--   0        0        0    22520 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/embeddings/base.py
+-rw-r--r--   0        0        0      146 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/llms/__init__.py
+-rw-r--r--   0        0        0     8354 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/llms/azure.py
+-rw-r--r--   0        0        0    24578 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/llms/base.py
+-rw-r--r--   0        0        0      229 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/output_parsers/__init__.py
+-rw-r--r--   0        0        0      229 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/output_parsers/tools.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/langchain_openai/py.typed
+-rw-r--r--   0        0        0     2839 2024-05-15 19:28:21.593074 langchain_openai-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2480 1970-01-01 00:00:00.000000 langchain_openai-0.1.7/PKG-INFO
```

### Comparing `langchain_openai-0.1.6/LICENSE` & `langchain_openai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.6/README.md` & `langchain_openai-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.6/langchain_openai/chat_models/azure.py` & `langchain_openai-0.1.7/langchain_openai/chat_models/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.6/langchain_openai/chat_models/base.py` & `langchain_openai-0.1.7/langchain_openai/chat_models/base.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.6/langchain_openai/embeddings/azure.py` & `langchain_openai-0.1.7/langchain_openai/embeddings/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.6/langchain_openai/embeddings/base.py` & `langchain_openai-0.1.7/langchain_openai/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.6/langchain_openai/llms/azure.py` & `langchain_openai-0.1.7/langchain_openai/llms/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.6/langchain_openai/llms/base.py` & `langchain_openai-0.1.7/langchain_openai/llms/base.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.6/pyproject.toml` & `langchain_openai-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "langchain-openai"
-version = "0.1.6"
+version = "0.1.7"
 description = "An integration package connecting OpenAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.46"
+langchain-core = ">=0.1.46,<0.3"
 openai = "^1.24.0"
-tiktoken = ">=0.5.2,<1"
+tiktoken = ">=0.7,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
```

### Comparing `langchain_openai-0.1.6/PKG-INFO` & `langchain_openai-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-openai
-Version: 0.1.6
+Version: 0.1.7
 Summary: An integration package connecting OpenAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1.46,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.46,<0.3)
 Requires-Dist: openai (>=1.24.0,<2.0.0)
-Requires-Dist: tiktoken (>=0.5.2,<1)
+Requires-Dist: tiktoken (>=0.7,<1)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai
 Description-Content-Type: text/markdown
 
 # langchain-openai
 
 This package contains the LangChain integrations for OpenAI through their `openai` SDK.
```

