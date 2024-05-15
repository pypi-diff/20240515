# Comparing `tmp/fastembed_haystack-1.0.0.tar.gz` & `tmp/fastembed_haystack-1.1.0.tar.gz`

## Comparing `fastembed_haystack-1.0.0.tar` & `fastembed_haystack-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/examples/example.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/examples/sparse_example.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/pydoc/config.yml
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/__init__.py
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_document_embedder.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_document_embedder.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_text_embedder.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_text_embedder.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/__init__.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/fastembed_backend.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/tests/test_fastembed_backend.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/tests/test_fastembed_document_embedder.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/tests/test_fastembed_sparse_document_embedder.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/tests/test_fastembed_sparse_text_embedder.py
--rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/tests/test_fastembed_text_embedder.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/README.md
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 fastembed_haystack-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/examples/example.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/examples/sparse_example.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/pydoc/config.yml
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/__init__.py
+-rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_document_embedder.py
+-rw-r--r--   0        0        0     6999 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_document_embedder.py
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_text_embedder.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_text_embedder.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/__init__.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/fastembed_backend.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/tests/test_fastembed_backend.py
+-rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/tests/test_fastembed_document_embedder.py
+-rw-r--r--   0        0        0    11966 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/tests/test_fastembed_sparse_document_embedder.py
+-rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/tests/test_fastembed_sparse_text_embedder.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/tests/test_fastembed_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/README.md
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 fastembed_haystack-1.1.0/PKG-INFO
```

### Comparing `fastembed_haystack-1.0.0/examples/example.py` & `fastembed_haystack-1.1.0/examples/example.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-1.0.0/examples/sparse_example.py` & `fastembed_haystack-1.1.0/examples/sparse_example.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-1.0.0/pydoc/config.yml` & `fastembed_haystack-1.1.0/pydoc/config.yml`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     expression:
     documented_only: true
     do_not_filter_modules: false
     skip_empty_modules: true
   - type: smart
   - type: crossref
 renderer:
-  type: haystack_pydoc_tools.renderers.ReadmePreviewRenderer
+  type: haystack_pydoc_tools.renderers.ReadmeIntegrationRenderer
   excerpt: FastEmbed integration for Haystack
   category_slug: integrations-api
   title: FastEmbed
   slug: fastembed-embedders
   order: 80
   markdown:
     descriptive_class_title: false
```

### Comparing `fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/__init__.py` & `fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/__init__.py`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_document_embedder.py` & `fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_document_embedder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 from typing import Any, Dict, List, Optional
 
 from haystack import Document, component, default_to_dict
 
-from .embedding_backend.fastembed_backend import _FastembedEmbeddingBackendFactory
+from .embedding_backend.fastembed_backend import _FastembedSparseEmbeddingBackendFactory
 
 
 @component
-class FastembedDocumentEmbedder:
+class FastembedSparseDocumentEmbedder:
     """
-    FastembedDocumentEmbedder computes Document embeddings using Fastembed embedding models.
-    The embedding of each Document is stored in the `embedding` field of the Document.
+    FastembedSparseDocumentEmbedder computes Document embeddings using Fastembed sparse models.
 
     Usage example:
     ```python
-    # To use this component, install the "fastembed-haystack" package.
-    # pip install fastembed-haystack
-
-    from haystack_integrations.components.embedders.fastembed import FastembedDocumentEmbedder
+    from haystack_integrations.components.embedders.fastembed import FastembedSparseDocumentEmbedder
     from haystack.dataclasses import Document
 
-    doc_embedder = FastembedDocumentEmbedder(
-        model="BAAI/bge-small-en-v1.5",
-        batch_size=256,
+    sparse_doc_embedder = FastembedSparseDocumentEmbedder(
+        model="prithvida/Splade_PP_en_v1",
+        batch_size=32,
     )
 
-    doc_embedder.warm_up()
+    sparse_doc_embedder.warm_up()
 
     # Text taken from PubMed QA Dataset (https://huggingface.co/datasets/pubmed_qa)
     document_list = [
         Document(
             content=("Oxidative stress generated within inflammatory joints can produce autoimmune phenomena and joint "
                      "destruction. Radical species with oxidative activity, including reactive nitrogen species, "
                      "represent mediators of inflammation and cartilage damage."),
@@ -44,132 +40,129 @@
             meta={
                 "pubid": "25,445,712",
                 "long_answer": "yes",
             },
         ),
     ]
 
-    result = doc_embedder.run(document_list)
+    result = sparse_doc_embedder.run(document_list)
     print(f"Document Text: {result['documents'][0].content}")
-    print(f"Document Embedding: {result['documents'][0].embedding}")
-    print(f"Embedding Dimension: {len(result['documents'][0].embedding)}")
+    print(f"Document Sparse Embedding: {result['documents'][0].sparse_embedding}")
+    print(f"Sparse Embedding Dimension: {len(result['documents'][0].sparse_embedding)}")
     ```
     """
 
     def __init__(
         self,
-        model: str = "BAAI/bge-small-en-v1.5",
+        model: str = "prithvida/Splade_PP_en_v1",
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
-        prefix: str = "",
-        suffix: str = "",
-        batch_size: int = 256,
+        batch_size: int = 32,
         progress_bar: bool = True,
         parallel: Optional[int] = None,
+        local_files_only: bool = False,
         meta_fields_to_embed: Optional[List[str]] = None,
         embedding_separator: str = "\n",
     ):
         """
         Create an FastembedDocumentEmbedder component.
 
         :param model: Local path or name of the model in Hugging Face's model hub,
-            such as `BAAI/bge-small-en-v1.5`.
+            such as `prithvida/Splade_PP_en_v1`.
         :param cache_dir: The path to the cache directory.
                 Can be set using the `FASTEMBED_CACHE_PATH` env variable.
                 Defaults to `fastembed_cache` in the system's temp directory.
-        :param threads: The number of threads single onnxruntime session can use. Defaults to None.
-        :param prefix: A string to add to the beginning of each text.
-        :param suffix: A string to add to the end of each text.
+        :param threads: The number of threads single onnxruntime session can use.
         :param batch_size: Number of strings to encode at once.
-        :param progress_bar: If true, displays progress bar during embedding.
+        :param progress_bar: If `True`, displays progress bar during embedding.
         :param parallel:
                 If > 1, data-parallel encoding will be used, recommended for offline encoding of large datasets.
                 If 0, use all available cores.
                 If None, don't use data-parallel processing, use default onnxruntime threading instead.
+        :param local_files_only: If `True`, only use the model files in the `cache_dir`.
         :param meta_fields_to_embed: List of meta fields that should be embedded along with the Document content.
         :param embedding_separator: Separator used to concatenate the meta fields to the Document content.
         """
 
         self.model_name = model
         self.cache_dir = cache_dir
         self.threads = threads
