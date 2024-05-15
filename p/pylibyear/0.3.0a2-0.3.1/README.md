# Comparing `tmp/pylibyear-0.3.0a2.tar.gz` & `tmp/pylibyear-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibyear-0.3.0a2.tar", last modified: Wed May 15 12:05:11 2024, max compression
+gzip compressed data, was "pylibyear-0.3.1.tar", last modified: Wed May 15 17:46:42 2024, max compression
```

## Comparing `pylibyear-0.3.0a2.tar` & `pylibyear-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 12:05:11.762125 pylibyear-0.3.0a2/
--rw-r--r--   0 sam        (501) staff       (20)     1067 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/LICENSE
--rw-r--r--   0 sam        (501) staff       (20)     6450 2024-05-15 12:05:11.761683 pylibyear-0.3.0a2/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)     5412 2024-05-15 08:42:21.000000 pylibyear-0.3.0a2/README.md
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 12:05:11.750206 pylibyear-0.3.0a2/libyear/
--rw-r--r--   0 sam        (501) staff       (20)        0 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/libyear/__init__.py
--rw-r--r--   0 sam        (501) staff       (20)     1329 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/libyear/main.py
--rw-r--r--   0 sam        (501) staff       (20)     3194 2024-05-15 07:31:25.000000 pylibyear-0.3.0a2/libyear/pypi.py
--rw-r--r--   0 sam        (501) staff       (20)      988 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/libyear/results.py
--rw-r--r--   0 sam        (501) staff       (20)     2470 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/libyear/toml.py
--rw-r--r--   0 sam        (501) staff       (20)     1651 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/libyear/utils.py
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 12:05:11.760923 pylibyear-0.3.0a2/pylibyear.egg-info/
--rw-r--r--   0 sam        (501) staff       (20)     6450 2024-05-15 12:05:11.000000 pylibyear-0.3.0a2/pylibyear.egg-info/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)      397 2024-05-15 12:05:11.000000 pylibyear-0.3.0a2/pylibyear.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (501) staff       (20)        1 2024-05-15 12:05:11.000000 pylibyear-0.3.0a2/pylibyear.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (501) staff       (20)       45 2024-05-15 12:05:11.000000 pylibyear-0.3.0a2/pylibyear.egg-info/entry_points.txt
--rw-r--r--   0 sam        (501) staff       (20)      147 2024-05-15 12:05:11.000000 pylibyear-0.3.0a2/pylibyear.egg-info/requires.txt
--rw-r--r--   0 sam        (501) staff       (20)        8 2024-05-15 12:05:11.000000 pylibyear-0.3.0a2/pylibyear.egg-info/top_level.txt
--rw-r--r--   0 sam        (501) staff       (20)     1160 2024-05-15 12:05:05.000000 pylibyear-0.3.0a2/pyproject.toml
--rw-r--r--   0 sam        (501) staff       (20)       38 2024-05-15 12:05:11.762181 pylibyear-0.3.0a2/setup.cfg
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 12:05:11.760543 pylibyear-0.3.0a2/tests/
--rw-r--r--   0 sam        (501) staff       (20)     4149 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/tests/test_libyear.py
--rw-r--r--   0 sam        (501) staff       (20)     1774 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/tests/test_toml.py
--rw-r--r--   0 sam        (501) staff       (20)      590 2024-05-14 19:54:29.000000 pylibyear-0.3.0a2/tests/test_utils.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 17:46:42.407688 pylibyear-0.3.1/
+-rw-r--r--   0 sam        (501) staff       (20)     1067 2024-05-15 17:38:45.000000 pylibyear-0.3.1/LICENSE
+-rw-r--r--   0 sam        (501) staff       (20)     6569 2024-05-15 17:46:42.407254 pylibyear-0.3.1/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)     5465 2024-05-15 17:39:03.000000 pylibyear-0.3.1/README.md
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 17:46:42.354378 pylibyear-0.3.1/libyear/
+-rw-r--r--   0 sam        (501) staff       (20)        0 2024-05-14 19:54:29.000000 pylibyear-0.3.1/libyear/__init__.py
+-rw-r--r--   0 sam        (501) staff       (20)     1329 2024-05-14 19:54:29.000000 pylibyear-0.3.1/libyear/main.py
+-rw-r--r--   0 sam        (501) staff       (20)     3194 2024-05-15 17:39:03.000000 pylibyear-0.3.1/libyear/pypi.py
+-rw-r--r--   0 sam        (501) staff       (20)      988 2024-05-14 19:54:29.000000 pylibyear-0.3.1/libyear/results.py
+-rw-r--r--   0 sam        (501) staff       (20)     2470 2024-05-14 19:54:29.000000 pylibyear-0.3.1/libyear/toml.py
+-rw-r--r--   0 sam        (501) staff       (20)     1651 2024-05-14 19:54:29.000000 pylibyear-0.3.1/libyear/utils.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 17:46:42.405690 pylibyear-0.3.1/pylibyear.egg-info/
+-rw-r--r--   0 sam        (501) staff       (20)     6569 2024-05-15 17:46:42.000000 pylibyear-0.3.1/pylibyear.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)      397 2024-05-15 17:46:42.000000 pylibyear-0.3.1/pylibyear.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (501) staff       (20)        1 2024-05-15 17:46:42.000000 pylibyear-0.3.1/pylibyear.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (501) staff       (20)       45 2024-05-15 17:46:42.000000 pylibyear-0.3.1/pylibyear.egg-info/entry_points.txt
+-rw-r--r--   0 sam        (501) staff       (20)      169 2024-05-15 17:46:42.000000 pylibyear-0.3.1/pylibyear.egg-info/requires.txt
+-rw-r--r--   0 sam        (501) staff       (20)        8 2024-05-15 17:46:42.000000 pylibyear-0.3.1/pylibyear.egg-info/top_level.txt
+-rw-r--r--   0 sam        (501) staff       (20)     1133 2024-05-15 17:45:52.000000 pylibyear-0.3.1/pyproject.toml
+-rw-r--r--   0 sam        (501) staff       (20)       38 2024-05-15 17:46:42.407741 pylibyear-0.3.1/setup.cfg
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-15 17:46:42.403837 pylibyear-0.3.1/tests/
+-rw-r--r--   0 sam        (501) staff       (20)     4149 2024-05-14 19:54:29.000000 pylibyear-0.3.1/tests/test_libyear.py
+-rw-r--r--   0 sam        (501) staff       (20)     1774 2024-05-14 19:54:29.000000 pylibyear-0.3.1/tests/test_toml.py
+-rw-r--r--   0 sam        (501) staff       (20)      590 2024-05-14 19:54:29.000000 pylibyear-0.3.1/tests/test_utils.py
```

### Comparing `pylibyear-0.3.0a2/LICENSE` & `pylibyear-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a2/PKG-INFO` & `pylibyear-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibyear
-Version: 0.3.0a2
+Version: 0.3.1
 Summary: A simple measure of software dependency freshness.
 Author: nasirhjafri
 Author-email: Sam Atkins <samatkins@outlook.com>
 License: MIT License
 Project-URL: Documentation, https://github.com/sam-atkins/pylibyear#readme
 Project-URL: Issues, https://github.com/sam-atkins/pylibyear/issues
 Project-URL: Source, https://github.com/sam-atkins/pylibyear
