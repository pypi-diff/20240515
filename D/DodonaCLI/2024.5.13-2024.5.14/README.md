# Comparing `tmp/dodonacli-2024.5.13.tar.gz` & `tmp/dodonacli-2024.5.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodonacli-2024.5.13.tar", last modified: Mon May 13 10:22:25 2024, max compression
+gzip compressed data, was "dodonacli-2024.5.14.tar", last modified: Tue May 14 20:48:17 2024, max compression
```

## Comparing `dodonacli-2024.5.13.tar` & `dodonacli-2024.5.14.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.213991 dodonacli-2024.5.13/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.205991 dodonacli-2024.5.13/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.209991 dodonacli-2024.5.13/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/.github/workflows/set_version.yml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.213991 dodonacli-2024.5.13/DodonaCLI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-13 10:22:25.000000 dodonacli-2024.5.13/DodonaCLI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-13 10:22:25.000000 dodonacli-2024.5.13/DodonaCLI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:22:25.000000 dodonacli-2024.5.13/DodonaCLI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 10:22:25.000000 dodonacli-2024.5.13/DodonaCLI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 10:22:25.000000 dodonacli-2024.5.13/DodonaCLI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 10:22:25.000000 dodonacli-2024.5.13/DodonaCLI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-13 10:22:25.213991 dodonacli-2024.5.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.209991 dodonacli-2024.5.13/dodonacli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.209991 dodonacli-2024.5.13/dodonacli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/cli_next.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/commands/up.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.213991 dodonacli-2024.5.13/dodonacli/source/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/get_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/interactive_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/pretty_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/set_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/submission_data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli/source/syntax_checker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/dodonacli_completion_script.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:22:25.213991 dodonacli-2024.5.13/man-page/
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/man-page/dodonacli.1
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/man-page/dodonacli.1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-13 10:22:18.000000 dodonacli-2024.5.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:22:25.213991 dodonacli-2024.5.13/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:17.700225 dodonacli-2024.5.14/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:17.696226 dodonacli-2024.5.14/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:17.696226 dodonacli-2024.5.14/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:17.700225 dodonacli-2024.5.14/DodonaCLI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-05-14 20:48:17.000000 dodonacli-2024.5.14/DodonaCLI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-14 20:48:17.000000 dodonacli-2024.5.14/DodonaCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:48:17.000000 dodonacli-2024.5.14/DodonaCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 20:48:17.000000 dodonacli-2024.5.14/DodonaCLI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 20:48:17.000000 dodonacli-2024.5.14/DodonaCLI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 20:48:17.000000 dodonacli-2024.5.14/DodonaCLI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-05-14 20:48:17.700225 dodonacli-2024.5.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:17.696226 dodonacli-2024.5.14/dodonacli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:17.700225 dodonacli-2024.5.14/dodonacli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/commands/cli_next.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/commands/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/commands/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/commands/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/commands/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/commands/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/commands/up.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:17.700225 dodonacli-2024.5.14/dodonacli/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/source/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/source/interactive_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/source/pretty_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/source/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/source/set_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/source/submission_data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli/source/syntax_checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/dodonacli_completion_script.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:48:17.700225 dodonacli-2024.5.14/man-page/
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/man-page/dodonacli.1
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-14 20:48:09.000000 dodonacli-2024.5.14/man-page/dodonacli.1.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-14 20:48:11.000000 dodonacli-2024.5.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:48:17.700225 dodonacli-2024.5.14/setup.cfg
```

### Comparing `dodonacli-2024.5.13/.github/workflows/publish_test.yml` & `dodonacli-2024.5.14/.github/workflows/publish_test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 name: Publish to test.PyPI
 
 on:
   workflow_dispatch
 
 jobs:
- build-and-publish:
-  runs-on: ubuntu-latest
+  build-and-publish:
+    runs-on: ubuntu-latest
 