-        self.prefix = prefix
-        self.suffix = suffix
         self.batch_size = batch_size
         self.progress_bar = progress_bar
         self.parallel = parallel
+        self.local_files_only = local_files_only
         self.meta_fields_to_embed = meta_fields_to_embed or []
         self.embedding_separator = embedding_separator
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
         :returns:
             Dictionary with serialized data.
         """
         return default_to_dict(
             self,
             model=self.model_name,
             cache_dir=self.cache_dir,
             threads=self.threads,
-            prefix=self.prefix,
-            suffix=self.suffix,
             batch_size=self.batch_size,
             progress_bar=self.progress_bar,
             parallel=self.parallel,
+            local_files_only=self.local_files_only,
             meta_fields_to_embed=self.meta_fields_to_embed,
             embedding_separator=self.embedding_separator,
         )
 
     def warm_up(self):
         """
         Initializes the component.
         """
         if not hasattr(self, "embedding_backend"):
-            self.embedding_backend = _FastembedEmbeddingBackendFactory.get_embedding_backend(
-                model_name=self.model_name, cache_dir=self.cache_dir, threads=self.threads
+            self.embedding_backend = _FastembedSparseEmbeddingBackendFactory.get_embedding_backend(
+                model_name=self.model_name,
+                cache_dir=self.cache_dir,
+                threads=self.threads,
+                local_files_only=self.local_files_only,
             )
 
     def _prepare_texts_to_embed(self, documents: List[Document]) -> List[str]:
         texts_to_embed = []
         for doc in documents:
             meta_values_to_embed = [
                 str(doc.meta[key]) for key in self.meta_fields_to_embed if key in doc.meta and doc.meta[key] is not None
             ]
-            text_to_embed = (
-                self.prefix + self.embedding_separator.join([*meta_values_to_embed, doc.content or ""]) + self.suffix
-            )
+            text_to_embed = self.embedding_separator.join([*meta_values_to_embed, doc.content or ""])
 
             texts_to_embed.append(text_to_embed)
         return texts_to_embed
 
     @component.output_types(documents=List[Document])
     def run(self, documents: List[Document]):
         """
         Embeds a list of Documents.
 
         :param documents: List of Documents to embed.
         :returns: A dictionary with the following keys:
-            - `documents`: List of Documents with each Document's `embedding` field set to the computed embeddings.
+            - `documents`: List of Documents with each Document's `sparse_embedding`
+                            field set to the computed embeddings.
         """
         if not isinstance(documents, list) or documents and not isinstance(documents[0], Document):
             msg = (
-                "FastembedDocumentEmbedder expects a list of Documents as input. "
+                "FastembedSparseDocumentEmbedder expects a list of Documents as input. "
                 "In case you want to embed a list of strings, please use the FastembedTextEmbedder."
             )
             raise TypeError(msg)
         if not hasattr(self, "embedding_backend"):
             msg = "The embedding model has not been loaded. Please call warm_up() before running."
             raise RuntimeError(msg)
 
         texts_to_embed = self._prepare_texts_to_embed(documents=documents)
         embeddings = self.embedding_backend.embed(
             texts_to_embed,
             batch_size=self.batch_size,
-            progress_bar=self.progress_bar,
+            show_progress_bar=self.progress_bar,
             parallel=self.parallel,
         )
 
         for doc, emb in zip(documents, embeddings):
-            doc.embedding = emb
-
+            doc.sparse_embedding = emb
         return {"documents": documents}
```

### Comparing `fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_document_embedder.py` & `fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_document_embedder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from typing import Any, Dict, List, Optional
 
 from haystack import Document, component, default_to_dict
 
-from .embedding_backend.fastembed_backend import _FastembedSparseEmbeddingBackendFactory
+from .embedding_backend.fastembed_backend import _FastembedEmbeddingBackendFactory
 
 
 @component
-class FastembedSparseDocumentEmbedder:
+class FastembedDocumentEmbedder:
     """
