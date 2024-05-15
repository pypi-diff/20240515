# Comparing `tmp/langchain_robocorp-0.0.6.tar.gz` & `tmp/langchain_robocorp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_robocorp-0.0.6.tar", max compression
+gzip compressed data, was "langchain_robocorp-0.0.7.tar", max compression
```

## Comparing `langchain_robocorp-0.0.6.tar` & `langchain_robocorp-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/LICENSE
--rw-r--r--   0        0        0      420 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/README.md
--rw-r--r--   0        0        0      102 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/langchain_robocorp/__init__.py
--rw-r--r--   0        0        0     4568 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/langchain_robocorp/_common.py
--rw-r--r--   0        0        0      525 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/langchain_robocorp/_prompts.py
--rw-r--r--   0        0        0        0 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/langchain_robocorp/py.typed
--rw-r--r--   0        0        0     7500 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/langchain_robocorp/toolkits.py
--rw-r--r--   0        0        0     2552 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 langchain_robocorp-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/LICENSE
+-rw-r--r--   0        0        0      420 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/README.md
+-rw-r--r--   0        0        0      102 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/langchain_robocorp/__init__.py
+-rw-r--r--   0        0        0     4568 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/langchain_robocorp/_common.py
+-rw-r--r--   0        0        0      525 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/langchain_robocorp/_prompts.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/langchain_robocorp/py.typed
+-rw-r--r--   0        0        0     7500 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/langchain_robocorp/toolkits.py
+-rw-r--r--   0        0        0     2558 2024-05-15 21:31:05.498281 langchain_robocorp-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 langchain_robocorp-0.0.7/PKG-INFO
```

### Comparing `langchain_robocorp-0.0.6/LICENSE` & `langchain_robocorp-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.6/langchain_robocorp/_common.py` & `langchain_robocorp-0.0.7/langchain_robocorp/_common.py`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.6/langchain_robocorp/_prompts.py` & `langchain_robocorp-0.0.7/langchain_robocorp/_prompts.py`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.6/langchain_robocorp/toolkits.py` & `langchain_robocorp-0.0.7/langchain_robocorp/toolkits.py`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.6/pyproject.toml` & `langchain_robocorp-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-robocorp"
-version = "0.0.6"
+version = "0.0.7"
 description = "An integration package connecting Robocorp Action Server and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/robocorp"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.31"
+langchain-core = ">=0.1.52,<0.3"
 requests = "^2.31.0"
 types-requests = "^2.31.0.6"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `langchain_robocorp-0.0.6/PKG-INFO` & `langchain_robocorp-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-robocorp
-Version: 0.0.6
+Version: 0.0.7
 Summary: An integration package connecting Robocorp Action Server and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1.31,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.52,<0.3)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: types-requests (>=2.31.0.6,<3.0.0.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/robocorp
 Description-Content-Type: text/markdown
 
 # langchain-robocorp
```

