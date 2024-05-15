# Comparing `tmp/treegp-1.0.0.tar.gz` & `tmp/treegp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treegp-1.0.0.tar", last modified: Mon Dec 11 02:37:35 2023, max compression
+gzip compressed data, was "treegp-1.0.1.tar", last modified: Mon Dec 11 03:00:54 2023, max compression
```

## Comparing `treegp-1.0.0.tar` & `treegp-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 leget      (502) staff       (20)        0 2023-12-11 02:37:35.900162 treegp-1.0.0/
--rw-r--r--   0 leget      (502) staff       (20)     1528 2023-12-03 21:15:03.000000 treegp-1.0.0/LICENCE
--rw-r--r--   0 leget      (502) staff       (20)       29 2023-12-11 02:21:55.000000 treegp-1.0.0/MANIFEST.in
--rw-r--r--   0 leget      (502) staff       (20)     2502 2023-12-11 02:37:35.899692 treegp-1.0.0/PKG-INFO
--rw-r--r--   0 leget      (502) staff       (20)     2152 2023-12-11 02:34:34.000000 treegp-1.0.0/README.md
--rw-r--r--   0 leget      (502) staff       (20)       38 2023-12-11 02:37:35.900381 treegp-1.0.0/setup.cfg
--rw-r--r--   0 leget      (502) staff       (20)     1960 2023-12-11 02:21:55.000000 treegp-1.0.0/setup.py
-drwxr-xr-x   0 leget      (502) staff       (20)        0 2023-12-11 02:37:35.889598 treegp-1.0.0/tests/
--rw-r--r--   0 leget      (502) staff       (20)     8052 2023-12-06 02:21:36.000000 treegp-1.0.0/tests/test_gp_interp.py
--rw-r--r--   0 leget      (502) staff       (20)     6897 2023-12-06 02:21:36.000000 treegp-1.0.0/tests/test_hyp_search.py
--rw-r--r--   0 leget      (502) staff       (20)     8075 2023-12-06 02:21:36.000000 treegp-1.0.0/tests/test_kernels.py
--rw-r--r--   0 leget      (502) staff       (20)     4290 2023-12-06 02:21:36.000000 treegp-1.0.0/tests/test_meanify.py
-drwxr-xr-x   0 leget      (502) staff       (20)        0 2023-12-11 02:37:35.895972 treegp-1.0.0/treegp/
--rw-r--r--   0 leget      (502) staff       (20)      728 2023-12-04 04:24:13.000000 treegp-1.0.0/treegp/__init__.py
--rw-r--r--   0 leget      (502) staff       (20)       81 2023-12-11 02:35:32.000000 treegp-1.0.0/treegp/_version.py
--rw-r--r--   0 leget      (502) staff       (20)    11412 2023-12-04 04:24:13.000000 treegp-1.0.0/treegp/gp_interp.py
--rw-r--r--   0 leget      (502) staff       (20)    17933 2023-12-04 04:24:13.000000 treegp-1.0.0/treegp/kernels.py
--rw-r--r--   0 leget      (502) staff       (20)     2005 2023-12-04 04:24:13.000000 treegp-1.0.0/treegp/log_likelihood.py
--rw-r--r--   0 leget      (502) staff       (20)     5579 2023-12-04 04:24:13.000000 treegp-1.0.0/treegp/meanify.py
--rw-r--r--   0 leget      (502) staff       (20)    16567 2023-12-04 04:24:13.000000 treegp-1.0.0/treegp/two_pcf.py
-drwxr-xr-x   0 leget      (502) staff       (20)        0 2023-12-11 02:37:35.899145 treegp-1.0.0/treegp.egg-info/
--rw-r--r--   0 leget      (502) staff       (20)     2502 2023-12-11 02:37:35.000000 treegp-1.0.0/treegp.egg-info/PKG-INFO
--rw-r--r--   0 leget      (502) staff       (20)      417 2023-12-11 02:37:35.000000 treegp-1.0.0/treegp.egg-info/SOURCES.txt
--rw-r--r--   0 leget      (502) staff       (20)        1 2023-12-11 02:37:35.000000 treegp-1.0.0/treegp.egg-info/dependency_links.txt
--rw-r--r--   0 leget      (502) staff       (20)       70 2023-12-11 02:37:35.000000 treegp-1.0.0/treegp.egg-info/requires.txt
--rw-r--r--   0 leget      (502) staff       (20)        7 2023-12-11 02:37:35.000000 treegp-1.0.0/treegp.egg-info/top_level.txt
+drwxr-xr-x   0 leget      (502) staff       (20)        0 2023-12-11 03:00:54.543348 treegp-1.0.1/
+-rw-r--r--   0 leget      (502) staff       (20)     1528 2023-12-03 21:15:03.000000 treegp-1.0.1/LICENCE
+-rw-r--r--   0 leget      (502) staff       (20)       29 2023-12-11 02:49:54.000000 treegp-1.0.1/MANIFEST.in
+-rw-r--r--   0 leget      (502) staff       (20)     2605 2023-12-11 03:00:54.542775 treegp-1.0.1/PKG-INFO
+-rw-r--r--   0 leget      (502) staff       (20)     2255 2023-12-11 02:58:28.000000 treegp-1.0.1/README.rst
+-rw-r--r--   0 leget      (502) staff       (20)       38 2023-12-11 03:00:54.543522 treegp-1.0.1/setup.cfg
+-rw-r--r--   0 leget      (502) staff       (20)     1961 2023-12-11 02:58:28.000000 treegp-1.0.1/setup.py
+drwxr-xr-x   0 leget      (502) staff       (20)        0 2023-12-11 03:00:54.530399 treegp-1.0.1/tests/
+-rw-r--r--   0 leget      (502) staff       (20)     8052 2023-12-06 02:21:36.000000 treegp-1.0.1/tests/test_gp_interp.py
+-rw-r--r--   0 leget      (502) staff       (20)     6897 2023-12-06 02:21:36.000000 treegp-1.0.1/tests/test_hyp_search.py
+-rw-r--r--   0 leget      (502) staff       (20)     8075 2023-12-06 02:21:36.000000 treegp-1.0.1/tests/test_kernels.py
+-rw-r--r--   0 leget      (502) staff       (20)     4290 2023-12-06 02:21:36.000000 treegp-1.0.1/tests/test_meanify.py
+drwxr-xr-x   0 leget      (502) staff       (20)        0 2023-12-11 03:00:54.538143 treegp-1.0.1/treegp/
+-rw-r--r--   0 leget      (502) staff       (20)      728 2023-12-04 04:24:13.000000 treegp-1.0.1/treegp/__init__.py
+-rw-r--r--   0 leget      (502) staff       (20)       81 2023-12-11 02:58:16.000000 treegp-1.0.1/treegp/_version.py
+-rw-r--r--   0 leget      (502) staff       (20)    11412 2023-12-04 04:24:13.000000 treegp-1.0.1/treegp/gp_interp.py
+-rw-r--r--   0 leget      (502) staff       (20)    17933 2023-12-04 04:24:13.000000 treegp-1.0.1/treegp/kernels.py
+-rw-r--r--   0 leget      (502) staff       (20)     2005 2023-12-04 04:24:13.000000 treegp-1.0.1/treegp/log_likelihood.py
+-rw-r--r--   0 leget      (502) staff       (20)     5579 2023-12-04 04:24:13.000000 treegp-1.0.1/treegp/meanify.py
+-rw-r--r--   0 leget      (502) staff       (20)    16567 2023-12-04 04:24:13.000000 treegp-1.0.1/treegp/two_pcf.py
+drwxr-xr-x   0 leget      (502) staff       (20)        0 2023-12-11 03:00:54.541893 treegp-1.0.1/treegp.egg-info/
+-rw-r--r--   0 leget      (502) staff       (20)     2605 2023-12-11 03:00:54.000000 treegp-1.0.1/treegp.egg-info/PKG-INFO
+-rw-r--r--   0 leget      (502) staff       (20)      418 2023-12-11 03:00:54.000000 treegp-1.0.1/treegp.egg-info/SOURCES.txt
+-rw-r--r--   0 leget      (502) staff       (20)        1 2023-12-11 03:00:54.000000 treegp-1.0.1/treegp.egg-info/dependency_links.txt
+-rw-r--r--   0 leget      (502) staff       (20)       70 2023-12-11 03:00:54.000000 treegp-1.0.1/treegp.egg-info/requires.txt
+-rw-r--r--   0 leget      (502) staff       (20)        7 2023-12-11 03:00:54.000000 treegp-1.0.1/treegp.egg-info/top_level.txt
```

### Comparing `treegp-1.0.0/LICENCE` & `treegp-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `treegp-1.0.0/PKG-INFO` & `treegp-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,73 @@
 Metadata-Version: 2.1
 Name: treegp
-Version: 1.0.0
+Version: 1.0.1
 Summary: treegp
 Home-page: https://github.com/PFLeget/treegp
-Download-URL: https://github.com/PFLeget/treegp/releases/tag/v1.0.0.zip
+Download-URL: https://github.com/PFLeget/treegp/releases/tag/v1.0.1.zip
 Author: PFLeget
 License: BSD License
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Intended Audience :: Science/Research
 License-File: LICENCE
 
-[![Build Status](https://github.com/PFLeget/treegp/actions/workflows/test_treegp.yaml/badge.svg)](https://github.com/PFLeget/treegp/actions)
-[![Codecov](https://codecov.io/gh/PFLeget/treegp/branch/master/graph/badge.svg)](https://codecov.io/gh/PFLeget/treegp)
-[![Read the Docs](https://readthedocs.org/projects/treegp/badge/?version=latest)](https://treegp.readthedocs.io/en/latest/?badge=latest)
-[![astro-ph.IM](https://img.shields.io/badge/astro--ph.IM-2103.09881-red)](https://arxiv.org/abs/2103.09881)
-[![DOI](https://img.shields.io/badge/DOI-10.1051%2F0004--6361%2F202140463-blue.svg)](https://doi.org/10.1051/0004-6361/202140463)
+.. image:: https://github.com/PFLeget/treegp/actions/workflows/test_treegp.yaml/badge.svg
+   :target: https://github.com/PFLeget/treegp/actions
+.. image:: https://codecov.io/gh/PFLeget/treegp/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/PFLeget/treegp
+.. image:: https://readthedocs.org/projects/treegp/badge/?version=latest
+  :target: https://treegp.readthedocs.io/en/latest/?badge=latest
+.. image:: https://img.shields.io/badge/astro--ph.IM-2103.09881-red
+    :target: https://arxiv.org/abs/2103.09881
+.. image:: https://img.shields.io/badge/DOI-10.1051%2F0004--6361%2F202140463-blue.svg
+   :target: https://doi.org/10.1051/0004-6361/202140463
+		
 
-## Overview
+.. inclusion-marker-do-not-remove
 
-`treegp` is a python gaussian process code that perform 1D and 2D interpolation.
+Overview
+--------
+
+``treegp`` is a python gaussian process code that perform 1D and 2D interpolation.
 
 `treegp` has some special features compared to other available Gaussian Processes codes:
 
-- Hyperparameters estimation will scale in $\cal{O}(n \ log(n))$ with the 2-points correlation function estimation compared to $\cal{O}(n^3)$ with the classical maximum likelihood.
-- Gaussian process interpolation can be performed around a mean function
-- A tool is provided to compute the mean function (`meanify`)
+*   Hyperparameters estimation will scale in O(N log(N)) with the the 2-points correlation function estimation compared to O(N^3) with the classical maximum likelihood.
+    
+*   Gaussian process interpolation can be performed around a mean function
+    
+*   A tool is provided to compute the mean function (``meanify``)
+
+``treegp`` was originally developed for Point Spread Function interpolation within `Piff <https://github.com/rmjarvis/Piff>`_. There is a specific article that describes the math used in ``treegp`` in the context of modelling astrometric shifts of the Subaru Telescope due to atmospheric turbulences. This article can be found 
+`here <https://arxiv.org/abs/2103.09881>`_.
 