-  steps:
-   - name: Checkout code
-     uses: actions/checkout@v3
-
-   - name: Set up Python
-     uses: actions/setup-python@v3
-     with:
-       python-version: '3.8'
-
-   - name: Install dependencies
-     run: |
-      python -m pip install --upgrade pip
-      pip install build
-
-   - name: Build package
-     run: python -m build
-
-   - name: Publish to TestPyPI
-     uses: pypa/gh-action-pypi-publish@release/v1
-     with:
-       user: __token__
-       password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-       repository-url: https://test.pypi.org/legacy/
+    steps:
+      - name: Checkout code
+        uses: actions/checkout@v4
+
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: '3.10'
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install build
+
+      - name: Build package
+        run: python -m build
+
+      - name: Publish to TestPyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          user: __token__
+          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
+          repository-url: https://test.pypi.org/legacy/
```

### Comparing `dodonacli-2024.5.13/DodonaCLI.egg-info/PKG-INFO` & `dodonacli-2024.5.14/DodonaCLI.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DodonaCLI
-Version: 2024.5.13
+Version: 2024.5.14
 Summary: A CLI tool for Dodona
 Author-email: Bram Windey <windey.bram@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Bram Windey
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -127,15 +127,15 @@
 - --use-link
 
 They are all context-specific. A short explanation can be found in the help-pages, a slightly longer one here:
 
 ### Force 
 This flag is used in combination with the `display` command, when viewing exercise-series and exercise-descriptions. 
 It will do its best to render the html and markdown of the web-page in your terminal. 
-You’ll quickly see why this is hidden behind this flag: the formatting can be aweful. 
+You’ll quickly see why this is hidden behind this flag: the formatting can be awful. 
 For some exercise-descriptions, this can, however, be a nice addition,
 and in the future the formatting-"engine" can improve.
 
 
 ### Hidden 
 This flag is used in combination with the `select` command, when selecting an exercise-series that is hidden. 
 Series can be hidden when they are used in tests or exams, and to get to them, you’ll receive a link to it from your 
@@ -175,20 +175,20 @@
 to see if this is indeed the issue.
 
 
 ## Roadmap
 This section has a bunch of ideas for me to work on, but also for you, the potential contributor!
 Remember to look at the recent branches/commits to see if I’m not working on one of these:
 - user-settings (f.e. auto-download of files, language, formatting, number of submissions shown, config location, ...)
+- improve `info` command (man-page and such)
+- improve `tutorial`
 - easy (automatic?) downloading of files mentioned in exercise description
 - improve the rendering of all html/markdown frankensteins, in descriptions of exercises and exercise-descriptions 
 - add connection time-out to prevent long waiting when IPv6 doesn’t want to work along
 - add support for more languages syntax checkers
 - caching some info for faster navigation and/or autocompletion
 - add indicator to series to mark if all their exercises are completely solved (maybe fetch from html-version)
-- get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30). Am I salty about that not being just field in the API, yes I am! Glad you noticed. Html-parsing isn’t a hobby of mine after all
-- format weird markup in some feedback of submissions (like the Python and bash exercises)
-- add "completions_script" and "manpage" as subcommands to "info"
+- get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30)
 
-Github stuff to figure out:
+GitHub stuff to figure out:
 - release by tag/release
 - action to check valid version before trying to push, if not valid, make it valid
```

### Comparing `dodonacli-2024.5.13/DodonaCLI.egg-info/SOURCES.txt` & `dodonacli-2024.5.14/DodonaCLI.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 LICENSE
 README.md
 dodonacli_completion_script.sh
 pyproject.toml
 .github/PULL_REQUEST_TEMPLATE.md
 .github/workflows/publish.yml
 .github/workflows/publish_test.yml
-.github/workflows/set_version.yml
 DodonaCLI.egg-info/PKG-INFO
 DodonaCLI.egg-info/SOURCES.txt
 DodonaCLI.egg-info/dependency_links.txt
 DodonaCLI.egg-info/entry_points.txt
 DodonaCLI.egg-info/requires.txt
 DodonaCLI.egg-info/top_level.txt
 dodonacli/__init__.py
