# Comparing `tmp/loose_dependency_manager-0.2.0.tar.gz` & `tmp/loose_dependency_manager-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loose_dependency_manager-0.2.0.tar", max compression
+gzip compressed data, was "loose_dependency_manager-0.2.1.tar", max compression
```

## Comparing `loose_dependency_manager-0.2.0.tar` & `loose_dependency_manager-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1056 2024-05-10 06:19:22.686343 loose_dependency_manager-0.2.0/LICENSE
--rw-r--r--   0        0        0     2170 2024-05-10 06:19:22.686343 loose_dependency_manager-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-10 06:19:22.686343 loose_dependency_manager-0.2.0/ldm/__init__.py
--rw-r--r--   0        0        0       59 2024-05-10 06:19:22.686343 loose_dependency_manager-0.2.0/ldm/__main__.py
--rw-r--r--   0        0        0        0 2024-05-10 06:19:22.686343 loose_dependency_manager-0.2.0/ldm/api/__init__.py
--rw-r--r--   0        0        0      190 2024-05-10 06:19:22.686343 loose_dependency_manager-0.2.0/ldm/api/config/__init__.py
--rw-r--r--   0        0        0      335 2024-05-10 06:19:22.686343 loose_dependency_manager-0.2.0/ldm/api/config/_dependency.py
--rw-r--r--   0        0        0      757 2024-05-10 06:19:22.686343 loose_dependency_manager-0.2.0/ldm/api/config/_installer.py
--rw-r--r--   0        0        0      215 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/config/_scheme.py
--rw-r--r--   0        0        0      175 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/factory/__init__.py
--rw-r--r--   0        0        0      250 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/factory/_factory.py
--rw-r--r--   0        0        0     1280 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/factory/_github.py
--rw-r--r--   0        0        0      678 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/factory/_http.py
--rw-r--r--   0        0        0      103 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/factory/_https.py
--rw-r--r--   0        0        0       92 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/installer/__init__.py
--rw-r--r--   0        0        0      365 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/installer/_dependency.py
--rw-r--r--   0        0        0     3062 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/installer/_installer.py
--rw-r--r--   0        0        0      204 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/installer/strategy/__init__.py
--rw-r--r--   0        0        0      632 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/installer/strategy/_create.py
--rw-r--r--   0        0        0      871 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/installer/strategy/_parallel.py
--rw-r--r--   0        0        0      385 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/installer/strategy/_sequential.py
--rw-r--r--   0        0        0      549 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/installer/strategy/_strategy.py
--rw-r--r--   0        0        0      192 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/parse.py
--rw-r--r--   0        0        0      114 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/scheme/__init__.py
--rw-r--r--   0        0        0     1037 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/scheme/_github.py
--rw-r--r--   0        0        0     1022 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/scheme/_http.py
--rw-r--r--   0        0        0      401 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/api/scheme/_scheme.py
--rw-r--r--   0        0        0       96 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/cli/__init__.py
--rw-r--r--   0        0        0      560 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/cli/_cli.py
--rw-r--r--   0        0        0      248 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/cli/_error.py
--rw-r--r--   0        0        0      478 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/cli/_logger.py
--rw-r--r--   0        0        0       89 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/commands/__init__.py
--rw-r--r--   0        0        0      362 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/commands/_command.py
--rw-r--r--   0        0        0      729 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/commands/_install.py
--rw-r--r--   0        0        0      202 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/component.py
--rw-r--r--   0        0        0      126 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/logger/__init__.py
--rw-r--r--   0        0        0     1575 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/logger/_click_logger.py
--rw-r--r--   0        0        0      831 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/logger/_logger.py
--rw-r--r--   0        0        0      428 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/logger/_noop_logger.py
--rw-r--r--   0        0        0        0 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/utils/__init__.py
--rw-r--r--   0        0        0       64 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/utils/mapping/__init__.py
--rw-r--r--   0        0        0      620 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/ldm/utils/mapping/_subscriptable.py
--rw-r--r--   0        0        0     1886 2024-05-10 06:19:22.690343 loose_dependency_manager-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3638 1970-01-01 00:00:00.000000 loose_dependency_manager-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2306 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/ldm/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/ldm/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/ldm/api/__init__.py
+-rw-r--r--   0        0        0      190 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/ldm/api/config/__init__.py
+-rw-r--r--   0        0        0      378 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/ldm/api/config/_dependency.py
+-rw-r--r--   0        0        0      757 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/ldm/api/config/_installer.py
+-rw-r--r--   0        0        0      215 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/ldm/api/config/_scheme.py
+-rw-r--r--   0        0        0      175 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/ldm/api/factory/__init__.py
+-rw-r--r--   0        0        0      250 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/ldm/api/factory/_factory.py
+-rw-r--r--   0        0        0     1280 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/ldm/api/factory/_github.py
+-rw-r--r--   0        0        0      678 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/ldm/api/factory/_http.py
+-rw-r--r--   0        0        0      103 2024-05-15 17:03:04.619178 loose_dependency_manager-0.2.1/ldm/api/factory/_https.py
+-rw-r--r--   0        0        0       92 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/installer/__init__.py
+-rw-r--r--   0        0        0      365 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/installer/_dependency.py
+-rw-r--r--   0        0        0     3062 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/installer/_installer.py
+-rw-r--r--   0        0        0      204 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/installer/strategy/__init__.py
+-rw-r--r--   0        0        0      632 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/installer/strategy/_create.py
+-rw-r--r--   0        0        0      871 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/installer/strategy/_parallel.py
+-rw-r--r--   0        0        0      385 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/installer/strategy/_sequential.py
+-rw-r--r--   0        0        0      549 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/installer/strategy/_strategy.py
+-rw-r--r--   0        0        0      192 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/parse.py
+-rw-r--r--   0        0        0      114 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/scheme/__init__.py
+-rw-r--r--   0        0        0     1037 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/scheme/_github.py
+-rw-r--r--   0        0        0     1022 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/scheme/_http.py
+-rw-r--r--   0        0        0      401 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/api/scheme/_scheme.py
+-rw-r--r--   0        0        0       96 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/cli/__init__.py
+-rw-r--r--   0        0        0      560 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/cli/_cli.py
+-rw-r--r--   0        0        0      248 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/cli/_error.py
+-rw-r--r--   0        0        0      478 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/cli/_logger.py
+-rw-r--r--   0        0        0       89 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/commands/__init__.py
+-rw-r--r--   0        0        0      362 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/commands/_command.py
+-rw-r--r--   0        0        0      729 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/commands/_install.py
+-rw-r--r--   0        0        0      202 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/component.py
+-rw-r--r--   0        0        0      126 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/logger/__init__.py
+-rw-r--r--   0        0        0     1575 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/logger/_click_logger.py
+-rw-r--r--   0        0        0      831 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/logger/_logger.py
+-rw-r--r--   0        0        0      428 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/logger/_noop_logger.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/utils/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/utils/mapping/__init__.py
+-rw-r--r--   0        0        0      620 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/ldm/utils/mapping/_subscriptable.py
+-rw-r--r--   0        0        0     1886 2024-05-15 17:03:04.623178 loose_dependency_manager-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3729 1970-01-01 00:00:00.000000 loose_dependency_manager-0.2.1/PKG-INFO
```

### Comparing `loose_dependency_manager-0.2.0/LICENSE` & `loose_dependency_manager-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/README.md` & `loose_dependency_manager-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,21 @@
 
 Finally, run `ldm install` to install the dependencies
 
 ```bash
 ldm install
 ```
 
