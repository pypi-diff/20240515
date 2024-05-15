# Comparing `tmp/pylibyear-0.3.0a0.tar.gz` & `tmp/pylibyear-0.3.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pylibyear-0.3.0a2.tar", last modified: Wed May 15 12:05:11 2024, max compression
```

## Comparing `pylibyear-0.3.0a0.tar` & `pylibyear-0.3.0a2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/Taskfile.yaml
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/.github/workflows/pythonpackage.yml
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/.github/workflows/pythonpublish.yml
--rw-r--r--   0        0        0   106530 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/docs/demo.png
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/libyear/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/libyear/__init__.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/libyear/main.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/libyear/pypi.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/libyear/results.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/libyear/toml.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/libyear/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/tests/__init__.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/tests/test_libyear.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/tests/test_toml.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/tests/test_utils.py
--rw-r--r--   0        0        0  6191903 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/tests/cassettes/tests.test_libyear/test_libyear_main_output.yaml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/tests/data/pyproject.toml
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/tests/data/pyproject_poetry.toml
--rw-r--r--   0        0        0    15432 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/tests/data/requirements.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/LICENSE
--rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/README.md
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/pyproject.toml
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 pylibyear-0.3.0a0/PKG-INFO
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 12:05:11.762125 pylibyear-0.3.0a2/
+-rw-r--r--   0 sam        (501) staff       (20)     1067 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/LICENSE
+-rw-r--r--   0 sam        (501) staff       (20)     6450 2024-05-15 12:05:11.761683 pylibyear-0.3.0a2/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)     5412 2024-05-15 08:42:21.000000 pylibyear-0.3.0a2/README.md
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 12:05:11.750206 pylibyear-0.3.0a2/libyear/
+-rw-r--r--   0 sam        (501) staff       (20)        0 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/libyear/__init__.py
+-rw-r--r--   0 sam        (501) staff       (20)     1329 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/libyear/main.py
+-rw-r--r--   0 sam        (501) staff       (20)     3194 2024-05-15 07:31:25.000000 pylibyear-0.3.0a2/libyear/pypi.py
+-rw-r--r--   0 sam        (501) staff       (20)      988 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/libyear/results.py
+-rw-r--r--   0 sam        (501) staff       (20)     2470 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/libyear/toml.py
+-rw-r--r--   0 sam        (501) staff       (20)     1651 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/libyear/utils.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 12:05:11.760923 pylibyear-0.3.0a2/pylibyear.egg-info/
+-rw-r--r--   0 sam        (501) staff       (20)     6450 2024-05-15 12:05:11.000000 pylibyear-0.3.0a2/pylibyear.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)      397 2024-05-15 12:05:11.000000 pylibyear-0.3.0a2/pylibyear.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (501) staff       (20)        1 2024-05-15 12:05:11.000000 pylibyear-0.3.0a2/pylibyear.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (501) staff       (20)       45 2024-05-15 12:05:11.000000 pylibyear-0.3.0a2/pylibyear.egg-info/entry_points.txt
+-rw-r--r--   0 sam        (501) staff       (20)      147 2024-05-15 12:05:11.000000 pylibyear-0.3.0a2/pylibyear.egg-info/requires.txt
+-rw-r--r--   0 sam        (501) staff       (20)        8 2024-05-15 12:05:11.000000 pylibyear-0.3.0a2/pylibyear.egg-info/top_level.txt
+-rw-r--r--   0 sam        (501) staff       (20)     1160 2024-05-15 12:05:05.000000 pylibyear-0.3.0a2/pyproject.toml
+-rw-r--r--   0 sam        (501) staff       (20)       38 2024-05-15 12:05:11.762181 pylibyear-0.3.0a2/setup.cfg
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 12:05:11.760543 pylibyear-0.3.0a2/tests/
+-rw-r--r--   0 sam        (501) staff       (20)     4149 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/tests/test_libyear.py
+-rw-r--r--   0 sam        (501) staff       (20)     1774 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/tests/test_toml.py
+-rw-r--r--   0 sam        (501) staff       (20)      590 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/tests/test_utils.py
```

### Comparing `pylibyear-0.3.0a0/libyear/main.py` & `pylibyear-0.3.0a2/libyear/main.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a0/libyear/pypi.py` & `pylibyear-0.3.0a2/libyear/pypi.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a0/libyear/results.py` & `pylibyear-0.3.0a2/libyear/results.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a0/libyear/toml.py` & `pylibyear-0.3.0a2/libyear/toml.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a0/libyear/utils.py` & `pylibyear-0.3.0a2/libyear/utils.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a0/tests/test_libyear.py` & `pylibyear-0.3.0a2/tests/test_libyear.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a0/tests/test_toml.py` & `pylibyear-0.3.0a2/tests/test_toml.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a0/tests/test_utils.py` & `pylibyear-0.3.0a2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a0/LICENSE` & `pylibyear-0.3.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a0/README.md` & `pylibyear-0.3.0a2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/nasirhjafri/libyear/)
-[![PyPI version fury.io](https://badge.fury.io/py/libyear.svg)](https://pypi.python.org/pypi/libyear/)
-[![GitHub contributors](https://img.shields.io/github/contributors/nasirhjafri/libyear.svg)](https://GitHub.com/nasirhjafri/libyear/graphs/contributors/)
+[![PyPI version fury.io](https://badge.fury.io/py/libyear.svg)](https://pypi.python.org/pypi/pylibyear/)
 
+# pylibyear
+
+**This is a fork of [libyear](https://github.com/nasirhjafri/libyear) as it appears to no longer be maintained.**
 
 # libyear
 
 A **simple** measure of software dependency freshness. It is a **single number** telling you how up-to-date your dependencies are.
 
 https://libyear.com/
```

### Comparing `pylibyear-0.3.0a0/pyproject.toml` & `pylibyear-0.3.0a2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools >= 61.0"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "pylibyear"
-dynamic = ["version"]
+version = "0.3.0a2"
 description = "A simple measure of software dependency freshness."
 readme = "README.md"
 requires-python = ">=3.11"
-license = "MIT"
+license = {text = "MIT License"}
 keywords = []
 authors = [
+  { name = "nasirhjafri" },
   { name = "Sam Atkins", email = "samatkins@outlook.com" },
 ]
 classifiers = [
-  "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
-  "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "requests>=2.31.0",
     "packaging>=24.0",
     "prettytable>=3.10.0",
     "python-dateutil>=2.9.0.post0",
@@ -40,38 +39,9 @@
 libyear = "libyear.main:app"
 
 [project.urls]
 Documentation = "https://github.com/sam-atkins/pylibyear#readme"
 Issues = "https://github.com/sam-atkins/pylibyear/issues"
 Source = "https://github.com/sam-atkins/pylibyear"
 
-[tool.hatch.version]
-path = "libyear/__about__.py"
-
-[tool.hatch.envs.types]
-extra-dependencies = [
-  "mypy>=1.0.0",
-]
-[tool.hatch.envs.types.scripts]
-check = "mypy --install-types --non-interactive {args:src/pylibyear tests}"
-
-[tool.coverage.run]
-source_pkgs = ["pylibyear", "tests"]
-branch = true
-parallel = true
-omit = [
-  "src/pylibyear/__about__.py",
-]
-
-[tool.coverage.paths]
-pylibyear = ["src/pylibyear", "*/pylibyear/src/pylibyear"]
-tests = ["tests", "*/pylibyear/tests"]
-
-[tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-]
-
 [tool.hatch.build.targets.wheel]
 packages = ["libyear"]
```

### Comparing `pylibyear-0.3.0a0/PKG-INFO` & `pylibyear-0.3.0a2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: pylibyear
-Version: 0.3.0a0
+Version: 0.3.0a2
 Summary: A simple measure of software dependency freshness.
+Author: nasirhjafri
+Author-email: Sam Atkins <samatkins@outlook.com>
+License: MIT License
 Project-URL: Documentation, https://github.com/sam-atkins/pylibyear#readme
 Project-URL: Issues, https://github.com/sam-atkins/pylibyear/issues
 Project-URL: Source, https://github.com/sam-atkins/pylibyear
-Author-email: Sam Atkins <samatkins@outlook.com>
-License-Expression: MIT
-License-File: LICENSE
-Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31.0
 Requires-Dist: packaging>=24.0
 Requires-Dist: prettytable>=3.10.0
 Requires-Dist: python-dateutil>=2.9.0.post0
-Requires-Dist: requests>=2.31.0
 Requires-Dist: typer>=0.12.3
 Provides-Extra: dev
-Requires-Dist: pytest-vcr>=1.0.2; extra == 'dev'
-Requires-Dist: pytest>=8.2.0; extra == 'dev'
-Requires-Dist: ruff>=0.4.4; extra == 'dev'
-Description-Content-Type: text/markdown
+Requires-Dist: pytest>=8.2.0; extra == "dev"
+Requires-Dist: pytest-vcr>=1.0.2; extra == "dev"
+Requires-Dist: ruff>=0.4.4; extra == "dev"
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/nasirhjafri/libyear/)
-[![PyPI version fury.io](https://badge.fury.io/py/libyear.svg)](https://pypi.python.org/pypi/libyear/)
-[![GitHub contributors](https://img.shields.io/github/contributors/nasirhjafri/libyear.svg)](https://GitHub.com/nasirhjafri/libyear/graphs/contributors/)
+[![PyPI version fury.io](https://badge.fury.io/py/libyear.svg)](https://pypi.python.org/pypi/pylibyear/)
+
+# pylibyear
 
+**This is a fork of [libyear](https://github.com/nasirhjafri/libyear) as it appears to no longer be maintained.**
 
 # libyear
 
 A **simple** measure of software dependency freshness. It is a **single number** telling you how up-to-date your dependencies are.
 
 https://libyear.com/
```

