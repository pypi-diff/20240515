# Comparing `tmp/talus-0.2.1.tar.gz` & `tmp/talus-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talus-0.2.1.tar", last modified: Fri Feb 24 15:35:22 2023, max compression
+gzip compressed data, was "talus-1.0.0rc1.tar", last modified: Tue May 14 21:46:30 2024, max compression
```

## Comparing `talus-0.2.1.tar` & `talus-1.0.0rc1.tar`

### file list

```diff
@@ -1,26 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-24 15:35:22.727003 talus-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     2448 2023-02-24 15:35:15.000000 talus-0.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-02-24 15:35:15.000000 talus-0.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1050 2023-02-24 15:35:15.000000 talus-0.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     2884 2023-02-24 15:35:22.727003 talus-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2300 2023-02-24 15:35:15.000000 talus-0.2.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-02-24 15:35:15.000000 talus-0.2.1/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-02-24 15:35:15.000000 talus-0.2.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1119 2023-02-24 15:35:22.727003 talus-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-02-24 15:35:15.000000 talus-0.2.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-24 15:35:22.727003 talus-0.2.1/talus/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-02-24 15:35:15.000000 talus-0.2.1/talus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-02-24 15:35:15.000000 talus-0.2.1/talus/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7056 2023-02-24 15:35:15.000000 talus-0.2.1/talus/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)     3758 2023-02-24 15:35:15.000000 talus-0.2.1/talus/message.py
--rw-rw-rw-   0 root         (0) root         (0)     7219 2023-02-24 15:35:15.000000 talus-0.2.1/talus/producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-24 15:35:22.727003 talus-0.2.1/talus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 15:35:15.000000 talus-0.2.1/talus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-02-24 15:35:15.000000 talus-0.2.1/talus/tests/test_message.py
--rw-rw-rw-   0 root         (0) root         (0)     6972 2023-02-24 15:35:15.000000 talus-0.2.1/talus/tests/test_wrappers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-24 15:35:22.727003 talus-0.2.1/talus.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2884 2023-02-24 15:35:22.000000 talus-0.2.1/talus.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-02-24 15:35:22.000000 talus-0.2.1/talus.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-02-24 15:35:22.000000 talus-0.2.1/talus.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-02-24 15:35:22.000000 talus-0.2.1/talus.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-02-24 15:35:22.000000 talus-0.2.1/talus.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-14 21:46:30.158894 talus-1.0.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-14 21:46:18.000000 talus-1.0.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-14 21:46:18.000000 talus-1.0.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-14 21:46:18.000000 talus-1.0.0rc1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-14 21:46:18.000000 talus-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-05-14 21:46:30.158894 talus-1.0.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-14 21:46:18.000000 talus-1.0.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-14 21:46:18.000000 talus-1.0.0rc1/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-14 21:46:18.000000 talus-1.0.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-14 21:46:30.158894 talus-1.0.0rc1/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-14 21:46:30.154894 talus-1.0.0rc1/talus/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-14 21:46:30.000000 talus-1.0.0rc1/talus/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6256 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/consumer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-14 21:46:30.154894 talus-1.0.0rc1/talus/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/binding.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     2415 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3969 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4703 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-14 21:46:30.154894 talus-1.0.0rc1/talus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4672 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-14 21:46:30.158894 talus-1.0.0rc1/talus/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/test_binding.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/test_connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3949 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/test_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     6266 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/test_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/test_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/test_retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/test_producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-14 21:46:30.158894 talus-1.0.0rc1/talus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-05-14 21:46:30.000000 talus-1.0.0rc1/talus.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-14 21:46:30.000000 talus-1.0.0rc1/talus.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-14 21:46:30.000000 talus-1.0.0rc1/talus.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-14 21:46:29.000000 talus-1.0.0rc1/talus.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-14 21:46:30.000000 talus-1.0.0rc1/talus.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-14 21:46:30.000000 talus-1.0.0rc1/talus.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-14 21:46:18.000000 talus-1.0.0rc1/tox.ini
```

### Comparing `talus-0.2.1/.gitignore` & `talus-1.0.0rc1/.gitignore`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,16 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
-__pycache__
 *.py[cod]
 *$py.class
-*.a
-*.o
-*.pyc
 
 # C extensions
 *.so
 
 # Distribution / packaging
-*.egg
-*.egg-info
-dist
-build
-eggs
-parts
-bin
-var
-sdist
-develop-eggs
-.installed.cfg
-distribute-*.tar.gz
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
@@ -35,14 +19,16 @@
 parts/
 sdist/
 var/
 wheels/
 pip-wheel-metadata/
 share/python-wheels/
 *.egg-info/
+.installed.cfg
+*.egg
 MANIFEST
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
@@ -136,53 +122,7 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
-
-
-# other
-*.fits
-.tox
-.*.sw[op]
-*~
-
-# Ignore .c files by default to avoid including generated code. If you want to
-# add a non-generated .c extension, use `git add -f filename.c`.
-*.c
-
-# Other generated files
-*/version.py
-*/cython_version.py
-htmlcov
-
-
-# Sphinx
-docs/api
-docs/_build
-
-# Eclipse editor project files
-.project
-.pydevproject
-.settings
-
-# Floobits project files
-.floo
-.flooignore
-
-# Mac OSX
-.DS_Store
-
-# Outputs and temp files
-*.png
-*.txt
-*.cprof
-vtfcal/dask-worker-space/
-vtfcal/data/
-tmp??_pars*.fits
-
-*data_tree
-dask-worker-space
-logging.*
-data-processing.code-workspace
```

### Comparing `talus-0.2.1/.pre-commit-config.yaml` & `talus-1.0.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `talus-0.2.1/LICENSE` & `talus-1.0.0rc1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+MIT License
+
 Copyright 2019 NSO / AURA
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `talus-0.2.1/README.rst` & `talus-1.0.0rc1/README.rst`

 * *Files identical despite different names*