-    FastembedSparseDocumentEmbedder computes Document embeddings using Fastembed sparse models.
+    FastembedDocumentEmbedder computes Document embeddings using Fastembed embedding models.
+    The embedding of each Document is stored in the `embedding` field of the Document.
 
     Usage example:
     ```python
-    from haystack_integrations.components.embedders.fastembed import FastembedSparseDocumentEmbedder
+    # To use this component, install the "fastembed-haystack" package.
+    # pip install fastembed-haystack
+
+    from haystack_integrations.components.embedders.fastembed import FastembedDocumentEmbedder
     from haystack.dataclasses import Document
 
-    sparse_doc_embedder = FastembedSparseDocumentEmbedder(
-        model="prithvida/Splade_PP_en_v1",
-        batch_size=32,
+    doc_embedder = FastembedDocumentEmbedder(
+        model="BAAI/bge-small-en-v1.5",
+        batch_size=256,
     )
 
-    sparse_doc_embedder.warm_up()
+    doc_embedder.warm_up()
 
     # Text taken from PubMed QA Dataset (https://huggingface.co/datasets/pubmed_qa)
     document_list = [
         Document(
             content=("Oxidative stress generated within inflammatory joints can produce autoimmune phenomena and joint "
                      "destruction. Radical species with oxidative activity, including reactive nitrogen species, "
                      "represent mediators of inflammation and cartilage damage."),
@@ -40,122 +44,139 @@
             meta={
                 "pubid": "25,445,712",
                 "long_answer": "yes",
             },
         ),
     ]
 
-    result = sparse_doc_embedder.run(document_list)
+    result = doc_embedder.run(document_list)
     print(f"Document Text: {result['documents'][0].content}")
-    print(f"Document Sparse Embedding: {result['documents'][0].sparse_embedding}")
-    print(f"Sparse Embedding Dimension: {len(result['documents'][0].sparse_embedding)}")
+    print(f"Document Embedding: {result['documents'][0].embedding}")
+    print(f"Embedding Dimension: {len(result['documents'][0].embedding)}")
     ```
     """
 
     def __init__(
         self,
-        model: str = "prithvida/Splade_PP_en_v1",
+        model: str = "BAAI/bge-small-en-v1.5",
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
-        batch_size: int = 32,
+        prefix: str = "",
+        suffix: str = "",
+        batch_size: int = 256,
         progress_bar: bool = True,
         parallel: Optional[int] = None,
+        local_files_only: bool = False,
         meta_fields_to_embed: Optional[List[str]] = None,
         embedding_separator: str = "\n",
     ):
         """
         Create an FastembedDocumentEmbedder component.
 
         :param model: Local path or name of the model in Hugging Face's model hub,
-            such as `prithvida/Splade_PP_en_v1`.
+            such as `BAAI/bge-small-en-v1.5`.
         :param cache_dir: The path to the cache directory.
                 Can be set using the `FASTEMBED_CACHE_PATH` env variable.
                 Defaults to `fastembed_cache` in the system's temp directory.
-        :param threads: The number of threads single onnxruntime session can use.
+        :param threads: The number of threads single onnxruntime session can use. Defaults to None.
+        :param prefix: A string to add to the beginning of each text.
+        :param suffix: A string to add to the end of each text.
         :param batch_size: Number of strings to encode at once.
         :param progress_bar: If `True`, displays progress bar during embedding.
         :param parallel:
                 If > 1, data-parallel encoding will be used, recommended for offline encoding of large datasets.
                 If 0, use all available cores.
                 If None, don't use data-parallel processing, use default onnxruntime threading instead.
+        :param local_files_only: If `True`, only use the model files in the `cache_dir`.
         :param meta_fields_to_embed: List of meta fields that should be embedded along with the Document content.
         :param embedding_separator: Separator used to concatenate the meta fields to the Document content.
         """
 
         self.model_name = model
         self.cache_dir = cache_dir
         self.threads = threads
+        self.prefix = prefix
+        self.suffix = suffix
         self.batch_size = batch_size
         self.progress_bar = progress_bar
         self.parallel = parallel
+        self.local_files_only = local_files_only
         self.meta_fields_to_embed = meta_fields_to_embed or []
         self.embedding_separator = embedding_separator
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
         :returns:
             Dictionary with serialized data.
         """
         return default_to_dict(
             self,
             model=self.model_name,
             cache_dir=self.cache_dir,
             threads=self.threads,
+            prefix=self.prefix,
+            suffix=self.suffix,
             batch_size=self.batch_size,
             progress_bar=self.progress_bar,
             parallel=self.parallel,
+            local_files_only=self.local_files_only,
             meta_fields_to_embed=self.meta_fields_to_embed,
             embedding_separator=self.embedding_separator,
         )
 
     def warm_up(self):
         """
         Initializes the component.
         """
         if not hasattr(self, "embedding_backend"):
