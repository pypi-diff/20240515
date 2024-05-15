# Comparing `tmp/llama_index_graph_stores_kuzu-0.1.3.tar.gz` & `tmp/llama_index_graph_stores_kuzu-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_graph_stores_kuzu-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_graph_stores_kuzu-0.1.4.tar", max compression
```

## Comparing `llama_index_graph_stores_kuzu-0.1.3.tar` & `llama_index_graph_stores_kuzu-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       44 2024-04-26 15:45:20.627714 llama_index_graph_stores_kuzu-0.1.3/README.md
--rw-r--r--   0        0        0       92 2024-04-26 15:45:20.627714 llama_index_graph_stores_kuzu-0.1.3/llama_index/graph_stores/kuzu/__init__.py
--rw-r--r--   0        0        0     8690 2024-04-26 15:45:20.627714 llama_index_graph_stores_kuzu-0.1.3/llama_index/graph_stores/kuzu/base.py
--rw-r--r--   0        0        0     1463 2024-04-26 15:45:20.627714 llama_index_graph_stores_kuzu-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 llama_index_graph_stores_kuzu-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-05-15 16:23:26.146178 llama_index_graph_stores_kuzu-0.1.4/README.md
+-rw-r--r--   0        0        0       92 2024-05-15 16:23:26.146178 llama_index_graph_stores_kuzu-0.1.4/llama_index/graph_stores/kuzu/__init__.py
+-rw-r--r--   0        0        0     8690 2024-05-15 16:23:26.146178 llama_index_graph_stores_kuzu-0.1.4/llama_index/graph_stores/kuzu/base.py
+-rw-r--r--   0        0        0     1463 2024-05-15 16:23:26.146178 llama_index_graph_stores_kuzu-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 llama_index_graph_stores_kuzu-0.1.4/PKG-INFO
```

### Comparing `llama_index_graph_stores_kuzu-0.1.3/llama_index/graph_stores/kuzu/base.py` & `llama_index_graph_stores_kuzu-0.1.4/llama_index/graph_stores/kuzu/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_graph_stores_kuzu-0.1.3/pyproject.toml` & `llama_index_graph_stores_kuzu-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index graph stores kuzu integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-graph-stores-kuzu"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-kuzu = "^0.1.0"
+kuzu = "^0.4.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_graph_stores_kuzu-0.1.3/PKG-INFO` & `llama_index_graph_stores_kuzu-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-graph-stores-kuzu
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index graph stores kuzu integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: kuzu (>=0.1.0,<0.2.0)
+Requires-Dist: kuzu (>=0.4.0,<0.5.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Graph Stores Integration: Kuzu
```