+> [!NOTE]
+> You can also run `ldm install [...dependencies]` to install specific dependencies.
+>  
+> ```bash
+> ldm install clamp
+> ```
+
 ## API Documentation
 
 > TODO: description
 
 ## Contributing
 
 Any contribution is welcome! Check out [CONTRIBUTING.md](https://github.com/01Joseph-Hwang10/loose-dependency-manager/blob/master/.github/CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](https://github.com/01Joseph-Hwang10/loose-dependency-manager/blob/master/.github/CODE_OF_CONDUCT.md) for more information on how to get started.
```

### Comparing `loose_dependency_manager-0.2.0/ldm/api/config/_installer.py` & `loose_dependency_manager-0.2.1/ldm/api/config/_installer.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/api/factory/_github.py` & `loose_dependency_manager-0.2.1/ldm/api/factory/_github.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/api/factory/_http.py` & `loose_dependency_manager-0.2.1/ldm/api/factory/_http.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/api/installer/_installer.py` & `loose_dependency_manager-0.2.1/ldm/api/installer/_installer.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/api/installer/strategy/_create.py` & `loose_dependency_manager-0.2.1/ldm/api/installer/strategy/_create.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/api/installer/strategy/_parallel.py` & `loose_dependency_manager-0.2.1/ldm/api/installer/strategy/_parallel.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/api/installer/strategy/_strategy.py` & `loose_dependency_manager-0.2.1/ldm/api/installer/strategy/_strategy.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/api/scheme/_github.py` & `loose_dependency_manager-0.2.1/ldm/api/scheme/_github.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/api/scheme/_http.py` & `loose_dependency_manager-0.2.1/ldm/api/scheme/_http.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/cli/_cli.py` & `loose_dependency_manager-0.2.1/ldm/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/commands/_install.py` & `loose_dependency_manager-0.2.1/ldm/commands/_install.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/logger/_click_logger.py` & `loose_dependency_manager-0.2.1/ldm/logger/_click_logger.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/logger/_logger.py` & `loose_dependency_manager-0.2.1/ldm/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/ldm/utils/mapping/_subscriptable.py` & `loose_dependency_manager-0.2.1/ldm/utils/mapping/_subscriptable.py`

 * *Files identical despite different names*

### Comparing `loose_dependency_manager-0.2.0/pyproject.toml` & `loose_dependency_manager-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "loose-dependency-manager"
-version = "0.2.0"
+version = "0.2.1"
 description = "Tool for managing code dependencies in a loosely-coupled way."
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Developers',
   'Natural Language :: English',
   'Topic :: Software Development',
   'Topic :: Software Development :: Libraries :: Python Modules',
@@ -30,23 +30,23 @@
 python = ">=3.8.1,<4.0"
 click = "^8.1.7"
 pydantic = "^2.7.1"
 colorama = "^0.4.6"
 yaml-replace = "^1.1.2"
 git-remote-get = "^0.3.1"
 httpx = "^0.27.0"
-pytest-order = "^1.2.1"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.1.0"
 black = "^23.10.1"
 poethepoet = "^0.24.4"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.3"
+pytest-order = "^1.2.1"
 
 
 [tool.poetry.scripts]
 loose-dependency-manager = "ldm.__main__:cli"
 ldm = "ldm.__main__:cli"
 
 [tool.poe.tasks]
```

### Comparing `loose_dependency_manager-0.2.0/PKG-INFO` & `loose_dependency_manager-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loose-dependency-manager
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tool for managing code dependencies in a loosely-coupled way.
 License: MIT
 Author: 01Joseph-Hwang10
 Author-email: joseph95501@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: git-remote-get (>=0.3.1,<0.4.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
-Requires-Dist: pytest-order (>=1.2.1,<2.0.0)
 Requires-Dist: yaml-replace (>=1.1.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # `ldm`: Loose Dependency Manager
 
 [![PyPI version](https://badge.fury.io/py/loose-dependency-manager.svg)](https://pypi.org/project/loose-dependency-manager)
 [![Testsuite](https://github.com/01Joseph-Hwang10/loose-dependency-manager/workflows/Test%20and%20Lint/badge.svg)](https://github.com/01Joseph-Hwang10/loose-dependency-manager/actions?query=workflow%3A"Test+and+Lint")
@@ -75,14 +74,21 @@
 
 Finally, run `ldm install` to install the dependencies
 
 ```bash
 ldm install
 ```
 
+> [!NOTE]
+> You can also run `ldm install [...dependencies]` to install specific dependencies.
+>  
+> ```bash
+> ldm install clamp
+> ```
+
 ## API Documentation
 
 > TODO: description
 
 ## Contributing
 
 Any contribution is welcome! Check out [CONTRIBUTING.md](https://github.com/01Joseph-Hwang10/loose-dependency-manager/blob/master/.github/CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](https://github.com/01Joseph-Hwang10/loose-dependency-manager/blob/master/.github/CODE_OF_CONDUCT.md) for more information on how to get started.
```