-            self.embedding_backend = _FastembedSparseEmbeddingBackendFactory.get_embedding_backend(
-                model_name=self.model_name, cache_dir=self.cache_dir, threads=self.threads
+            self.embedding_backend = _FastembedEmbeddingBackendFactory.get_embedding_backend(
+                model_name=self.model_name,
+                cache_dir=self.cache_dir,
+                threads=self.threads,
+                local_files_only=self.local_files_only,
             )
 
     def _prepare_texts_to_embed(self, documents: List[Document]) -> List[str]:
         texts_to_embed = []
         for doc in documents:
             meta_values_to_embed = [
                 str(doc.meta[key]) for key in self.meta_fields_to_embed if key in doc.meta and doc.meta[key] is not None
             ]
-            text_to_embed = self.embedding_separator.join([*meta_values_to_embed, doc.content or ""])
+            text_to_embed = (
+                self.prefix + self.embedding_separator.join([*meta_values_to_embed, doc.content or ""]) + self.suffix
+            )
 
             texts_to_embed.append(text_to_embed)
         return texts_to_embed
 
     @component.output_types(documents=List[Document])
     def run(self, documents: List[Document]):
         """
         Embeds a list of Documents.
 
         :param documents: List of Documents to embed.
         :returns: A dictionary with the following keys:
-            - `documents`: List of Documents with each Document's `sparse_embedding`
-                            field set to the computed embeddings.
+            - `documents`: List of Documents with each Document's `embedding` field set to the computed embeddings.
         """
         if not isinstance(documents, list) or documents and not isinstance(documents[0], Document):
             msg = (
-                "FastembedSparseDocumentEmbedder expects a list of Documents as input. "
+                "FastembedDocumentEmbedder expects a list of Documents as input. "
                 "In case you want to embed a list of strings, please use the FastembedTextEmbedder."
             )
             raise TypeError(msg)
         if not hasattr(self, "embedding_backend"):
             msg = "The embedding model has not been loaded. Please call warm_up() before running."
             raise RuntimeError(msg)
 
         texts_to_embed = self._prepare_texts_to_embed(documents=documents)
         embeddings = self.embedding_backend.embed(
             texts_to_embed,
             batch_size=self.batch_size,
-            show_progress_bar=self.progress_bar,
+            progress_bar=self.progress_bar,
             parallel=self.parallel,
         )
 
         for doc, emb in zip(documents, embeddings):
-            doc.sparse_embedding = emb
+            doc.embedding = emb
+
         return {"documents": documents}
```

### Comparing `fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_text_embedder.py` & `fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_sparse_text_embedder.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,35 +30,38 @@
     def __init__(
         self,
         model: str = "prithvida/Splade_PP_en_v1",
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
         progress_bar: bool = True,
         parallel: Optional[int] = None,
+        local_files_only: bool = False,
     ):
         """
         Create a FastembedSparseTextEmbedder component.
 
         :param model: Local path or name of the model in Fastembed's model hub, such as `prithvida/Splade_PP_en_v1`
         :param cache_dir: The path to the cache directory.
                 Can be set using the `FASTEMBED_CACHE_PATH` env variable.
                 Defaults to `fastembed_cache` in the system's temp directory.
         :param threads: The number of threads single onnxruntime session can use. Defaults to None.
-        :param progress_bar: If true, displays progress bar during embedding.
+        :param progress_bar: If `True`, displays progress bar during embedding.
         :param parallel:
                 If > 1, data-parallel encoding will be used, recommended for offline encoding of large datasets.
                 If 0, use all available cores.
                 If None, don't use data-parallel processing, use default onnxruntime threading instead.
+        :param local_files_only: If `True`, only use the model files in the `cache_dir`.
         """
 
         self.model_name = model
         self.cache_dir = cache_dir
         self.threads = threads
         self.progress_bar = progress_bar
         self.parallel = parallel
+        self.local_files_only = local_files_only
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
@@ -66,23 +69,27 @@
         return default_to_dict(
             self,
             model=self.model_name,
             cache_dir=self.cache_dir,
             threads=self.threads,
             progress_bar=self.progress_bar,
             parallel=self.parallel,
+            local_files_only=self.local_files_only,
         )
 
     def warm_up(self):
         """
         Initializes the component.
         """
         if not hasattr(self, "embedding_backend"):
             self.embedding_backend = _FastembedSparseEmbeddingBackendFactory.get_embedding_backend(
-                model_name=self.model_name, cache_dir=self.cache_dir, threads=self.threads
+                model_name=self.model_name,
+                cache_dir=self.cache_dir,
+                threads=self.threads,
+                local_files_only=self.local_files_only,
             )
 
     @component.output_types(sparse_embedding=SparseEmbedding)
     def run(self, text: str):
         """
         Embeds text using the Fastembed model.
```

### Comparing `fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/fastembed_text_embedder.py` & `fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/fastembed_text_embedder.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,39 +31,42 @@
         model: str = "BAAI/bge-small-en-v1.5",
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
         prefix: str = "",
         suffix: str = "",
         progress_bar: bool = True,
         parallel: Optional[int] = None,
+        local_files_only: bool = False,
     ):
         """
         Create a FastembedTextEmbedder component.
 
         :param model: Local path or name of the model in Fastembed's model hub, such as `BAAI/bge-small-en-v1.5`
         :param cache_dir: The path to the cache directory.
                 Can be set using the `FASTEMBED_CACHE_PATH` env variable.
                 Defaults to `fastembed_cache` in the system's temp directory.
         :param threads: The number of threads single onnxruntime session can use. Defaults to None.
         :param prefix: A string to add to the beginning of each text.
         :param suffix: A string to add to the end of each text.
-        :param progress_bar: If true, displays progress bar during embedding.
+        :param progress_bar: If `True`, displays progress bar during embedding.
         :param parallel:
                 If > 1, data-parallel encoding will be used, recommended for offline encoding of large datasets.
                 If 0, use all available cores.
                 If None, don't use data-parallel processing, use default onnxruntime threading instead.
+        :param local_files_only: If `True`, only use the model files in the `cache_dir`.
         """
 
         self.model_name = model
         self.cache_dir = cache_dir
         self.threads = threads
         self.prefix = prefix
         self.suffix = suffix
         self.progress_bar = progress_bar
         self.parallel = parallel
+        self.local_files_only = local_files_only
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
@@ -73,23 +76,27 @@
             model=self.model_name,
             cache_dir=self.cache_dir,
             threads=self.threads,
             prefix=self.prefix,
             suffix=self.suffix,
             progress_bar=self.progress_bar,
             parallel=self.parallel,
+            local_files_only=self.local_files_only,
         )
 
     def warm_up(self):
         """
         Initializes the component.
         """
         if not hasattr(self, "embedding_backend"):
             self.embedding_backend = _FastembedEmbeddingBackendFactory.get_embedding_backend(
-                model_name=self.model_name, cache_dir=self.cache_dir, threads=self.threads
+                model_name=self.model_name,
+                cache_dir=self.cache_dir,
+                threads=self.threads,
+                local_files_only=self.local_files_only,
             )
 
     @component.output_types(embedding=List[float])
     def run(self, text: str):
         """
         Embeds text using the Fastembed model.
```

### Comparing `fastembed_haystack-1.0.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/fastembed_backend.py` & `fastembed_haystack-1.1.0/src/haystack_integrations/components/embedders/fastembed/embedding_backend/fastembed_backend.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,37 +15,43 @@
     _instances: ClassVar[Dict[str, "_FastembedEmbeddingBackend"]] = {}
 
     @staticmethod
     def get_embedding_backend(
         model_name: str,
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
+        local_files_only: bool = False,
     ):
         embedding_backend_id = f"{model_name}{cache_dir}{threads}"
 
         if embedding_backend_id in _FastembedEmbeddingBackendFactory._instances:
             return _FastembedEmbeddingBackendFactory._instances[embedding_backend_id]
 
-        embedding_backend = _FastembedEmbeddingBackend(model_name=model_name, cache_dir=cache_dir, threads=threads)
+        embedding_backend = _FastembedEmbeddingBackend(
+            model_name=model_name, cache_dir=cache_dir, threads=threads, local_files_only=local_files_only
+        )
         _FastembedEmbeddingBackendFactory._instances[embedding_backend_id] = embedding_backend
         return embedding_backend
 
 
 class _FastembedEmbeddingBackend:
     """
     Class to manage fastembed embeddings.
     """
 
     def __init__(
         self,
         model_name: str,
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
+        local_files_only: bool = False,
     ):
-        self.model = TextEmbedding(model_name=model_name, cache_dir=cache_dir, threads=threads)
+        self.model = TextEmbedding(
+            model_name=model_name, cache_dir=cache_dir, threads=threads, local_files_only=local_files_only
+        )
 
     def embed(self, data: List[str], progress_bar=True, **kwargs) -> List[List[float]]:
         # the embed method returns a Iterable[np.ndarray], so we convert it to a list of lists
         embeddings = []
         embeddings_iterable = self.model.embed(data, **kwargs)
         for np_array in tqdm(
             embeddings_iterable, disable=not progress_bar, desc="Calculating embeddings", total=len(data)
@@ -62,22 +68,23 @@
     _instances: ClassVar[Dict[str, "_FastembedSparseEmbeddingBackend"]] = {}
 
     @staticmethod
     def get_embedding_backend(
         model_name: str,
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
+        local_files_only: bool = False,
     ):
         embedding_backend_id = f"{model_name}{cache_dir}{threads}"
 
         if embedding_backend_id in _FastembedSparseEmbeddingBackendFactory._instances:
             return _FastembedSparseEmbeddingBackendFactory._instances[embedding_backend_id]
 
         embedding_backend = _FastembedSparseEmbeddingBackend(
-            model_name=model_name, cache_dir=cache_dir, threads=threads
+            model_name=model_name, cache_dir=cache_dir, threads=threads, local_files_only=local_files_only
         )
         _FastembedSparseEmbeddingBackendFactory._instances[embedding_backend_id] = embedding_backend
         return embedding_backend
 
 
 class _FastembedSparseEmbeddingBackend:
     """
@@ -85,16 +92,19 @@
     """
 
     def __init__(
         self,
         model_name: str,
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
+        local_files_only: bool = False,
     ):
-        self.model = SparseTextEmbedding(model_name=model_name, cache_dir=cache_dir, threads=threads)
+        self.model = SparseTextEmbedding(
+            model_name=model_name, cache_dir=cache_dir, threads=threads, local_files_only=local_files_only
+        )
 
     def embed(self, data: List[List[str]], progress_bar=True, **kwargs) -> List[SparseEmbedding]:
         # The embed method returns a Iterable[SparseEmbedding], so we convert to Haystack SparseEmbedding type.
         # Each SparseEmbedding contains an `indices` key containing a list of int and
         # an `values` key containing a list of floats.
 
         sparse_embeddings = []
```

### Comparing `fastembed_haystack-1.0.0/tests/test_fastembed_backend.py` & `fastembed_haystack-1.1.0/tests/test_fastembed_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 @patch("haystack_integrations.components.embedders.fastembed.embedding_backend.fastembed_backend.TextEmbedding")
 def test_model_initialization(mock_instructor):
     _FastembedEmbeddingBackendFactory.get_embedding_backend(
         model_name="BAAI/bge-small-en-v1.5",
     )
-    mock_instructor.assert_called_once_with(model_name="BAAI/bge-small-en-v1.5", cache_dir=None, threads=None)
+    mock_instructor.assert_called_once_with(
+        model_name="BAAI/bge-small-en-v1.5", cache_dir=None, threads=None, local_files_only=False
+    )
     # restore the factory state
     _FastembedEmbeddingBackendFactory._instances = {}
 
 
 @patch("haystack_integrations.components.embedders.fastembed.embedding_backend.fastembed_backend.TextEmbedding")
 def test_embedding_function_with_kwargs(mock_instructor):  # noqa: ARG001
     embedding_backend = _FastembedEmbeddingBackendFactory.get_embedding_backend(model_name="BAAI/bge-small-en-v1.5")
```

### Comparing `fastembed_haystack-1.0.0/tests/test_fastembed_document_embedder.py` & `fastembed_haystack-1.1.0/tests/test_fastembed_document_embedder.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         assert embedder.cache_dir is None
         assert embedder.threads is None
         assert embedder.prefix == ""
         assert embedder.suffix == ""
         assert embedder.batch_size == 256
         assert embedder.progress_bar is True
         assert embedder.parallel is None
+        assert not embedder.local_files_only
         assert embedder.meta_fields_to_embed == []
         assert embedder.embedding_separator == "\n"
 
     def test_init_with_parameters(self):
         """
         Test custom initialization parameters for FastembedDocumentEmbedder.
         """
@@ -34,25 +35,27 @@
             cache_dir="fake_dir",
             threads=2,
             prefix="prefix",
             suffix="suffix",
             batch_size=64,
             progress_bar=False,
             parallel=1,
+            local_files_only=True,
             meta_fields_to_embed=["test_field"],
             embedding_separator=" | ",
         )
         assert embedder.model_name == "BAAI/bge-small-en-v1.5"
         assert embedder.cache_dir == "fake_dir"
         assert embedder.threads == 2
         assert embedder.prefix == "prefix"
         assert embedder.suffix == "suffix"
         assert embedder.batch_size == 64
         assert embedder.progress_bar is False
         assert embedder.parallel == 1
+        assert embedder.local_files_only
         assert embedder.meta_fields_to_embed == ["test_field"]
         assert embedder.embedding_separator == " | "
 
     def test_to_dict(self):
         """
         Test serialization of FastembedDocumentEmbedder to a dictionary, using default initialization parameters.
         """
@@ -65,14 +68,15 @@
                 "cache_dir": None,
                 "threads": None,
                 "prefix": "",
                 "suffix": "",
                 "batch_size": 256,
                 "progress_bar": True,
                 "parallel": None,
+                "local_files_only": False,
                 "embedding_separator": "\n",
                 "meta_fields_to_embed": [],
             },
         }
 
     def test_to_dict_with_custom_init_parameters(self):
         """
@@ -83,14 +87,15 @@
             cache_dir="fake_dir",
             threads=2,
             prefix="prefix",
             suffix="suffix",
             batch_size=64,
             progress_bar=False,
             parallel=1,
+            local_files_only=True,
             meta_fields_to_embed=["test_field"],
             embedding_separator=" | ",
         )
         embedder_dict = embedder.to_dict()
         assert embedder_dict == {
             "type": "haystack_integrations.components.embedders.fastembed.fastembed_document_embedder.FastembedDocumentEmbedder",  #  noqa
             "init_parameters": {
@@ -98,14 +103,15 @@
                 "cache_dir": "fake_dir",
                 "threads": 2,
                 "prefix": "prefix",
                 "suffix": "suffix",
                 "batch_size": 64,
                 "progress_bar": False,
                 "parallel": 1,
+                "local_files_only": True,
                 "meta_fields_to_embed": ["test_field"],
                 "embedding_separator": " | ",
             },
         }
 
     def test_from_dict(self):
         """
