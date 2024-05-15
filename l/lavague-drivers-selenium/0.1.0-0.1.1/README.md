# Comparing `tmp/lavague_drivers_selenium-0.1.0.tar.gz` & `tmp/lavague_drivers_selenium-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_drivers_selenium-0.1.0.tar", max compression
+gzip compressed data, was "lavague_drivers_selenium-0.1.1.tar", max compression
```

## Comparing `lavague_drivers_selenium-0.1.0.tar` & `lavague_drivers_selenium-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       34 2024-05-07 15:58:18.809098 lavague_drivers_selenium-0.1.0/README.md
--rw-r--r--   0        0        0       56 2024-05-07 15:49:52.721907 lavague_drivers_selenium-0.1.0/lavague/drivers/selenium/__init__.py
--rw-r--r--   0        0        0     9380 2024-05-07 23:54:46.316092 lavague_drivers_selenium-0.1.0/lavague/drivers/selenium/base.py
--rw-r--r--   0        0        0      973 2024-05-07 15:57:47.649413 lavague_drivers_selenium-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1236 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-05-15 19:17:05.222186 lavague_drivers_selenium-0.1.1/README.md
+-rw-r--r--   0        0        0       57 2024-05-15 19:17:05.222186 lavague_drivers_selenium-0.1.1/lavague/drivers/selenium/__init__.py
+-rw-r--r--   0        0        0    12962 2024-05-15 19:17:05.222186 lavague_drivers_selenium-0.1.1/lavague/drivers/selenium/base.py
+-rw-r--r--   0        0        0      976 2024-05-15 21:18:31.036236 lavague_drivers_selenium-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.1.1/PKG-INFO
```

### Comparing `lavague_drivers_selenium-0.1.0/pyproject.toml` & `lavague_drivers_selenium-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-drivers-selenium"
-version = "0.1.0"
+version = "0.1.1"
 description = "Selenium integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -16,14 +16,14 @@
 keywords = ["LAM", "action", "automation", "LLM", "NLP", "RAG", "selenium", "selenium"]
 homepage = "https://lavague.ai"
 repository = "https://github.com/lavague-ai/LaVague/"
 documentation = "https://docs.lavague.ai/en/latest/"
 packages = [{include = "lavague/"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-lavague-core = "^0.1.0"
+python = "^3.10.0"
+lavague-core = "^0.1.1"
 selenium = "^4.18.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lavague_drivers_selenium-0.1.0/PKG-INFO` & `lavague_drivers_selenium-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: lavague-drivers-selenium
-Version: 0.1.0
+Version: 0.1.1
 Summary: Selenium integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,selenium
 Author: lavague-ai
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: lavague-core (>=0.1.0,<0.2.0)
+Requires-Dist: lavague-core (>=0.1.1,<0.2.0)
 Requires-Dist: selenium (>=4.18.1,<5.0.0)
 Project-URL: Documentation, https://docs.lavague.ai/en/latest/
 Project-URL: Repository, https://github.com/lavague-ai/LaVague/
 Description-Content-Type: text/markdown
 
 # Selenium integration for lavague
```

