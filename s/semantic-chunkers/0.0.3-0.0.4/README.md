# Comparing `tmp/semantic_chunkers-0.0.3.tar.gz` & `tmp/semantic_chunkers-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_chunkers-0.0.3.tar", max compression
+gzip compressed data, was "semantic_chunkers-0.0.4.tar", max compression
```

## Comparing `semantic_chunkers-0.0.3.tar` & `semantic_chunkers-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1067 2024-05-13 08:11:18.775424 semantic_chunkers-0.0.3/LICENSE
--rw-r--r--   0        0        0     1391 2024-05-13 08:11:18.775424 semantic_chunkers-0.0.3/README.md
--rw-r--r--   0        0        0     1006 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      358 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/__init__.py
--rw-r--r--   0        0        0      375 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/chunkers/__init__.py
--rw-r--r--   0        0        0     1521 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/chunkers/base.py
--rw-r--r--   0        0        0     2734 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/chunkers/consecutive.py
--rw-r--r--   0        0        0     3582 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/chunkers/cumulative.py
--rw-r--r--   0        0        0    18475 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/chunkers/statistical.py
--rw-r--r--   0        0        0      353 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/schema.py
--rw-r--r--   0        0        0        0 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/splitters/__init__.py
--rw-r--r--   0        0        0     2003 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/splitters/sentence.py
--rw-r--r--   0        0        0        0 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/utils/__init__.py
--rw-r--r--   0        0        0     1008 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/utils/logger.py
--rw-r--r--   0        0        0      192 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/utils/text.py
--rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 semantic_chunkers-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-15 17:40:17.975943 semantic_chunkers-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1397 2024-05-15 17:40:17.975943 semantic_chunkers-0.0.4/README.md
+-rw-r--r--   0        0        0     1015 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      358 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/__init__.py
+-rw-r--r--   0        0        0      375 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/chunkers/__init__.py
+-rw-r--r--   0        0        0     1521 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/chunkers/base.py
+-rw-r--r--   0        0        0     2734 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/chunkers/consecutive.py
+-rw-r--r--   0        0        0     3582 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/chunkers/cumulative.py
+-rw-r--r--   0        0        0    18475 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/chunkers/statistical.py
+-rw-r--r--   0        0        0      353 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/schema.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/splitters/__init__.py
+-rw-r--r--   0        0        0     2003 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/splitters/sentence.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/utils/__init__.py
+-rw-r--r--   0        0        0     1008 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/utils/logger.py
+-rw-r--r--   0        0        0      192 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/utils/text.py
+-rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 semantic_chunkers-0.0.4/PKG-INFO
```

### Comparing `semantic_chunkers-0.0.3/LICENSE` & `semantic_chunkers-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.3/README.md` & `semantic_chunkers-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,8 +19,10 @@
 
 ## 📚 Resources
 
 ### Docs
 
 | Notebook | Description |
 | -------- | ----------- |
-| [Introduction](https://github.com/aurelio-labs/semantic-chunkers/blob/main/docs/video-chunker.ipynb) | Chunking videos with semantics |
+| [Introduction](https://github.com/aurelio-labs/semantic-chunkers/blob/main/docs/01-video-chunking.ipynb) | Chunking videos with semantics |
+
+
```

### Comparing `semantic_chunkers-0.0.3/pyproject.toml` & `semantic_chunkers-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-chunkers"
-version = "0.0.3"
+version = "0.0.4"
 description = "Super advanced chunking methods for AI"
 authors = ["Aurelio AI <hello@aurelio.ai>"]
 readme = "README.md"
 packages = [{include = "semantic_chunkers"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
@@ -12,30 +12,30 @@
 numpy = "^1.25.2"
 colorlog = "^6.8.0"
 colorama = "^0.4.6"
 regex = "^2023.12.25"
 tiktoken = "^0.6.0"
 matplotlib = { version = "^3.8.3", optional = true}
 requests-mock = "^1.12.1"
-semantic-router = "^0.0.39"
+semantic-router = ">=0.0.20,<0.1.0"
 
 [tool.poetry.extras]
 stats = ["matplotlib"]
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.25.0"
 ruff = "^0.1.5"
 pytest = "^7.4.3"
 pytest-mock = "^3.12.0"
 pytest-cov = "^4.1.0"
 pytest-xdist = "^3.5.0"
 mypy = "^1.7.1"
 types-pyyaml = "^6.0.12.12"
 types-requests = "^2.31.0"
-black = "^24.0.0"
+black = "^23.12.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff.per-file-ignores]
 "*.ipynb" = ["ALL"]
```

### Comparing `semantic_chunkers-0.0.3/semantic_chunkers/chunkers/base.py` & `semantic_chunkers-0.0.4/semantic_chunkers/chunkers/base.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.3/semantic_chunkers/chunkers/consecutive.py` & `semantic_chunkers-0.0.4/semantic_chunkers/chunkers/consecutive.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.3/semantic_chunkers/chunkers/cumulative.py` & `semantic_chunkers-0.0.4/semantic_chunkers/chunkers/cumulative.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.3/semantic_chunkers/chunkers/statistical.py` & `semantic_chunkers-0.0.4/semantic_chunkers/chunkers/statistical.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.3/semantic_chunkers/splitters/sentence.py` & `semantic_chunkers-0.0.4/semantic_chunkers/splitters/sentence.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.3/semantic_chunkers/utils/logger.py` & `semantic_chunkers-0.0.4/semantic_chunkers/utils/logger.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.3/PKG-INFO` & `semantic_chunkers-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-chunkers
-Version: 0.0.3
+Version: 0.0.4
 Summary: Super advanced chunking methods for AI
 Author: Aurelio AI
 Author-email: hello@aurelio.ai
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: colorlog (>=6.8.0,<7.0.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0) ; extra == "stats"
 Requires-Dist: numpy (>=1.25.2,<2.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: regex (>=2023.12.25,<2024.0.0)
 Requires-Dist: requests-mock (>=1.12.1,<2.0.0)
-Requires-Dist: semantic-router (>=0.0.39,<0.0.40)
+Requires-Dist: semantic-router (>=0.0.20,<0.1.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Description-Content-Type: text/markdown
 
 [![Aurelio AI](https://pbs.twimg.com/profile_banners/1671498317455581184/1696285195/1500x500)](https://aurelio.ai)
 
 # Semantic Chunkers
 
@@ -42,9 +42,11 @@
 
 ## 📚 Resources
 
 ### Docs
 
 | Notebook | Description |
 | -------- | ----------- |
-| [Introduction](https://github.com/aurelio-labs/semantic-chunkers/blob/main/docs/video-chunker.ipynb) | Chunking videos with semantics |
+| [Introduction](https://github.com/aurelio-labs/semantic-chunkers/blob/main/docs/01-video-chunking.ipynb) | Chunking videos with semantics |
+
+
```

