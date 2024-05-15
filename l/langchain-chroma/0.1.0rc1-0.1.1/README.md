# Comparing `tmp/langchain_chroma-0.1.0rc1.tar.gz` & `tmp/langchain_chroma-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_chroma-0.1.0rc1.tar", max compression
+gzip compressed data, was "langchain_chroma-0.1.1.tar", max compression
```

## Comparing `langchain_chroma-0.1.0rc1.tar` & `langchain_chroma-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2024-04-11 18:30:01.144052 langchain_chroma-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0      373 2024-04-11 18:30:01.144052 langchain_chroma-0.1.0rc1/README.md
--rw-r--r--   0        0        0       78 2024-04-11 18:30:01.144052 langchain_chroma-0.1.0rc1/langchain_chroma/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 18:30:01.144052 langchain_chroma-0.1.0rc1/langchain_chroma/py.typed
--rw-r--r--   0        0        0    31062 2024-04-11 18:30:01.144052 langchain_chroma-0.1.0rc1/langchain_chroma/vectorstores.py
--rw-r--r--   0        0        0     2834 2024-04-11 18:30:01.148052 langchain_chroma-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 langchain_chroma-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-15 21:03:08.951439 langchain_chroma-0.1.1/LICENSE
+-rw-r--r--   0        0        0      373 2024-05-15 21:03:08.951439 langchain_chroma-0.1.1/README.md
+-rw-r--r--   0        0        0       78 2024-05-15 21:03:08.951439 langchain_chroma-0.1.1/langchain_chroma/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:03:08.951439 langchain_chroma-0.1.1/langchain_chroma/py.typed
+-rw-r--r--   0        0        0    31265 2024-05-15 21:03:08.951439 langchain_chroma-0.1.1/langchain_chroma/vectorstores.py
+-rw-r--r--   0        0        0     3009 2024-05-15 21:03:08.951439 langchain_chroma-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 langchain_chroma-0.1.1/PKG-INFO
```

### Comparing `langchain_chroma-0.1.0rc1/LICENSE` & `langchain_chroma-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_chroma-0.1.0rc1/langchain_chroma/vectorstores.py` & `langchain_chroma-0.1.1/langchain_chroma/vectorstores.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,16 @@
     if len(X) == 0 or len(Y) == 0:
         return np.array([])
 
     X = np.array(X)
     Y = np.array(Y)
     if X.shape[1] != Y.shape[1]:
         raise ValueError(
-            f"Number of columns in X and Y must be the same. X has shape {X.shape} "
+            "Number of columns in X and Y must be the same. X has shape"
+            f"{X.shape} "
             f"and Y has shape {Y.shape}."
         )
 
     X_norm = np.linalg.norm(X, axis=1)
     Y_norm = np.linalg.norm(Y, axis=1)
     # Ignore divide by zero errors run time warnings as those are handled below.
     with np.errstate(divide="ignore", invalid="ignore"):
@@ -111,16 +112,16 @@
     """`ChromaDB` vector store.
 
     To use, you should have the ``chromadb`` python package installed.
 
     Example:
         .. code-block:: python
 
-                from langchain_community.vectorstores import Chroma
-                from langchain_community.embeddings.openai import OpenAIEmbeddings
+                from langchain_chroma import Chroma
+                from langchain_openai import OpenAIEmbeddings
 
                 embeddings = OpenAIEmbeddings()
                 vectorstore = Chroma("langchain_store", embeddings)
     """
 
     _LANGCHAIN_DEFAULT_COLLECTION_NAME = "langchain"
 
@@ -129,14 +130,15 @@
         collection_name: str = _LANGCHAIN_DEFAULT_COLLECTION_NAME,
         embedding_function: Optional[Embeddings] = None,
         persist_directory: Optional[str] = None,
         client_settings: Optional[chromadb.config.Settings] = None,
         collection_metadata: Optional[Dict] = None,
         client: Optional[chromadb.ClientAPI] = None,
         relevance_score_fn: Optional[Callable[[float], float]] = None,
+        create_collection_if_not_exists: Optional[bool] = True,
     ) -> None:
         """Initialize with a Chroma client."""
 
         if client is not None:
             self._client_settings = client_settings
             self._client = client
             self._persist_directory = persist_directory
@@ -157,19 +159,22 @@
             self._client_settings = _client_settings
             self._client = chromadb.Client(_client_settings)
             self._persist_directory = (
                 _client_settings.persist_directory or persist_directory
             )
 
         self._embedding_function = embedding_function
-        self._collection = self._client.get_or_create_collection(
-            name=collection_name,
-            embedding_function=None,
-            metadata=collection_metadata,
-        )
+        if create_collection_if_not_exists:
+            self._collection = self._client.get_or_create_collection(
+                name=collection_name,
+                embedding_function=None,
+                metadata=collection_metadata,
+            )
+        else:
+            self._collection = self._client.get_collection(name=collection_name)
         self.override_relevance_score_fn = relevance_score_fn
 
     @property
     def embeddings(self) -> Optional[Embeddings]:
         return self._embedding_function
 
     @xor_args(("query_texts", "query_embeddings"))
@@ -646,15 +651,16 @@
 
         Args:
             document_id (str): ID of the document to update.
             document (Document): Document to update.
         """
         return self.update_documents([document_id], [document])
 
-    def update_documents(self, ids: List[str], documents: List[Document]) -> None:  # type: ignore
+    # type: ignore
+    def update_documents(self, ids: List[str], documents: List[Document]) -> None:
         """Update a document in the collection.
 
         Args:
             ids (List[str]): List of ids of the document to update.
             documents (List[Document]): List of documents to update.
         """
         text = [document.page_content for document in documents]
```

### Comparing `langchain_chroma-0.1.0rc1/pyproject.toml` & `langchain_chroma-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-chroma"
-version = "0.1.0rc1"
+version = "0.1.1"
 description = "An integration package connecting Chroma and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/chroma"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.13"
-langchain-core = "^0.1.40"
-chromadb = { version = "^0.4.0" }
+langchain-core = ">=0.1.40,<0.3"
+chromadb = { version = ">=0.4.0,<0.6.0" }
 numpy = "^1"
 fastapi = { version = ">=0.95.2,<1", optional = true }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
@@ -36,36 +36,38 @@
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
-langchain-openai = ">=0.0.3,<0.1"
+langchain-openai = { path = "../openai", develop = true }
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
-mypy = "^0.991"
+mypy = "^1.10.0"
 langchain-core = { path = "../../core", develop = true }
 langchain-community = { path = "../../community", develop = true }
 types-requests = "^2.31.0.20240406"
+langchain-text-splitters = { path = "../../text-splitters", develop = true }
+langchain = { path = "../../langchain", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 langchain-core = { path = "../../core", develop = true }
 langchain-community = { path = "../../community", develop = true }
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
   "E",    # pycodestyle
   "F",    # pyflakes
   "I",    # isort
   "T201", # print
 
 ]
```

### Comparing `langchain_chroma-0.1.0rc1/PKG-INFO` & `langchain_chroma-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-chroma
-Version: 0.1.0rc1
+Version: 0.1.1
 Summary: An integration package connecting Chroma and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: chromadb (>=0.4.0,<0.5.0)
+Requires-Dist: chromadb (>=0.4.0,<0.6.0)
 Requires-Dist: fastapi (>=0.95.2,<1)
-Requires-Dist: langchain-core (>=0.1.40,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.40,<0.3)
 Requires-Dist: numpy (>=1,<2)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/chroma
 Description-Content-Type: text/markdown
 
 # langchain-chroma
```

