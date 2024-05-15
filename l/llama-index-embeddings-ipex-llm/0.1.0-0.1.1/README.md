# Comparing `tmp/llama_index_embeddings_ipex_llm-0.1.0.tar.gz` & `tmp/llama_index_embeddings_ipex_llm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_ipex_llm-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_embeddings_ipex_llm-0.1.1.tar", max compression
```

## Comparing `llama_index_embeddings_ipex_llm-0.1.0.tar` & `llama_index_embeddings_ipex_llm-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      324 2024-04-15 18:08:36.516335 llama_index_embeddings_ipex_llm-0.1.0/README.md
--rw-r--r--   0        0        0       17 2024-04-15 18:08:36.516335 llama_index_embeddings_ipex_llm-0.1.0/llama_index/embeddings/ipex_llm/BUILD
--rw-r--r--   0        0        0       99 2024-04-15 18:08:36.516335 llama_index_embeddings_ipex_llm-0.1.0/llama_index/embeddings/ipex_llm/__init__.py
--rw-r--r--   0        0        0     5197 2024-04-15 18:08:36.516335 llama_index_embeddings_ipex_llm-0.1.0/llama_index/embeddings/ipex_llm/base.py
--rw-r--r--   0        0        0     2391 2024-04-15 18:08:36.516335 llama_index_embeddings_ipex_llm-0.1.0/llama_index/embeddings/ipex_llm/utils.py
--rw-r--r--   0        0        0     1962 2024-04-15 18:08:36.516335 llama_index_embeddings_ipex_llm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 llama_index_embeddings_ipex_llm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      324 2024-05-15 21:02:03.552233 llama_index_embeddings_ipex_llm-0.1.1/README.md
+-rw-r--r--   0        0        0       17 2024-05-15 21:02:03.552233 llama_index_embeddings_ipex_llm-0.1.1/llama_index/embeddings/ipex_llm/BUILD
+-rw-r--r--   0        0        0       99 2024-05-15 21:02:03.552233 llama_index_embeddings_ipex_llm-0.1.1/llama_index/embeddings/ipex_llm/__init__.py
+-rw-r--r--   0        0        0     5243 2024-05-15 21:02:03.552233 llama_index_embeddings_ipex_llm-0.1.1/llama_index/embeddings/ipex_llm/base.py
+-rw-r--r--   0        0        0     2391 2024-05-15 21:02:03.552233 llama_index_embeddings_ipex_llm-0.1.1/llama_index/embeddings/ipex_llm/utils.py
+-rw-r--r--   0        0        0     2460 2024-05-15 21:02:03.552233 llama_index_embeddings_ipex_llm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 llama_index_embeddings_ipex_llm-0.1.1/PKG-INFO
```

### Comparing `llama_index_embeddings_ipex_llm-0.1.0/llama_index/embeddings/ipex_llm/base.py` & `llama_index_embeddings_ipex_llm-0.1.1/llama_index/embeddings/ipex_llm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file is adapted from
 # https://github.com/run-llama/llama_index/blob/main/llama-index-integrations/embeddings/llama-index-embeddings-huggingface/llama_index/embeddings/huggingface/base.py
 
 import logging
 from typing import Any, List, Optional
+from ipex_llm.transformers.convert import _optimize_pre, _optimize_post
 
 from llama_index.core.base.embeddings.base import (
     DEFAULT_EMBED_BATCH_SIZE,
     BaseEmbedding,
 )
 from llama_index.core.bridge.pydantic import Field, PrivateAttr
 from llama_index.core.callbacks import CallbackManager
@@ -79,19 +80,18 @@
                 or get_query_instruct_for_model_name(model_name),
                 "text": text_instruction
                 or get_text_instruct_for_model_name(model_name),
             },
             **model_kwargs,
         )
 
-        from ipex_llm.transformers.convert import _optimize_pre, _optimize_post
-
         if self._device == "cpu":
             self._model = _optimize_pre(self._model)
             self._model = _optimize_post(self._model)
+        # TODO: optimize using ipex-llm optimize_model
         elif self._device == "xpu":
             self._model = _optimize_pre(self._model)
             self._model = _optimize_post(self._model)
             self._model = self._model.half().to(self._device)
 
         if max_length:
             self._model.max_seq_length = max_length
```

### Comparing `llama_index_embeddings_ipex_llm-0.1.0/llama_index/embeddings/ipex_llm/utils.py` & `llama_index_embeddings_ipex_llm-0.1.1/llama_index/embeddings/ipex_llm/utils.py`

 * *Files identical despite different names*