@@ -118,27 +124,29 @@
                 "cache_dir": None,
                 "threads": None,
                 "prefix": "",
                 "suffix": "",
                 "batch_size": 256,
                 "progress_bar": True,
                 "parallel": None,
+                "local_files_only": False,
                 "meta_fields_to_embed": [],
                 "embedding_separator": "\n",
             },
         }
         embedder = default_from_dict(FastembedDocumentEmbedder, embedder_dict)
         assert embedder.model_name == "BAAI/bge-small-en-v1.5"
         assert embedder.cache_dir is None
         assert embedder.threads is None
         assert embedder.prefix == ""
         assert embedder.suffix == ""
         assert embedder.batch_size == 256
         assert embedder.progress_bar is True
         assert embedder.parallel is None
+        assert not embedder.local_files_only
         assert embedder.meta_fields_to_embed == []
         assert embedder.embedding_separator == "\n"
 
     def test_from_dict_with_custom_init_parameters(self):
         """
         Test deserialization of FastembedDocumentEmbedder from a dictionary, using custom initialization parameters.
         """
@@ -149,42 +157,44 @@
                 "cache_dir": "fake_dir",
                 "threads": 2,
                 "prefix": "prefix",
                 "suffix": "suffix",
                 "batch_size": 64,
                 "progress_bar": False,
                 "parallel": 1,