-`treegp` was originally developed for Point Spread Function interpolation within [Piff](https://github.com/rmjarvis/Piff). There is a specific article that describes the math used in `treegp` in the context of modeling astrometric shifts of the Subaru Telescope due to atmospheric turbulences. This article can be found [here](	https://doi.org/10.1051/0004-6361/202140463).
 
-## Installation
+Installation
+------------
 
-The easiest way to install is usually:
+The easiest way to install is usually::
 
-```bash
-pip install treegp
-```
+  pip install treegp
 
 which will install the latest released version.
 
-If you would instead like to install the development version, you can do so via:
+If you would instead like to install the development version, you can do so via::
+
+  git clone https://github.com/PFLeget/treegp.git
+  cd treegp/
+  python setup.py install
+
 
-```bash
-git clone https://github.com/PFLeget/treegp.git
-cd treegp/
-python setup.py install
-```
+Dependencies
+------------
 
-## Dependencies
+``treegp`` has for now the following dependencies (see the quick
+installs below):
 
-treegp has for now the following dependencies (see the quick installs below):
+- libraries listed in the `requirements <requirements.txt>`_ file
 
-libraries listed in the [requirements](requirements.txt) file
 
-## Python
+Python
+``````
 
-treegp is regularly tested on Python 3.7, 3.8, 3.9 and 3.10 It may work in other versions of Python (e.g. pypy), but these are not currently supported.
+``treegp`` is regularly tested on Python 3.7, 3.8, 3.9 and 3.10.  It may work in other
+versions of Python (e.g. pypy), but these are not currently supported.
```

### Comparing `treegp-1.0.0/README.md` & `treegp-1.0.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,61 @@
-[![Build Status](https://github.com/PFLeget/treegp/actions/workflows/test_treegp.yaml/badge.svg)](https://github.com/PFLeget/treegp/actions)
-[![Codecov](https://codecov.io/gh/PFLeget/treegp/branch/master/graph/badge.svg)](https://codecov.io/gh/PFLeget/treegp)
-[![Read the Docs](https://readthedocs.org/projects/treegp/badge/?version=latest)](https://treegp.readthedocs.io/en/latest/?badge=latest)
-[![astro-ph.IM](https://img.shields.io/badge/astro--ph.IM-2103.09881-red)](https://arxiv.org/abs/2103.09881)
-[![DOI](https://img.shields.io/badge/DOI-10.1051%2F0004--6361%2F202140463-blue.svg)](https://doi.org/10.1051/0004-6361/202140463)
+.. image:: https://github.com/PFLeget/treegp/actions/workflows/test_treegp.yaml/badge.svg
+   :target: https://github.com/PFLeget/treegp/actions
+.. image:: https://codecov.io/gh/PFLeget/treegp/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/PFLeget/treegp
+.. image:: https://readthedocs.org/projects/treegp/badge/?version=latest
+  :target: https://treegp.readthedocs.io/en/latest/?badge=latest
+.. image:: https://img.shields.io/badge/astro--ph.IM-2103.09881-red
+    :target: https://arxiv.org/abs/2103.09881
+.. image:: https://img.shields.io/badge/DOI-10.1051%2F0004--6361%2F202140463-blue.svg
+   :target: https://doi.org/10.1051/0004-6361/202140463
+		
 
-## Overview
+.. inclusion-marker-do-not-remove
 
-`treegp` is a python gaussian process code that perform 1D and 2D interpolation.
+Overview
+--------
+
+``treegp`` is a python gaussian process code that perform 1D and 2D interpolation.
 
 `treegp` has some special features compared to other available Gaussian Processes codes:
 
-- Hyperparameters estimation will scale in $\cal{O}(n \ log(n))$ with the 2-points correlation function estimation compared to $\cal{O}(n^3)$ with the classical maximum likelihood.
-- Gaussian process interpolation can be performed around a mean function
-- A tool is provided to compute the mean function (`meanify`)
+*   Hyperparameters estimation will scale in O(N log(N)) with the the 2-points correlation function estimation compared to O(N^3) with the classical maximum likelihood.
+    
+*   Gaussian process interpolation can be performed around a mean function
+    
+*   A tool is provided to compute the mean function (``meanify``)
+
+``treegp`` was originally developed for Point Spread Function interpolation within `Piff <https://github.com/rmjarvis/Piff>`_. There is a specific article that describes the math used in ``treegp`` in the context of modelling astrometric shifts of the Subaru Telescope due to atmospheric turbulences. This article can be found 
+`here <https://arxiv.org/abs/2103.09881>`_.
 
-`treegp` was originally developed for Point Spread Function interpolation within [Piff](https://github.com/rmjarvis/Piff). There is a specific article that describes the math used in `treegp` in the context of modeling astrometric shifts of the Subaru Telescope due to atmospheric turbulences. This article can be found [here](	https://doi.org/10.1051/0004-6361/202140463).
 
-## Installation
+Installation
+------------
 
-The easiest way to install is usually:
+The easiest way to install is usually::
 
-```bash
-pip install treegp
-```
+  pip install treegp
 
 which will install the latest released version.
 
-If you would instead like to install the development version, you can do so via:
+If you would instead like to install the development version, you can do so via::
+
+  git clone https://github.com/PFLeget/treegp.git
+  cd treegp/
+  python setup.py install
+
 
-```bash
-git clone https://github.com/PFLeget/treegp.git
-cd treegp/
-python setup.py install
-```
+Dependencies
+------------
 
-## Dependencies
+``treegp`` has for now the following dependencies (see the quick
+installs below):
 
-treegp has for now the following dependencies (see the quick installs below):
+- libraries listed in the `requirements <requirements.txt>`_ file
 
-libraries listed in the [requirements](requirements.txt) file
 
-## Python
+Python
+``````
 
-treegp is regularly tested on Python 3.7, 3.8, 3.9 and 3.10 It may work in other versions of Python (e.g. pypy), but these are not currently supported.
+``treegp`` is regularly tested on Python 3.7, 3.8, 3.9 and 3.10.  It may work in other
+versions of Python (e.g. pypy), but these are not currently supported.
```

### Comparing `treegp-1.0.0/setup.py` & `treegp-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import setuptools
 from setuptools import setup, find_packages
 
 # Print some useful information in case there are problems, this info will help troubleshoot.
 print("Using setuptools version", setuptools.__version__)
 print("Python version = ", sys.version)
 
-with open("README.md") as f:
+with open("README.rst") as f:
     long_description = f.read()
 
 # Read in the version from treegp/_version.py
 # cf. http://stackoverflow.com/questions/458550/standard-way-to-embed-version-into-python-package
 version_file = os.path.join("treegp", "_version.py")
 with open(version_file, "rt") as f:
     VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
```

### Comparing `treegp-1.0.0/tests/test_gp_interp.py` & `treegp-1.0.1/tests/test_gp_interp.py`

 * *Files identical despite different names*

### Comparing `treegp-1.0.0/tests/test_hyp_search.py` & `treegp-1.0.1/tests/test_hyp_search.py`

 * *Files identical despite different names*

### Comparing `treegp-1.0.0/tests/test_kernels.py` & `treegp-1.0.1/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `treegp-1.0.0/tests/test_meanify.py` & `treegp-1.0.1/tests/test_meanify.py`

 * *Files identical despite different names*

### Comparing `treegp-1.0.0/treegp/__init__.py` & `treegp-1.0.1/treegp/__init__.py`

 * *Files identical despite different names*

### Comparing `treegp-1.0.0/treegp/gp_interp.py` & `treegp-1.0.1/treegp/gp_interp.py`

 * *Files identical despite different names*

### Comparing `treegp-1.0.0/treegp/kernels.py` & `treegp-1.0.1/treegp/kernels.py`

 * *Files identical despite different names*

### Comparing `treegp-1.0.0/treegp/log_likelihood.py` & `treegp-1.0.1/treegp/log_likelihood.py`

 * *Files identical despite different names*

### Comparing `treegp-1.0.0/treegp/meanify.py` & `treegp-1.0.1/treegp/meanify.py`

 * *Files identical despite different names*

### Comparing `treegp-1.0.0/treegp/two_pcf.py` & `treegp-1.0.1/treegp/two_pcf.py`

 * *Files identical despite different names*

### Comparing `treegp-1.0.0/treegp.egg-info/PKG-INFO` & `treegp-1.0.1/treegp.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,73 @@
 Metadata-Version: 2.1
 Name: treegp
-Version: 1.0.0
+Version: 1.0.1
 Summary: treegp
 Home-page: https://github.com/PFLeget/treegp
-Download-URL: https://github.com/PFLeget/treegp/releases/tag/v1.0.0.zip
+Download-URL: https://github.com/PFLeget/treegp/releases/tag/v1.0.1.zip
 Author: PFLeget
 License: BSD License
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Intended Audience :: Science/Research
 License-File: LICENCE
 
-[![Build Status](https://github.com/PFLeget/treegp/actions/workflows/test_treegp.yaml/badge.svg)](https://github.com/PFLeget/treegp/actions)
-[![Codecov](https://codecov.io/gh/PFLeget/treegp/branch/master/graph/badge.svg)](https://codecov.io/gh/PFLeget/treegp)
-[![Read the Docs](https://readthedocs.org/projects/treegp/badge/?version=latest)](https://treegp.readthedocs.io/en/latest/?badge=latest)
-[![astro-ph.IM](https://img.shields.io/badge/astro--ph.IM-2103.09881-red)](https://arxiv.org/abs/2103.09881)
-[![DOI](https://img.shields.io/badge/DOI-10.1051%2F0004--6361%2F202140463-blue.svg)](https://doi.org/10.1051/0004-6361/202140463)
+.. image:: https://github.com/PFLeget/treegp/actions/workflows/test_treegp.yaml/badge.svg
+   :target: https://github.com/PFLeget/treegp/actions
+.. image:: https://codecov.io/gh/PFLeget/treegp/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/PFLeget/treegp
+.. image:: https://readthedocs.org/projects/treegp/badge/?version=latest
+  :target: https://treegp.readthedocs.io/en/latest/?badge=latest
+.. image:: https://img.shields.io/badge/astro--ph.IM-2103.09881-red
+    :target: https://arxiv.org/abs/2103.09881
+.. image:: https://img.shields.io/badge/DOI-10.1051%2F0004--6361%2F202140463-blue.svg
+   :target: https://doi.org/10.1051/0004-6361/202140463
+		
 
-## Overview
+.. inclusion-marker-do-not-remove
 
-`treegp` is a python gaussian process code that perform 1D and 2D interpolation.
+Overview
+--------
+
+``treegp`` is a python gaussian process code that perform 1D and 2D interpolation.
 
 `treegp` has some special features compared to other available Gaussian Processes codes:
 
-- Hyperparameters estimation will scale in $\cal{O}(n \ log(n))$ with the 2-points correlation function estimation compared to $\cal{O}(n^3)$ with the classical maximum likelihood.
-- Gaussian process interpolation can be performed around a mean function
-- A tool is provided to compute the mean function (`meanify`)
+*   Hyperparameters estimation will scale in O(N log(N)) with the the 2-points correlation function estimation compared to O(N^3) with the classical maximum likelihood.
+    
+*   Gaussian process interpolation can be performed around a mean function
+    
+*   A tool is provided to compute the mean function (``meanify``)
+
+``treegp`` was originally developed for Point Spread Function interpolation within `Piff <https://github.com/rmjarvis/Piff>`_. There is a specific article that describes the math used in ``treegp`` in the context of modelling astrometric shifts of the Subaru Telescope due to atmospheric turbulences. This article can be found 
+`here <https://arxiv.org/abs/2103.09881>`_.
 
-`treegp` was originally developed for Point Spread Function interpolation within [Piff](https://github.com/rmjarvis/Piff). There is a specific article that describes the math used in `treegp` in the context of modeling astrometric shifts of the Subaru Telescope due to atmospheric turbulences. This article can be found [here](	https://doi.org/10.1051/0004-6361/202140463).
 
-## Installation
+Installation
+------------
 
-The easiest way to install is usually:
+The easiest way to install is usually::
 
-```bash
-pip install treegp
-```
+  pip install treegp
 
 which will install the latest released version.
 
-If you would instead like to install the development version, you can do so via:
+If you would instead like to install the development version, you can do so via::
+
+  git clone https://github.com/PFLeget/treegp.git
+  cd treegp/
+  python setup.py install
+
 
-```bash
-git clone https://github.com/PFLeget/treegp.git
-cd treegp/
-python setup.py install
-```
+Dependencies
+------------
 
-## Dependencies
+``treegp`` has for now the following dependencies (see the quick
+installs below):
 
-treegp has for now the following dependencies (see the quick installs below):
+- libraries listed in the `requirements <requirements.txt>`_ file
 
-libraries listed in the [requirements](requirements.txt) file
 
-## Python
+Python
+``````
 
-treegp is regularly tested on Python 3.7, 3.8, 3.9 and 3.10 It may work in other versions of Python (e.g. pypy), but these are not currently supported.
+``treegp`` is regularly tested on Python 3.7, 3.8, 3.9 and 3.10.  It may work in other
+versions of Python (e.g. pypy), but these are not currently supported.
```

