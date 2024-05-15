# Comparing `tmp/rcmpy-1.5.4.tar.gz` & `tmp/rcmpy-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-1.5.4.tar", last modified: Mon Apr 29 04:18:15 2024, max compression
+gzip compressed data, was "rcmpy-1.5.5.tar", last modified: Wed May 15 07:39:41 2024, max compression
```

## Comparing `rcmpy-1.5.4.tar` & `rcmpy-1.5.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.318467 rcmpy-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-29 04:17:00.000000 rcmpy-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-29 04:18:15.318467 rcmpy-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-29 04:17:00.000000 rcmpy-1.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-29 04:17:00.000000 rcmpy-1.5.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.310467 rcmpy-1.5.4/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/config/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.310467 rcmpy-1.5.4/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/environment/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/watch/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/watch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/watch/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.314468 rcmpy-1.5.4/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-29 04:17:00.000000 rcmpy-1.5.4/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.318467 rcmpy-1.5.4/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-29 04:18:15.000000 rcmpy-1.5.4/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 04:18:15.000000 rcmpy-1.5.4/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:18:15.000000 rcmpy-1.5.4/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 04:18:15.000000 rcmpy-1.5.4/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-29 04:18:15.000000 rcmpy-1.5.4/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 04:18:15.000000 rcmpy-1.5.4/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 04:18:15.318467 rcmpy-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-29 04:17:00.000000 rcmpy-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:18:15.318467 rcmpy-1.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-29 04:17:00.000000 rcmpy-1.5.4/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-29 04:17:00.000000 rcmpy-1.5.4/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-29 04:17:00.000000 rcmpy-1.5.4/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.191437 rcmpy-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 07:38:41.000000 rcmpy-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-05-15 07:39:41.191437 rcmpy-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-15 07:38:41.000000 rcmpy-1.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-15 07:38:41.000000 rcmpy-1.5.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.187436 rcmpy-1.5.5/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.187436 rcmpy-1.5.5/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.187436 rcmpy-1.5.5/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/config/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.183436 rcmpy-1.5.5/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.187436 rcmpy-1.5.5/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.187436 rcmpy-1.5.5/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/environment/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.191437 rcmpy-1.5.5/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.191437 rcmpy-1.5.5/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.191437 rcmpy-1.5.5/rcmpy/watch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/watch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/watch/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.191437 rcmpy-1.5.5/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-15 07:38:41.000000 rcmpy-1.5.5/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.191437 rcmpy-1.5.5/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-05-15 07:39:41.000000 rcmpy-1.5.5/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-15 07:39:41.000000 rcmpy-1.5.5/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:39:41.000000 rcmpy-1.5.5/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 07:39:41.000000 rcmpy-1.5.5/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-15 07:39:41.000000 rcmpy-1.5.5/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 07:39:41.000000 rcmpy-1.5.5/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:39:41.191437 rcmpy-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-15 07:38:41.000000 rcmpy-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:39:41.191437 rcmpy-1.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-15 07:38:41.000000 rcmpy-1.5.5/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-15 07:38:41.000000 rcmpy-1.5.5/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-15 07:38:41.000000 rcmpy-1.5.5/tests/test_xdg.py
```

### Comparing `rcmpy-1.5.4/LICENSE` & `rcmpy-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/PKG-INFO` & `rcmpy-1.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.5.4
+Version: 1.5.5
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,16 +14,16 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vcorelib>=1.6.6
 Requires-Dist: datazen
+Requires-Dist: vcorelib>=1.6.6
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -35,19 +35,19 @@
 Requires-Dist: setuptools-wrapper; extra == "test"
 Requires-Dist: types-setuptools; extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=4a63d867ef56ebbd2d59aaddb06364c5
+    hash=625e7606ffc71be06c919432e86f94e2
     =====================================
 -->
 
