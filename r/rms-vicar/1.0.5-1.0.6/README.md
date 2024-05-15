# Comparing `tmp/rms_vicar-1.0.5.tar.gz` & `tmp/rms_vicar-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms_vicar-1.0.5.tar", last modified: Tue May 14 19:07:42 2024, max compression
+gzip compressed data, was "rms_vicar-1.0.6.tar", last modified: Wed May 15 20:26:30 2024, max compression
```

## Comparing `rms_vicar-1.0.5.tar` & `rms_vicar-1.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.750450 rms_vicar-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.734450 rms_vicar-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.734450 rms_vicar-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-14 19:07:42.750450 rms_vicar-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.750450 rms_vicar-1.0.5/rms_vicar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-14 19:07:42.000000 rms_vicar-1.0.5/rms_vicar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-14 19:07:42.000000 rms_vicar-1.0.5/rms_vicar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:07:42.000000 rms_vicar-1.0.5/rms_vicar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 19:07:42.000000 rms_vicar-1.0.5/rms_vicar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 19:07:42.000000 rms_vicar-1.0.5/rms_vicar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 19:07:42.750450 rms_vicar-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.742450 rms_vicar-1.0.5/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)   831488 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/test_files/C0532836239R.IMG
--rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/test_files/C2069302_GEOMA.DAT
--rw-r--r--   0 runner    (1001) docker     (127)  2002000 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/test_files/C2069302_GEOMED.IMG
--rw-r--r--   0 runner    (1001) docker     (127)   823296 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/test_files/C2069302_RAW.IMG
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/test_files/C2069302_RESLOC.DAT
--rwxr-xr-x   0 runner    (1001) docker     (127)  4202496 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/test_files/N1536633072_1_CALIB.IMG
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.746450 rms_vicar-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/tests/test_LABEL_GRAMMAR.py
--rw-r--r--   0 runner    (1001) docker     (127)    23629 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/tests/test_vicarimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/tests/test_vicarlabel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.750450 rms_vicar-1.0.5/vicar/
--rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/vicar/_LABEL_GRAMMAR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/vicar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:07:42.000000 rms_vicar-1.0.5/vicar/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    29610 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/vicar/vicarimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    51298 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/vicar/vicarlabel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:30.201144 rms_vicar-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:30.185144 rms_vicar-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:30.185144 rms_vicar-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-15 20:26:30.201144 rms_vicar-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:30.201144 rms_vicar-1.0.6/rms_vicar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-15 20:26:30.000000 rms_vicar-1.0.6/rms_vicar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-15 20:26:30.000000 rms_vicar-1.0.6/rms_vicar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:26:30.000000 rms_vicar-1.0.6/rms_vicar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 20:26:30.000000 rms_vicar-1.0.6/rms_vicar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 20:26:30.000000 rms_vicar-1.0.6/rms_vicar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 20:26:30.201144 rms_vicar-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:30.193144 rms_vicar-1.0.6/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   831488 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/test_files/C0532836239R.IMG
+-rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/test_files/C2069302_GEOMA.DAT
+-rw-r--r--   0 runner    (1001) docker     (127)  2002000 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/test_files/C2069302_GEOMED.IMG
+-rw-r--r--   0 runner    (1001) docker     (127)   823296 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/test_files/C2069302_RAW.IMG
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/test_files/C2069302_RESLOC.DAT
+-rwxr-xr-x   0 runner    (1001) docker     (127)  4202496 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/test_files/N1536633072_1_CALIB.IMG
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:30.197144 rms_vicar-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/tests/test_LABEL_GRAMMAR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23629 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/tests/test_vicarimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/tests/test_vicarlabel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:30.197144 rms_vicar-1.0.6/vicar/
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/vicar/_LABEL_GRAMMAR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/vicar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 20:26:30.000000 rms_vicar-1.0.6/vicar/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29610 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/vicar/vicarimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51298 2024-05-15 20:26:17.000000 rms_vicar-1.0.6/vicar/vicarlabel.py
```

### Comparing `rms_vicar-1.0.5/.github/workflows/publish_to_pypi.yml` & `rms_vicar-1.0.6/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/.github/workflows/publish_to_test_pypi.yml` & `rms_vicar-1.0.6/.github/workflows/publish_to_test_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/.github/workflows/run-tests.yml` & `rms_vicar-1.0.6/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/.gitignore` & `rms_vicar-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/CODE_OF_CONDUCT.md` & `rms_vicar-1.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/CONTRIBUTING.md` & `rms_vicar-1.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/LICENSE` & `rms_vicar-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/PKG-INFO` & `rms_vicar-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-vicar
-Version: 1.0.5
+Version: 1.0.6
 Summary: Routines for converting to and from VICAR image files
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-vicar
 Project-URL: Repository, https://github.com/SETI/rms-vicar
 Project-URL: Source, https://github.com/SETI/rms-vicar
 Project-URL: Issues, https://github.com/SETI/rms-vicar/issues
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
 Requires-Dist: rms-vax
 
 [![GitHub release; latest by date](https://img.shields.io/github/v/release/SETI/rms-vicar)](https://github.com/SETI/rms-vicar/releases)
 [![GitHub Release Date](https://img.shields.io/github/release-date/SETI/rms-vicar)](https://github.com/SETI/rms-vicar/releases)
```

### Comparing `rms_vicar-1.0.5/README.md` & `rms_vicar-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/pyproject.toml` & `rms_vicar-1.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rms-vicar"
 dynamic = ["version"]
 description = "Routines for converting to and from VICAR image files"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "numpy",
     "rms-vax"
 ]
 license = {text = "Apache-2.0"}
 maintainers = [
   {name = "Robert S. French", email = "rfrench@seti.org"}
@@ -21,15 +21,14 @@
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

### Comparing `rms_vicar-1.0.5/rms_vicar.egg-info/PKG-INFO` & `rms_vicar-1.0.6/rms_vicar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-vicar
-Version: 1.0.5
+Version: 1.0.6
 Summary: Routines for converting to and from VICAR image files
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-vicar
 Project-URL: Repository, https://github.com/SETI/rms-vicar
 Project-URL: Source, https://github.com/SETI/rms-vicar
 Project-URL: Issues, https://github.com/SETI/rms-vicar/issues
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
 Requires-Dist: rms-vax
 
 [![GitHub release; latest by date](https://img.shields.io/github/v/release/SETI/rms-vicar)](https://github.com/SETI/rms-vicar/releases)
 [![GitHub Release Date](https://img.shields.io/github/release-date/SETI/rms-vicar)](https://github.com/SETI/rms-vicar/releases)
```

### Comparing `rms_vicar-1.0.5/rms_vicar.egg-info/SOURCES.txt` & `rms_vicar-1.0.6/rms_vicar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/test_files/C0532836239R.IMG` & `rms_vicar-1.0.6/test_files/C0532836239R.IMG`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/test_files/C2069302_GEOMA.DAT` & `rms_vicar-1.0.6/test_files/C2069302_GEOMA.DAT`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/test_files/C2069302_GEOMED.IMG` & `rms_vicar-1.0.6/test_files/C2069302_GEOMED.IMG`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/test_files/C2069302_RAW.IMG` & `rms_vicar-1.0.6/test_files/C2069302_RAW.IMG`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/test_files/C2069302_RESLOC.DAT` & `rms_vicar-1.0.6/test_files/C2069302_RESLOC.DAT`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/test_files/N1536633072_1_CALIB.IMG` & `rms_vicar-1.0.6/test_files/N1536633072_1_CALIB.IMG`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/tests/__init__.py` & `rms_vicar-1.0.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/tests/test_LABEL_GRAMMAR.py` & `rms_vicar-1.0.6/tests/test_LABEL_GRAMMAR.py`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/tests/test_vicarimage.py` & `rms_vicar-1.0.6/tests/test_vicarimage.py`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/tests/test_vicarlabel.py` & `rms_vicar-1.0.6/tests/test_vicarlabel.py`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/vicar/_LABEL_GRAMMAR.py` & `rms_vicar-1.0.6/vicar/_LABEL_GRAMMAR.py`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/vicar/__init__.py` & `rms_vicar-1.0.6/vicar/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/vicar/vicarimage.py` & `rms_vicar-1.0.6/vicar/vicarimage.py`

 * *Files identical despite different names*

### Comparing `rms_vicar-1.0.5/vicar/vicarlabel.py` & `rms_vicar-1.0.6/vicar/vicarlabel.py`

 * *Files identical despite different names*

