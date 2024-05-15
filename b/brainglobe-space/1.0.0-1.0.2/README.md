# Comparing `tmp/brainglobe_space-1.0.0.tar.gz` & `tmp/brainglobe_space-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe_space-1.0.0.tar", last modified: Wed Jan 24 12:05:23 2024, max compression
+gzip compressed data, was "brainglobe_space-1.0.2.tar", last modified: Wed May 15 10:06:16 2024, max compression
```

## Comparing `brainglobe_space-1.0.0.tar` & `brainglobe_space-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 ccaegra   (1000) ccaegra   (1000)        0 2024-01-24 12:05:23.097496 brainglobe_space-1.0.0/
-drwxrwxr-x   0 ccaegra   (1000) ccaegra   (1000)        0 2024-01-24 12:05:23.097496 brainglobe_space-1.0.0/.github/
-drwxrwxr-x   0 ccaegra   (1000) ccaegra   (1000)        0 2024-01-24 12:05:23.097496 brainglobe_space-1.0.0/.github/workflows/
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)     1498 2024-01-24 12:02:00.000000 brainglobe_space-1.0.0/.github/workflows/test_and_deploy.yml
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)     1817 2024-01-10 15:32:36.000000 brainglobe_space-1.0.0/.gitignore
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)     1510 2024-01-10 15:32:36.000000 brainglobe_space-1.0.0/LICENSE
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)      136 2024-01-24 12:02:00.000000 brainglobe_space-1.0.0/MANIFEST.in
--rw-r--r--   0 ccaegra   (1000) ccaegra   (1000)     6897 2024-01-24 12:05:23.097496 brainglobe_space-1.0.0/PKG-INFO
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)     6016 2024-01-24 12:02:00.000000 brainglobe_space-1.0.0/README.md
-drwxrwxr-x   0 ccaegra   (1000) ccaegra   (1000)        0 2024-01-24 12:05:23.097496 brainglobe_space-1.0.0/brainglobe_space/
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)      264 2024-01-24 12:02:00.000000 brainglobe_space-1.0.0/brainglobe_space/__init__.py
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)    15850 2024-01-24 12:02:00.000000 brainglobe_space-1.0.0/brainglobe_space/core.py
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)     2175 2024-01-24 12:02:00.000000 brainglobe_space-1.0.0/brainglobe_space/functions.py
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)      889 2024-01-24 12:02:00.000000 brainglobe_space-1.0.0/brainglobe_space/utils.py
-drwxrwxr-x   0 ccaegra   (1000) ccaegra   (1000)        0 2024-01-24 12:05:23.097496 brainglobe_space-1.0.0/brainglobe_space.egg-info/
--rw-r--r--   0 ccaegra   (1000) ccaegra   (1000)     6897 2024-01-24 12:05:23.000000 brainglobe_space-1.0.0/brainglobe_space.egg-info/PKG-INFO
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)      402 2024-01-24 12:05:23.000000 brainglobe_space-1.0.0/brainglobe_space.egg-info/SOURCES.txt
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)        1 2024-01-24 12:05:23.000000 brainglobe_space-1.0.0/brainglobe_space.egg-info/dependency_links.txt
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)       58 2024-01-24 12:05:23.000000 brainglobe_space-1.0.0/brainglobe_space.egg-info/requires.txt
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)       17 2024-01-24 12:05:23.000000 brainglobe_space-1.0.0/brainglobe_space.egg-info/top_level.txt
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)     1530 2024-01-24 12:02:00.000000 brainglobe_space-1.0.0/pyproject.toml
--rw-rw-r--   0 ccaegra   (1000) ccaegra   (1000)       38 2024-01-24 12:05:23.097496 brainglobe_space-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:06:16.186123 brainglobe_space-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:06:16.182123 brainglobe_space-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:06:16.186123 brainglobe_space-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-15 10:06:10.000000 brainglobe_space-1.0.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-15 10:06:10.000000 brainglobe_space-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-15 10:06:10.000000 brainglobe_space-1.0.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-15 10:06:10.000000 brainglobe_space-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-15 10:06:10.000000 brainglobe_space-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-15 10:06:16.186123 brainglobe_space-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-15 10:06:10.000000 brainglobe_space-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:06:16.186123 brainglobe_space-1.0.2/brainglobe_space/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-15 10:06:10.000000 brainglobe_space-1.0.2/brainglobe_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-05-15 10:06:10.000000 brainglobe_space-1.0.2/brainglobe_space/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-15 10:06:10.000000 brainglobe_space-1.0.2/brainglobe_space/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-15 10:06:10.000000 brainglobe_space-1.0.2/brainglobe_space/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:06:16.186123 brainglobe_space-1.0.2/brainglobe_space.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-15 10:06:16.000000 brainglobe_space-1.0.2/brainglobe_space.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 10:06:16.000000 brainglobe_space-1.0.2/brainglobe_space.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:06:16.000000 brainglobe_space-1.0.2/brainglobe_space.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 10:06:16.000000 brainglobe_space-1.0.2/brainglobe_space.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 10:06:16.000000 brainglobe_space-1.0.2/brainglobe_space.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-15 10:06:10.000000 brainglobe_space-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 10:06:16.186123 brainglobe_space-1.0.2/setup.cfg
```

### Comparing `brainglobe_space-1.0.0/.github/workflows/test_and_deploy.yml` & `brainglobe_space-1.0.2/.github/workflows/test_and_deploy.yml`

 * *Files 6% similar despite different names*

```diff
@@ -26,38 +26,44 @@
   manifest:
     name: Check Manifest
     runs-on: ubuntu-latest
     steps:
       - uses: neuroinformatics-unit/actions/lint@v2
 
   test:
+    needs: [linting, manifest]
     name: Run package tests
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         include:
         - os: ubuntu-latest
           python-version: "3.11"
-        - os: macos-latest
+        - os: macos-13 # Intel Mac
           python-version: "3.10"
+        - os: macos-latest # ARM Mac
+          python-version: "3.11"
         - os: windows-latest
           python-version: "3.9"
 
     steps:
-      - uses: neuroinformatics-unit/actions/test@v1
+      - uses: neuroinformatics-unit/actions/test@v2
         with:
           python-version: ${{ matrix.python-version }}
 
-  build_sdist_wheel:
-    name: Build source distribution and wheel
-    needs: [test, linting, manifest]
+  build_sdist_wheels:
+    name: Build source distribution
+    needs: [test]
     if: github.event_name == 'push' && github.ref_type == 'tag'
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/download-artifact@v3
-        with:
-          name: artifact
-          path: dist
-      - uses: pypa/gh-action-pypi-publish@v1.5.0
-        with:
-          user: __token__
-          password: ${{ secrets.TWINE_API_KEY }}
+    - uses: neuroinformatics-unit/actions/build_sdist_wheels@v2
+
+
+  upload_all:
+    name: Publish build distributions
+    needs: [build_sdist_wheels]
+    runs-on: ubuntu-latest
+    steps:
+    - uses: neuroinformatics-unit/actions/upload_pypi@v2
+      with:
+        secret-pypi-key: ${{ secrets.TWINE_API_KEY }}
```

### Comparing `brainglobe_space-1.0.0/.gitignore` & `brainglobe_space-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `brainglobe_space-1.0.0/LICENSE` & `brainglobe_space-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe_space-1.0.0/PKG-INFO` & `brainglobe_space-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe_space
-Version: 1.0.0
+Version: 1.0.2
 Summary: Anatomical space conventions made easy
 Author-email: Luigi Petrucco <luigi.petrucco@gmail.com>
 Project-URL: Homepage, https://github.com/brainglobe/brainglobe-space
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -20,19 +20,27 @@
 Requires-Dist: gitpython; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 
 [![Python Version](https://img.shields.io/pypi/pyversions/brainglobe-space.svg)](https://pypi.org/project/brainglobe-space)
 [![PyPI](https://img.shields.io/pypi/v/brainglobe-space.svg)](https://pypi.org/project/brainglobe-space)
-[![Build Status](https://travis-ci.com/brainglobe/brainglobe-space.svg?branch=master)](https://travis-ci.com/brainglobe/brainglobe-space)
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Coverage Status](https://coveralls.io/repos/github/brainglobe/brainglobe-space/badge.svg)](https://coveralls.io/github/brainglobe/brainglobe-space)
+[![Downloads](https://pepy.tech/badge/brainglobe-space)](https://pepy.tech/project/brainglobe-space)
+[![Wheel](https://img.shields.io/pypi/wheel/brainglobe-space.svg)](https://pypi.org/project/brainglobe-space)
+[![Development Status](https://img.shields.io/pypi/status/brainglobe-space.svg)](https://github.com/brainglobe/brainglobe-space)
+[![Tests](https://img.shields.io/github/actions/workflow/status/brainglobe/brainglobe-space/test_and_deploy.yml?branch=main)](https://github.com/brainglobe/brainglobe-space/actions)
+[![codecov](https://codecov.io/gh/brainglobe/brainglobe-space/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/brainglobe-space)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4552537.svg)](https://doi.org/10.5281/zenodo.4552537)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://brainglobe.info/community/developers/index.html)
+[![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![DOI](https://zenodo.org/badge/267813717.svg)](https://zenodo.org/doi/10.5281/zenodo.4552536)
+
 
 # brainglobe-space
 
 Anatomical space conventions made easy.
 
 Working with anatomical images, one often encounters the problem of matching the orientation of stacks with different conventions about axes orientation and order. Moreover, when multiple swaps and flips are involved, it can be annoying to map the same transformations to volumes and points (e.g., coordinates or meshes).
```

