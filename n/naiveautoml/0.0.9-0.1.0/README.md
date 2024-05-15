# Comparing `tmp/naiveautoml-0.0.9.tar.gz` & `tmp/naiveautoml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/naiveautoml-0.0.9.tar", last modified: Tue Oct 18 19:03:19 2022, max compression
+gzip compressed data, was "naiveautoml-0.1.0.tar", last modified: Wed May 15 12:19:31 2024, max compression
```

## Comparing `naiveautoml-0.0.9.tar` & `naiveautoml-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-10-18 19:03:19.000000 naiveautoml-0.0.9/
--rw-r--r--   0 felix     (1000) felix     (1000)     1062 2021-10-27 14:20:45.000000 naiveautoml-0.0.9/LICENSE.txt
--rw-r--r--   0 felix     (1000) felix     (1000)      717 2022-10-18 19:03:19.000000 naiveautoml-0.0.9/PKG-INFO
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-10-18 19:03:19.000000 naiveautoml-0.0.9/naiveautoml/
--rw-r--r--   0 felix     (1000) felix     (1000)       47 2021-10-27 14:18:32.000000 naiveautoml-0.0.9/naiveautoml/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    45806 2022-10-18 17:53:44.000000 naiveautoml-0.0.9/naiveautoml/commons.py
--rw-r--r--   0 felix     (1000) felix     (1000)    20413 2022-10-18 18:24:51.000000 naiveautoml-0.0.9/naiveautoml/naiveautoml.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-10-18 19:03:19.000000 naiveautoml-0.0.9/naiveautoml.egg-info/
--rw-r--r--   0 felix     (1000) felix     (1000)      717 2022-10-18 19:03:18.000000 naiveautoml-0.0.9/naiveautoml.egg-info/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)      303 2022-10-18 19:03:18.000000 naiveautoml-0.0.9/naiveautoml.egg-info/SOURCES.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        1 2022-10-18 19:03:18.000000 naiveautoml-0.0.9/naiveautoml.egg-info/dependency_links.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       62 2022-10-18 19:03:18.000000 naiveautoml-0.0.9/naiveautoml.egg-info/requires.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       12 2022-10-18 19:03:18.000000 naiveautoml-0.0.9/naiveautoml.egg-info/top_level.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       79 2022-10-18 19:03:19.000000 naiveautoml-0.0.9/setup.cfg
--rw-r--r--   0 felix     (1000) felix     (1000)     1512 2022-10-18 19:02:33.000000 naiveautoml-0.0.9/setup.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-10-18 19:03:19.000000 naiveautoml-0.0.9/test/
--rw-r--r--   0 felix     (1000) felix     (1000)    11260 2022-10-18 19:02:01.000000 naiveautoml-0.0.9/test/test_naiveautoml.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-15 12:19:31.705381 naiveautoml-0.1.0/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1062 2021-10-27 14:20:45.000000 naiveautoml-0.1.0/LICENSE.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      842 2024-05-15 12:19:31.705381 naiveautoml-0.1.0/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)     5338 2024-05-11 15:11:20.000000 naiveautoml-0.1.0/README.md
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-15 12:19:31.702047 naiveautoml-0.1.0/naiveautoml/
+-rw-r--r--   0 felix     (1000) felix     (1000)       87 2024-03-01 21:07:57.000000 naiveautoml-0.1.0/naiveautoml/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    10429 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/naiveautoml/_interfaces.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     9384 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/naiveautoml/commons.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8913 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/naiveautoml/evaluators.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    11228 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/naiveautoml/naiveautoml.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    56249 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/naiveautoml/searchspace-classification.json
+-rw-r--r--   0 felix     (1000) felix     (1000)    59071 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/naiveautoml/searchspace-regression.json
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-15 12:19:31.705381 naiveautoml-0.1.0/naiveautoml.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)      842 2024-05-15 12:19:31.000000 naiveautoml-0.1.0/naiveautoml.egg-info/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)      465 2024-05-15 12:19:31.000000 naiveautoml-0.1.0/naiveautoml.egg-info/SOURCES.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        1 2024-05-15 12:19:31.000000 naiveautoml-0.1.0/naiveautoml.egg-info/dependency_links.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      122 2024-05-15 12:19:31.000000 naiveautoml-0.1.0/naiveautoml.egg-info/requires.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       12 2024-05-15 12:19:31.000000 naiveautoml-0.1.0/naiveautoml.egg-info/top_level.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      471 2024-03-01 21:07:57.000000 naiveautoml-0.1.0/pyproject.toml
+-rw-r--r--   0 felix     (1000) felix     (1000)       79 2024-05-15 12:19:31.705381 naiveautoml-0.1.0/setup.cfg
+-rw-r--r--   0 felix     (1000) felix     (1000)     1383 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/setup.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-15 12:19:31.705381 naiveautoml-0.1.0/test/
+-rw-r--r--   0 felix     (1000) felix     (1000)    31813 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/test/test_naiveautoml.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `naiveautoml-0.0.9/LICENSE.txt` & `naiveautoml-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naiveautoml-0.0.9/PKG-INFO` & `naiveautoml-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: naiveautoml
-Version: 0.0.9
-Summary: The official package for the Naive AutoML paper
+Version: 0.1.0
+Summary: Fast and Timeout-Free Automated Machine Learning for Multi-Class classification, Multi-Label classification, and regression.
 Home-page: https://github.com/fmohr/naiveautoml
-Download-URL: https://github.com/fmohr/naiveautoml/archive/refs/tags/v0.0.9.tar.gz
+Download-URL: https://github.com/fmohr/naiveautoml/archive/refs/tags/v0.0.27.tar.gz
 Author: Felix Mohr
 Author-email: mail@felixmohr.de
 License: MIT
-Keywords: AutoML,sklearn,naive,simple
+Keywords: AutoML,sklearn,naive,simple,multi-class,multi-label,regression,no timeouts
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `naiveautoml-0.0.9/naiveautoml.egg-info/PKG-INFO` & `naiveautoml-0.1.0/naiveautoml.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: naiveautoml
-Version: 0.0.9
-Summary: The official package for the Naive AutoML paper
+Version: 0.1.0
+Summary: Fast and Timeout-Free Automated Machine Learning for Multi-Class classification, Multi-Label classification, and regression.
 Home-page: https://github.com/fmohr/naiveautoml
-Download-URL: https://github.com/fmohr/naiveautoml/archive/refs/tags/v0.0.9.tar.gz
+Download-URL: https://github.com/fmohr/naiveautoml/archive/refs/tags/v0.0.27.tar.gz
 Author: Felix Mohr
 Author-email: mail@felixmohr.de
 License: MIT
-Keywords: AutoML,sklearn,naive,simple
+Keywords: AutoML,sklearn,naive,simple,multi-class,multi-label,regression,no timeouts
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