```

### Comparing `dodonacli-2024.5.13/LICENSE` & `dodonacli-2024.5.14/LICENSE`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/PKG-INFO` & `dodonacli-2024.5.14/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DodonaCLI
-Version: 2024.5.13
+Version: 2024.5.14
 Summary: A CLI tool for Dodona
 Author-email: Bram Windey <windey.bram@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Bram Windey
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -127,15 +127,15 @@
 - --use-link
 
 They are all context-specific. A short explanation can be found in the help-pages, a slightly longer one here:
 
 ### Force 
 This flag is used in combination with the `display` command, when viewing exercise-series and exercise-descriptions. 
 It will do its best to render the html and markdown of the web-page in your terminal. 
-You’ll quickly see why this is hidden behind this flag: the formatting can be aweful. 
+You’ll quickly see why this is hidden behind this flag: the formatting can be awful. 
 For some exercise-descriptions, this can, however, be a nice addition,
 and in the future the formatting-"engine" can improve.
 
 
 ### Hidden 
 This flag is used in combination with the `select` command, when selecting an exercise-series that is hidden. 
 Series can be hidden when they are used in tests or exams, and to get to them, you’ll receive a link to it from your 
@@ -175,20 +175,20 @@
 to see if this is indeed the issue.
 
 
 ## Roadmap
 This section has a bunch of ideas for me to work on, but also for you, the potential contributor!
 Remember to look at the recent branches/commits to see if I’m not working on one of these:
 - user-settings (f.e. auto-download of files, language, formatting, number of submissions shown, config location, ...)
+- improve `info` command (man-page and such)
+- improve `tutorial`
 - easy (automatic?) downloading of files mentioned in exercise description
 - improve the rendering of all html/markdown frankensteins, in descriptions of exercises and exercise-descriptions 
 - add connection time-out to prevent long waiting when IPv6 doesn’t want to work along
 - add support for more languages syntax checkers
 - caching some info for faster navigation and/or autocompletion
 - add indicator to series to mark if all their exercises are completely solved (maybe fetch from html-version)
-- get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30). Am I salty about that not being just field in the API, yes I am! Glad you noticed. Html-parsing isn’t a hobby of mine after all
-- format weird markup in some feedback of submissions (like the Python and bash exercises)
-- add "completions_script" and "manpage" as subcommands to "info"
+- get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30)
 
-Github stuff to figure out:
+GitHub stuff to figure out:
 - release by tag/release
 - action to check valid version before trying to push, if not valid, make it valid
```

### Comparing `dodonacli-2024.5.13/README.md` & `dodonacli-2024.5.14/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 - --use-link
 
 They are all context-specific. A short explanation can be found in the help-pages, a slightly longer one here:
 
 ### Force 
 This flag is used in combination with the `display` command, when viewing exercise-series and exercise-descriptions. 
 It will do its best to render the html and markdown of the web-page in your terminal. 
-You’ll quickly see why this is hidden behind this flag: the formatting can be aweful. 
+You’ll quickly see why this is hidden behind this flag: the formatting can be awful. 
 For some exercise-descriptions, this can, however, be a nice addition,
 and in the future the formatting-"engine" can improve.
 
 
 ### Hidden 
 This flag is used in combination with the `select` command, when selecting an exercise-series that is hidden. 
 Series can be hidden when they are used in tests or exams, and to get to them, you’ll receive a link to it from your 
@@ -132,20 +132,20 @@
 to see if this is indeed the issue.
 
 
 ## Roadmap
 This section has a bunch of ideas for me to work on, but also for you, the potential contributor!
 Remember to look at the recent branches/commits to see if I’m not working on one of these:
 - user-settings (f.e. auto-download of files, language, formatting, number of submissions shown, config location, ...)
+- improve `info` command (man-page and such)
+- improve `tutorial`
 - easy (automatic?) downloading of files mentioned in exercise description
 - improve the rendering of all html/markdown frankensteins, in descriptions of exercises and exercise-descriptions 
 - add connection time-out to prevent long waiting when IPv6 doesn’t want to work along
 - add support for more languages syntax checkers
 - caching some info for faster navigation and/or autocompletion
 - add indicator to series to mark if all their exercises are completely solved (maybe fetch from html-version)
-- get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30). Am I salty about that not being just field in the API, yes I am! Glad you noticed. Html-parsing isn’t a hobby of mine after all
-- format weird markup in some feedback of submissions (like the Python and bash exercises)
-- add "completions_script" and "manpage" as subcommands to "info"
+- get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30)
 
-Github stuff to figure out:
+GitHub stuff to figure out:
 - release by tag/release
 - action to check valid version before trying to push, if not valid, make it valid
