# Comparing `tmp/langchain_mongodb-0.1.4.tar.gz` & `tmp/langchain_mongodb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_mongodb-0.1.4.tar", max compression
+gzip compressed data, was "langchain_mongodb-0.1.5.tar", max compression
```

## Comparing `langchain_mongodb-0.1.4.tar` & `langchain_mongodb-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-05-14 18:55:01.295252 langchain_mongodb-0.1.4/LICENSE
--rw-r--r--   0        0        0     1449 2024-05-14 18:55:01.295252 langchain_mongodb-0.1.4/README.md
--rw-r--r--   0        0        0      365 2024-05-14 18:55:01.295252 langchain_mongodb-0.1.4/langchain_mongodb/__init__.py
--rw-r--r--   0        0        0    10505 2024-05-14 18:55:01.295252 langchain_mongodb-0.1.4/langchain_mongodb/cache.py
--rw-r--r--   0        0        0     2617 2024-05-14 18:55:01.295252 langchain_mongodb-0.1.4/langchain_mongodb/chat_message_histories.py
--rw-r--r--   0        0        0        0 2024-05-14 18:55:01.295252 langchain_mongodb-0.1.4/langchain_mongodb/py.typed
--rw-r--r--   0        0        0     3176 2024-05-14 18:55:01.299252 langchain_mongodb-0.1.4/langchain_mongodb/utils.py
--rw-r--r--   0        0        0    17861 2024-05-14 18:55:01.299252 langchain_mongodb-0.1.4/langchain_mongodb/vectorstores.py
--rw-r--r--   0        0        0     2636 2024-05-14 18:55:01.299252 langchain_mongodb-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2298 1970-01-01 00:00:00.000000 langchain_mongodb-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-15 21:30:24.104348 langchain_mongodb-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1449 2024-05-15 21:30:24.104348 langchain_mongodb-0.1.5/README.md
+-rw-r--r--   0        0        0      365 2024-05-15 21:30:24.104348 langchain_mongodb-0.1.5/langchain_mongodb/__init__.py
+-rw-r--r--   0        0        0    10505 2024-05-15 21:30:24.104348 langchain_mongodb-0.1.5/langchain_mongodb/cache.py
+-rw-r--r--   0        0        0     2617 2024-05-15 21:30:24.104348 langchain_mongodb-0.1.5/langchain_mongodb/chat_message_histories.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:30:24.104348 langchain_mongodb-0.1.5/langchain_mongodb/py.typed
+-rw-r--r--   0        0        0     3176 2024-05-15 21:30:24.104348 langchain_mongodb-0.1.5/langchain_mongodb/utils.py
+-rw-r--r--   0        0        0    18127 2024-05-15 21:30:24.104348 langchain_mongodb-0.1.5/langchain_mongodb/vectorstores.py
+-rw-r--r--   0        0        0     2636 2024-05-15 21:30:24.104348 langchain_mongodb-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2298 1970-01-01 00:00:00.000000 langchain_mongodb-0.1.5/PKG-INFO
```

### Comparing `langchain_mongodb-0.1.4/LICENSE` & `langchain_mongodb-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_mongodb-0.1.4/README.md` & `langchain_mongodb-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `langchain_mongodb-0.1.4/langchain_mongodb/cache.py` & `langchain_mongodb-0.1.5/langchain_mongodb/cache.py`

 * *Files identical despite different names*

### Comparing `langchain_mongodb-0.1.4/langchain_mongodb/chat_message_histories.py` & `langchain_mongodb-0.1.5/langchain_mongodb/chat_message_histories.py`

 * *Files identical despite different names*

### Comparing `langchain_mongodb-0.1.4/langchain_mongodb/utils.py` & `langchain_mongodb-0.1.5/langchain_mongodb/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_mongodb-0.1.4/langchain_mongodb/vectorstores.py` & `langchain_mongodb-0.1.5/langchain_mongodb/vectorstores.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from langchain_mongodb.utils import maximal_marginal_relevance
 
 MongoDBDocumentType = TypeVar("MongoDBDocumentType", bound=Dict[str, Any])
 VST = TypeVar("VST", bound=VectorStore)
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_INSERT_BATCH_SIZE = 100
+DEFAULT_INSERT_BATCH_SIZE = 100_000
 
 
 class MongoDBAtlasVectorSearch(VectorStore):
     """`MongoDB Atlas Vector Search` vector store.
 
     To use, you should have both:
     - the ``pymongo`` python package installed
@@ -147,26 +147,32 @@
             metadatas: Optional list of metadatas associated with the texts.
 
         Returns:
             List of ids from adding the texts into the vectorstore.
         """
         batch_size = kwargs.get("batch_size", DEFAULT_INSERT_BATCH_SIZE)
         _metadatas: Union[List, Generator] = metadatas or ({} for _ in texts)
-        texts_batch = []
-        metadatas_batch = []
+        texts_batch = texts
+        metadatas_batch = _metadatas
         result_ids = []
-        for i, (text, metadata) in enumerate(zip(texts, _metadatas)):
-            texts_batch.append(text)
-            metadatas_batch.append(metadata)
-            if (i + 1) % batch_size == 0:
-                result_ids.extend(self._insert_texts(texts_batch, metadatas_batch))
-                texts_batch = []
-                metadatas_batch = []
+        if batch_size:
+            texts_batch = []
+            metadatas_batch = []
+            size = 0
+            for i, (text, metadata) in enumerate(zip(texts, _metadatas)):
+                size += len(text) + len(metadata)
+                texts_batch.append(text)
+                metadatas_batch.append(metadata)
+                if (i + 1) % batch_size == 0 or size >= 47_000_000:
+                    result_ids.extend(self._insert_texts(texts_batch, metadatas_batch))
+                    texts_batch = []
+                    metadatas_batch = []
+                    size = 0
         if texts_batch:
-            result_ids.extend(self._insert_texts(texts_batch, metadatas_batch))
+            result_ids.extend(self._insert_texts(texts_batch, metadatas_batch))  # type: ignore
         return result_ids
 
     def _insert_texts(self, texts: List[str], metadatas: List[Dict[str, Any]]) -> List:
         if not texts:
             return []
         # Embed and create the documents
         embeddings = self._embedding.embed_documents(texts)
```

### Comparing `langchain_mongodb-0.1.4/pyproject.toml` & `langchain_mongodb-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-mongodb"
-version = "0.1.4"
+version = "0.1.5"
 description = "An integration package connecting MongoDB and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_mongodb-0.1.4/PKG-INFO` & `langchain_mongodb-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-mongodb
-Version: 0.1.4
+Version: 0.1.5
 Summary: An integration package connecting MongoDB and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

