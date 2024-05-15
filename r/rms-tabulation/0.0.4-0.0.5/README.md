# Comparing `tmp/rms_tabulation-0.0.4.tar.gz` & `tmp/rms_tabulation-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms_tabulation-0.0.4.tar", last modified: Tue May 14 19:02:57 2024, max compression
+gzip compressed data, was "rms_tabulation-0.0.5.tar", last modified: Wed May 15 20:26:08 2024, max compression
```

## Comparing `rms_tabulation-0.0.4.tar` & `rms_tabulation-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:02:57.666304 rms_tabulation-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:02:57.662304 rms_tabulation-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:02:57.662304 rms_tabulation-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-14 19:02:57.666304 rms_tabulation-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:02:57.666304 rms_tabulation-0.0.4/rms_tabulation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-14 19:02:57.000000 rms_tabulation-0.0.4/rms_tabulation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 19:02:57.000000 rms_tabulation-0.0.4/rms_tabulation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:02:57.000000 rms_tabulation-0.0.4/rms_tabulation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 19:02:57.000000 rms_tabulation-0.0.4/rms_tabulation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 19:02:57.000000 rms_tabulation-0.0.4/rms_tabulation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 19:02:57.666304 rms_tabulation-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:02:57.666304 rms_tabulation-0.0.4/tabulation/
--rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/tabulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:02:57.000000 rms_tabulation-0.0.4/tabulation/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:02:57.666304 rms_tabulation-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-14 19:02:44.000000 rms_tabulation-0.0.4/tests/test_tabulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:08.589644 rms_tabulation-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:08.585644 rms_tabulation-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:08.585644 rms_tabulation-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-15 20:26:08.589644 rms_tabulation-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:08.589644 rms_tabulation-0.0.5/rms_tabulation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-15 20:26:08.000000 rms_tabulation-0.0.5/rms_tabulation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-15 20:26:08.000000 rms_tabulation-0.0.5/rms_tabulation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:26:08.000000 rms_tabulation-0.0.5/rms_tabulation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 20:26:08.000000 rms_tabulation-0.0.5/rms_tabulation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 20:26:08.000000 rms_tabulation-0.0.5/rms_tabulation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-15 20:26:08.589644 rms_tabulation-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:08.585644 rms_tabulation-0.0.5/tabulation/
+-rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/tabulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 20:26:08.000000 rms_tabulation-0.0.5/tabulation/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:08.585644 rms_tabulation-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-15 20:25:47.000000 rms_tabulation-0.0.5/tests/test_tabulation.py
```

### Comparing `rms_tabulation-0.0.4/.github/workflows/publish_to_pypi.yml` & `rms_tabulation-0.0.5/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_tabulation-0.0.4/.github/workflows/publish_to_test_pypi.yml` & `rms_tabulation-0.0.5/.github/workflows/publish_to_test_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_tabulation-0.0.4/.github/workflows/run-tests.yml` & `rms_tabulation-0.0.5/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `rms_tabulation-0.0.4/.gitignore` & `rms_tabulation-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rms_tabulation-0.0.4/CODE_OF_CONDUCT.md` & `rms_tabulation-0.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rms_tabulation-0.0.4/CONTRIBUTING.md` & `rms_tabulation-0.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rms_tabulation-0.0.4/LICENSE` & `rms_tabulation-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rms_tabulation-0.0.4/PKG-INFO` & `rms_tabulation-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-tabulation
-Version: 0.0.4
+Version: 0.0.5
 Summary: A class that performs linear interpolation
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-tabulation
 Project-URL: Repository, https://github.com/SETI/rms-tabulation
 Project-URL: Source, https://github.com/SETI/rms-tabulation
 Project-URL: Issues, https://github.com/SETI/rms-tabulation/issues
@@ -12,24 +12,23 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 
 [![GitHub release; latest by date](https://img.shields.io/github/v/release/SETI/rms-tabulation)](https://github.com/SETI/rms-tabulation/releases)
 [![GitHub Release Date](https://img.shields.io/github/release-date/SETI/rms-tabulation)](https://github.com/SETI/rms-tabulation/releases)
```

### Comparing `rms_tabulation-0.0.4/README.md` & `rms_tabulation-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rms_tabulation-0.0.4/pyproject.toml` & `rms_tabulation-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rms-tabulation"
 dynamic = ["version"]
 description = "A class that performs linear interpolation"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "numpy",
     "scipy"
 ]
 license = {text = "Apache-2.0"}
 maintainers = [
   {name = "Robert S. French", email = "rfrench@seti.org"}
@@ -21,15 +21,14 @@
   "Development Status :: 5 - Production/Stable",
   "Natural Language :: English",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Mathematics",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Utilities",
   "License :: OSI Approved :: Apache Software License",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: POSIX :: Linux",
```

### Comparing `rms_tabulation-0.0.4/rms_tabulation.egg-info/PKG-INFO` & `rms_tabulation-0.0.5/rms_tabulation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-tabulation
-Version: 0.0.4
+Version: 0.0.5
 Summary: A class that performs linear interpolation
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-tabulation
 Project-URL: Repository, https://github.com/SETI/rms-tabulation
 Project-URL: Source, https://github.com/SETI/rms-tabulation
 Project-URL: Issues, https://github.com/SETI/rms-tabulation/issues
@@ -12,24 +12,23 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 
 [![GitHub release; latest by date](https://img.shields.io/github/v/release/SETI/rms-tabulation)](https://github.com/SETI/rms-tabulation/releases)
 [![GitHub Release Date](https://img.shields.io/github/release-date/SETI/rms-tabulation)](https://github.com/SETI/rms-tabulation/releases)
```

### Comparing `rms_tabulation-0.0.4/tabulation/__init__.py` & `rms_tabulation-0.0.5/tabulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_tabulation-0.0.4/tests/test_tabulation.py` & `rms_tabulation-0.0.5/tests/test_tabulation.py`

 * *Files identical despite different names*