```

### Comparing `dodonacli-2024.5.13/dodonacli/commands/cli_next.py` & `dodonacli-2024.5.14/dodonacli/commands/cli_next.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/dodonacli/commands/display.py` & `dodonacli-2024.5.14/dodonacli/commands/display.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/dodonacli/commands/info.py` & `dodonacli-2024.5.14/dodonacli/commands/info.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 def changelog():
     from rich.markdown import Markdown
     from dodonacli.source import pretty_console
 
     changelog_raw = """
 - Working on rendering feedback. Please report any troubles you have. 
 I may not be able to solve them, but I can definitly hide them =D
-This is not a full implementation, you should only be able to see which tabs were wrong and wich were correct.
+- I think this is in its final state, so definitly report all bugs
 
 As always, you can use the "--help" flag after every command and sub-command to learn more.
 Happy coding!
     """
     md = Markdown(changelog_raw)
     pretty_console.console.print(md)
```

### Comparing `dodonacli-2024.5.13/dodonacli/commands/post.py` & `dodonacli-2024.5.14/dodonacli/commands/post.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/dodonacli/commands/select.py` & `dodonacli-2024.5.14/dodonacli/commands/select.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/dodonacli/commands/submission.py` & `dodonacli-2024.5.14/dodonacli/commands/submission.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/dodonacli/commands/up.py` & `dodonacli-2024.5.14/dodonacli/commands/up.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/dodonacli/main.py` & `dodonacli-2024.5.14/dodonacli/main.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/dodonacli/source/get_data.py` & `dodonacli-2024.5.14/dodonacli/source/get_data.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/dodonacli/source/interactive_tutorial.py` & `dodonacli-2024.5.14/dodonacli/source/interactive_tutorial.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/dodonacli/source/pretty_print.py` & `dodonacli-2024.5.14/dodonacli/source/pretty_print.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,14 @@
     Print out the results of a submission in a neat way
     :param json_results: json object with data about a submission
     """
     if json_results['accepted']:
         # Everything passed, well done!
         pretty_console.console.print("[bold bright_green]All tests passed![/] You can continue to next exercise.")
     else:
-        pretty_console.console.print("[bold bright_red]Some tests faild.[/]")
         pretty_console.console.print(submission_data_handler.submission_data_handler(json_results))
 
 
 def print_status(config: dict):
     """
     Print out the current selection of course, exercise-series and exercise.
     :param config: Dictionary with the configs
```

### Comparing `dodonacli-2024.5.13/dodonacli/source/set_data.py` & `dodonacli-2024.5.14/dodonacli/source/set_data.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/dodonacli/source/submission_data_handler.py` & `dodonacli-2024.5.14/dodonacli/source/submission_data_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,97 +15,109 @@
     correct_tabs = []
     for tab in submission_data['groups']:
         if tab['badgeCount'] > 0:
             failed_tabs.append(tab)
         else:
             correct_tabs.append(tab)
 
-    result = "\n[bold bright_red]Wrong tabs[/]:"
-    for failed_tab in failed_tabs:
-        result += failed_tab_handler(failed_tab)
+    result = "[bold bright_red]Wrong tabs[/]:"
+    result += ''.join(failed_tab_handler(failed_tab) for failed_tab in failed_tabs)
 
     if len(correct_tabs) > 0:
         result += "\n\n[bold bright_green]Correct tabs:[/] "
         result += ', '.join([tab['description'] for tab in correct_tabs])
 
     return result
 
 
 def failed_tab_handler(tab: dict) -> str:
     """
     Handle failed tabs by delegating the first 3 failed contexts
     :param tab: dictionary with a failed tab
     :return: formatted string with failed tab things
     """
-    result = f"\n[bold bright_red] \u00B7 [/]{tab['description']} ({tab['badgeCount']}):"
+    result = f"\n[bold bright_red] \u00B7 [/][u]{str(tab['description']).capitalize()} ({tab['badgeCount']}):[/]"
     contexts = tab['groups']
     index = 0
     amount_failed = 0
 
-    # while index < len(contexts) and amount_failed < 3:
-    #     context = contexts[index]
-    #     if context['accepted']:
-    #         index += 1
-    #         continue
-    #     result += failed_context_handler(context)
-    #     amount_failed += 1
-    #     index += 1
+    while index < len(contexts) and amount_failed < 3:
+        context = contexts[index]
+        if context['accepted']:
+            index += 1
+            continue
+        result += failed_context_handler(context)
+        amount_failed += 1
+        index += 1
     return result
 
 
 def failed_context_handler(context: dict) -> str:
     result = ""
