# Comparing `tmp/rms-pdsparser-0.0.4.tar.gz` & `tmp/rms_pdsparser-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-pdsparser-0.0.4.tar", last modified: Wed Nov  1 19:58:38 2023, max compression
+gzip compressed data, was "rms_pdsparser-0.0.5.tar", last modified: Tue May 14 19:17:14 2024, max compression
```

## Comparing `rms-pdsparser-0.0.4.tar` & `rms_pdsparser-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 19:58:38.237615 rms-pdsparser-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-01 19:58:22.000000 rms-pdsparser-0.0.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 19:58:38.233615 rms-pdsparser-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 19:58:38.237615 rms-pdsparser-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-11-01 19:58:22.000000 rms-pdsparser-0.0.4/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-11-01 19:58:22.000000 rms-pdsparser-0.0.4/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-11-01 19:58:22.000000 rms-pdsparser-0.0.4/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2023-11-01 19:58:22.000000 rms-pdsparser-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-01 19:58:22.000000 rms-pdsparser-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-11-01 19:58:38.237615 rms-pdsparser-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-11-01 19:58:22.000000 rms-pdsparser-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 19:58:38.237615 rms-pdsparser-0.0.4/pdsparser/
--rwxr-xr-x   0 runner    (1001) docker     (127)    54905 2023-11-01 19:58:22.000000 rms-pdsparser-0.0.4/pdsparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-01 19:58:38.000000 rms-pdsparser-0.0.4/pdsparser/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-11-01 19:58:22.000000 rms-pdsparser-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-01 19:58:22.000000 rms-pdsparser-0.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 19:58:38.237615 rms-pdsparser-0.0.4/rms_pdsparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-11-01 19:58:38.000000 rms-pdsparser-0.0.4/rms_pdsparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-11-01 19:58:38.000000 rms-pdsparser-0.0.4/rms_pdsparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 19:58:38.000000 rms-pdsparser-0.0.4/rms_pdsparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-01 19:58:38.000000 rms-pdsparser-0.0.4/rms_pdsparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-01 19:58:38.000000 rms-pdsparser-0.0.4/rms_pdsparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-01 19:58:38.237615 rms-pdsparser-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:14.431191 rms_pdsparser-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:17:08.000000 rms_pdsparser-0.0.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:14.427191 rms_pdsparser-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:14.431191 rms_pdsparser-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-14 19:17:08.000000 rms_pdsparser-0.0.5/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-14 19:17:08.000000 rms_pdsparser-0.0.5/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-14 19:17:08.000000 rms_pdsparser-0.0.5/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:17:08.000000 rms_pdsparser-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:17:08.000000 rms_pdsparser-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-05-14 19:17:08.000000 rms_pdsparser-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:17:08.000000 rms_pdsparser-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-14 19:17:14.431191 rms_pdsparser-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-14 19:17:08.000000 rms_pdsparser-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:14.431191 rms_pdsparser-0.0.5/pdsparser/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54906 2024-05-14 19:17:08.000000 rms_pdsparser-0.0.5/pdsparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:17:14.000000 rms_pdsparser-0.0.5/pdsparser/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-14 19:17:08.000000 rms_pdsparser-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 19:17:08.000000 rms_pdsparser-0.0.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:14.431191 rms_pdsparser-0.0.5/rms_pdsparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-14 19:17:14.000000 rms_pdsparser-0.0.5/rms_pdsparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-14 19:17:14.000000 rms_pdsparser-0.0.5/rms_pdsparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:17:14.000000 rms_pdsparser-0.0.5/rms_pdsparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 19:17:14.000000 rms_pdsparser-0.0.5/rms_pdsparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 19:17:14.000000 rms_pdsparser-0.0.5/rms_pdsparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 19:17:14.431191 rms_pdsparser-0.0.5/setup.cfg
```

### Comparing `rms-pdsparser-0.0.4/.github/workflows/publish_to_pypi.yml` & `rms_pdsparser-0.0.5/.github/workflows/publish_to_pypi.yml`

 * *Files 15% similar despite different names*

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

### Comparing `rms-pdsparser-0.0.4/.github/workflows/publish_to_test_pypi.yml` & `rms_pdsparser-0.0.5/.github/workflows/publish_to_test_pypi.yml`

 * *Files 18% similar despite different names*

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

### Comparing `rms-pdsparser-0.0.4/.github/workflows/run-tests.yml` & `rms_pdsparser-0.0.5/.github/workflows/run-tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Run Tests
-run-name: Run Tests triggered by ${{ github.ref_type }} ${{ github.ref_name }} or ${{ github.triggering_actor }}
+run-name: "Run Tests: ${{ github.ref_type }} ${{ github.ref_name }} by ${{ github.triggering_actor }}"
 
 on:
   workflow_dispatch:
   # pull_request:
   #   branches: [ main ]
   # push:
   #   branches: [ main ]
@@ -22,23 +22,29 @@
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
+        uses: codecov/codecov-action@v4
+        if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
         with:
+          token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `rms-pdsparser-0.0.4/.gitignore` & `rms_pdsparser-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-pdsparser-0.0.4/LICENSE` & `rms_pdsparser-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-pdsparser-0.0.4/pdsparser/__init__.py` & `rms_pdsparser-0.0.5/pdsparser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 from pyparsing import *
 del __author__ # Imported from pyparsing
 import decimal as dec
 import datetime as dt
 import sys
 
 try:
-    from _version import __version__
+    from ._version import __version__
 except ImportError as err:
     __version__ = 'Version unspecified'
 
 
 # We need to specify encoding when we open labels in Python 3; we can't in
 # Python 2
 if sys.version_info >= (3,0):
```

### Comparing `rms-pdsparser-0.0.4/pyproject.toml` & `rms_pdsparser-0.0.5/pyproject.toml`

 * *Files identical despite different names*

