# Comparing `tmp/cdbclerk-0.0.0.tar.gz` & `tmp/cdbclerk-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdbclerk-0.0.0.tar", last modified: Wed May 15 19:19:03 2024, max compression
+gzip compressed data, was "cdbclerk-0.1.tar", last modified: Wed May 15 19:27:22 2024, max compression
```

## Comparing `cdbclerk-0.0.0.tar` & `cdbclerk-0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:19:03.598704 cdbclerk-0.0.0/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      143 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/AUTHORS.rst
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3008 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/CONTRIBUTING.rst
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     1872 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/LICENSE
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      361 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/MANIFEST.in
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     2117 2024-05-15 19:19:03.596699 cdbclerk-0.0.0/PKG-INFO
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     1258 2024-05-15 19:16:05.000000 cdbclerk-0.0.0/README.rst
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:19:03.391720 cdbclerk-0.0.0/docs/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      626 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/docs/Makefile
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     2257 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/docs/conf.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      796 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/docs/make.bat
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:19:03.399711 cdbclerk-0.0.0/docs/source/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      104 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/docs/source/api.rst
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3624 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/docs/source/conf.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      382 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/docs/source/index.rst
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      820 2024-05-15 19:18:06.000000 cdbclerk-0.0.0/pyproject.toml
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       38 2024-05-15 19:19:03.598717 cdbclerk-0.0.0/setup.cfg
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:19:03.365710 cdbclerk-0.0.0/src/
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:19:03.419706 cdbclerk-0.0.0/src/cdbclerk/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      159 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/src/cdbclerk/__init__.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      850 2024-05-15 18:56:49.000000 cdbclerk-0.0.0/src/cdbclerk/__main__.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)    18450 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/src/cdbclerk/_version.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     1084 2024-05-15 19:02:37.000000 cdbclerk-0.0.0/src/cdbclerk/ioc_io.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      431 2024-05-15 19:13:12.000000 cdbclerk-0.0.0/src/cdbclerk/store_fields.py
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:19:03.590698 cdbclerk-0.0.0/src/cdbclerk/tests/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)        0 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/src/cdbclerk/tests/__init__.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)        0 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/src/cdbclerk/tests/conftest.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      470 2024-05-15 18:22:38.000000 cdbclerk-0.0.0/src/cdbclerk/tests/test_read_pvs.py
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:19:03.593699 cdbclerk-0.0.0/src/cdbclerk.egg-info/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     2117 2024-05-15 19:19:03.000000 cdbclerk-0.0.0/src/cdbclerk.egg-info/PKG-INFO
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      634 2024-05-15 19:19:03.000000 cdbclerk-0.0.0/src/cdbclerk.egg-info/SOURCES.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)        1 2024-05-15 19:19:03.000000 cdbclerk-0.0.0/src/cdbclerk.egg-info/dependency_links.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       52 2024-05-15 19:19:03.000000 cdbclerk-0.0.0/src/cdbclerk.egg-info/entry_points.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       70 2024-05-15 19:19:03.000000 cdbclerk-0.0.0/src/cdbclerk.egg-info/requires.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)        9 2024-05-15 19:19:03.000000 cdbclerk-0.0.0/src/cdbclerk.egg-info/top_level.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)    68614 2024-04-12 16:59:30.000000 cdbclerk-0.0.0/versioneer.py
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:27:22.693546 cdbclerk-0.1/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      143 2024-04-12 16:59:30.000000 cdbclerk-0.1/AUTHORS.rst
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3008 2024-04-12 16:59:30.000000 cdbclerk-0.1/CONTRIBUTING.rst
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     1872 2024-04-12 16:59:30.000000 cdbclerk-0.1/LICENSE
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      361 2024-04-12 16:59:30.000000 cdbclerk-0.1/MANIFEST.in
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     2152 2024-05-15 19:27:22.691547 cdbclerk-0.1/PKG-INFO
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     1258 2024-05-15 19:16:05.000000 cdbclerk-0.1/README.rst
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:27:22.649542 cdbclerk-0.1/docs/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      626 2024-04-12 16:59:30.000000 cdbclerk-0.1/docs/Makefile
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     2257 2024-04-12 16:59:30.000000 cdbclerk-0.1/docs/conf.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      796 2024-04-12 16:59:30.000000 cdbclerk-0.1/docs/make.bat
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:27:22.655550 cdbclerk-0.1/docs/source/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      104 2024-04-12 16:59:30.000000 cdbclerk-0.1/docs/source/api.rst
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3624 2024-04-12 16:59:30.000000 cdbclerk-0.1/docs/source/conf.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      382 2024-04-12 16:59:30.000000 cdbclerk-0.1/docs/source/index.rst
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      827 2024-05-15 19:26:48.000000 cdbclerk-0.1/pyproject.toml
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       38 2024-05-15 19:27:22.694540 cdbclerk-0.1/setup.cfg
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:27:22.624543 cdbclerk-0.1/src/
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:27:22.667543 cdbclerk-0.1/src/cdbclerk/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      159 2024-04-12 16:59:30.000000 cdbclerk-0.1/src/cdbclerk/__init__.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      850 2024-05-15 18:56:49.000000 cdbclerk-0.1/src/cdbclerk/__main__.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    18450 2024-04-12 16:59:30.000000 cdbclerk-0.1/src/cdbclerk/_version.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     1084 2024-05-15 19:02:37.000000 cdbclerk-0.1/src/cdbclerk/ioc_io.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      431 2024-05-15 19:13:12.000000 cdbclerk-0.1/src/cdbclerk/store_fields.py
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:27:22.686543 cdbclerk-0.1/src/cdbclerk/tests/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)        0 2024-04-12 16:59:30.000000 cdbclerk-0.1/src/cdbclerk/tests/__init__.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)        0 2024-04-12 16:59:30.000000 cdbclerk-0.1/src/cdbclerk/tests/conftest.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      470 2024-05-15 18:22:38.000000 cdbclerk-0.1/src/cdbclerk/tests/test_read_pvs.py
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-15 19:27:22.688563 cdbclerk-0.1/src/cdbclerk.egg-info/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     2152 2024-05-15 19:27:22.000000 cdbclerk-0.1/src/cdbclerk.egg-info/PKG-INFO
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      634 2024-05-15 19:27:22.000000 cdbclerk-0.1/src/cdbclerk.egg-info/SOURCES.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)        1 2024-05-15 19:27:22.000000 cdbclerk-0.1/src/cdbclerk.egg-info/dependency_links.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       52 2024-05-15 19:27:22.000000 cdbclerk-0.1/src/cdbclerk.egg-info/entry_points.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       76 2024-05-15 19:27:22.000000 cdbclerk-0.1/src/cdbclerk.egg-info/requires.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)        9 2024-05-15 19:27:22.000000 cdbclerk-0.1/src/cdbclerk.egg-info/top_level.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    68614 2024-04-12 16:59:30.000000 cdbclerk-0.1/versioneer.py
```

### Comparing `cdbclerk-0.0.0/CONTRIBUTING.rst` & `cdbclerk-0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cdbclerk-0.0.0/LICENSE` & `cdbclerk-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdbclerk-0.0.0/PKG-INFO` & `cdbclerk-0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdbclerk
-Version: 0.0.0
+Version: 0.1
 Summary: A tool for updating CA/PVA PVs from the components database.
 Author-email: Mark Wolfman <wolfman@anl.gov>
 Project-URL: Homepage, https://github.com/spc-group/cdbclerk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
