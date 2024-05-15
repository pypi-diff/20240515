# Comparing `tmp/dsi_cocoa-0.3.0.tar.gz` & `tmp/dsi_cocoa-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.3.0.tar", last modified: Wed May 15 20:14:30 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.4.0.tar", last modified: Wed May 15 20:27:22 2024, max compression
```

## Comparing `dsi_cocoa-0.3.0.tar` & `dsi_cocoa-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:14:30.274829 dsi_cocoa-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 20:14:27.000000 dsi_cocoa-0.3.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:14:30.270828 dsi_cocoa-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:14:30.270828 dsi_cocoa-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-15 20:14:30.274829 dsi_cocoa-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/eval-repo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 20:14:30.274829 dsi_cocoa-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 20:14:27.000000 dsi_cocoa-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:14:30.270828 dsi_cocoa-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:14:30.274829 dsi_cocoa-0.3.0/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 20:14:27.000000 dsi_cocoa-0.3.0/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-15 20:14:21.000000 dsi_cocoa-0.3.0/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:14:30.274829 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-15 20:14:30.000000 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 20:14:30.000000 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:14:30.000000 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 20:14:30.000000 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 20:14:30.000000 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 20:14:30.000000 dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:27:22.547509 dsi_cocoa-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 20:27:19.000000 dsi_cocoa-0.4.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:27:22.543509 dsi_cocoa-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:27:22.547509 dsi_cocoa-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-15 20:27:22.547509 dsi_cocoa-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/eval-repo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 20:27:22.547509 dsi_cocoa-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 20:27:19.000000 dsi_cocoa-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:27:22.543509 dsi_cocoa-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:27:22.547509 dsi_cocoa-0.4.0/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 20:27:19.000000 dsi_cocoa-0.4.0/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-15 20:27:12.000000 dsi_cocoa-0.4.0/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:27:22.547509 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-15 20:27:22.000000 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 20:27:22.000000 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:27:22.000000 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 20:27:22.000000 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 20:27:22.000000 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 20:27:22.000000 dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.3.0/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.4.0/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.3.0/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.4.0/.github/workflows/publish.workflow.yml`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,16 @@
       - name: Set up Git identity
         run: |
           git config --global user.name "chenhuifei01"
           git config --global user.email "chenhui1@uchicago.edu"
 
       - name: Bump minor version
         # haven't settip the cfg yet
-        run: bump2version minor --config-file .bumpversion.cfg
+        # run: bump2version minor --config-file .bumpversion.cfg
+        run: bump2version minor
 
       - name: Build a binary wheel and a source tarball
         run: python3 -m build
 
       - name: Store the distribution packages
         uses: actions/upload-artifact@v3
         with:
```

### Comparing `dsi_cocoa-0.3.0/.gitignore` & `dsi_cocoa-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.3.0/.pre-commit-config.yaml` & `dsi_cocoa-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.3.0/PKG-INFO` & `dsi_cocoa-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.3.0
+Version: 0.4.0
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -13,27 +13,26 @@
 Requires-Dist: pylint
 Requires-Dist: nbconvert
 Requires-Dist: ipython
 Requires-Dist: termcolor
 Requires-Dist: black
 Requires-Dist: requests
 
-update readme for testing
-
 # Clinic Opinionated Codebase Oversight and Analysis
 
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
-```pip install dsi-cocoa```
+`pip install dsi-cocoa`
 
 To install the package from the local files, run the following command from the root of the repository:
+
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
 
 This package contains a module `evaluate_repo` which runs code testing libraries against a repository. There are multiple ways that we want to be able to run this repo:
@@ -41,38 +40,42 @@
 1. We want to be able to clone `cocoa` and then use it as part of their process.
 2. We want administrators to be able to give it a list of repos to generate reports on all repos.
 3. (Eventually) We want it to be able to run as a github action _on the repo itself_.
 4. (Eventually) We want to be able to have adminstrative repo that can run it on other repos.
 
 ### How to run
 
-Via command line: 
+Via command line:
+
 ```bash
 cocoa /path/to/repo
 ```
 
-As a python script: 
+As a python script:
+
 ```bash
 python3 src/cocoa/evaluate_repo.py /path/to/repo
 ```
 
 As a Python module:
+
 ```python
 from cocoa.evaluate_repo import evaluate_repo
 
 evaluate_repo('/path/to/repo', False)
 ```
 
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
+
 If you want to do linting on Python files, then you can add the argument "--lint" to the command:
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
@@ -81,31 +84,30 @@
 cocoa /path/to/repo --verbose
 ```
 
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
-1. WARNING: Most likely this needs to be fixed. 
+1. WARNING: Most likely this needs to be fixed.
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
 
 For each of the checks below we have denoted what the check generates.
 
 - Branch Hygiene:
-    - [WARNING] Branch names 
-    - [INFO] Commit information for live branches.
+  - [WARNING] Branch names
+  - [INFO] Commit information for live branches.
 - File Hygiene:
-    - [ERROR] Unnecessary and cache file (such as .DS\_Store or pycache files)
-- Notebook Files (*.ipynb):
-    - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
-    - [ERROR] Linting: PyLint, Black, Flake and iSort
+  - [ERROR] Unnecessary and cache file (such as .DS_Store or pycache files)
+- Notebook Files (\*.ipynb):
+  - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
+  - [ERROR] Linting: PyLint, Black, Flake and iSort
 - Python Files
-    - [ERROR] All Code in Functions
-    - [ERROR] All functions have docstrings
-    - [ERROR] Code uses off-limit libraries (subprocess)
-    - [ERROR] Linting: PyLint, Black, Flake and iSort
-    
+  - [ERROR] All Code in Functions
+  - [ERROR] All functions have docstrings
+  - [ERROR] Code uses off-limit libraries (subprocess)
+  - [ERROR] Linting: PyLint, Black, Flake and iSort
+
 ### Github actions
 
 For each of the ERRORS and WARNINGS above there is an associated github action that can be run to create a badge which we put in a table at the top of each clinic repo.
-
```

### Comparing `dsi_cocoa-0.3.0/README.md` & `dsi_cocoa-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-update readme for testing
-
 # Clinic Opinionated Codebase Oversight and Analysis
 
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
-```pip install dsi-cocoa```
+`pip install dsi-cocoa`
 
 To install the package from the local files, run the following command from the root of the repository:
+
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
 
 This package contains a module `evaluate_repo` which runs code testing libraries against a repository. There are multiple ways that we want to be able to run this repo:
@@ -22,38 +21,42 @@
 1. We want to be able to clone `cocoa` and then use it as part of their process.
 2. We want administrators to be able to give it a list of repos to generate reports on all repos.
 3. (Eventually) We want it to be able to run as a github action _on the repo itself_.
 4. (Eventually) We want to be able to have adminstrative repo that can run it on other repos.
 
 ### How to run
 
-Via command line: 
+Via command line:
+
 ```bash
 cocoa /path/to/repo
 ```
 
-As a python script: 
+As a python script:
+
 ```bash
 python3 src/cocoa/evaluate_repo.py /path/to/repo
 ```
 
 As a Python module:
+
 ```python
 from cocoa.evaluate_repo import evaluate_repo
 
 evaluate_repo('/path/to/repo', False)
 ```
 
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
+
 If you want to do linting on Python files, then you can add the argument "--lint" to the command:
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
@@ -62,31 +65,30 @@
 cocoa /path/to/repo --verbose
 ```
 
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
-1. WARNING: Most likely this needs to be fixed. 
+1. WARNING: Most likely this needs to be fixed.
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
 
 For each of the checks below we have denoted what the check generates.
 
 - Branch Hygiene:
-    - [WARNING] Branch names 
-    - [INFO] Commit information for live branches.
+  - [WARNING] Branch names
+  - [INFO] Commit information for live branches.
 - File Hygiene:
-    - [ERROR] Unnecessary and cache file (such as .DS\_Store or pycache files)
-- Notebook Files (*.ipynb):
-    - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
-    - [ERROR] Linting: PyLint, Black, Flake and iSort
+  - [ERROR] Unnecessary and cache file (such as .DS_Store or pycache files)
+- Notebook Files (\*.ipynb):
+  - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
+  - [ERROR] Linting: PyLint, Black, Flake and iSort
 - Python Files
-    - [ERROR] All Code in Functions
-    - [ERROR] All functions have docstrings
-    - [ERROR] Code uses off-limit libraries (subprocess)
-    - [ERROR] Linting: PyLint, Black, Flake and iSort
-    
+  - [ERROR] All Code in Functions
+  - [ERROR] All functions have docstrings
+  - [ERROR] Code uses off-limit libraries (subprocess)
+  - [ERROR] Linting: PyLint, Black, Flake and iSort
+
 ### Github actions
 
 For each of the ERRORS and WARNINGS above there is an associated github action that can be run to create a badge which we put in a table at the top of each clinic repo.
-
```

