# Comparing `tmp/rms_vax-1.0.2.tar.gz` & `tmp/rms_vax-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms_vax-1.0.2.tar", last modified: Tue May 14 19:06:23 2024, max compression
+gzip compressed data, was "rms_vax-1.0.3.tar", last modified: Wed May 15 20:26:12 2024, max compression
```

## Comparing `rms_vax-1.0.2.tar` & `rms_vax-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.087470 rms_vax-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:06:13.000000 rms_vax-1.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 19:06:13.000000 rms_vax-1.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.083470 rms_vax-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.083470 rms_vax-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:06:13.000000 rms_vax-1.0.2/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:06:13.000000 rms_vax-1.0.2/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-14 19:06:13.000000 rms_vax-1.0.2/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:06:13.000000 rms_vax-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:06:13.000000 rms_vax-1.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-05-14 19:06:13.000000 rms_vax-1.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:06:13.000000 rms_vax-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-14 19:06:23.087470 rms_vax-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-14 19:06:13.000000 rms_vax-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-14 19:06:13.000000 rms_vax-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 19:06:13.000000 rms_vax-1.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.087470 rms_vax-1.0.2/rms_vax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-14 19:06:23.000000 rms_vax-1.0.2/rms_vax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-14 19:06:23.000000 rms_vax-1.0.2/rms_vax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:06:23.000000 rms_vax-1.0.2/rms_vax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 19:06:23.000000 rms_vax-1.0.2/rms_vax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 19:06:23.000000 rms_vax-1.0.2/rms_vax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 19:06:23.087470 rms_vax-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.083470 rms_vax-1.0.2/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-05-14 19:06:13.000000 rms_vax-1.0.2/test_files/C3490702_GEOMA.DAT
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-14 19:06:13.000000 rms_vax-1.0.2/test_files/C3490702_GEOMA.LBL
--rw-r--r--   0 runner    (1001) docker     (127)    20424 2024-05-14 19:06:13.000000 rms_vax-1.0.2/test_files/C3490702_GEOMA.TAB
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.087470 rms_vax-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-05-14 19:06:13.000000 rms_vax-1.0.2/tests/test_vax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:23.087470 rms_vax-1.0.2/vax/
--rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-14 19:06:13.000000 rms_vax-1.0.2/vax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:06:22.000000 rms_vax-1.0.2/vax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:12.920657 rms_vax-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 20:26:03.000000 rms_vax-1.0.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-15 20:26:03.000000 rms_vax-1.0.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:12.916657 rms_vax-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:12.916657 rms_vax-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-15 20:26:03.000000 rms_vax-1.0.3/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-15 20:26:03.000000 rms_vax-1.0.3/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-15 20:26:03.000000 rms_vax-1.0.3/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-15 20:26:03.000000 rms_vax-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-15 20:26:03.000000 rms_vax-1.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-05-15 20:26:03.000000 rms_vax-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 20:26:03.000000 rms_vax-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-15 20:26:12.920657 rms_vax-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-15 20:26:03.000000 rms_vax-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-15 20:26:03.000000 rms_vax-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 20:26:03.000000 rms_vax-1.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:12.920657 rms_vax-1.0.3/rms_vax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-15 20:26:12.000000 rms_vax-1.0.3/rms_vax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-15 20:26:12.000000 rms_vax-1.0.3/rms_vax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:26:12.000000 rms_vax-1.0.3/rms_vax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 20:26:12.000000 rms_vax-1.0.3/rms_vax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 20:26:12.000000 rms_vax-1.0.3/rms_vax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 20:26:12.920657 rms_vax-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:12.920657 rms_vax-1.0.3/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-05-15 20:26:03.000000 rms_vax-1.0.3/test_files/C3490702_GEOMA.DAT
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-15 20:26:03.000000 rms_vax-1.0.3/test_files/C3490702_GEOMA.LBL
+-rw-r--r--   0 runner    (1001) docker     (127)    20424 2024-05-15 20:26:03.000000 rms_vax-1.0.3/test_files/C3490702_GEOMA.TAB
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:12.920657 rms_vax-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-05-15 20:26:03.000000 rms_vax-1.0.3/tests/test_vax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:12.920657 rms_vax-1.0.3/vax/
+-rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-15 20:26:03.000000 rms_vax-1.0.3/vax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 20:26:12.000000 rms_vax-1.0.3/vax/_version.py
```

### Comparing `rms_vax-1.0.2/.github/workflows/publish_to_pypi.yml` & `rms_vax-1.0.3/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/.github/workflows/publish_to_test_pypi.yml` & `rms_vax-1.0.3/.github/workflows/publish_to_test_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/.github/workflows/run-tests.yml` & `rms_vax-1.0.3/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/.gitignore` & `rms_vax-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/CODE_OF_CONDUCT.md` & `rms_vax-1.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/CONTRIBUTING.md` & `rms_vax-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/LICENSE` & `rms_vax-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/PKG-INFO` & `rms_vax-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-vax
-Version: 1.0.2
+Version: 1.0.3
 Summary: Routines for converting to and from vax single-precision floating-point values
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-vax
 Project-URL: Repository, https://github.com/SETI/rms-vax
 Project-URL: Source, https://github.com/SETI/rms-vax
 Project-URL: Issues, https://github.com/SETI/rms-vax/issues
