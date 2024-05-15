# Comparing `tmp/anjana-0.2.1.tar.gz` & `tmp/anjana-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anjana-0.2.1.tar", max compression
+gzip compressed data, was "anjana-0.2.2.tar", max compression
```

## Comparing `anjana-0.2.1.tar` & `anjana-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11353 2024-05-13 14:49:49.797227 anjana-0.2.1/LICENSE
--rw-r--r--   0        0        0     9993 2024-05-13 14:49:49.797227 anjana-0.2.1/README.md
--rw-r--r--   0        0        0      743 2024-05-13 14:49:49.797227 anjana-0.2.1/anjana/__init__.py
--rw-r--r--   0        0        0     1277 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/__init__.py
--rw-r--r--   0        0        0     6416 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/_beta_likeness.py
--rw-r--r--   0        0        0     3633 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/_delta_disclosure.py
--rw-r--r--   0        0        0    10183 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/_k_anonymity.py
--rw-r--r--   0        0        0    13604 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/_l_diversity.py
--rw-r--r--   0        0        0     3501 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/_t_closeness.py
--rw-r--r--   0        0        0      990 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/utils/__init__.py
--rw-r--r--   0        0        0     6032 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/utils/utils.py
--rw-r--r--   0        0        0     2048 2024-05-13 14:49:49.829227 anjana-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    11482 1970-01-01 00:00:00.000000 anjana-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11353 2024-05-15 12:13:59.037415 anjana-0.2.2/LICENSE
+-rw-r--r--   0        0        0    10022 2024-05-15 12:13:59.037415 anjana-0.2.2/README.md
+-rw-r--r--   0        0        0      743 2024-05-15 12:13:59.037415 anjana-0.2.2/anjana/__init__.py
+-rw-r--r--   0        0        0     1277 2024-05-15 12:13:59.037415 anjana-0.2.2/anjana/anonymity/__init__.py
+-rw-r--r--   0        0        0     6416 2024-05-15 12:13:59.037415 anjana-0.2.2/anjana/anonymity/_beta_likeness.py
+-rw-r--r--   0        0        0     3633 2024-05-15 12:13:59.037415 anjana-0.2.2/anjana/anonymity/_delta_disclosure.py
+-rw-r--r--   0        0        0    10183 2024-05-15 12:13:59.037415 anjana-0.2.2/anjana/anonymity/_k_anonymity.py
+-rw-r--r--   0        0        0    13604 2024-05-15 12:13:59.037415 anjana-0.2.2/anjana/anonymity/_l_diversity.py
+-rw-r--r--   0        0        0     3501 2024-05-15 12:13:59.037415 anjana-0.2.2/anjana/anonymity/_t_closeness.py
+-rw-r--r--   0        0        0      990 2024-05-15 12:13:59.037415 anjana-0.2.2/anjana/anonymity/utils/__init__.py
+-rw-r--r--   0        0        0     6032 2024-05-15 12:13:59.037415 anjana-0.2.2/anjana/anonymity/utils/utils.py
+-rw-r--r--   0        0        0     2029 2024-05-15 12:13:59.069416 anjana-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    11477 1970-01-01 00:00:00.000000 anjana-0.2.2/PKG-INFO
```

### Comparing `anjana-0.2.1/LICENSE` & `anjana-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anjana-0.2.1/README.md` & `anjana-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ANJANA
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://gitlab.ifca.es/privacy-security/anjana/-/blob/main/LICENSE)
 [![codecov](https://codecov.io/gh/IFCA-Advanced-Computing/anjana/graph/badge.svg?token=AVI53GZ7YD)](https://codecov.io/gh/IFCA-Advanced-Computing/anjana)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11184468.svg)](https://doi.org/10.5281/zenodo.11184468)
 ![PyPI](https://img.shields.io/pypi/v/anjana)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/anjana)
+[![Downloads](https://static.pepy.tech/badge/anjana)](https://pepy.tech/project/anjana)
 [![Documentation Status](https://readthedocs.org/projects/anjana/badge/?version=latest)](https://anjana.readthedocs.io/en/latest/?badge=latest)
 [![release-please](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/release-please.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/release-please.yml)
 [![Publish Package in PyPI](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/pypi.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/pypi.yml)
 [![CI/CD Pipeline](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/cicd.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/cicd.yml)
 [![Code Coverage](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/.codecov.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/.codecov.yml)
 ![Python version](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue)
```

### Comparing `anjana-0.2.1/anjana/__init__.py` & `anjana-0.2.2/anjana/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """ANJANA is an open source framework for anonymizing data with different techniques."""
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `anjana-0.2.1/anjana/anonymity/__init__.py` & `anjana-0.2.2/anjana/anonymity/__init__.py`

 * *Files identical despite different names*

### Comparing `anjana-0.2.1/anjana/anonymity/_beta_likeness.py` & `anjana-0.2.2/anjana/anonymity/_beta_likeness.py`

 * *Files identical despite different names*

### Comparing `anjana-0.2.1/anjana/anonymity/_delta_disclosure.py` & `anjana-0.2.2/anjana/anonymity/_delta_disclosure.py`

 * *Files identical despite different names*

### Comparing `anjana-0.2.1/anjana/anonymity/_k_anonymity.py` & `anjana-0.2.2/anjana/anonymity/_k_anonymity.py`

 * *Files identical despite different names*

### Comparing `anjana-0.2.1/anjana/anonymity/_l_diversity.py` & `anjana-0.2.2/anjana/anonymity/_l_diversity.py`

 * *Files identical despite different names*

### Comparing `anjana-0.2.1/anjana/anonymity/_t_closeness.py` & `anjana-0.2.2/anjana/anonymity/_t_closeness.py`

 * *Files identical despite different names*

### Comparing `anjana-0.2.1/anjana/anonymity/utils/__init__.py` & `anjana-0.2.2/anjana/anonymity/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anjana-0.2.1/anjana/anonymity/utils/utils.py` & `anjana-0.2.2/anjana/anonymity/utils/utils.py`

 * *Files identical despite different names*

### Comparing `anjana-0.2.1/pyproject.toml` & `anjana-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anjana"
-version = "0.2.1"
+version = "0.2.2"
 description = "ANJANA is an open source framework for applying different anonymity techniques."
 authors = [
     "Judith Sáinz-Pardo Díaz <sainzpardo@ifca.unican.es>",
     "Álvaro López García <aloga@ifca.unican.es>"
 ]
 maintainers = ["Judith Sáinz-Pardo Díaz <sainzpardo@ifca.unican.es>"]
 license = "Apache License 2.0"
@@ -29,15 +29,14 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "1.26.4"
 pandas = "2.1.4"
 pycanon = "1.0.1.post2"
-tabulate = "0.9.0"
 typing_extensions = "4.9.0"
 beartype = "0.17.2"
 docutils = "0.20.1"
 
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.11.4"
```

### Comparing `anjana-0.2.1/PKG-INFO` & `anjana-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anjana
-Version: 0.2.1
+Version: 0.2.2
 Summary: ANJANA is an open source framework for applying different anonymity techniques.
 Home-page: https://gitlab.ifca.es/privacy-security/anjana
 License: Apache-2.0
 Keywords: anonymity,privacy
 Author: Judith Sáinz-Pardo Díaz
 Author-email: sainzpardo@ifca.unican.es
 Maintainer: Judith Sáinz-Pardo Díaz
@@ -25,25 +25,24 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Security
 Requires-Dist: beartype (==0.17.2)
 Requires-Dist: docutils (==0.20.1)
 Requires-Dist: numpy (==1.26.4)
 Requires-Dist: pandas (==2.1.4)
 Requires-Dist: pycanon (==1.0.1.post2)
-Requires-Dist: tabulate (==0.9.0)
 Requires-Dist: typing_extensions (==4.9.0)
 Project-URL: Repository, https://gitlab.ifca.es/privacy-security/anjana
 Description-Content-Type: text/markdown
 
 # ANJANA
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://gitlab.ifca.es/privacy-security/anjana/-/blob/main/LICENSE)
 [![codecov](https://codecov.io/gh/IFCA-Advanced-Computing/anjana/graph/badge.svg?token=AVI53GZ7YD)](https://codecov.io/gh/IFCA-Advanced-Computing/anjana)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11184468.svg)](https://doi.org/10.5281/zenodo.11184468)
 ![PyPI](https://img.shields.io/pypi/v/anjana)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/anjana)
+[![Downloads](https://static.pepy.tech/badge/anjana)](https://pepy.tech/project/anjana)
 [![Documentation Status](https://readthedocs.org/projects/anjana/badge/?version=latest)](https://anjana.readthedocs.io/en/latest/?badge=latest)
 [![release-please](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/release-please.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/release-please.yml)
 [![Publish Package in PyPI](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/pypi.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/pypi.yml)
 [![CI/CD Pipeline](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/cicd.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/cicd.yml)
 [![Code Coverage](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/.codecov.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/.codecov.yml)
 ![Python version](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue)
```

