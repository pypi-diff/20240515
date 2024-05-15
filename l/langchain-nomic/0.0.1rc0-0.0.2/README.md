# Comparing `tmp/langchain_nomic-0.0.1rc0.tar.gz` & `tmp/langchain_nomic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_nomic-0.0.1rc0.tar", max compression
+gzip compressed data, was "langchain_nomic-0.0.2.tar", max compression
```

## Comparing `langchain_nomic-0.0.1rc0.tar` & `langchain_nomic-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2024-01-30 19:54:38.675879 langchain_nomic-0.0.1rc0/LICENSE
--rw-r--r--   0        0        0      476 2024-01-30 19:54:38.676457 langchain_nomic-0.0.1rc0/README.md
--rw-r--r--   0        0        0       93 2024-01-30 19:54:38.676759 langchain_nomic-0.0.1rc0/langchain_nomic/__init__.py
--rw-r--r--   0        0        0     1817 2024-01-30 19:54:38.677003 langchain_nomic-0.0.1rc0/langchain_nomic/embeddings.py
--rw-r--r--   0        0        0        0 2024-01-30 19:54:38.677031 langchain_nomic-0.0.1rc0/langchain_nomic/py.typed
--rw-r--r--   0        0        0     2473 2024-01-30 19:54:49.804170 langchain_nomic-0.0.1rc0/pyproject.toml
--rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 langchain_nomic-0.0.1rc0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-02-14 16:59:06.735263 langchain_nomic-0.0.2/LICENSE
+-rw-r--r--   0        0        0      476 2024-02-14 16:59:06.735263 langchain_nomic-0.0.2/README.md
+-rw-r--r--   0        0        0       93 2024-02-14 16:59:06.735263 langchain_nomic-0.0.2/langchain_nomic/__init__.py
+-rw-r--r--   0        0        0     2045 2024-02-14 16:59:06.735263 langchain_nomic-0.0.2/langchain_nomic/embeddings.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:59:06.735263 langchain_nomic-0.0.2/langchain_nomic/py.typed
+-rw-r--r--   0        0        0     2494 2024-02-14 16:59:06.739263 langchain_nomic-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 langchain_nomic-0.0.2/PKG-INFO
```

### Comparing `langchain_nomic-0.0.1rc0/LICENSE` & `langchain_nomic-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_nomic-0.0.1rc0/langchain_nomic/embeddings.py` & `langchain_nomic-0.0.2/langchain_nomic/embeddings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from typing import List, Optional
 
 import nomic  # type: ignore
 from langchain_core.embeddings import Embeddings
-from nomic import embed
+from nomic import embed  # type: ignore
 
 
 class NomicEmbeddings(Embeddings):
     """NomicEmbeddings embedding model.
 
     Example:
         .. code-block:: python
@@ -18,35 +18,44 @@
     """
 
     def __init__(
         self,
         *,
         model: str,
         nomic_api_key: Optional[str] = None,
+        dimensionality: Optional[int] = None,
     ):
         """Initialize NomicEmbeddings model.
 
         Args:
             model: model name
             nomic_api_key: optionally, set the Nomic API key. Uses the NOMIC_API_KEY
                 environment variable by default.
         """
         _api_key = nomic_api_key or os.environ.get("NOMIC_API_KEY")
-        nomic.login(_api_key)
+        if _api_key:
+            nomic.login(_api_key)
         self.model = model
+        self.dimensionality = dimensionality
 
     def embed(self, texts: List[str], *, task_type: str) -> List[List[float]]:
         """Embed texts.
 
         Args:
             texts: list of texts to embed
             task_type: the task type to use when embedding. One of `search_query`,
                 `search_document`, `classification`, `clustering`
         """
-        output = embed.text(texts=texts, model=self.model, task_type=task_type)
+
+        output = embed.text(
+            texts=texts,
+            model=self.model,
+            task_type=task_type,
+            dimensionality=self.dimensionality,
+        )
         return output["embeddings"]
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Embed search docs.
 
         Args:
             texts: list of texts to embed as documents
```

### Comparing `langchain_nomic-0.0.1rc0/pyproject.toml` & `langchain_nomic-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [tool.poetry]
 name = "langchain-nomic"
-version = "0.0.1rc0"
+version = "0.0.2"
 description = "An integration package connecting Nomic and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/nomic"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = ">=0.0.12"
-nomic = "^3.0.7"
+langchain-core = "^0.1"
+nomic = "^3.0.12"
 
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
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -42,36 +42,35 @@
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
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
-  "E",  # pycodestyle
-  "F",  # pyflakes
-  "I",  # isort
+  "E",    # pycodestyle
+  "F",    # pyflakes
+  "I",    # isort
+  "T201", # print
 ]
 
 [tool.mypy]
 disallow_untyped_defs = "True"
 
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

### Comparing `langchain_nomic-0.0.1rc0/PKG-INFO` & `langchain_nomic-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-nomic
-Version: 0.0.1rc0
+Version: 0.0.2
 Summary: An integration package connecting Nomic and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.0.12)
-Requires-Dist: nomic (>=3.0.7,<4.0.0)
+Requires-Dist: langchain-core (>=0.1,<0.2)
+Requires-Dist: nomic (>=3.0.12,<4.0.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/nomic
 Description-Content-Type: text/markdown
 
 # langchain-nomic
 
 This package contains the LangChain integration with Nomic
```