@@ -18,14 +18,15 @@
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 ===============================
 cdbclerk
 ===============================
 
 |CI badge| |PyPI badge|
```

### Comparing `cdbclerk-0.0.0/README.rst` & `cdbclerk-0.1/README.rst`

 * *Files identical despite different names*

### Comparing `cdbclerk-0.0.0/docs/Makefile` & `cdbclerk-0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cdbclerk-0.0.0/docs/conf.py` & `cdbclerk-0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cdbclerk-0.0.0/docs/make.bat` & `cdbclerk-0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cdbclerk-0.0.0/docs/source/conf.py` & `cdbclerk-0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cdbclerk-0.0.0/pyproject.toml` & `cdbclerk-0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cdbclerk"
-version = "0.0.0"
+version = "0.1"
 authors = [
   { name="Mark Wolfman", email="wolfman@anl.gov" },
 ]
 description = "A tool for updating CA/PVA PVs from the components database."
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,14 +18,14 @@
     "Topic :: Scientific/Engineering",
     "Topic :: System :: Hardware",
 ]
 keywords = []
 dependencies = ["pyepics", "caproto"]
 
 [project.optional-dependencies]
-dev = ["black", "pytest", "flake8", "isort", "pytest-asyncio", "build"]
+dev = ["black", "pytest", "flake8", "isort", "pytest-asyncio", "build", "twine"]
 
 [project.urls]
 Homepage = "https://github.com/spc-group/cdbclerk"
 
 [project.scripts]
 cdbclerk = "cdbclerk.__main__:main"
```

### Comparing `cdbclerk-0.0.0/src/cdbclerk/__main__.py` & `cdbclerk-0.1/src/cdbclerk/__main__.py`

 * *Files identical despite different names*

### Comparing `cdbclerk-0.0.0/src/cdbclerk/_version.py` & `cdbclerk-0.1/src/cdbclerk/_version.py`

 * *Files identical despite different names*

### Comparing `cdbclerk-0.0.0/src/cdbclerk/ioc_io.py` & `cdbclerk-0.1/src/cdbclerk/ioc_io.py`

 * *Files identical despite different names*

### Comparing `cdbclerk-0.0.0/src/cdbclerk.egg-info/PKG-INFO` & `cdbclerk-0.1/src/cdbclerk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdbclerk
-Version: 0.0.0
+Version: 0.1
 Summary: A tool for updating CA/PVA PVs from the components database.
 Author-email: Mark Wolfman <wolfman@anl.gov>
 Project-URL: Homepage, https://github.com/spc-group/cdbclerk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
@@ -18,14 +18,15 @@
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 ===============================
 cdbclerk
 ===============================
 
 |CI badge| |PyPI badge|
```

### Comparing `cdbclerk-0.0.0/src/cdbclerk.egg-info/SOURCES.txt` & `cdbclerk-0.1/src/cdbclerk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdbclerk-0.0.0/versioneer.py` & `cdbclerk-0.1/versioneer.py`

 * *Files identical despite different names*

