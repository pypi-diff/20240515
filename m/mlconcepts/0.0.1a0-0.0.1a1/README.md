# Comparing `tmp/mlconcepts-0.0.1a0.tar.gz` & `tmp/mlconcepts-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlconcepts-0.0.1a0.tar", last modified: Tue May 14 14:12:34 2024, max compression
+gzip compressed data, was "mlconcepts-0.0.1a1.tar", last modified: Wed May 15 09:30:47 2024, max compression
```

## Comparing `mlconcepts-0.0.1a0.tar` & `mlconcepts-0.0.1a1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:12:34.451792 mlconcepts-0.0.1a0/
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-14 14:12:21.427746 mlconcepts-0.0.1a0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-14 14:12:34.439792 mlconcepts-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-14 14:12:21.000000 mlconcepts-0.0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:12:34.451792 mlconcepts-0.0.1a0/include/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/BasicMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    18343 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/Bitset.h
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/Bitstream.h
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/CNClassifier.h
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/ContextConcepts.h
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/ContextSelector.h
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/Dataset.h
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/EigenDataset.h
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/FeatureAssigner.h
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/GradientDescent.h
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/Model.h
--rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/PartialContext.h
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/Settings.h
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/StandardConceptifier.h
--rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/SupervisedOutlierDetectionModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/include/UnsupervisedOutlierDetectionModel.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:12:34.455792 mlconcepts-0.0.1a0/mlconcepts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-14 14:12:34.000000 mlconcepts-0.0.1a0/mlconcepts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-14 14:12:34.455792 mlconcepts-0.0.1a0/mlconcepts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:12:34.000000 mlconcepts-0.0.1a0/mlconcepts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:12:34.000000 mlconcepts-0.0.1a0/mlconcepts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 14:12:34.000000 mlconcepts-0.0.1a0/mlconcepts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 14:12:34.000000 mlconcepts-0.0.1a0/mlconcepts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-14 14:12:21.000000 mlconcepts-0.0.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-14 14:12:34.443792 mlconcepts-0.0.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-14 14:12:21.000000 mlconcepts-0.0.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:12:34.443792 mlconcepts-0.0.1a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:12:34.443792 mlconcepts-0.0.1a0/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:12:34.447792 mlconcepts-0.0.1a0/src/python/mlconcepts/
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/src/python/mlconcepts/SODModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/src/python/mlconcepts/UODModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/src/python/mlconcepts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:12:34.447792 mlconcepts-0.0.1a0/src/python/mlconcepts/data/
--rw-r--r--   0 runner    (1001) docker     (127)    15385 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/src/python/mlconcepts/data/Dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/src/python/mlconcepts/data/NumpyLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/src/python/mlconcepts/data/PandasLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/src/python/mlconcepts/data/PathLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/src/python/mlconcepts/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:12:34.447792 mlconcepts-0.0.1a0/src/python/mlconcepts/mlconceptscore/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/src/python/mlconcepts/mlconceptscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/src/python/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/src/python_mlconcepts.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:12:34.451792 mlconcepts-0.0.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/tests/tests.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-14 14:12:21.431746 mlconcepts-0.0.1a0/tests/tests_partial_context.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:30:47.544419 mlconcepts-0.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-15 09:30:33.216348 mlconcepts-0.0.1a1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-15 09:30:47.532419 mlconcepts-0.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-15 09:30:33.000000 mlconcepts-0.0.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:30:47.544419 mlconcepts-0.0.1a1/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-15 09:30:33.216348 mlconcepts-0.0.1a1/include/BasicMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18343 2024-05-15 09:30:33.216348 mlconcepts-0.0.1a1/include/Bitset.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-15 09:30:33.216348 mlconcepts-0.0.1a1/include/Bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-05-15 09:30:33.216348 mlconcepts-0.0.1a1/include/CNClassifier.h
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-15 09:30:33.216348 mlconcepts-0.0.1a1/include/ContextConcepts.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-15 09:30:33.216348 mlconcepts-0.0.1a1/include/ContextSelector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-15 09:30:33.216348 mlconcepts-0.0.1a1/include/Dataset.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-15 09:30:33.216348 mlconcepts-0.0.1a1/include/EigenDataset.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-15 09:30:33.216348 mlconcepts-0.0.1a1/include/FeatureAssigner.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-15 09:30:33.216348 mlconcepts-0.0.1a1/include/GradientDescent.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/include/Model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/include/PartialContext.h
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/include/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/include/StandardConceptifier.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/include/SupervisedOutlierDetectionModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/include/UnsupervisedOutlierDetectionModel.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:30:47.548419 mlconcepts-0.0.1a1/mlconcepts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-15 09:30:47.000000 mlconcepts-0.0.1a1/mlconcepts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-15 09:30:47.548419 mlconcepts-0.0.1a1/mlconcepts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:30:47.000000 mlconcepts-0.0.1a1/mlconcepts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:30:47.000000 mlconcepts-0.0.1a1/mlconcepts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 09:30:47.000000 mlconcepts-0.0.1a1/mlconcepts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 09:30:47.000000 mlconcepts-0.0.1a1/mlconcepts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-15 09:30:33.000000 mlconcepts-0.0.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-15 09:30:47.536419 mlconcepts-0.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-15 09:30:33.000000 mlconcepts-0.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:30:47.536419 mlconcepts-0.0.1a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:30:47.536419 mlconcepts-0.0.1a1/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:30:47.540419 mlconcepts-0.0.1a1/src/python/mlconcepts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/src/python/mlconcepts/SODModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/src/python/mlconcepts/UODModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/src/python/mlconcepts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:30:47.540419 mlconcepts-0.0.1a1/src/python/mlconcepts/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    15385 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/src/python/mlconcepts/data/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/src/python/mlconcepts/data/NumpyLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/src/python/mlconcepts/data/PandasLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/src/python/mlconcepts/data/PathLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/src/python/mlconcepts/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:30:47.540419 mlconcepts-0.0.1a1/src/python/mlconcepts/mlconceptscore/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/src/python/mlconcepts/mlconceptscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/src/python/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/src/python_mlconcepts.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:30:47.544419 mlconcepts-0.0.1a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/tests/tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-15 09:30:33.220348 mlconcepts-0.0.1a1/tests/tests_partial_context.cpp
```

### Comparing `mlconcepts-0.0.1a0/CMakeLists.txt` & `mlconcepts-0.0.1a1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/PKG-INFO` & `mlconcepts-0.0.1a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mlconcepts
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: A small library implementing several interpretable machine learning algorithms based on FCA.
-Home-page: https://gitlab.com/xeredent/libmlconcepts
+Home-page: https://github.com/xeredent/libmlconcepts
 Author: Mattia Panettiere
 Author-email: mattia.panettiere@gmail.com
 License: BSD3
