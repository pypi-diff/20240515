# Comparing `tmp/langchain_together-0.1.1.tar.gz` & `tmp/langchain_together-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_together-0.1.1.tar", max compression
+gzip compressed data, was "langchain_together-0.1.2.tar", max compression
```

## Comparing `langchain_together-0.1.1.tar` & `langchain_together-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-07 01:26:34.899991 langchain_together-0.1.1/LICENSE
--rw-r--r--   0        0        0      905 2024-05-07 01:26:34.899991 langchain_together-0.1.1/README.md
--rw-r--r--   0        0        0      224 2024-05-07 01:26:34.899991 langchain_together-0.1.1/langchain_together/__init__.py
--rw-r--r--   0        0        0     3329 2024-05-07 01:26:34.903992 langchain_together-0.1.1/langchain_together/chat_models.py
--rw-r--r--   0        0        0     9173 2024-05-07 01:26:34.903992 langchain_together-0.1.1/langchain_together/embeddings.py
--rw-r--r--   0        0        0     7891 2024-05-07 01:26:34.903992 langchain_together-0.1.1/langchain_together/llms.py
--rw-r--r--   0        0        0        0 2024-05-07 01:26:34.903992 langchain_together-0.1.1/langchain_together/py.typed
--rw-r--r--   0        0        0     2765 2024-05-07 01:26:34.903992 langchain_together-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 langchain_together-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-15 21:31:12.726945 langchain_together-0.1.2/LICENSE
+-rw-r--r--   0        0        0      905 2024-05-15 21:31:12.726945 langchain_together-0.1.2/README.md
+-rw-r--r--   0        0        0      224 2024-05-15 21:31:12.726945 langchain_together-0.1.2/langchain_together/__init__.py
+-rw-r--r--   0        0        0     3329 2024-05-15 21:31:12.726945 langchain_together-0.1.2/langchain_together/chat_models.py
+-rw-r--r--   0        0        0     9173 2024-05-15 21:31:12.726945 langchain_together-0.1.2/langchain_together/embeddings.py
+-rw-r--r--   0        0        0     7891 2024-05-15 21:31:12.726945 langchain_together-0.1.2/langchain_together/llms.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:31:12.726945 langchain_together-0.1.2/langchain_together/py.typed
+-rw-r--r--   0        0        0     2771 2024-05-15 21:31:12.730945 langchain_together-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1814 1970-01-01 00:00:00.000000 langchain_together-0.1.2/PKG-INFO
```

### Comparing `langchain_together-0.1.1/LICENSE` & `langchain_together-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_together-0.1.1/README.md` & `langchain_together-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_together-0.1.1/langchain_together/chat_models.py` & `langchain_together-0.1.2/langchain_together/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_together-0.1.1/langchain_together/embeddings.py` & `langchain_together-0.1.2/langchain_together/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_together-0.1.1/langchain_together/llms.py` & `langchain_together-0.1.2/langchain_together/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_together-0.1.1/pyproject.toml` & `langchain_together-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-together"
-version = "0.1.1"
+version = "0.1.2"
 description = "An integration package connecting Together AI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/together"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.44"
+langchain-core = ">=0.1.52,<0.3"
 langchain-openai = "^0.1.3"
 requests = "^2"
 aiohttp = "^3.9.1"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `langchain_together-0.1.1/PKG-INFO` & `langchain_together-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-together
-Version: 0.1.1
+Version: 0.1.2
 Summary: An integration package connecting Together AI and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
-Requires-Dist: langchain-core (>=0.1.44,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.52,<0.3)
 Requires-Dist: langchain-openai (>=0.1.3,<0.2.0)
 Requires-Dist: requests (>=2,<3)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/together
 Description-Content-Type: text/markdown
 
 # langchain-together
```

