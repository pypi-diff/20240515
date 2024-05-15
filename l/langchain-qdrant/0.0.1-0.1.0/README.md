# Comparing `tmp/langchain_qdrant-0.0.1.tar.gz` & `tmp/langchain_qdrant-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_qdrant-0.0.1.tar", max compression
+gzip compressed data, was "langchain_qdrant-0.1.0.tar", max compression
```

## Comparing `langchain_qdrant-0.0.1.tar` & `langchain_qdrant-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-05-14 01:20:34.670611 langchain_qdrant-0.0.1/LICENSE
--rw-r--r--   0        0        0      503 2024-05-14 01:20:34.670611 langchain_qdrant-0.0.1/README.md
--rw-r--r--   0        0        0       71 2024-05-14 01:20:34.670611 langchain_qdrant-0.0.1/langchain_qdrant/__init__.py
--rw-r--r--   0        0        0     2554 2024-05-14 01:20:34.670611 langchain_qdrant-0.0.1/langchain_qdrant/_utils.py
--rw-r--r--   0        0        0        0 2024-05-14 01:20:34.670611 langchain_qdrant-0.0.1/langchain_qdrant/py.typed
--rw-r--r--   0        0        0    93129 2024-05-14 01:20:34.670611 langchain_qdrant-0.0.1/langchain_qdrant/vectorstores.py
--rw-r--r--   0        0        0     2505 2024-05-14 01:20:34.670611 langchain_qdrant-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 langchain_qdrant-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-15 21:30:53.010642 langchain_qdrant-0.1.0/LICENSE
+-rw-r--r--   0        0        0      503 2024-05-15 21:30:53.010642 langchain_qdrant-0.1.0/README.md
+-rw-r--r--   0        0        0       71 2024-05-15 21:30:53.010642 langchain_qdrant-0.1.0/langchain_qdrant/__init__.py
+-rw-r--r--   0        0        0     2554 2024-05-15 21:30:53.010642 langchain_qdrant-0.1.0/langchain_qdrant/_utils.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:30:53.010642 langchain_qdrant-0.1.0/langchain_qdrant/py.typed
+-rw-r--r--   0        0        0    93129 2024-05-15 21:30:53.010642 langchain_qdrant-0.1.0/langchain_qdrant/vectorstores.py
+-rw-r--r--   0        0        0     2500 2024-05-15 21:30:53.010642 langchain_qdrant-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 langchain_qdrant-0.1.0/PKG-INFO
```

### Comparing `langchain_qdrant-0.0.1/LICENSE` & `langchain_qdrant-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_qdrant-0.0.1/langchain_qdrant/_utils.py` & `langchain_qdrant-0.1.0/langchain_qdrant/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_qdrant-0.0.1/langchain_qdrant/vectorstores.py` & `langchain_qdrant-0.1.0/langchain_qdrant/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain_qdrant-0.0.1/pyproject.toml` & `langchain_qdrant-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-qdrant"
-version = "0.0.1"
+version = "0.1.0"
 description = "An integration package connecting Qdrant and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
@@ -17,19 +17,19 @@
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
-pytest-mock  = "^3.10.0"
+pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
-langchain-core = {path = "../../core", develop = true}
+langchain-core = { path = "../../core", develop = true }
 requests = "^2.31.0"
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
@@ -43,36 +43,34 @@
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
-langchain-core = {path = "../../core", develop = true}
+langchain-core = { path = "../../core", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-langchain-core = {path = "../../core", develop = true}
+langchain-core = { path = "../../core", develop = true }
 
 [tool.ruff]
 select = [
-  "E",  # pycodestyle
-  "F",  # pyflakes
-  "I",  # isort
+  "E", # pycodestyle
+  "F", # pyflakes
+  "I", # isort
 ]
 
 [tool.mypy]
 disallow_untyped_defs = true
 
 [tool.coverage.run]
-omit = [
-    "tests/*",
-]
+omit = ["tests/*"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 # --strict-markers will raise errors on unknown marks.
```

### Comparing `langchain_qdrant-0.0.1/PKG-INFO` & `langchain_qdrant-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-qdrant
-Version: 0.0.1
+Version: 0.1.0
 Summary: An integration package connecting Qdrant and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