+                "local_files_only": True,
                 "meta_fields_to_embed": ["test_field"],
                 "embedding_separator": " | ",
             },
         }
         embedder = default_from_dict(FastembedDocumentEmbedder, embedder_dict)
         assert embedder.model_name == "BAAI/bge-small-en-v1.5"
         assert embedder.cache_dir == "fake_dir"
         assert embedder.threads == 2
         assert embedder.prefix == "prefix"
         assert embedder.suffix == "suffix"
         assert embedder.batch_size == 64
         assert embedder.progress_bar is False
         assert embedder.parallel == 1
+        assert embedder.local_files_only
         assert embedder.meta_fields_to_embed == ["test_field"]
         assert embedder.embedding_separator == " | "
 
     @patch(
         "haystack_integrations.components.embedders.fastembed.fastembed_document_embedder._FastembedEmbeddingBackendFactory"
     )
     def test_warmup(self, mocked_factory):
         """
         Test for checking embedder instances after warm-up.
         """
         embedder = FastembedDocumentEmbedder(model="BAAI/bge-small-en-v1.5")
         mocked_factory.get_embedding_backend.assert_not_called()
         embedder.warm_up()
         mocked_factory.get_embedding_backend.assert_called_once_with(
-            model_name="BAAI/bge-small-en-v1.5", cache_dir=None, threads=None
+            model_name="BAAI/bge-small-en-v1.5", cache_dir=None, threads=None, local_files_only=False
         )
 
     @patch(
         "haystack_integrations.components.embedders.fastembed.fastembed_document_embedder._FastembedEmbeddingBackendFactory"
     )
     def test_warmup_does_not_reload(self, mocked_factory):
         """
```

### Comparing `fastembed_haystack-1.0.0/tests/test_fastembed_sparse_document_embedder.py` & `fastembed_haystack-1.1.0/tests/test_fastembed_sparse_document_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,37 +17,40 @@
         embedder = FastembedSparseDocumentEmbedder(model="prithvida/Splade_PP_en_v1")
         assert embedder.model_name == "prithvida/Splade_PP_en_v1"
         assert embedder.cache_dir is None
         assert embedder.threads is None
         assert embedder.batch_size == 32
         assert embedder.progress_bar is True
         assert embedder.parallel is None
+        assert not embedder.local_files_only
         assert embedder.meta_fields_to_embed == []
         assert embedder.embedding_separator == "\n"
 
     def test_init_with_parameters(self):
         """
         Test custom initialization parameters for FastembedSparseDocumentEmbedder.
         """
         embedder = FastembedSparseDocumentEmbedder(
             model="prithvida/Splade_PP_en_v1",
             cache_dir="fake_dir",
             threads=2,
             batch_size=64,
             progress_bar=False,
             parallel=1,
+            local_files_only=True,
             meta_fields_to_embed=["test_field"],
             embedding_separator=" | ",
         )
         assert embedder.model_name == "prithvida/Splade_PP_en_v1"
         assert embedder.cache_dir == "fake_dir"
         assert embedder.threads == 2
         assert embedder.batch_size == 64
         assert embedder.progress_bar is False
         assert embedder.parallel == 1
+        assert embedder.local_files_only
         assert embedder.meta_fields_to_embed == ["test_field"]
         assert embedder.embedding_separator == " | "
 
     def test_to_dict(self):
         """
         Test serialization of FastembedSparseDocumentEmbedder to a dictionary, using default initialization parameters.
         """
@@ -58,14 +61,15 @@
             "init_parameters": {
                 "model": "prithvida/Splade_PP_en_v1",
                 "cache_dir": None,
                 "threads": None,
                 "batch_size": 32,
                 "progress_bar": True,
                 "parallel": None,
+                "local_files_only": False,
                 "embedding_separator": "\n",
                 "meta_fields_to_embed": [],
             },
         }
 
     def test_to_dict_with_custom_init_parameters(self):
         """
