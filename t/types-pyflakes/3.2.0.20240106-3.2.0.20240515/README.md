# Comparing `tmp/types-pyflakes-3.2.0.20240106.tar.gz` & `tmp/types-pyflakes-3.2.0.20240515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyflakes-3.2.0.20240106.tar", last modified: Sat Jan  6 02:20:57 2024, max compression
+gzip compressed data, was "types-pyflakes-3.2.0.20240515.tar", last modified: Wed May 15 02:24:45 2024, max compression
```

## Comparing `types-pyflakes-3.2.0.20240106.tar` & `types-pyflakes-3.2.0.20240515.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:20:57.391746 types-pyflakes-3.2.0.20240106/
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-01-06 02:20:56.000000 types-pyflakes-3.2.0.20240106/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-06 02:20:56.000000 types-pyflakes-3.2.0.20240106/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-01-06 02:20:57.391746 types-pyflakes-3.2.0.20240106/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:20:57.391746 types-pyflakes-3.2.0.20240106/pyflakes-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-06 02:20:56.000000 types-pyflakes-3.2.0.20240106/pyflakes-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-06 02:18:46.000000 types-pyflakes-3.2.0.20240106/pyflakes-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-01-06 02:18:46.000000 types-pyflakes-3.2.0.20240106/pyflakes-stubs/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14417 2024-01-06 02:18:46.000000 types-pyflakes-3.2.0.20240106/pyflakes-stubs/checker.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-01-06 02:18:46.000000 types-pyflakes-3.2.0.20240106/pyflakes-stubs/messages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-06 02:20:56.000000 types-pyflakes-3.2.0.20240106/pyflakes-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-06 02:18:46.000000 types-pyflakes-3.2.0.20240106/pyflakes-stubs/reporter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 02:20:57.391746 types-pyflakes-3.2.0.20240106/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-01-06 02:20:56.000000 types-pyflakes-3.2.0.20240106/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:20:57.391746 types-pyflakes-3.2.0.20240106/types_pyflakes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-01-06 02:20:57.000000 types-pyflakes-3.2.0.20240106/types_pyflakes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-01-06 02:20:57.000000 types-pyflakes-3.2.0.20240106/types_pyflakes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 02:20:57.000000 types-pyflakes-3.2.0.20240106/types_pyflakes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-06 02:20:57.000000 types-pyflakes-3.2.0.20240106/types_pyflakes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:45.470125 types-pyflakes-3.2.0.20240515/
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-15 02:24:44.000000 types-pyflakes-3.2.0.20240515/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 02:24:44.000000 types-pyflakes-3.2.0.20240515/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-15 02:24:45.470125 types-pyflakes-3.2.0.20240515/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:45.466125 types-pyflakes-3.2.0.20240515/pyflakes-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 02:24:44.000000 types-pyflakes-3.2.0.20240515/pyflakes-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 02:24:30.000000 types-pyflakes-3.2.0.20240515/pyflakes-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-15 02:24:30.000000 types-pyflakes-3.2.0.20240515/pyflakes-stubs/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14417 2024-05-15 02:24:30.000000 types-pyflakes-3.2.0.20240515/pyflakes-stubs/checker.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-15 02:24:30.000000 types-pyflakes-3.2.0.20240515/pyflakes-stubs/messages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 02:24:44.000000 types-pyflakes-3.2.0.20240515/pyflakes-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-15 02:24:30.000000 types-pyflakes-3.2.0.20240515/pyflakes-stubs/reporter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:45.466125 types-pyflakes-3.2.0.20240515/pyflakes-stubs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:30.000000 types-pyflakes-3.2.0.20240515/pyflakes-stubs/scripts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 02:24:30.000000 types-pyflakes-3.2.0.20240515/pyflakes-stubs/scripts/pyflakes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 02:24:45.470125 types-pyflakes-3.2.0.20240515/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-15 02:24:44.000000 types-pyflakes-3.2.0.20240515/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:24:45.470125 types-pyflakes-3.2.0.20240515/types_pyflakes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-15 02:24:45.000000 types-pyflakes-3.2.0.20240515/types_pyflakes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-15 02:24:45.000000 types-pyflakes-3.2.0.20240515/types_pyflakes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 02:24:45.000000 types-pyflakes-3.2.0.20240515/types_pyflakes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 02:24:45.000000 types-pyflakes-3.2.0.20240515/types_pyflakes.egg-info/top_level.txt
```

### Comparing `types-pyflakes-3.2.0.20240106/CHANGELOG.md` & `types-pyflakes-3.2.0.20240515/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.2.0.20240515 (2024-05-15)
+
+[pyflakes] add backwards compatibility module (#11910)
+
 ## 3.2.0.20240106 (2024-01-06)
 
 [stubsabot] Bump pyflakes to 3.2.* (#11252)
 
 Release: https://pypi.org/pypi/pyflakes/3.2.0
 Homepage: https://github.com/PyCQA/pyflakes
 Repository: https://github.com/PyCQA/pyflakes
```

### Comparing `types-pyflakes-3.2.0.20240106/PKG-INFO` & `types-pyflakes-3.2.0.20240515/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyflakes
-Version: 3.2.0.20240106
+Version: 3.2.0.20240515
 Summary: Typing stubs for pyflakes
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyflakes.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1de5830a2703936a96a126248227d5c7db883674` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `a86115a19ddf2ca57645fea5fb6287fafa1cc1a0` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
+pytype 2024.4.11.
```

### Comparing `types-pyflakes-3.2.0.20240106/pyflakes-stubs/api.pyi` & `types-pyflakes-3.2.0.20240515/pyflakes-stubs/api.pyi`

 * *Files identical despite different names*

### Comparing `types-pyflakes-3.2.0.20240106/pyflakes-stubs/checker.pyi` & `types-pyflakes-3.2.0.20240515/pyflakes-stubs/checker.pyi`

 * *Files identical despite different names*

### Comparing `types-pyflakes-3.2.0.20240106/pyflakes-stubs/messages.pyi` & `types-pyflakes-3.2.0.20240515/pyflakes-stubs/messages.pyi`

 * *Files identical despite different names*

### Comparing `types-pyflakes-3.2.0.20240106/setup.py` & `types-pyflakes-3.2.0.20240515/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,34 +21,34 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1de5830a2703936a96a126248227d5c7db883674` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `a86115a19ddf2ca57645fea5fb6287fafa1cc1a0` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="3.2.0.20240106",
+      version="3.2.0.20240515",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyflakes.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['pyflakes-stubs'],
-      package_data={'pyflakes-stubs': ['__init__.pyi', 'api.pyi', 'checker.pyi', 'messages.pyi', 'reporter.pyi', 'METADATA.toml', 'py.typed']},
+      package_data={'pyflakes-stubs': ['__init__.pyi', 'api.pyi', 'checker.pyi', 'messages.pyi', 'reporter.pyi', 'scripts/__init__.pyi', 'scripts/pyflakes.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-pyflakes-3.2.0.20240106/types_pyflakes.egg-info/PKG-INFO` & `types-pyflakes-3.2.0.20240515/types_pyflakes.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyflakes
-Version: 3.2.0.20240106
+Version: 3.2.0.20240515
 Summary: Typing stubs for pyflakes
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyflakes.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1de5830a2703936a96a126248227d5c7db883674` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `a86115a19ddf2ca57645fea5fb6287fafa1cc1a0` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
+pytype 2024.4.11.
```

