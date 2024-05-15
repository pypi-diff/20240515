# Comparing `tmp/rms-pdslogger-0.0.5.tar.gz` & `tmp/rms_pdslogger-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-pdslogger-0.0.5.tar", last modified: Wed Nov  1 20:59:10 2023, max compression
+gzip compressed data, was "rms_pdslogger-0.0.6.tar", last modified: Tue May 14 19:17:00 2024, max compression
```

## Comparing `rms-pdslogger-0.0.5.tar` & `rms_pdslogger-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 20:59:10.576003 rms-pdslogger-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-01 20:58:58.000000 rms-pdslogger-0.0.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 20:59:10.572003 rms-pdslogger-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 20:59:10.572003 rms-pdslogger-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-11-01 20:58:58.000000 rms-pdslogger-0.0.5/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-11-01 20:58:58.000000 rms-pdslogger-0.0.5/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-11-01 20:58:58.000000 rms-pdslogger-0.0.5/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2023-11-01 20:58:58.000000 rms-pdslogger-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-01 20:58:58.000000 rms-pdslogger-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-11-01 20:59:10.576003 rms-pdslogger-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-11-01 20:58:58.000000 rms-pdslogger-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 20:59:10.572003 rms-pdslogger-0.0.5/pdslogger/
--rwxr-xr-x   0 runner    (1001) docker     (127)    28827 2023-11-01 20:58:58.000000 rms-pdslogger-0.0.5/pdslogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-01 20:59:10.000000 rms-pdslogger-0.0.5/pdslogger/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1705 2023-11-01 20:58:58.000000 rms-pdslogger-0.0.5/pdslogger/finder_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-11-01 20:58:58.000000 rms-pdslogger-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-01 20:58:58.000000 rms-pdslogger-0.0.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 20:59:10.576003 rms-pdslogger-0.0.5/rms_pdslogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-11-01 20:59:10.000000 rms-pdslogger-0.0.5/rms_pdslogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-11-01 20:59:10.000000 rms-pdslogger-0.0.5/rms_pdslogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 20:59:10.000000 rms-pdslogger-0.0.5/rms_pdslogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-01 20:59:10.000000 rms-pdslogger-0.0.5/rms_pdslogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-01 20:59:10.000000 rms-pdslogger-0.0.5/rms_pdslogger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-01 20:59:10.576003 rms-pdslogger-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:00.805063 rms_pdslogger-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:00.801063 rms_pdslogger-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:00.801063 rms_pdslogger-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-14 19:17:00.805063 rms_pdslogger-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:00.805063 rms_pdslogger-0.0.6/pdslogger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28828 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/pdslogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:17:00.000000 rms_pdslogger-0.0.6/pdslogger/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1705 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/pdslogger/finder_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 19:16:46.000000 rms_pdslogger-0.0.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:17:00.805063 rms_pdslogger-0.0.6/rms_pdslogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-14 19:17:00.000000 rms_pdslogger-0.0.6/rms_pdslogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-14 19:17:00.000000 rms_pdslogger-0.0.6/rms_pdslogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:17:00.000000 rms_pdslogger-0.0.6/rms_pdslogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 19:17:00.000000 rms_pdslogger-0.0.6/rms_pdslogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 19:17:00.000000 rms_pdslogger-0.0.6/rms_pdslogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 19:17:00.805063 rms_pdslogger-0.0.6/setup.cfg
```

### Comparing `rms-pdslogger-0.0.5/.github/workflows/publish_to_pypi.yml` & `rms_pdslogger-0.0.6/.github/workflows/publish_to_pypi.yml`

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

### Comparing `rms-pdslogger-0.0.5/.github/workflows/publish_to_test_pypi.yml` & `rms_pdslogger-0.0.6/.github/workflows/publish_to_test_pypi.yml`

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

### Comparing `rms-pdslogger-0.0.5/.github/workflows/run-tests.yml` & `rms_pdslogger-0.0.6/.github/workflows/run-tests.yml`

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
@@ -22,25 +22,29 @@
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
+          token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `rms-pdslogger-0.0.5/.gitignore` & `rms_pdslogger-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-pdslogger-0.0.5/LICENSE` & `rms_pdslogger-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-pdslogger-0.0.5/pdslogger/__init__.py` & `rms_pdslogger-0.0.6/pdslogger/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 try:
     import pdslogger.finder_colors as finder_colors
 except ImportError:         # OK because finder_colors are not always used
     pass
 
 try:
-    from _version import __version__
+    from ._version import __version__
 except ImportError as err:
     __version__ = 'Version unspecified'
 
 
 TIME_FMT = '%Y-%m-%d %H:%M:%S.%f'
 MAX_DEPTH = 8           # To avoid runaway opens that lack closes
```

### Comparing `rms-pdslogger-0.0.5/pdslogger/finder_colors.py` & `rms_pdslogger-0.0.6/pdslogger/finder_colors.py`

 * *Files identical despite different names*

### Comparing `rms-pdslogger-0.0.5/pyproject.toml` & `rms_pdslogger-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [build-system]
 requires = ["setuptools", "setuptools_scm[toml]"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rms-pdslogger"
 dynamic = ["version"]
-description = "Routines for converting to and from pdslogger dates"
+description = "Extension to the Python logging module"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "numpy",
     "pyparsing",
-    "rms-textkernel",
     "xattr; platform_system!='Windows'"
 ]
 license = {text = "Apache-2.0"}
 maintainers = [
   {name = "Robert S. French", email = "rfrench@seti.org"}
 ]
 keywords = ["pdslogger"]
```