@@ -74,27 +78,29 @@
         embedder = FastembedSparseDocumentEmbedder(
             model="prithvida/Splade_PP_en_v1",
             cache_dir="fake_dir",
             threads=2,
             batch_size=64,
             progress_bar=False,
             parallel=1,
+            local_files_only=True,
             meta_fields_to_embed=["test_field"],
             embedding_separator=" | ",
         )
         embedder_dict = embedder.to_dict()
         assert embedder_dict == {
             "type": "haystack_integrations.components.embedders.fastembed.fastembed_sparse_document_embedder.FastembedSparseDocumentEmbedder",  #  noqa
             "init_parameters": {
                 "model": "prithvida/Splade_PP_en_v1",
                 "cache_dir": "fake_dir",
                 "threads": 2,
                 "batch_size": 64,
                 "progress_bar": False,
                 "parallel": 1,
+                "local_files_only": True,
                 "meta_fields_to_embed": ["test_field"],
                 "embedding_separator": " | ",
             },
         }
 
     def test_from_dict(self):
         """
@@ -106,25 +112,27 @@
             "init_parameters": {
                 "model": "prithvida/Splade_PP_en_v1",
                 "cache_dir": None,
                 "threads": None,
                 "batch_size": 32,
                 "progress_bar": True,
                 "parallel": None,
+                "local_files_only": False,
                 "meta_fields_to_embed": [],
                 "embedding_separator": "\n",
             },
         }
         embedder = default_from_dict(FastembedSparseDocumentEmbedder, embedder_dict)
         assert embedder.model_name == "prithvida/Splade_PP_en_v1"
         assert embedder.cache_dir is None
         assert embedder.threads is None
         assert embedder.batch_size == 32
         assert embedder.progress_bar is True
         assert embedder.parallel is None
+        assert not embedder.local_files_only
         assert embedder.meta_fields_to_embed == []
         assert embedder.embedding_separator == "\n"
 
     def test_from_dict_with_custom_init_parameters(self):
         """
         Test deserialization of FastembedSparseDocumentEmbedder from a dictionary,
         using custom initialization parameters.
@@ -134,40 +142,42 @@
             "init_parameters": {
                 "model": "prithvida/Splade_PP_en_v1",
                 "cache_dir": "fake_dir",
                 "threads": 2,
                 "batch_size": 64,
                 "progress_bar": False,
                 "parallel": 1,
+                "local_files_only": True,
                 "meta_fields_to_embed": ["test_field"],
                 "embedding_separator": " | ",
             },
         }
         embedder = default_from_dict(FastembedSparseDocumentEmbedder, embedder_dict)
         assert embedder.model_name == "prithvida/Splade_PP_en_v1"
         assert embedder.cache_dir == "fake_dir"
         assert embedder.threads == 2
         assert embedder.batch_size == 64
         assert embedder.progress_bar is False
         assert embedder.parallel == 1
