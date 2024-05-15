# Comparing `tmp/dsi_cocoa-0.2.2.tar.gz` & `tmp/dsi_cocoa-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.2.2.tar", last modified: Tue May 14 16:07:18 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.3.0.tar", last modified: Wed May 15 20:14:30 2024, max compression
```

## Comparing `dsi_cocoa-0.2.2.tar` & `dsi_cocoa-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:18.607231 dsi_cocoa-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:18.599231 dsi_cocoa-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:18.603231 dsi_cocoa-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-14 16:07:18.607231 dsi_cocoa-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-14 16:07:18.607231 dsi_cocoa-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:18.603231 dsi_cocoa-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:18.603231 dsi_cocoa-0.2.2/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-14 16:07:14.000000 dsi_cocoa-0.2.2/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:07:18.607231 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-14 16:07:18.000000 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-14 16:07:18.000000 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:07:18.000000 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 16:07:18.000000 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 16:07:18.000000 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 16:07:18.000000 dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:14:30.274829 dsi_cocoa-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 20:14:27.000000 dsi_cocoa-0.3.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:14:30.270828 dsi_cocoa-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:14:30.270828 dsi_cocoa-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-15 20:14:30.274829 dsi_cocoa-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/eval-repo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 20:14:30.274829 dsi_cocoa-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 20:14:27.000000 dsi_cocoa-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:14:30.270828 dsi_cocoa-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:14:30.274829 dsi_cocoa-0.3.0/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 20:14:27.000000 dsi_cocoa-0.3.0/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:14:30.274829 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-15 20:14:30.000000 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 20:14:30.000000 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:14:30.000000 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 20:14:30.000000 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 20:14:30.000000 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 20:14:30.000000 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.2.2/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.3.0/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.2/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.3.0/.github/workflows/publish.workflow.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,67 @@
 name: Publish Python Distribution to PyPI
 # adapted from
 # https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
 
 on:
   push:
-    tags:
-      - 'v[0-9]+.[0-9]+.[0-9]+'
-# publish when a new tag is pushed with semantic version
+    # trigger the workflow on push events to main branch
+    branches:
+      # - main
+      - publish-to-pypi
 
 jobs:
   build:
     name: Build distribution
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
+
       - name: Install pypa/build
         run: >-
           python3 -m
           pip install
-          build
+          build bump2version
           --user
+
+      - name: Set up Git identity
+        run: |
+          git config --global user.name "chenhuifei01"
+          git config --global user.email "chenhui1@uchicago.edu"
+
+      - name: Bump minor version
+        # haven't settip the cfg yet
+        run: bump2version minor --config-file .bumpversion.cfg
+
       - name: Build a binary wheel and a source tarball
         run: python3 -m build
+
       - name: Store the distribution packages
         uses: actions/upload-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
+
   publish-to-pypi:
     name: PublishPython distribution to PyPI
     needs:
       - build
     runs-on: ubuntu-latest
     environment:
       name: pypi
       url: https://pypi.org/p/dsi-cocoa
     permissions:
       id-token: write
-    
+
     steps:
       - name: Download all the dists
         uses: actions/download-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
       - name: Publish distributions to PyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `dsi_cocoa-0.2.2/.gitignore` & `dsi_cocoa-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.2/.pre-commit-config.yaml` & `dsi_cocoa-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.2/PKG-INFO` & `dsi_cocoa-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.2.2
+Version: 0.3.0
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -13,25 +13,27 @@
 Requires-Dist: pylint
 Requires-Dist: nbconvert
 Requires-Dist: ipython
 Requires-Dist: termcolor
 Requires-Dist: black
 Requires-Dist: requests
 
+update readme for testing
+
 # Clinic Opinionated Codebase Oversight and Analysis
 
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
 ```pip install dsi-cocoa```
 
-To install the package locally, run the following command from the root of the repository:
+To install the package from the local files, run the following command from the root of the repository:
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
 
 This package contains a module `evaluate_repo` which runs code testing libraries against a repository. There are multiple ways that we want to be able to run this repo:
@@ -63,34 +65,26 @@
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
-If you want to turn on linting, add the argument "--lint":
+If you want to do linting on Python files, then you can add the argument "--lint" to the command:
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
 
 ```bash
 cocoa /path/to/repo --verbose
 ```
 
-To report remote branch information, use the `--branchinfo` option.
-
-To run cocoa on files changed after a certain date, use the `--date` option with a date formatted as below.
-```bash
-cocoa /path/to/repo --date YYYY-MM-DD
-```
-
-
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
 1. WARNING: Most likely this needs to be fixed. 
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
```

