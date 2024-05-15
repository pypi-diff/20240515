# Comparing `tmp/langchain_voyageai-0.1.0.tar.gz` & `tmp/langchain_voyageai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_voyageai-0.1.0.tar", max compression
+gzip compressed data, was "langchain_voyageai-0.1.1.tar", max compression
```

## Comparing `langchain_voyageai-0.1.0.tar` & `langchain_voyageai-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-03-15 01:38:36.439124 langchain_voyageai-0.1.0/LICENSE
--rw-r--r--   0        0        0      555 2024-03-15 01:38:36.439124 langchain_voyageai-0.1.0/README.md
--rw-r--r--   0        0        0      102 2024-03-15 01:38:36.439124 langchain_voyageai-0.1.0/langchain_voyageai/__init__.py
--rw-r--r--   0        0        0     4148 2024-03-15 01:38:36.439124 langchain_voyageai-0.1.0/langchain_voyageai/embeddings.py
--rw-r--r--   0        0        0        0 2024-03-15 01:38:36.439124 langchain_voyageai-0.1.0/langchain_voyageai/py.typed
--rw-r--r--   0        0        0     2457 2024-03-15 01:38:36.439124 langchain_voyageai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 langchain_voyageai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-15 21:31:27.761971 langchain_voyageai-0.1.1/LICENSE
+-rw-r--r--   0        0        0      555 2024-05-15 21:31:27.761971 langchain_voyageai-0.1.1/README.md
+-rw-r--r--   0        0        0      166 2024-05-15 21:31:27.761971 langchain_voyageai-0.1.1/langchain_voyageai/__init__.py
+-rw-r--r--   0        0        0     4148 2024-05-15 21:31:27.761971 langchain_voyageai-0.1.1/langchain_voyageai/embeddings.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:31:27.761971 langchain_voyageai-0.1.1/langchain_voyageai/py.typed
+-rw-r--r--   0        0        0     5123 2024-05-15 21:31:27.761971 langchain_voyageai-0.1.1/langchain_voyageai/rerank.py
+-rw-r--r--   0        0        0     2468 2024-05-15 21:31:27.761971 langchain_voyageai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 langchain_voyageai-0.1.1/PKG-INFO
```

### Comparing `langchain_voyageai-0.1.0/LICENSE` & `langchain_voyageai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_voyageai-0.1.0/README.md` & `langchain_voyageai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_voyageai-0.1.0/langchain_voyageai/embeddings.py` & `langchain_voyageai-0.1.1/langchain_voyageai/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_voyageai-0.1.0/pyproject.toml` & `langchain_voyageai-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-voyageai"
-version = "0.1.0"
+version = "0.1.1"
 description = "An integration package connecting VoyageAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/voyageai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.32"
+langchain-core = ">=0.1.52,<0.3"
 voyageai = ">=0.2.1,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
@@ -50,15 +50,15 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 langchain-core = { path = "../../core", develop = true }
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
 ]
 
 [tool.mypy]
```

### Comparing `langchain_voyageai-0.1.0/PKG-INFO` & `langchain_voyageai-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-voyageai
-Version: 0.1.0
+Version: 0.1.1
 Summary: An integration package connecting VoyageAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1.32,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.52,<0.3)
 Requires-Dist: voyageai (>=0.2.1,<1)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/voyageai
 Description-Content-Type: text/markdown
 
 # langchain-voyageai
```

