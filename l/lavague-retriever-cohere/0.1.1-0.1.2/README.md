# Comparing `tmp/lavague_retriever_cohere-0.1.1.tar.gz` & `tmp/lavague_retriever_cohere-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_retriever_cohere-0.1.1.tar", max compression
+gzip compressed data, was "lavague_retriever_cohere-0.1.2.tar", max compression
```

## Comparing `lavague_retriever_cohere-0.1.1.tar` & `lavague_retriever_cohere-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       30 2024-05-10 16:23:07.987264 lavague_retriever_cohere-0.1.1/README.md
--rw-r--r--   0        0        0       58 2024-05-10 16:50:10.843592 lavague_retriever_cohere-0.1.1/lavague/retrievers/cohere/__init__.py
--rw-r--r--   0        0        0     1490 2024-05-14 14:23:05.342586 lavague_retriever_cohere-0.1.1/lavague/retrievers/cohere/base.py
--rw-r--r--   0        0        0      970 2024-05-14 14:24:30.496501 lavague_retriever_cohere-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 lavague_retriever_cohere-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-05-15 19:17:05.222186 lavague_retriever_cohere-0.1.2/README.md
+-rw-r--r--   0        0        0       59 2024-05-15 19:17:05.222186 lavague_retriever_cohere-0.1.2/lavague/retrievers/cohere/__init__.py
+-rw-r--r--   0        0        0     1677 2024-05-15 19:17:05.222186 lavague_retriever_cohere-0.1.2/lavague/retrievers/cohere/base.py
+-rw-r--r--   0        0        0      971 2024-05-15 21:18:49.639971 lavague_retriever_cohere-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 lavague_retriever_cohere-0.1.2/PKG-INFO
```

### Comparing `lavague_retriever_cohere-0.1.1/lavague/retrievers/cohere/base.py` & `lavague_retriever_cohere-0.1.2/lavague/retrievers/cohere/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 from typing import Optional
 from lavague.core.retrievers import OpsmSplitRetriever
 import cohere
 
+
 class CohereRetriever(OpsmSplitRetriever):
     """This retriever uses cohere as a backend, which means it will not use the provided embedding model (which can be None)"""
-    def __init__(self, cohere_model: str = "rerank-english-v3.0", cohere_api_key: Optional[str] = None, top_k: int = 5, rank_fields = ["element", "placeholder", "text", "name"]):
+
+    def __init__(
+        self,
+        cohere_model: str = "rerank-english-v3.0",
+        cohere_api_key: Optional[str] = None,
+        top_k: int = 5,
+        rank_fields=["element", "placeholder", "text", "name"],
+    ):
         self.cohere_model = cohere_model
         self.cohere_session = cohere.Client(cohere_api_key)
         super().__init__(top_k=top_k, rank_fields=rank_fields)
 
     def _get_results(self, _embedding, query, html):
         attributes_list = self._create_nodes_dict(html)
         l = len(attributes_list)
         list_of_results = []
         for j in range(0, l, 1000):
-            attr = attributes_list[j:j+1000]
-            results = self.cohere_session.rerank(model=self.cohere_model, query=query, documents=attr, top_n=self.top_k, return_documents=True, rank_fields=self.rank_fields)
+            attr = attributes_list[j : j + 1000]
+            results = self.cohere_session.rerank(
+                model=self.cohere_model,
+                query=query,
+                documents=attr,
+                top_n=self.top_k,
+                return_documents=True,
+                rank_fields=self.rank_fields,
+            )
             results = [r.dict() for r in results.results]
             for r in results:
-                r['index']+=j
+                r["index"] += j
             list_of_results += results
-        list_of_results = sorted(list_of_results, key=lambda x: x['relevance_score'], reverse=True)
-        results = list_of_results[:self.top_k]
-        results_dict = [r['document'] for r in results]
-        score = [r['relevance_score'] for r in results]
+        list_of_results = sorted(
+            list_of_results, key=lambda x: x["relevance_score"], reverse=True
+        )
+        results = list_of_results[: self.top_k]
+        results_dict = [r["document"] for r in results]
+        score = [r["relevance_score"] for r in results]
         return results_dict, score
```

### Comparing `lavague_retriever_cohere-0.1.1/pyproject.toml` & `lavague_retriever_cohere-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-retriever-cohere"
-version = "0.1.1"
+version = "0.1.2"
 description = "Cohere retriever for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -16,14 +16,14 @@
 keywords = ["LAM", "action", "automation", "LLM", "NLP", "RAG", "selenium", "playwright"]
 homepage = "https://lavague.ai"
 repository = "https://github.com/lavague-ai/LaVague/"
 documentation = "https://docs.lavague.ai/en/latest/"
 packages = [{include = "lavague/"}]
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
-lavague-core = "^0.1.0"
+python = "^3.10.0"
+lavague-core = "^0.1.1"
 cohere = "^5.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lavague_retriever_cohere-0.1.1/PKG-INFO` & `lavague_retriever_cohere-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: lavague-retriever-cohere
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cohere retriever for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cohere (>=5.4.0,<6.0.0)
-Requires-Dist: lavague-core (>=0.1.0,<0.2.0)
+Requires-Dist: lavague-core (>=0.1.1,<0.2.0)
 Project-URL: Documentation, https://docs.lavague.ai/en/latest/
 Project-URL: Repository, https://github.com/lavague-ai/LaVague/
 Description-Content-Type: text/markdown
 
 # Cohere retriever for lavague
```

