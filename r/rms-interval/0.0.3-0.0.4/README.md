# Comparing `tmp/rms-interval-0.0.3.tar.gz` & `tmp/rms_interval-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-interval-0.0.3.tar", last modified: Wed Jan 24 23:28:54 2024, max compression
+gzip compressed data, was "rms_interval-0.0.4.tar", last modified: Tue May 14 19:00:59 2024, max compression
```

## Comparing `rms-interval-0.0.3.tar` & `rms_interval-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:28:54.531830 rms-interval-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-24 23:28:38.000000 rms-interval-0.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:28:54.527830 rms-interval-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:28:54.527830 rms-interval-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-24 23:28:38.000000 rms-interval-0.0.3/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-24 23:28:38.000000 rms-interval-0.0.3/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-01-24 23:28:38.000000 rms-interval-0.0.3/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-24 23:28:38.000000 rms-interval-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-24 23:28:38.000000 rms-interval-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-01-24 23:28:54.531830 rms-interval-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-24 23:28:38.000000 rms-interval-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:28:54.527830 rms-interval-0.0.3/interval/
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-01-24 23:28:38.000000 rms-interval-0.0.3/interval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-24 23:28:54.000000 rms-interval-0.0.3/interval/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-01-24 23:28:38.000000 rms-interval-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-24 23:28:38.000000 rms-interval-0.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:28:54.531830 rms-interval-0.0.3/rms_interval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-01-24 23:28:54.000000 rms-interval-0.0.3/rms_interval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-24 23:28:54.000000 rms-interval-0.0.3/rms_interval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 23:28:54.000000 rms-interval-0.0.3/rms_interval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-24 23:28:54.000000 rms-interval-0.0.3/rms_interval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-24 23:28:54.000000 rms-interval-0.0.3/rms_interval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-24 23:28:54.531830 rms-interval-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:28:54.531830 rms-interval-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-01-24 23:28:38.000000 rms-interval-0.0.3/tests/test_interval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:59.216191 rms_interval-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:00:50.000000 rms_interval-0.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:59.212191 rms_interval-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:59.216191 rms_interval-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:00:50.000000 rms_interval-0.0.4/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:00:50.000000 rms_interval-0.0.4/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-14 19:00:50.000000 rms_interval-0.0.4/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:00:50.000000 rms_interval-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:00:50.000000 rms_interval-0.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-05-14 19:00:50.000000 rms_interval-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:00:50.000000 rms_interval-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-14 19:00:59.216191 rms_interval-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-14 19:00:50.000000 rms_interval-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:59.216191 rms_interval-0.0.4/interval/
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-14 19:00:50.000000 rms_interval-0.0.4/interval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:00:59.000000 rms_interval-0.0.4/interval/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-14 19:00:50.000000 rms_interval-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 19:00:50.000000 rms_interval-0.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:59.216191 rms_interval-0.0.4/rms_interval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-14 19:00:59.000000 rms_interval-0.0.4/rms_interval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-14 19:00:59.000000 rms_interval-0.0.4/rms_interval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:00:59.000000 rms_interval-0.0.4/rms_interval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 19:00:59.000000 rms_interval-0.0.4/rms_interval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 19:00:59.000000 rms_interval-0.0.4/rms_interval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 19:00:59.216191 rms_interval-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:59.216191 rms_interval-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-05-14 19:00:50.000000 rms_interval-0.0.4/tests/test_interval.py
```

### Comparing `rms-interval-0.0.3/.github/workflows/publish_to_pypi.yml` & `rms_interval-0.0.4/.github/workflows/publish_to_pypi.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Publish to PyPI
-run-name: Publish to PyPI triggered by ${{ github.ref_type }} ${{ github.ref_name }}
+run-name: "Publish to PyPI: ${{ github.ref_type }} ${{ github.ref_name }}"
 
 on:
   release:
     types: [published]
 
 jobs:
   upload_pypi:
@@ -11,15 +11,15 @@
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
```

### Comparing `rms-interval-0.0.3/.github/workflows/publish_to_test_pypi.yml` & `rms_interval-0.0.4/.github/workflows/publish_to_test_pypi.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 name: Publish to Test PyPI
-run-name: Publish to Test PyPI triggered by ${{ github.ref_type }} ${{ github.ref_name }}
+run-name: "Publish to Test PyPI: ${{ github.ref_type }} ${{ github.ref_name }}"
 
 on:
   workflow_dispatch:
 
 jobs:
   upload_pypi:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
```

### Comparing `rms-interval-0.0.3/.github/workflows/run-tests.yml` & `rms_interval-0.0.4/.github/workflows/run-tests.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Run Tests
-run-name: Run Tests triggered by ${{ github.ref_type }} ${{ github.ref_name }} or ${{ github.triggering_actor }}
+run-name: "Run Tests: ${{ github.ref_type }} ${{ github.ref_name }} by ${{ github.triggering_actor }}"
 
 on:
   workflow_dispatch:
   pull_request:
     branches: [ main ]
   push:
     branches: [ main ]
@@ -13,35 +13,38 @@
 jobs:
   test:
     name: Test interval
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [ '3.7', '3.8', '3.9', '3.10', '3.11', '3.12' ]
+        python-version: [ '3.8', '3.9', '3.10', '3.11', '3.12' ]
       fail-fast: false
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           ref: ${{ github.event.pull_request.head.sha }}
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
 
       - name: Test with coverage
         run: |
           coverage run -m pytest
 
+      - name: Print coverage report
+        run: |
+          coverage report -m
+
       - name: Upload coverage report to codecov
-        uses: codecov/codecov-action@v3
-        env:
-          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+        uses: codecov/codecov-action@v4
+        if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `rms-interval-0.0.3/.gitignore` & `rms_interval-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-interval-0.0.3/LICENSE` & `rms_interval-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-interval-0.0.3/interval/__init__.py` & `rms_interval-0.0.4/interval/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 # interval.py
 #
 # Deukkwon Yoon & Mark Showalter, PDS Rings Node, SETI Institute, November 2011
 ################################################################################
 
 import numpy as np
 
+try:
+    from ._version import __version__
+except ImportError as err:
+    __version__ = 'Version unspecified'
+
+
 class Interval(object):
     """The interval class behaves like a dictionary keyed by ranges of
     floating-point numbers. Each value of the dictionary applies for any key
     value within the numeric range. Later entries into the dictionary can
     partially or completely replace earlier values."""
 
     def __init__(self, min=-np.inf, max=np.inf, value=None):
```

### Comparing `rms-interval-0.0.3/pyproject.toml` & `rms_interval-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-interval-0.0.3/tests/test_interval.py` & `rms_interval-0.0.4/tests/test_interval.py`

 * *Files identical despite different names*