-    if 'data' in context:
-        result += f"\n\t- {context['data']['statements'].strip()}:"
-    elif 'description' in context:
-        result += f"\n\t- {context['description']['description']}:"
+    # if 'data' in context:
+    #     result += f"\n\t[bright_red]\u00B7[/] {context['data']['statements'].strip()}:"
+    # elif 'description' in context:
+    #     result += f"\n\t[bright_red]\u00B7[/] {context['description']['description']}:"
 
     test_cases = context['groups']
     index = 0
     amount_failed = 0
 
+    context_content = []
+
     while index < len(test_cases) and amount_failed < 3:
         test_case = test_cases[index]
 
         if 'tests' in test_case:
-            result += failed_tests_handler(test_case)
-            pass
+            context_content.extend(failed_tests_handler(test_case))
         else:
-            result += f"\n\t\t- {test_case['description']['description']}"
+            if test_case['accepted']:
+                emoji = '[bright_green]:heavy_check_mark:[/] '
+            else:
+                emoji = "[bright_red]:heavy_multiplication_x:[/] "
+            context_content.append(emoji + test_case['description']['description'].rstrip())
 
         if not test_case['accepted']:
             amount_failed += 1
         index += 1
 
+    if len(context_content) > 1:
+        result += f"\n   \u256D {context_content[0]}" + (len(context_content[1:-1]) > 0) * "\n   \u2502 "
+        result += "\n   \u2502 ".join(cc for cc in context_content[1:-1])
+        result += f"\n   \u2570 {context_content[-1]}\n"
+    else:
+        result += "\n   - " + context_content[0] + "\n"
+
     return result
 
 
-def failed_tests_handler(test_case: dict) -> str:
-    result = ""
+def failed_tests_handler(test_case: dict) -> list:
+    result = []
     if 'data' in test_case:
-        result += f"\n\t- {test_case['data']['statements'].strip()}:"
+        result.append(test_case['data']['statements'].rstrip())
     elif 'description' in test_case:
-        result += f"\n\t- {test_case['description']['description']}:"
+        result.append(test_case['description']['description'].rstrip())
 
     tests = test_case['tests']
     if all(test['accepted'] for test in tests):
-        result = result.rstrip('\n') + " [bright_green]:heavy_check_mark:[/]"
+        result[-1] = "[bright_green]:heavy_check_mark:[/] " + result[-1]
         return result
+    else:
+        result[-1] = "[bright_red]:heavy_multiplication_x:[/] " + result[-1]
 
     index = 0
     amount_failed = 0
 
     while index < len(tests) and amount_failed < 3:
         test = tests[index]
-
-        result += f"\n\t\tExpected:\t{test['expected']}"
-        result += f"\n\t\tActual:  \t{test['generated']}"
-        index += 1
         if not test['accepted']:
-            amount_failed += 1
+            result.append("\t    Expected:\t" + test['expected'].rstrip())
+            result.append("\t    Actual:  \t" + test['generated'].rstrip())
+        amount_failed += 1
+        index += 1
 
     return result
 
 
 def submission_code_annotations(submission_data: dict) -> str:
     """
     Get code annotations out of the submission data
@@ -120,11 +132,11 @@
     return result
 
 
 if __name__ == '__main__':
     import json
     import pretty_console
 
-    with open('/home/bram/tijdelijk4.json', 'r') as test_file:
+    with open(f'/home/bram/tijdelijk{input()}.json', 'r') as test_file:
         test_data: dict = json.load(test_file)
 
     pretty_console.console.print(submission_data_handler(test_data))
```

### Comparing `dodonacli-2024.5.13/dodonacli/source/syntax_checker.py` & `dodonacli-2024.5.14/dodonacli/source/syntax_checker.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/dodonacli_completion_script.sh` & `dodonacli-2024.5.14/dodonacli_completion_script.sh`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.13/man-page/dodonacli.1` & `dodonacli-2024.5.14/man-page/dodonacli.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 '\" t
-.TH DODONA 18/02/2024
+.TH DODONACLI 14/05/2024
 .SH NAME
-dodona \- a 3rd party Command Line Interface for Dodona
+dodonacli \- a 3rd party Command Line Interface for Dodona
 
 .SH SYNOPSIS
 .B dodona
 [display|info|next|post|select|status|sub|tutorial|up] [--help]
 
 .SH DESCRIPTION
 This documents the usage of a Command Line Interface made for Dodona. 
 .B DodonaCLI
-connects to Dodona to enable you to read, submit and get feedback (if possible) on exercises. 
+connects to Dodona to enable you to read, submit and get (minimal) feedback on exercises.
 You are able to switch courses, series and exercises, as long as you have acces to it on the official Dodona website.
 
 .SH SUBCOMMANDS
 .IP display
 Displays the courses/series/exercises you can select. When used while an exercise is selected, it will link you to the exercise page of the Dodona website. It can be used in combination with the flags
 .BR [-force|--force]
 to force the web-pages content in your terminal. This formatting is often quite broken, so don't rely on this for tests.
 
 .IP info
-Gives some practical info about DodonaCLI itself. It has 4 subcommands: version [default], changelog, check_update and github. They're pretty self-explanatory tbh.
+Gives some practical info about DodonaCLI itself. It has some subcommands: version [default], changelog, check-update, completion and github. They're pretty self-explanatory tbh.
 
 .IP next
 Selects the next course/series/exercise. This subcommand is equivalent to using 'up + select' and can be a nice time-saver. It is possible to go to the next unsolved exercise by appending the
 .BR [-u|--unsolved]
 flag. It is also possible to reverse the order in which it cycles with the
 .BR [-r|--reverse]
-flag.
+flag. Both flags can be used together.
 
 .IP post
-Posts the file given as an extra argument to the currently selected exercise. This will return if the tests are passed and if possible, extra information about the wrong tests. You can also use the
+Posts the file given as an extra argument to the currently selected exercise. This will return if the tests are passed, or information about the wrong tests. You can also use the
 .BR [-c|--check]
-flag to check your solutionfile for syntax-errors before uploading. This is currently supported for Bash, Java(Script) and Python. There is also the
+flag to check your solutionfile for syntax-errors before uploading. This is currently supported for Bash, Java, JavaScript and Python. There is also the
 .BR [-l|--link]
 flag to post your solutionfile directly to the exercise specified in a link on the first line of the file. This link has to be written in a comment!
 
 .IP select
 Select a course/series/exercise of those available when using 
 .BR dodona
 .BR display.
 Requires an extra argument 
 .BR [id|name] 
-where name can be a distinct part of the cours/series/exercise. If the name is not distinct, it will select the first item it matches with (case-insensitive). It is not guarenteed that this matching happens in the same order as displayed.
+where name can be a distinct part of the cours/series/exercise. If the name is not distinct, it will select the first item it matches with (case-insensitive). It is not guarenteed that this matching happens in the same order as displayed, but often it is.
 
 .IP status
-Show the current selected course/series/exercise. No selection for an item is indicated with  
+Show the current selected course/series/exercise. If there is nothing selected for a category, it will be displayed as
 .B None.
 
 .IP sub
 Shows the most recent submissions. If an exercise is selected, then it will display the most recent 10 for that exercise, else it will display the most recent 30 submissions for the user. The code for a submssion can be loaded in with the subcommand 'load INT'.
 
 .IP tutorial
 Starts an interactive tutorial to learn how the CLI works.
@@ -80,28 +80,29 @@
 .PP
 dodona display
 .RS 4
 Shows the available series
 .RE
 
 .PP
-dodona select Pyt
+dodona select pyt
 .RS 4
-Matches the series with 'Pyt' in it's name if it's the only one
+Matches the series with 'pyt' in it's name if it's the only one (case-insensitive)
 .RE
 
-.PP dodona select 'Exercise 1'
+.PP
+dodona select 'Exercise 1'
 .RS 4
 Selects  the exercise with the name: "Exercise 1"
 .RE
 
 .PP 
 dodona post test.py
 .RS 4
-Submits the document test.py to the currently selected exercise
+Submits the document test.py to the currently selected exercise, and displays feedback.
 .RE
 
 .PP
 dodona sub [view]
 .RS 4
 Shows the last submissions.
 .RE
```

### Comparing `dodonacli-2024.5.13/pyproject.toml` & `dodonacli-2024.5.14/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DodonaCLI"
-version = "2024.5.13"
+version = "2024.5.14"
 authors = [
     { name = "Bram Windey", email = "windey.bram@gmail.com" },
 ]
 description = "A CLI tool for Dodona"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
```