@@ -20,35 +20,43 @@
 Requires-Dist: prettytable>=3.10.0
 Requires-Dist: python-dateutil>=2.9.0.post0
 Requires-Dist: typer>=0.12.3
 Provides-Extra: dev
 Requires-Dist: pytest>=8.2.0; extra == "dev"
 Requires-Dist: pytest-vcr>=1.0.2; extra == "dev"
 Requires-Dist: ruff>=0.4.4; extra == "dev"
+Provides-Extra: build
+Requires-Dist: build==1.2.1; extra == "build"
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/nasirhjafri/libyear/)
+[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/sam-atkins/pylibyear/)
 [![PyPI version fury.io](https://badge.fury.io/py/libyear.svg)](https://pypi.python.org/pypi/pylibyear/)
 
-# pylibyear
-
 **This is a fork of [libyear](https://github.com/nasirhjafri/libyear) as it appears to no longer be maintained.**
 
-# libyear
+# [py]libyear
 
 A **simple** measure of software dependency freshness. It is a **single number** telling you how up-to-date your dependencies are.
 
 https://libyear.com/
 
 ![Demo Image](./docs/demo.png)
 
 ## How to install
 
+Using pip
+
+```bash
+pip install pylibyear
+```
+
+Using pipx
+
 ```bash
-pip install libyear
+pipx install pylibyear
 ```
 
 ## Usage
 
 ```bash
 libyear --help
 ```
```

### Comparing `pylibyear-0.3.0a2/README.md` & `pylibyear-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/nasirhjafri/libyear/)
+[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/sam-atkins/pylibyear/)
 [![PyPI version fury.io](https://badge.fury.io/py/libyear.svg)](https://pypi.python.org/pypi/pylibyear/)
 
-# pylibyear
-
 **This is a fork of [libyear](https://github.com/nasirhjafri/libyear) as it appears to no longer be maintained.**
 
-# libyear
+# [py]libyear
 
 A **simple** measure of software dependency freshness. It is a **single number** telling you how up-to-date your dependencies are.
 
 https://libyear.com/
 
 ![Demo Image](./docs/demo.png)
 
 ## How to install
 
+Using pip
+
+```bash
+pip install pylibyear
+```
+
+Using pipx
+
 ```bash
-pip install libyear
+pipx install pylibyear
 ```
 
 ## Usage
 
 ```bash
 libyear --help
 ```
```

### Comparing `pylibyear-0.3.0a2/libyear/main.py` & `pylibyear-0.3.1/libyear/main.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a2/libyear/pypi.py` & `pylibyear-0.3.1/libyear/pypi.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a2/libyear/results.py` & `pylibyear-0.3.1/libyear/results.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a2/libyear/toml.py` & `pylibyear-0.3.1/libyear/toml.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a2/libyear/utils.py` & `pylibyear-0.3.1/libyear/utils.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a2/pylibyear.egg-info/PKG-INFO` & `pylibyear-0.3.1/pylibyear.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibyear
-Version: 0.3.0a2
+Version: 0.3.1
 Summary: A simple measure of software dependency freshness.
 Author: nasirhjafri
 Author-email: Sam Atkins <samatkins@outlook.com>
 License: MIT License
 Project-URL: Documentation, https://github.com/sam-atkins/pylibyear#readme
 Project-URL: Issues, https://github.com/sam-atkins/pylibyear/issues
 Project-URL: Source, https://github.com/sam-atkins/pylibyear
@@ -20,35 +20,43 @@
 Requires-Dist: prettytable>=3.10.0
 Requires-Dist: python-dateutil>=2.9.0.post0
 Requires-Dist: typer>=0.12.3
 Provides-Extra: dev
 Requires-Dist: pytest>=8.2.0; extra == "dev"
 Requires-Dist: pytest-vcr>=1.0.2; extra == "dev"
 Requires-Dist: ruff>=0.4.4; extra == "dev"
+Provides-Extra: build
+Requires-Dist: build==1.2.1; extra == "build"
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/nasirhjafri/libyear/)
+[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/sam-atkins/pylibyear/)
 [![PyPI version fury.io](https://badge.fury.io/py/libyear.svg)](https://pypi.python.org/pypi/pylibyear/)
 
-# pylibyear
-
 **This is a fork of [libyear](https://github.com/nasirhjafri/libyear) as it appears to no longer be maintained.**
 
-# libyear
+# [py]libyear
 
 A **simple** measure of software dependency freshness. It is a **single number** telling you how up-to-date your dependencies are.
 
 https://libyear.com/
 
 ![Demo Image](./docs/demo.png)
 
 ## How to install
 
+Using pip
+
+```bash
+pip install pylibyear
+```
+
+Using pipx
+
 ```bash
-pip install libyear
+pipx install pylibyear
 ```
 
 ## Usage
 
 ```bash
 libyear --help
 ```
```

### Comparing `pylibyear-0.3.0a2/pyproject.toml` & `pylibyear-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pylibyear"
-version = "0.3.0a2"
+version = "0.3.1"
 description = "A simple measure of software dependency freshness."
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "MIT License"}
 keywords = []
 authors = [
   { name = "nasirhjafri" },
@@ -30,18 +30,18 @@
 
 [project.optional-dependencies]
 dev = [
     "pytest>=8.2.0",
     "pytest-vcr>=1.0.2",
     "ruff>=0.4.4",
 ]
+build = [
+    "build==1.2.1",
+]
 
 [project.scripts]
 libyear = "libyear.main:app"
 
 [project.urls]
 Documentation = "https://github.com/sam-atkins/pylibyear#readme"
 Issues = "https://github.com/sam-atkins/pylibyear/issues"
 Source = "https://github.com/sam-atkins/pylibyear"
-
-[tool.hatch.build.targets.wheel]
-packages = ["libyear"]
```

### Comparing `pylibyear-0.3.0a2/tests/test_libyear.py` & `pylibyear-0.3.1/tests/test_libyear.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a2/tests/test_toml.py` & `pylibyear-0.3.1/tests/test_toml.py`

 * *Files identical despite different names*

### Comparing `pylibyear-0.3.0a2/tests/test_utils.py` & `pylibyear-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