### Comparing `dsi_cocoa-0.2.2/README.md` & `dsi_cocoa-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+update readme for testing
+
 # Clinic Opinionated Codebase Oversight and Analysis
 
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
 ```pip install dsi-cocoa```
 
-To install the package locally, run the following command from the root of the repository:
+To install the package from the local files, run the following command from the root of the repository:
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
 
 This package contains a module `evaluate_repo` which runs code testing libraries against a repository. There are multiple ways that we want to be able to run this repo:
@@ -44,34 +46,26 @@
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
-If you want to turn on linting, add the argument "--lint":
+If you want to do linting on Python files, then you can add the argument "--lint" to the command:
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
 
 ```bash
 cocoa /path/to/repo --verbose
 ```
 
-To report remote branch information, use the `--branchinfo` option.
-
-To run cocoa on files changed after a certain date, use the `--date` option with a date formatted as below.
-```bash
-cocoa /path/to/repo --date YYYY-MM-DD
-```
-
-
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
 1. WARNING: Most likely this needs to be fixed. 
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
```

### Comparing `dsi_cocoa-0.2.2/pyproject.toml` & `dsi_cocoa-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.2/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.3.0/src/cocoa/evaluate_repo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
 Main entry point for complete evaluation of a python codebase in git
 """
 
 import argparse
 import os
-import shutil
 
 from termcolor import cprint
 
 from cocoa.constants import (
     MAX_CELLS_PER_NOTEBOOK,
     MAX_FUNCTIONS_PER_NOTEBOOK,
     MAX_LINES_PER_CELL,
-    PREAMBLE_TEXT,
 )
 from cocoa.linting import (
     black_python_file,
     code_contains_subprocess,
     functions_without_docstrings,
     get_pylint_warnings,
     is_code_in_functions_or_main,
@@ -56,116 +54,94 @@
             for f in files
             if not any(x in os.path.join(root, f) for x in paths_to_flag)
         ]
 
     for file_path in files_to_process:
         if os.path.exists(file_path):
             if file_path.endswith(".ipynb") or file_path.endswith(".py"):
+                print(f"Analyzing {file_path}:")
                 if file_path.endswith(".ipynb"):
                     analyze_notebook(file_path, no_filter_flag, verbose)
                 elif file_path.endswith(".py"):
                     analyze_python_file(file_path, lint_flag, verbose)
+                print("-" * 80)
 
 
 def analyze_notebook(file_path, no_filter_flag, verbose):
     """Analyze a notebook"""
     num_cells, num_lines, num_functions, max_lines_in_cell = process_notebook(
         file_path
     )
     pyflake_results = pyflakes_notebook(file_path)
-
-    if (
-        pyflake_results
-        or num_cells > MAX_CELLS_PER_NOTEBOOK
+    print_results("PyFlakes", pyflake_results, verbose=verbose)
+    if no_filter_flag or (
+        num_cells > MAX_CELLS_PER_NOTEBOOK
         or max_lines_in_cell > MAX_LINES_PER_CELL
         or num_functions > MAX_FUNCTIONS_PER_NOTEBOOK
     ):
-        print(f"Analyzing {file_path}:")
-        if pyflake_results:
-            print_results("PyFlakes", pyflake_results, verbose=verbose)
-
-        if num_cells > MAX_CELLS_PER_NOTEBOOK:
-            print(f"\tMax number of cells exceeded: {num_cells}")
-        if max_lines_in_cell > MAX_LINES_PER_CELL:
-            print(
-                f"\tMax number of lines per cell exceeded: {max_lines_in_cell}"
-            )
-        if num_functions > MAX_FUNCTIONS_PER_NOTEBOOK:
-            print(f"\tFunction definitions detected: {num_functions}")
-
-        print("-" * 80)
+        print(f"\tNumber of cells: {num_cells}")
+        print(f"\tLines of code: {num_lines}")
+        print(f"\tNumber of function definitions: {num_functions}")
+        print(f"\tMax lines in a cell: {max_lines_in_cell}")
 
 
 def analyze_python_file(file_path, lint_flag, verbose):
     """Analyze a Python file"""
     pyflake_results = pyflakes_python_file(file_path)
-    black_results = black_python_file(file_path)
-    functions_no_docstrings = functions_without_docstrings(file_path)
-    contains_subprocess = code_contains_subprocess(file_path)
-    code_in_functions = is_code_in_functions_or_main(file_path)
     pylint_warnings = get_pylint_warnings(file_path)
+    black_results = black_python_file(file_path)
 
-    if (
-        (lint_flag and pylint_warnings)
-        or pyflake_results
-        or black_results
-        or functions_no_docstrings
-        or contains_subprocess
-        or not code_in_functions
-    ):
-        print(f"Analyzing {file_path}:")
+    if lint_flag:
+        print_results("Pylint", pylint_warnings, verbose=verbose)
+
+    print_results("PyFlakes", pyflake_results, verbose=verbose)
+
+    if black_results:
+        print(f"\tPlease run black. {len(black_results)} changes needed.")
 
-        if pyflake_results:
-            print_results("PyFlakes", pyflake_results, verbose=verbose)
-        if black_results:
-            print(f"\tBlack found {len(black_results)} issues")
-        if functions_no_docstrings:
-            print(
-                "\tFunctions without docstrings detected:",
-                functions_no_docstrings,
-            )
-        if contains_subprocess:
-            print("\tSubprocess usage detected.")
-        if not code_in_functions:
-            print("\tCode outside functions or main block detected.")
-        if lint_flag:
-            print_results("Pylint", pylint_warnings, verbose=verbose)
-        print("-" * 80)
+    if not is_code_in_functions_or_main(file_path):
+        print("\tCode outside functions or main block detected.")
+
+    if code_contains_subprocess(file_path):
+        print("\tWarning: subprocess usage detected.")
+
+    functions_no_docstrings = functions_without_docstrings(file_path)
+    if functions_no_docstrings:
+        print(
+            "\tFunctions without docstrings detected:", functions_no_docstrings
+        )
 
 
 def print_results(tool_name, results, verbose=False):
     """Print results from pylint or pyflake"""
     if results:
         if verbose:
-            print(f"\t{tool_name} found {len(results)} issues:")
+            print(f"{tool_name} found {len(results)} issues:")
             for result in results:
-                print(f"\t  {result}")
+                print(f"  {result}")
         else:
-            print(f"\t{tool_name} found {len(results)} issues:")
+            print(f"{tool_name} found {len(results)} issues:")
             for result in results[:5]:
-                print(f"\t  {result}")
+                print(f"  {result}")
             if len(results) > 5:
-                print(f"\t  ...and {len(results) - 5} more issues.")
+                print(f"  ...and {len(results) - 5} more issues.")
 
 
-def evaluate_repo(
-    path_or_url, lint_flag, start_date=None, verbose=False, branchinfo=False
-):
+def evaluate_repo(path_or_url, lint_flag, start_date=None, verbose=False):
     """
     This is the entry point to running the automated code review.
     """
-    cprint(PREAMBLE_TEXT, color="green")
+
     if os.path.isdir(path_or_url):
         if not is_git_repo(path_or_url):
             print(f"Error: {path_or_url} is not a Git repository.")
             exit(1)
 
         check_branch_names(path_or_url)
-        if branchinfo:
-            get_remote_branches_info(path_or_url)
+        get_remote_branches_info(path_or_url)
         walk_and_process(
             path_or_url,
             None,
             lint_flag=lint_flag,
             start_date=start_date,
             verbose=verbose,
         )
@@ -173,19 +149,16 @@
         repo_path = clone_repo(path_or_url)
         evaluate_repo(
             repo_path,
             lint_flag=lint_flag,
             start_date=start_date,
             verbose=verbose,
         )
-        shutil.rmtree(repo_path)
     else:
-        print(
-            f"Error: {path_or_url} is either private or not a git repository. 404."
-        )
+        print(f"Error: {path_or_url} is not a Git repository URL.")
         exit(1)
     return 0
 
 
 def main():
     parser = argparse.ArgumentParser(description="COCOA CLI")
 
@@ -196,24 +169,20 @@
     )
     parser.add_argument(
         "--date",
         default=None,
         help="Start date in YYYY-MM-DD format to filter files by commit date",
         type=str,
     )
-    parser.add_argument(
-        "--branchinfo", help="Report branch information", action="store_true"
-    )
 
     args = parser.parse_args()
 
     dir_path = args.repo
     lint_flag = args.lint
     start_date = args.date
     verbose = args.verbose
-    branchinfo = args.branchinfo
 
-    evaluate_repo(dir_path, lint_flag, start_date, verbose, branchinfo)
+    evaluate_repo(dir_path, lint_flag, start_date, verbose)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dsi_cocoa-0.2.2/src/cocoa/linting.py` & `dsi_cocoa-0.3.0/src/cocoa/linting.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.2/src/cocoa/notebooks.py` & `dsi_cocoa-0.3.0/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.2/src/cocoa/repo.py` & `dsi_cocoa-0.3.0/src/cocoa/repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.2/src/cocoa/spring2024.py` & `dsi_cocoa-0.3.0/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.2.2
+Version: 0.3.0
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -13,25 +13,27 @@
 Requires-Dist: pylint
 Requires-Dist: nbconvert
 Requires-Dist: ipython
 Requires-Dist: termcolor
 Requires-Dist: black
 Requires-Dist: requests
 
+update readme for testing
+
 # Clinic Opinionated Codebase Oversight and Analysis
 
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
 ```pip install dsi-cocoa```
 
-To install the package locally, run the following command from the root of the repository:
+To install the package from the local files, run the following command from the root of the repository:
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
 
 This package contains a module `evaluate_repo` which runs code testing libraries against a repository. There are multiple ways that we want to be able to run this repo:
@@ -63,34 +65,26 @@
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
-If you want to turn on linting, add the argument "--lint":
+If you want to do linting on Python files, then you can add the argument "--lint" to the command:
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
 
 ```bash
 cocoa /path/to/repo --verbose
 ```
 
-To report remote branch information, use the `--branchinfo` option.
-
-To run cocoa on files changed after a certain date, use the `--date` option with a date formatted as below.
-```bash
-cocoa /path/to/repo --date YYYY-MM-DD
-```
-
-
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
 1. WARNING: Most likely this needs to be fixed. 
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
```

### Comparing `dsi_cocoa-0.2.2/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+.bumpversion.cfg
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 README.md
+eval-repo.sh
 pyproject.toml
 requirements.txt
 setup.cfg
+setup.py
 .github/workflows/main.workflow.yml
 .github/workflows/publish.workflow.yml
 src/cocoa/__init__.py
 src/cocoa/constants.py
 src/cocoa/evaluate_repo.py
 src/cocoa/linting.py
 src/cocoa/notebooks.py
```