+        assert embedder.local_files_only
         assert embedder.meta_fields_to_embed == ["test_field"]
         assert embedder.embedding_separator == " | "
 
     @patch(
         "haystack_integrations.components.embedders.fastembed.fastembed_sparse_document_embedder._FastembedSparseEmbeddingBackendFactory"
     )
     def test_warmup(self, mocked_factory):
         """
         Test for checking embedder instances after warm-up.
         """
         embedder = FastembedSparseDocumentEmbedder(model="prithvida/Splade_PP_en_v1")
         mocked_factory.get_embedding_backend.assert_not_called()
         embedder.warm_up()
         mocked_factory.get_embedding_backend.assert_called_once_with(
-            model_name="prithvida/Splade_PP_en_v1", cache_dir=None, threads=None
+            model_name="prithvida/Splade_PP_en_v1", cache_dir=None, threads=None, local_files_only=False
         )
 
     @patch(
         "haystack_integrations.components.embedders.fastembed.fastembed_sparse_document_embedder._FastembedSparseEmbeddingBackendFactory"
     )
     def test_warmup_does_not_reload(self, mocked_factory):
         """
```

### Comparing `fastembed_haystack-1.0.0/tests/test_fastembed_sparse_text_embedder.py` & `fastembed_haystack-1.1.0/tests/test_fastembed_sparse_text_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,37 +48,40 @@
             "type": "haystack_integrations.components.embedders.fastembed.fastembed_sparse_text_embedder.FastembedSparseTextEmbedder",  # noqa
             "init_parameters": {
                 "model": "prithvida/Splade_PP_en_v1",
                 "cache_dir": None,
                 "threads": None,
                 "progress_bar": True,
                 "parallel": None,
+                "local_files_only": False,
             },
         }
 
     def test_to_dict_with_custom_init_parameters(self):
         """
         Test serialization of FastembedSparseTextEmbedder to a dictionary, using custom initialization parameters.
         """
         embedder = FastembedSparseTextEmbedder(
             model="prithvida/Splade_PP_en_v1",
             cache_dir="fake_dir",
             threads=2,
             progress_bar=False,
             parallel=1,
+            local_files_only=True,
         )
         embedder_dict = embedder.to_dict()
         assert embedder_dict == {
             "type": "haystack_integrations.components.embedders.fastembed.fastembed_sparse_text_embedder.FastembedSparseTextEmbedder",  # noqa
             "init_parameters": {
                 "model": "prithvida/Splade_PP_en_v1",
                 "cache_dir": "fake_dir",
                 "threads": 2,
                 "progress_bar": False,
                 "parallel": 1,
+                "local_files_only": True,
             },
         }
 
     def test_from_dict(self):
         """
         Test deserialization of FastembedSparseTextEmbedder from a dictionary, using default initialization parameters.
         """
@@ -127,15 +130,15 @@
         """
         Test for checking embedder instances after warm-up.
         """
         embedder = FastembedSparseTextEmbedder(model="prithvida/Splade_PP_en_v1")
         mocked_factory.get_embedding_backend.assert_not_called()
         embedder.warm_up()
         mocked_factory.get_embedding_backend.assert_called_once_with(
-            model_name="prithvida/Splade_PP_en_v1", cache_dir=None, threads=None
+            model_name="prithvida/Splade_PP_en_v1", cache_dir=None, threads=None, local_files_only=False
         )
 
     @patch(
         "haystack_integrations.components.embedders.fastembed.fastembed_sparse_text_embedder._FastembedSparseEmbeddingBackendFactory"
     )
     def test_warmup_does_not_reload(self, mocked_factory):
         """
```

### Comparing `fastembed_haystack-1.0.0/tests/test_fastembed_text_embedder.py` & `fastembed_haystack-1.1.0/tests/test_fastembed_text_embedder.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,15 @@
                 "model": "BAAI/bge-small-en-v1.5",
                 "cache_dir": None,
                 "threads": None,
                 "prefix": "",
                 "suffix": "",
                 "progress_bar": True,
                 "parallel": None,
+                "local_files_only": False,
             },
         }
 
     def test_to_dict_with_custom_init_parameters(self):
         """
         Test serialization of FastembedTextEmbedder to a dictionary, using custom initialization parameters.
         """
@@ -70,26 +71,28 @@
             model="BAAI/bge-small-en-v1.5",
             cache_dir="fake_dir",
             threads=2,
             prefix="prefix",
             suffix="suffix",
             progress_bar=False,
             parallel=1,
+            local_files_only=True,
         )
         embedder_dict = embedder.to_dict()
         assert embedder_dict == {
             "type": "haystack_integrations.components.embedders.fastembed.fastembed_text_embedder.FastembedTextEmbedder",  # noqa
             "init_parameters": {
                 "model": "BAAI/bge-small-en-v1.5",
                 "cache_dir": "fake_dir",
                 "threads": 2,
                 "prefix": "prefix",
                 "suffix": "suffix",
                 "progress_bar": False,
                 "parallel": 1,
+                "local_files_only": True,
             },
         }
 
     def test_from_dict(self):
         """
         Test deserialization of FastembedTextEmbedder from a dictionary, using default initialization parameters.
         """
@@ -146,15 +149,15 @@
         """
         Test for checking embedder instances after warm-up.
         """
         embedder = FastembedTextEmbedder(model="BAAI/bge-small-en-v1.5")
         mocked_factory.get_embedding_backend.assert_not_called()
         embedder.warm_up()
         mocked_factory.get_embedding_backend.assert_called_once_with(
-            model_name="BAAI/bge-small-en-v1.5", cache_dir=None, threads=None
+            model_name="BAAI/bge-small-en-v1.5", cache_dir=None, threads=None, local_files_only=False
         )
 
     @patch(
         "haystack_integrations.components.embedders.fastembed.fastembed_text_embedder._FastembedEmbeddingBackendFactory"
     )
     def test_warmup_does_not_reload(self, mocked_factory):
         """
```

### Comparing `fastembed_haystack-1.0.0/.gitignore` & `fastembed_haystack-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-1.0.0/LICENSE.txt` & `fastembed_haystack-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-1.0.0/README.md` & `fastembed_haystack-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-1.0.0/pyproject.toml` & `fastembed_haystack-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastembed_haystack-1.0.0/PKG-INFO` & `fastembed_haystack-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fastembed-haystack
-Version: 1.0.0
+Version: 1.1.0
 Summary: Haystack 2.x component to embed strings and Documents using fastembed embedding model
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/fastembed/README.md
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

