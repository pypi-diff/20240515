# Comparing `tmp/lavague_contexts_openai-0.1.0.tar.gz` & `tmp/lavague_contexts_openai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_contexts_openai-0.1.0.tar", max compression
+gzip compressed data, was "lavague_contexts_openai-0.1.1.tar", max compression
```

## Comparing `lavague_contexts_openai-0.1.0.tar` & `lavague_contexts_openai-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       32 2024-05-07 16:10:54.225089 lavague_contexts_openai-0.1.0/README.md
--rw-r--r--   0        0        0       54 2024-05-07 16:05:20.928684 lavague_contexts_openai-0.1.0/lavague/contexts/openai/__init__.py
--rw-r--r--   0        0        0     1084 2024-05-07 21:39:25.553331 lavague_contexts_openai-0.1.0/lavague/contexts/openai/base.py
--rw-r--r--   0        0        0     1029 2024-05-07 23:05:38.817404 lavague_contexts_openai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 lavague_contexts_openai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       32 2024-05-15 19:17:05.222186 lavague_contexts_openai-0.1.1/README.md
+-rw-r--r--   0        0        0       75 2024-05-15 19:17:05.222186 lavague_contexts_openai-0.1.1/lavague/contexts/openai/__init__.py
+-rw-r--r--   0        0        0     3021 2024-05-15 19:17:05.222186 lavague_contexts_openai-0.1.1/lavague/contexts/openai/base.py
+-rw-r--r--   0        0        0     1171 2024-05-15 21:18:44.468045 lavague_contexts_openai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 lavague_contexts_openai-0.1.1/PKG-INFO
```

### Comparing `lavague_contexts_openai-0.1.0/pyproject.toml` & `lavague_contexts_openai-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-contexts-openai"
-version = "0.1.0"
+version = "0.1.1"
 description = "Openai integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -16,15 +16,18 @@
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
 llama-index-llms-openai = "^0.1.9"
 llama-index-embeddings-openai = "^0.1.9"
+llama-index-llms-azure-openai = "^0.1.8"
+llama-index-multi-modal-llms-openai = "^0.1.6"
+llama-index-multi-modal-llms-azure-openai = "^0.1.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

