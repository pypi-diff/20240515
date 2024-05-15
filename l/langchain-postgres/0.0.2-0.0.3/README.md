# Comparing `tmp/langchain_postgres-0.0.2.tar.gz` & `tmp/langchain_postgres-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_postgres-0.0.2.tar", max compression
+gzip compressed data, was "langchain_postgres-0.0.3.tar", max compression
```

## Comparing `langchain_postgres-0.0.2.tar` & `langchain_postgres-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-15 16:22:55.224292 langchain_postgres-0.0.2/LICENSE
--rw-r--r--   0        0        0     4238 2024-04-15 16:22:55.224292 langchain_postgres-0.0.2/README.md
--rw-r--r--   0        0        0      621 2024-04-15 16:22:55.224292 langchain_postgres-0.0.2/langchain_postgres/__init__.py
--rw-r--r--   0        0        0     2914 2024-04-15 16:22:55.224292 langchain_postgres-0.0.2/langchain_postgres/_utils.py
--rw-r--r--   0        0        0    14033 2024-04-15 16:22:55.224292 langchain_postgres-0.0.2/langchain_postgres/chat_message_histories.py
--rw-r--r--   0        0        0    23519 2024-04-15 16:22:55.228292 langchain_postgres-0.0.2/langchain_postgres/checkpoint.py
--rw-r--r--   0        0        0        0 2024-04-15 16:22:55.228292 langchain_postgres-0.0.2/langchain_postgres/py.typed
--rw-r--r--   0        0        0    49908 2024-04-15 16:22:55.228292 langchain_postgres-0.0.2/langchain_postgres/vectorstores.py
--rw-r--r--   0        0        0     2127 2024-04-15 16:22:55.228292 langchain_postgres-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5186 1970-01-01 00:00:00.000000 langchain_postgres-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-17 02:13:43.091163 langchain_postgres-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4238 2024-04-17 02:13:43.091163 langchain_postgres-0.0.3/README.md
+-rw-r--r--   0        0        0      621 2024-04-17 02:13:43.091163 langchain_postgres-0.0.3/langchain_postgres/__init__.py
+-rw-r--r--   0        0        0     2914 2024-04-17 02:13:43.091163 langchain_postgres-0.0.3/langchain_postgres/_utils.py
+-rw-r--r--   0        0        0    14033 2024-04-17 02:13:43.091163 langchain_postgres-0.0.3/langchain_postgres/chat_message_histories.py
+-rw-r--r--   0        0        0    23519 2024-04-17 02:13:43.091163 langchain_postgres-0.0.3/langchain_postgres/checkpoint.py
+-rw-r--r--   0        0        0        0 2024-04-17 02:13:43.091163 langchain_postgres-0.0.3/langchain_postgres/py.typed
+-rw-r--r--   0        0        0    49908 2024-04-17 02:13:43.091163 langchain_postgres-0.0.3/langchain_postgres/vectorstores.py
+-rw-r--r--   0        0        0     2112 2024-04-17 02:13:43.095163 langchain_postgres-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5159 1970-01-01 00:00:00.000000 langchain_postgres-0.0.3/PKG-INFO
```

### Comparing `langchain_postgres-0.0.2/LICENSE` & `langchain_postgres-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.2/README.md` & `langchain_postgres-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.2/langchain_postgres/__init__.py` & `langchain_postgres-0.0.3/langchain_postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.2/langchain_postgres/_utils.py` & `langchain_postgres-0.0.3/langchain_postgres/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.2/langchain_postgres/chat_message_histories.py` & `langchain_postgres-0.0.3/langchain_postgres/chat_message_histories.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.2/langchain_postgres/checkpoint.py` & `langchain_postgres-0.0.3/langchain_postgres/checkpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.2/langchain_postgres/vectorstores.py` & `langchain_postgres-0.0.3/langchain_postgres/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain_postgres-0.0.2/pyproject.toml` & `langchain_postgres-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "langchain-postgres"
-version = "0.0.2"
+version = "0.0.3"
 description = "An integration package connecting Postgres and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-postgres"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 langchain-core = "^0.1"
-psycopg = "^3.1.18"
+psycopg = "^3"
 langgraph = "^0.0.32"
 psycopg-pool = "^3.2.1"
-sqlalchemy = "^2.0.29"
+sqlalchemy = "^2"
 pgvector = "^0.2.5"
-numpy = "^1.26.4"
+numpy = "^1"
 
 [tool.poetry.group.docs.dependencies]
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^3.6.1"
 
 [tool.poetry.group.test]
```

### Comparing `langchain_postgres-0.0.2/PKG-INFO` & `langchain_postgres-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: langchain-postgres
-Version: 0.0.2
+Version: 0.0.3
 Summary: An integration package connecting Postgres and LangChain
 Home-page: https://github.com/langchain-ai/langchain-postgres
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: langchain-core (>=0.1,<0.2)
 Requires-Dist: langgraph (>=0.0.32,<0.0.33)
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: numpy (>=1,<2)
 Requires-Dist: pgvector (>=0.2.5,<0.3.0)
-Requires-Dist: psycopg (>=3.1.18,<4.0.0)
+Requires-Dist: psycopg (>=3,<4)
 Requires-Dist: psycopg-pool (>=3.2.1,<4.0.0)
-Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
+Requires-Dist: sqlalchemy (>=2,<3)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-postgres
 Description-Content-Type: text/markdown
 
 # langchain-postgres
 
 The `langchain-postgres` package implementations of core LangChain abstractions using `Postgres`.
```

