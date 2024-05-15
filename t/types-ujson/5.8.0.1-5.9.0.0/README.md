# Comparing `tmp/types-ujson-5.8.0.1.tar.gz` & `tmp/types-ujson-5.9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-ujson-5.8.0.1.tar", last modified: Thu Jul 20 15:19:23 2023, max compression
+gzip compressed data, was "types-ujson-5.9.0.0.tar", last modified: Tue Dec 12 02:22:24 2023, max compression
```

## Comparing `types-ujson-5.8.0.1.tar` & `types-ujson-5.9.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:23.959476 types-ujson-5.8.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-20 15:19:23.955476 types-ujson-5.8.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:19:23.959476 types-ujson-5.8.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:23.955476 types-ujson-5.8.0.1/types_ujson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/types_ujson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/types_ujson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/types_ujson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/types_ujson.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:23.955476 types-ujson-5.8.0.1/ujson-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/ujson-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/ujson-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 02:22:24.437981 types-ujson-5.9.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2023-12-12 02:22:22.000000 types-ujson-5.9.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-12 02:22:22.000000 types-ujson-5.9.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2023-12-12 02:22:24.437981 types-ujson-5.9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-12 02:22:24.437981 types-ujson-5.9.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-12-12 02:22:22.000000 types-ujson-5.9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 02:22:24.433981 types-ujson-5.9.0.0/types_ujson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2023-12-12 02:22:24.000000 types-ujson-5.9.0.0/types_ujson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2023-12-12 02:22:24.000000 types-ujson-5.9.0.0/types_ujson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 02:22:24.000000 types-ujson-5.9.0.0/types_ujson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-12 02:22:24.000000 types-ujson-5.9.0.0/types_ujson.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 02:22:24.437981 types-ujson-5.9.0.0/ujson-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-12 02:22:22.000000 types-ujson-5.9.0.0/ujson-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2023-12-12 02:22:22.000000 types-ujson-5.9.0.0/ujson-stubs/__init__.pyi
```

### Comparing `types-ujson-5.8.0.1/CHANGELOG.md` & `types-ujson-5.9.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 5.9.0.0 (2023-12-12)
+
+[stubsabot] Bump ujson to 5.9.* (#11143)
+
 ## 5.8.0.1 (2023-07-20)
 
 Add an upstream_repository field to METADATA.toml (#10487)
 
 Closes: #10478
 
 ## 5.8.0.0 (2023-06-12)
```

### Comparing `types-ujson-5.8.0.1/PKG-INFO` & `types-ujson-5.9.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: types-ujson
-Version: 5.8.0.1
+Version: 5.9.0.0
 Summary: Typing stubs for ujson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Typing stubs for ujson
 
-This is a PEP 561 type stub package for the `ujson` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`ujson`](https://github.com/ultrajson/ultrajson) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`ujson`. The source for this package can be found at
+`ujson`.
+
+This version of `types-ujson` aims to provide accurate annotations
+for `ujson==5.9.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `cff2b3db0ca291e153a8bd407f48ac220a381dd8` and was tested
+with mypy 1.7.1, pyright 1.1.339, and
+pytype 2023.12.8.
```

### Comparing `types-ujson-5.8.0.1/setup.py` & `types-ujson-5.9.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 from setuptools import setup
 
 name = "types-ujson"
 description = "Typing stubs for ujson"
 long_description = '''
 ## Typing stubs for ujson
 
-This is a PEP 561 type stub package for the `ujson` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`ujson`](https://github.com/ultrajson/ultrajson) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`ujson`. The source for this package can be found at
+`ujson`.
+
+This version of `types-ujson` aims to provide accurate annotations
+for `ujson==5.9.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `cff2b3db0ca291e153a8bd407f48ac220a381dd8` and was tested
+with mypy 1.7.1, pyright 1.1.339, and
+pytype 2023.12.8.
 '''.lstrip()
 
 setup(name=name,
-      version="5.8.0.1",
+      version="5.9.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['ujson-stubs'],
       package_data={'ujson-stubs': ['__init__.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
+      python_requires=">=3.7",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-ujson-5.8.0.1/types_ujson.egg-info/PKG-INFO` & `types-ujson-5.9.0.0/types_ujson.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: types-ujson
-Version: 5.8.0.1
+Version: 5.9.0.0
 Summary: Typing stubs for ujson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Typing stubs for ujson
 
-This is a PEP 561 type stub package for the `ujson` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`ujson`](https://github.com/ultrajson/ultrajson) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`ujson`. The source for this package can be found at
+`ujson`.
+
+This version of `types-ujson` aims to provide accurate annotations
+for `ujson==5.9.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `cff2b3db0ca291e153a8bd407f48ac220a381dd8` and was tested
+with mypy 1.7.1, pyright 1.1.339, and
+pytype 2023.12.8.
```

### Comparing `types-ujson-5.8.0.1/ujson-stubs/__init__.pyi` & `types-ujson-5.9.0.0/ujson-stubs/__init__.pyi`

 * *Files identical despite different names*