@@ -12,24 +12,23 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
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
 
 [![GitHub release; latest by date](https://img.shields.io/github/v/release/SETI/rms-vax)](https://github.com/SETI/rms-vax/releases)
 [![GitHub Release Date](https://img.shields.io/github/release-date/SETI/rms-vax)](https://github.com/SETI/rms-vax/releases)
 [![Test Status](https://img.shields.io/github/actions/workflow/status/SETI/rms-vax/run-tests.yml?branch=main)](https://github.com/SETI/rms-vax/actions)
```

### Comparing `rms_vax-1.0.2/README.md` & `rms_vax-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/pyproject.toml` & `rms_vax-1.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rms-vax"
 dynamic = ["version"]
 description = "Routines for converting to and from vax single-precision floating-point values"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "numpy"
 ]
 license = {text = "Apache-2.0"}
 maintainers = [
   {name = "Robert S. French", email = "rfrench@seti.org"}
 ]
@@ -20,15 +20,14 @@
   "Development Status :: 5 - Production/Stable",
   "Natural Language :: English",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Astronomy",
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

### Comparing `rms_vax-1.0.2/rms_vax.egg-info/PKG-INFO` & `rms_vax-1.0.3/rms_vax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-vax
-Version: 1.0.2
+Version: 1.0.3
 Summary: Routines for converting to and from vax single-precision floating-point values
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-vax
 Project-URL: Repository, https://github.com/SETI/rms-vax
 Project-URL: Source, https://github.com/SETI/rms-vax
 Project-URL: Issues, https://github.com/SETI/rms-vax/issues
@@ -12,24 +12,23 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
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
 
 [![GitHub release; latest by date](https://img.shields.io/github/v/release/SETI/rms-vax)](https://github.com/SETI/rms-vax/releases)
 [![GitHub Release Date](https://img.shields.io/github/release-date/SETI/rms-vax)](https://github.com/SETI/rms-vax/releases)
 [![Test Status](https://img.shields.io/github/actions/workflow/status/SETI/rms-vax/run-tests.yml?branch=main)](https://github.com/SETI/rms-vax/actions)
```

### Comparing `rms_vax-1.0.2/rms_vax.egg-info/SOURCES.txt` & `rms_vax-1.0.3/rms_vax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/test_files/C3490702_GEOMA.DAT` & `rms_vax-1.0.3/test_files/C3490702_GEOMA.DAT`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/test_files/C3490702_GEOMA.LBL` & `rms_vax-1.0.3/test_files/C3490702_GEOMA.LBL`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/test_files/C3490702_GEOMA.TAB` & `rms_vax-1.0.3/test_files/C3490702_GEOMA.TAB`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/tests/test_vax.py` & `rms_vax-1.0.3/tests/test_vax.py`

 * *Files identical despite different names*

### Comparing `rms_vax-1.0.2/vax/__init__.py` & `rms_vax-1.0.3/vax/__init__.py`

 * *Files identical despite different names*

