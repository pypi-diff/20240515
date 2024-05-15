# Comparing `tmp/metatensor_core-0.1.7.tar.gz` & `tmp/metatensor_core-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metatensor_core-0.1.7.tar", last modified: Mon May 13 13:20:56 2024, max compression
+gzip compressed data, was "metatensor_core-0.1.8.tar", last modified: Mon May 13 15:31:35 2024, max compression
```

## Comparing `metatensor_core-0.1.7.tar` & `metatensor_core-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:56.048074 metatensor_core-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 13:20:56.048074 metatensor_core-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:56.048074 metatensor_core-0.1.7/metatensor/
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/_c_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/_c_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18074 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:56.048074 metatensor_core-0.1.7/metatensor/data/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/data/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/data/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    38710 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/status.py
--rw-r--r--   0 runner    (1001) docker     (127)    28174 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/metatensor/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    85657 2024-05-13 13:20:56.000000 metatensor_core-0.1.7/metatensor-core-cxx-0.1.7.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:56.048074 metatensor_core-0.1.7/metatensor_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 13:20:56.000000 metatensor_core-0.1.7/metatensor_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-13 13:20:56.000000 metatensor_core-0.1.7/metatensor_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:20:56.000000 metatensor_core-0.1.7/metatensor_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:20:55.000000 metatensor_core-0.1.7/metatensor_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 13:20:56.000000 metatensor_core-0.1.7/metatensor_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 13:20:56.000000 metatensor_core-0.1.7/metatensor_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:20:55.000000 metatensor_core-0.1.7/n_commits_since_last_tag
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:20:56.048074 metatensor_core-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-05-13 13:20:44.000000 metatensor_core-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:31:35.174988 metatensor_core-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 15:31:35.174988 metatensor_core-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:31:35.174988 metatensor_core-0.1.8/metatensor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/_c_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/_c_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18074 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:31:35.174988 metatensor_core-0.1.8/metatensor/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/data/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/data/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38710 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28174 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/metatensor/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85697 2024-05-13 15:31:35.000000 metatensor_core-0.1.8/metatensor-core-cxx-0.1.8.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:31:35.174988 metatensor_core-0.1.8/metatensor_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 15:31:35.000000 metatensor_core-0.1.8/metatensor_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-13 15:31:35.000000 metatensor_core-0.1.8/metatensor_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:31:35.000000 metatensor_core-0.1.8/metatensor_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:31:33.000000 metatensor_core-0.1.8/metatensor_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 15:31:35.000000 metatensor_core-0.1.8/metatensor_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 15:31:35.000000 metatensor_core-0.1.8/metatensor_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:31:33.000000 metatensor_core-0.1.8/n_commits_since_last_tag
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:31:35.174988 metatensor_core-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-05-13 15:31:22.000000 metatensor_core-0.1.8/setup.py
```

### Comparing `metatensor_core-0.1.7/LICENSE` & `metatensor_core-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/PKG-INFO` & `metatensor_core-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metatensor-core
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python bindings for metatensor
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
 Project-URL: homepage, https://docs.metatensor.org/latest/
 Project-URL: documentation, https://docs.metatensor.org/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
 Project-URL: changelog, https://docs.metatensor.org/latest/core/CHANGELOG.html
```

### Comparing `metatensor_core-0.1.7/metatensor/__init__.py` & `metatensor_core-0.1.8/metatensor/__init__.py`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/metatensor/_c_api.py` & `metatensor_core-0.1.8/metatensor/_c_api.py`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/metatensor/_c_lib.py` & `metatensor_core-0.1.8/metatensor/_c_lib.py`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/metatensor/block.py` & `metatensor_core-0.1.8/metatensor/block.py`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/metatensor/data/array.py` & `metatensor_core-0.1.8/metatensor/data/array.py`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/metatensor/data/extract.py` & `metatensor_core-0.1.8/metatensor/data/extract.py`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/metatensor/io.py` & `metatensor_core-0.1.8/metatensor/io.py`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/metatensor/labels.py` & `metatensor_core-0.1.8/metatensor/labels.py`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/metatensor/status.py` & `metatensor_core-0.1.8/metatensor/status.py`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/metatensor/tensor.py` & `metatensor_core-0.1.8/metatensor/tensor.py`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/metatensor/utils.py` & `metatensor_core-0.1.8/metatensor/utils.py`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/metatensor_core.egg-info/PKG-INFO` & `metatensor_core-0.1.8/metatensor_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metatensor-core
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python bindings for metatensor
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
 Project-URL: homepage, https://docs.metatensor.org/latest/
 Project-URL: documentation, https://docs.metatensor.org/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
 Project-URL: changelog, https://docs.metatensor.org/latest/core/CHANGELOG.html
```

### Comparing `metatensor_core-0.1.7/metatensor_core.egg-info/SOURCES.txt` & `metatensor_core-0.1.8/metatensor_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.rst
-metatensor-core-cxx-0.1.7.tar.gz
+metatensor-core-cxx-0.1.8.tar.gz
 n_commits_since_last_tag
 pyproject.toml
 setup.py
 metatensor/__init__.py
 metatensor/_c_api.py
 metatensor/_c_lib.py
 metatensor/block.py
```

### Comparing `metatensor_core-0.1.7/pyproject.toml` & `metatensor_core-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metatensor_core-0.1.7/setup.py` & `metatensor_core-0.1.8/setup.py`

 * *Files identical despite different names*