-Project-URL: Source, https://gitlab.com/xeredent/libmlconcepts
-Project-URL: Tracker, https://gitlab.com/xeredent/libmlconcepts/issues
+Project-URL: Source, https://github.com/xeredent/libmlconcepts
+Project-URL: Tracker, https://github.com/xeredent/libmlconcepts/issues
 Keywords: outlier-detection machine-learning formal-concepts-analysis
 Platform: any
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
@@ -39,14 +39,22 @@
 
 # mlconcepts
 
 This library is a wrapper around [libmlconcepts](https://github/xeredent/libmlconcepts), namely
 a `c++` library which implements a series of (interpretable) machine learning algorithms
 based on FCA, e.g. [[3]](https://www.sciencedirect.com/science/article/pii/S0167923624000290).
 
+Installing `mlconcepts` from a source distribution only requires a `c++23` compiler, all the
+other dependencies are automatically fetched. If `cmake` is not able to find the compiler
+during the installation process, please set the environment variable `CXX` as follows
+
+```bash
+CXX = /path/to/c++/compiler
+```
+
 
 ### Basic example
 Assuming that a dataset containing a column `outlier` is stored in the file 
 `dataset.csv`, a basic model could be trained as follows.
 
 ```python
 import mlconcepts
```

### Comparing `mlconcepts-0.0.1a0/README.md` & `mlconcepts-0.0.1a1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # mlconcepts
 
 This library is a wrapper around [libmlconcepts](https://github/xeredent/libmlconcepts), namely
 a `c++` library which implements a series of (interpretable) machine learning algorithms
 based on FCA, e.g. [[3]](https://www.sciencedirect.com/science/article/pii/S0167923624000290).
 
+Installing `mlconcepts` from a source distribution only requires a `c++23` compiler, all the
+other dependencies are automatically fetched. If `cmake` is not able to find the compiler
+during the installation process, please set the environment variable `CXX` as follows
+
+```bash
+CXX = /path/to/c++/compiler
+```
+
 
 ### Basic example
 Assuming that a dataset containing a column `outlier` is stored in the file 
 `dataset.csv`, a basic model could be trained as follows.
 
 ```python
 import mlconcepts
```

### Comparing `mlconcepts-0.0.1a0/include/BasicMath.h` & `mlconcepts-0.0.1a1/include/BasicMath.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/Bitset.h` & `mlconcepts-0.0.1a1/include/Bitset.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/Bitstream.h` & `mlconcepts-0.0.1a1/include/Bitstream.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/CNClassifier.h` & `mlconcepts-0.0.1a1/include/CNClassifier.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/ContextConcepts.h` & `mlconcepts-0.0.1a1/include/ContextConcepts.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/ContextSelector.h` & `mlconcepts-0.0.1a1/include/ContextSelector.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/Dataset.h` & `mlconcepts-0.0.1a1/include/Dataset.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/EigenDataset.h` & `mlconcepts-0.0.1a1/include/EigenDataset.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/FeatureAssigner.h` & `mlconcepts-0.0.1a1/include/FeatureAssigner.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/GradientDescent.h` & `mlconcepts-0.0.1a1/include/GradientDescent.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/Model.h` & `mlconcepts-0.0.1a1/include/Model.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/PartialContext.h` & `mlconcepts-0.0.1a1/include/PartialContext.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/Settings.h` & `mlconcepts-0.0.1a1/include/Settings.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/StandardConceptifier.h` & `mlconcepts-0.0.1a1/include/StandardConceptifier.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/SupervisedOutlierDetectionModel.h` & `mlconcepts-0.0.1a1/include/SupervisedOutlierDetectionModel.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/include/UnsupervisedOutlierDetectionModel.h` & `mlconcepts-0.0.1a1/include/UnsupervisedOutlierDetectionModel.h`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/mlconcepts.egg-info/PKG-INFO` & `mlconcepts-0.0.1a1/mlconcepts.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mlconcepts
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: A small library implementing several interpretable machine learning algorithms based on FCA.
-Home-page: https://gitlab.com/xeredent/libmlconcepts
+Home-page: https://github.com/xeredent/libmlconcepts
 Author: Mattia Panettiere
 Author-email: mattia.panettiere@gmail.com
 License: BSD3
-Project-URL: Source, https://gitlab.com/xeredent/libmlconcepts
-Project-URL: Tracker, https://gitlab.com/xeredent/libmlconcepts/issues
+Project-URL: Source, https://github.com/xeredent/libmlconcepts
+Project-URL: Tracker, https://github.com/xeredent/libmlconcepts/issues
 Keywords: outlier-detection machine-learning formal-concepts-analysis
 Platform: any
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
@@ -39,14 +39,22 @@
 
 # mlconcepts
 
 This library is a wrapper around [libmlconcepts](https://github/xeredent/libmlconcepts), namely
 a `c++` library which implements a series of (interpretable) machine learning algorithms
 based on FCA, e.g. [[3]](https://www.sciencedirect.com/science/article/pii/S0167923624000290).
 
+Installing `mlconcepts` from a source distribution only requires a `c++23` compiler, all the
+other dependencies are automatically fetched. If `cmake` is not able to find the compiler
+during the installation process, please set the environment variable `CXX` as follows
+
+```bash
+CXX = /path/to/c++/compiler
+```
+
 
 ### Basic example
 Assuming that a dataset containing a column `outlier` is stored in the file 
 `dataset.csv`, a basic model could be trained as follows.
 
 ```python
 import mlconcepts
```

### Comparing `mlconcepts-0.0.1a0/mlconcepts.egg-info/SOURCES.txt` & `mlconcepts-0.0.1a1/mlconcepts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/setup.cfg` & `mlconcepts-0.0.1a1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 description = A small library implementing several interpretable machine learning algorithms based on FCA.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Mattia Panettiere
 author_email = mattia.panettiere@gmail.com
 license = BSD3
 platforms = any
-url = https://gitlab.com/xeredent/libmlconcepts
+url = https://github.com/xeredent/libmlconcepts
 project_urls = 
-	Source = https://gitlab.com/xeredent/libmlconcepts
-	Tracker = https://gitlab.com/xeredent/libmlconcepts/issues
+	Source = https://github.com/xeredent/libmlconcepts
+	Tracker = https://github.com/xeredent/libmlconcepts/issues
 keywords = outlier-detection machine-learning formal-concepts-analysis
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Operating System :: OS Independent
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
```

### Comparing `mlconcepts-0.0.1a0/setup.py` & `mlconcepts-0.0.1a1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import abc
 import os
 
 from pathlib import Path
 from shutil import copy2
 from typing import Generator, List
 
+import cmake
 import cmake_build_extension
 import setuptools
 import setuptools.command.sdist
 import setuptools_scm
 
 
 
@@ -73,14 +74,18 @@
 if (Path(".") / "CMakeLists.txt").exists():
     # Install from sdist
     source_dir = str(Path(".").absolute())
 else:
     # Install from sources or build wheel
     source_dir = str(Path(".").absolute().parent.parent)
 
+#Prioritize the cmake bin from cmake's installation
+if os.path.isdir(cmake.CMAKE_BIN_DIR):
+    os.environ["PATH"] = cmake.CMAKE_BIN_DIR + ";" + os.environ["PATH"]
+
 setuptools.setup(
     ext_modules=[
         cmake_build_extension.CMakeExtension(
             name="CMakeProject",
             install_prefix="mlconcepts",
             cmake_depends_on=["pybind11"],
             disable_editable=True,
```

### Comparing `mlconcepts-0.0.1a0/src/python/mlconcepts/SODModel.py` & `mlconcepts-0.0.1a1/src/python/mlconcepts/SODModel.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/src/python/mlconcepts/UODModel.py` & `mlconcepts-0.0.1a1/src/python/mlconcepts/UODModel.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/src/python/mlconcepts/data/Dataset.py` & `mlconcepts-0.0.1a1/src/python/mlconcepts/data/Dataset.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/src/python/mlconcepts/data/NumpyLoader.py` & `mlconcepts-0.0.1a1/src/python/mlconcepts/data/NumpyLoader.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/src/python/mlconcepts/data/PandasLoader.py` & `mlconcepts-0.0.1a1/src/python/mlconcepts/data/PandasLoader.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/src/python/mlconcepts/data/PathLoader.py` & `mlconcepts-0.0.1a1/src/python/mlconcepts/data/PathLoader.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/src/python/mlconcepts/data/__init__.py` & `mlconcepts-0.0.1a1/src/python/mlconcepts/data/__init__.py`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/src/python_mlconcepts.cpp` & `mlconcepts-0.0.1a1/src/python_mlconcepts.cpp`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/tests/tests.cpp` & `mlconcepts-0.0.1a1/tests/tests.cpp`

 * *Files identical despite different names*

### Comparing `mlconcepts-0.0.1a0/tests/tests_partial_context.cpp` & `mlconcepts-0.0.1a1/tests/tests_partial_context.cpp`

 * *Files identical despite different names*

