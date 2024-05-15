# Comparing `tmp/dify_knowledge_pipline-0.1.0.tar.gz` & `tmp/dify_knowledge_pipline-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dify_knowledge_pipline-0.1.0.tar", max compression
+gzip compressed data, was "dify_knowledge_pipline-0.1.1.tar", max compression
```

## Comparing `dify_knowledge_pipline-0.1.0.tar` & `dify_knowledge_pipline-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      445 2024-05-14 12:54:46.334252 dify_knowledge_pipline-0.1.0/dify_knowledge_pipline/__init__.py
--rw-r--r--   0        0        0    13885 2024-05-14 12:54:45.319572 dify_knowledge_pipline-0.1.0/dify_knowledge_pipline/client.py
--rw-r--r--   0        0        0     1738 2024-04-18 05:27:44.022979 dify_knowledge_pipline-0.1.0/dify_knowledge_pipline/errors.py
--rw-r--r--   0        0        0     8704 2024-05-14 02:07:08.811504 dify_knowledge_pipline-0.1.0/dify_knowledge_pipline/fire_drop.py
--rw-r--r--   0        0        0     1358 2024-05-14 02:07:08.723509 dify_knowledge_pipline-0.1.0/dify_knowledge_pipline/models.py
--rw-r--r--   0        0        0    10124 2024-05-14 12:39:24.703372 dify_knowledge_pipline-0.1.0/dify_knowledge_pipline/pipline.py
--rw-r--r--   0        0        0    11558 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.0/LICENSE
--rw-r--r--   0        0        0     2713 2024-05-14 12:42:20.773626 dify_knowledge_pipline-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       81 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.0/README.md
--rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 dify_knowledge_pipline-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      445 2024-05-14 12:54:46.334252 dify_knowledge_pipline-0.1.1/dify_knowledge_pipline/__init__.py
+-rw-r--r--   0        0        0    13885 2024-05-14 12:54:45.319572 dify_knowledge_pipline-0.1.1/dify_knowledge_pipline/client.py
+-rw-r--r--   0        0        0     1738 2024-04-18 05:27:44.022979 dify_knowledge_pipline-0.1.1/dify_knowledge_pipline/errors.py
+-rw-r--r--   0        0        0     8704 2024-05-14 02:07:08.811504 dify_knowledge_pipline-0.1.1/dify_knowledge_pipline/fire_drop.py
+-rw-r--r--   0        0        0     1358 2024-05-14 02:07:08.723509 dify_knowledge_pipline-0.1.1/dify_knowledge_pipline/models.py
+-rw-r--r--   0        0        0    10124 2024-05-14 12:39:24.703372 dify_knowledge_pipline-0.1.1/dify_knowledge_pipline/pipline.py
+-rw-r--r--   0        0        0    11558 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2717 2024-05-14 13:02:48.397221 dify_knowledge_pipline-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-05-14 12:36:07.583583 dify_knowledge_pipline-0.1.1/README.md
+-rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 dify_knowledge_pipline-0.1.1/PKG-INFO
```

### Comparing `dify_knowledge_pipline-0.1.0/dify_knowledge_pipline/client.py` & `dify_knowledge_pipline-0.1.1/dify_knowledge_pipline/client.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.0/dify_knowledge_pipline/errors.py` & `dify_knowledge_pipline-0.1.1/dify_knowledge_pipline/errors.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.0/dify_knowledge_pipline/fire_drop.py` & `dify_knowledge_pipline-0.1.1/dify_knowledge_pipline/fire_drop.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.0/dify_knowledge_pipline/models.py` & `dify_knowledge_pipline-0.1.1/dify_knowledge_pipline/models.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.0/dify_knowledge_pipline/pipline.py` & `dify_knowledge_pipline-0.1.1/dify_knowledge_pipline/pipline.py`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.0/LICENSE` & `dify_knowledge_pipline-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dify_knowledge_pipline-0.1.0/pyproject.toml` & `dify_knowledge_pipline-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # https://python-poetry.org/docs/libraries/#versioning
 # https://pypi.org/project/hcaptcha-challenger/#history
 
 [tool.poetry]
 name = "dify-knowledge-pipline"
-version = "0.1.0"
+version = "0.1.1"
 description = "🥂 Gracefully embedding multimodal-knowledge to Dify"
 license = "Apache License 2.0"
 authors = ["QIN2DIM <yaoqinse@gmail.com>", "Bingjie Yan <bj.yan.pa@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/QIN2DIM/hcaptcha-challenger"
 repository = "https://github.com/QIN2DIM/hcaptcha-challenger"
 documentation = "https://github.com/QIN2DIM/hcaptcha-challenger"
@@ -31,20 +31,20 @@
 
 # https://python-poetry.org/docs/pyproject/#dependencies-and-dependency-groups
 [tool.poetry.dependencies]
 python = "^3.10"
 
 # Run `poetry install` in the project root
 loguru = "*"
-pydantic = "^2.5.1"
+pydantic = "^2"
 tiktoken = "^0.7.0"
 tqdm = "*"
 python-dotenv = "*"
 langchain_text_splitters = "*"
-httpx = { version = "*", extras = ["http2"] }
+httpx = "*"
 
 [tool.poetry.group.test.dependencies]
 # https://docs.pytest.org/en/stable/reference/plugin_list.html#plugin-list
 # https://docs.pytest.org/en/stable/contents.html
 pytest = "*"
 # https://pytest-asyncio.readthedocs.io/en/latest/
 pytest-asyncio = "*"
@@ -65,9 +65,10 @@
 
 [tool.black]
 line-length = 100
 target-version = ["py310", "py311", "py312"]
 skip-magic-trailing-comma = true
 
 [build-system]
+# python -m build && twine upload dist/*
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dify_knowledge_pipline-0.1.0/PKG-INFO` & `dify_knowledge_pipline-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dify-knowledge-pipline
-Version: 0.1.0
+Version: 0.1.1
 Summary: 🥂 Gracefully embedding multimodal-knowledge to Dify
 Home-page: https://github.com/QIN2DIM/hcaptcha-challenger
 License: Apache-2.0
 Keywords: dify,RAG,dify-knowledge-pipline,multimodal-knowledge
 Author: QIN2DIM
 Author-email: yaoqinse@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -16,18 +16,18 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: httpx[http2]
+Requires-Dist: httpx
 Requires-Dist: langchain_text_splitters
 Requires-Dist: loguru
-Requires-Dist: pydantic (>=2.5.1,<3.0.0)
+Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: python-dotenv
 Requires-Dist: tiktoken (>=0.7.0,<0.8.0)
 Requires-Dist: tqdm
 Project-URL: Documentation, https://github.com/QIN2DIM/hcaptcha-challenger
 Project-URL: Repository, https://github.com/QIN2DIM/hcaptcha-challenger
 Description-Content-Type: text/markdown
```