### Comparing `brainglobe_space-1.0.0/README.md` & `brainglobe_space-1.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/brainglobe-space.svg)](https://pypi.org/project/brainglobe-space)
 [![PyPI](https://img.shields.io/pypi/v/brainglobe-space.svg)](https://pypi.org/project/brainglobe-space)
-[![Build Status](https://travis-ci.com/brainglobe/brainglobe-space.svg?branch=master)](https://travis-ci.com/brainglobe/brainglobe-space)
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Coverage Status](https://coveralls.io/repos/github/brainglobe/brainglobe-space/badge.svg)](https://coveralls.io/github/brainglobe/brainglobe-space)
+[![Downloads](https://pepy.tech/badge/brainglobe-space)](https://pepy.tech/project/brainglobe-space)
+[![Wheel](https://img.shields.io/pypi/wheel/brainglobe-space.svg)](https://pypi.org/project/brainglobe-space)
+[![Development Status](https://img.shields.io/pypi/status/brainglobe-space.svg)](https://github.com/brainglobe/brainglobe-space)
+[![Tests](https://img.shields.io/github/actions/workflow/status/brainglobe/brainglobe-space/test_and_deploy.yml?branch=main)](https://github.com/brainglobe/brainglobe-space/actions)
+[![codecov](https://codecov.io/gh/brainglobe/brainglobe-space/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/brainglobe-space)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4552537.svg)](https://doi.org/10.5281/zenodo.4552537)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://brainglobe.info/community/developers/index.html)
+[![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![DOI](https://zenodo.org/badge/267813717.svg)](https://zenodo.org/doi/10.5281/zenodo.4552536)
+
 
 # brainglobe-space
 
 Anatomical space conventions made easy.
 
 Working with anatomical images, one often encounters the problem of matching the orientation of stacks with different conventions about axes orientation and order. Moreover, when multiple swaps and flips are involved, it can be annoying to map the same transformations to volumes and points (e.g., coordinates or meshes).
```

### Comparing `brainglobe_space-1.0.0/brainglobe_space/core.py` & `brainglobe_space-1.0.2/brainglobe_space/core.py`

 * *Files identical despite different names*

### Comparing `brainglobe_space-1.0.0/brainglobe_space/functions.py` & `brainglobe_space-1.0.2/brainglobe_space/functions.py`

 * *Files identical despite different names*

### Comparing `brainglobe_space-1.0.0/brainglobe_space/utils.py` & `brainglobe_space-1.0.2/brainglobe_space/utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe_space-1.0.0/brainglobe_space.egg-info/PKG-INFO` & `brainglobe_space-1.0.2/brainglobe_space.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe_space
-Version: 1.0.0
+Version: 1.0.2
 Summary: Anatomical space conventions made easy
 Author-email: Luigi Petrucco <luigi.petrucco@gmail.com>
 Project-URL: Homepage, https://github.com/brainglobe/brainglobe-space
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -20,19 +20,27 @@
 Requires-Dist: gitpython; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 
 [![Python Version](https://img.shields.io/pypi/pyversions/brainglobe-space.svg)](https://pypi.org/project/brainglobe-space)
 [![PyPI](https://img.shields.io/pypi/v/brainglobe-space.svg)](https://pypi.org/project/brainglobe-space)
-[![Build Status](https://travis-ci.com/brainglobe/brainglobe-space.svg?branch=master)](https://travis-ci.com/brainglobe/brainglobe-space)
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Coverage Status](https://coveralls.io/repos/github/brainglobe/brainglobe-space/badge.svg)](https://coveralls.io/github/brainglobe/brainglobe-space)
+[![Downloads](https://pepy.tech/badge/brainglobe-space)](https://pepy.tech/project/brainglobe-space)
+[![Wheel](https://img.shields.io/pypi/wheel/brainglobe-space.svg)](https://pypi.org/project/brainglobe-space)
+[![Development Status](https://img.shields.io/pypi/status/brainglobe-space.svg)](https://github.com/brainglobe/brainglobe-space)
+[![Tests](https://img.shields.io/github/actions/workflow/status/brainglobe/brainglobe-space/test_and_deploy.yml?branch=main)](https://github.com/brainglobe/brainglobe-space/actions)
+[![codecov](https://codecov.io/gh/brainglobe/brainglobe-space/branch/main/graph/badge.svg?token=nx1lhNI7ox)](https://codecov.io/gh/brainglobe/brainglobe-space)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4552537.svg)](https://doi.org/10.5281/zenodo.4552537)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://brainglobe.info/community/developers/index.html)
+[![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![DOI](https://zenodo.org/badge/267813717.svg)](https://zenodo.org/doi/10.5281/zenodo.4552536)
+
 
 # brainglobe-space
 
 Anatomical space conventions made easy.
 
 Working with anatomical images, one often encounters the problem of matching the orientation of stacks with different conventions about axes orientation and order. Moreover, when multiple swaps and flips are involved, it can be annoying to map the same transformations to volumes and points (e.g., coordinates or meshes).
```

### Comparing `brainglobe_space-1.0.0/pyproject.toml` & `brainglobe_space-1.0.2/pyproject.toml`

 * *Files identical despite different names*