### Comparing `dsi_cocoa-0.3.0/pyproject.toml` & `dsi_cocoa-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.3.0/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.4.0/src/cocoa/evaluate_repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.3.0/src/cocoa/linting.py` & `dsi_cocoa-0.4.0/src/cocoa/linting.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.3.0/src/cocoa/notebooks.py` & `dsi_cocoa-0.4.0/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.3.0/src/cocoa/repo.py` & `dsi_cocoa-0.4.0/src/cocoa/repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.3.0/src/cocoa/spring2024.py` & `dsi_cocoa-0.4.0/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.3.0
+Version: 0.4.0
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -13,27 +13,26 @@
 Requires-Dist: pylint
 Requires-Dist: nbconvert
 Requires-Dist: ipython
 Requires-Dist: termcolor
 Requires-Dist: black
 Requires-Dist: requests
 
-update readme for testing
-
 # Clinic Opinionated Codebase Oversight and Analysis
 
 This repository was developed in order to generate automated reports on how well codebases adhere to the [coding standards](https://github.com/dsi-clinic/coding-standards) of the University of Chicago's DSI [Clinic course](https://datascience.uchicago.edu/education/data-science-clinic/).
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
-```pip install dsi-cocoa```
+`pip install dsi-cocoa`
 
 To install the package from the local files, run the following command from the root of the repository:
+
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
 
 This package contains a module `evaluate_repo` which runs code testing libraries against a repository. There are multiple ways that we want to be able to run this repo:
@@ -41,38 +40,42 @@
 1. We want to be able to clone `cocoa` and then use it as part of their process.
 2. We want administrators to be able to give it a list of repos to generate reports on all repos.
 3. (Eventually) We want it to be able to run as a github action _on the repo itself_.
 4. (Eventually) We want to be able to have adminstrative repo that can run it on other repos.
 
 ### How to run
 
-Via command line: 
+Via command line:
+
 ```bash
 cocoa /path/to/repo
 ```
 
-As a python script: 
+As a python script:
+
 ```bash
 python3 src/cocoa/evaluate_repo.py /path/to/repo
 ```
 
 As a Python module:
+
 ```python
 from cocoa.evaluate_repo import evaluate_repo
 
 evaluate_repo('/path/to/repo', False)
 ```
 
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
+
 If you want to do linting on Python files, then you can add the argument "--lint" to the command:
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
@@ -81,31 +84,30 @@
 cocoa /path/to/repo --verbose
 ```
 
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
-1. WARNING: Most likely this needs to be fixed. 
+1. WARNING: Most likely this needs to be fixed.
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
 
 For each of the checks below we have denoted what the check generates.
 
 - Branch Hygiene:
-    - [WARNING] Branch names 
-    - [INFO] Commit information for live branches.
+  - [WARNING] Branch names
+  - [INFO] Commit information for live branches.
 - File Hygiene:
-    - [ERROR] Unnecessary and cache file (such as .DS\_Store or pycache files)
-- Notebook Files (*.ipynb):
-    - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
-    - [ERROR] Linting: PyLint, Black, Flake and iSort
+  - [ERROR] Unnecessary and cache file (such as .DS_Store or pycache files)
+- Notebook Files (\*.ipynb):
+  - [ERROR] Cells per notebook < 10, lines per cell < 15 and 0 functions defined
+  - [ERROR] Linting: PyLint, Black, Flake and iSort
 - Python Files
-    - [ERROR] All Code in Functions
-    - [ERROR] All functions have docstrings
-    - [ERROR] Code uses off-limit libraries (subprocess)
-    - [ERROR] Linting: PyLint, Black, Flake and iSort
-    
+  - [ERROR] All Code in Functions
+  - [ERROR] All functions have docstrings
+  - [ERROR] Code uses off-limit libraries (subprocess)
+  - [ERROR] Linting: PyLint, Black, Flake and iSort
+
 ### Github actions
 
 For each of the ERRORS and WARNINGS above there is an associated github action that can be run to create a badge which we put in a table at the top of each clinic repo.
-
```

### Comparing `dsi_cocoa-0.3.0/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.4.0/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