-# rcmpy ([1.5.4](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.5](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -156,23 +156,26 @@
 [top-level configuration file](md/data_repository.md#top-level-configuration).
 
 # Command-line Options
 
 ```
 $ ./venv3.12/bin/rcmpy -h
 
-usage: rcmpy [-h] [--version] [-v] [-C DIR]
+usage: rcmpy [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
              {apply,dump,use,variant,watch,noop} ...
 
 A configuration-file management system.
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
+  -q, --quiet           set to reduce output
+  --curses              whether or not to use curses.wrapper when starting
+  --no-uvloop           whether or not to disable uvloop as event loop driver
   -C DIR, --dir DIR     execute from a specific directory
 
 commands:
   {apply,dump,use,variant,watch,noop}
                         set of available commands
     apply               apply any pending changes from the active data
                         repository
```

### Comparing `rcmpy-1.5.4/README.md` & `rcmpy-1.5.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=4a63d867ef56ebbd2d59aaddb06364c5
+    hash=625e7606ffc71be06c919432e86f94e2
     =====================================
 -->
 
-# rcmpy ([1.5.4](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.5](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -119,23 +119,26 @@
 [top-level configuration file](md/data_repository.md#top-level-configuration).
 
 # Command-line Options
 
 ```
 $ ./venv3.12/bin/rcmpy -h
 
-usage: rcmpy [-h] [--version] [-v] [-C DIR]
+usage: rcmpy [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
              {apply,dump,use,variant,watch,noop} ...
 
 A configuration-file management system.
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
+  -q, --quiet           set to reduce output
+  --curses              whether or not to use curses.wrapper when starting
+  --no-uvloop           whether or not to disable uvloop as event loop driver
   -C DIR, --dir DIR     execute from a specific directory
 
 commands:
   {apply,dump,use,variant,watch,noop}
                         set of available commands
     apply               apply any pending changes from the active data
                         repository
```

### Comparing `rcmpy-1.5.4/pyproject.toml` & `rcmpy-1.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "rcmpy"
-version = "1.5.4"
+version = "1.5.5"
 description = "A configuration-file management system."
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `rcmpy-1.5.4/rcmpy/app.py` & `rcmpy-1.5.5/rcmpy/app.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/commands/all.py` & `rcmpy-1.5.5/rcmpy/commands/all.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/commands/apply.py` & `rcmpy-1.5.5/rcmpy/commands/apply.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/commands/common.py` & `rcmpy-1.5.5/rcmpy/commands/common.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/commands/dump.py` & `rcmpy-1.5.5/rcmpy/commands/dump.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/commands/use.py` & `rcmpy-1.5.5/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/commands/variant.py` & `rcmpy-1.5.5/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/commands/watch.py` & `rcmpy-1.5.5/rcmpy/commands/watch.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/config/__init__.py` & `rcmpy-1.5.5/rcmpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/config/file.py` & `rcmpy-1.5.5/rcmpy/config/file.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/data/schemas/ManagedFile.yaml` & `rcmpy-1.5.5/rcmpy/data/schemas/ManagedFile.yaml`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/entry.py` & `rcmpy-1.5.5/rcmpy/entry.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/environment/__init__.py` & `rcmpy-1.5.5/rcmpy/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/environment/base.py` & `rcmpy-1.5.5/rcmpy/environment/base.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/environment/data.py` & `rcmpy-1.5.5/rcmpy/environment/data.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/environment/template.py` & `rcmpy-1.5.5/rcmpy/environment/template.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/paths/__init__.py` & `rcmpy-1.5.5/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/schemas.py` & `rcmpy-1.5.5/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/state/__init__.py` & `rcmpy-1.5.5/rcmpy/state/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,13 +204,15 @@
     root: Pathlike = None, name: str = "state.json"
 ) -> Iterator[State]:
     """This needs to be a context manager, so it get's written back to disk."""
 
     if root is None:
         root = default_state_directory()
 
-    with FileCache(normalize(root, name)).loaded() as data:
+    with ExitStack() as stack:
+        data = stack.enter_context(FileCache(normalize(root, name)).loaded())
+
         state = State.create(data, verify=False)
         yield state
 
         # Update the original dictionary with any changes to the state object.
         data.update(state.asdict())
```

### Comparing `rcmpy-1.5.4/rcmpy/watch/__init__.py` & `rcmpy-1.5.5/rcmpy/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/watch/params.py` & `rcmpy-1.5.5/rcmpy/watch/params.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy/xdg/__init__.py` & `rcmpy-1.5.5/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/rcmpy.egg-info/PKG-INFO` & `rcmpy-1.5.5/rcmpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.5.4
+Version: 1.5.5
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,16 +14,16 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vcorelib>=1.6.6
 Requires-Dist: datazen
+Requires-Dist: vcorelib>=1.6.6
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -35,19 +35,19 @@
 Requires-Dist: setuptools-wrapper; extra == "test"
 Requires-Dist: types-setuptools; extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=4a63d867ef56ebbd2d59aaddb06364c5
+    hash=625e7606ffc71be06c919432e86f94e2
     =====================================
 -->
 
-# rcmpy ([1.5.4](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.5](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -156,23 +156,26 @@
 [top-level configuration file](md/data_repository.md#top-level-configuration).
 
 # Command-line Options
 
 ```
 $ ./venv3.12/bin/rcmpy -h
 
-usage: rcmpy [-h] [--version] [-v] [-C DIR]
+usage: rcmpy [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
              {apply,dump,use,variant,watch,noop} ...
 
 A configuration-file management system.
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
+  -q, --quiet           set to reduce output
+  --curses              whether or not to use curses.wrapper when starting
+  --no-uvloop           whether or not to disable uvloop as event loop driver
   -C DIR, --dir DIR     execute from a specific directory
 
 commands:
   {apply,dump,use,variant,watch,noop}
                         set of available commands
     apply               apply any pending changes from the active data
                         repository
```

### Comparing `rcmpy-1.5.4/rcmpy.egg-info/SOURCES.txt` & `rcmpy-1.5.5/rcmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/setup.py` & `rcmpy-1.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.4/tests/test_entry.py` & `rcmpy-1.5.5/tests/test_entry.py`

 * *Files identical despite different names*

