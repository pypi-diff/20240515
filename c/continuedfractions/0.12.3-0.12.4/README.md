# Comparing `tmp/continuedfractions-0.12.3.tar.gz` & `tmp/continuedfractions-0.12.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuedfractions-0.12.3.tar", last modified: Wed May 15 06:24:17 2024, max compression
+gzip compressed data, was "continuedfractions-0.12.4.tar", last modified: Wed May 15 08:51:10 2024, max compression
```

## Comparing `continuedfractions-0.12.3.tar` & `continuedfractions-0.12.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.3/LICENSE
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.3/LICENSE
--rw-r--r--   0        0        0     3159 2024-05-15 05:58:00.271106 continuedfractions-0.12.3/README.md
--rw-r--r--   0        0        0     3159 2024-05-15 05:58:00.271106 continuedfractions-0.12.3/README.md
--rw-r--r--   0        0        0     3506 2024-05-15 06:24:17.210703 continuedfractions-0.12.3/pyproject.toml
--rw-r--r--   0        0        0    31312 2024-03-28 15:58:08.840824 continuedfractions-0.12.3/src/continuedfractions/continuedfraction.py
--rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.3/src/continuedfractions/lib.py
--rw-r--r--   0        0        0    40745 2024-05-15 06:11:07.304519 continuedfractions-0.12.3/src/continuedfractions/sequences.py
--rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.3/src/continuedfractions/utils.py
--rw-r--r--   0        0        0       23 2024-05-14 22:03:02.380992 continuedfractions-0.12.3/src/continuedfractions/version.py
--rw-r--r--   0        0        0    24143 1970-01-01 00:00:00.000000 continuedfractions-0.12.3/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.4/LICENSE
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.4/LICENSE
+-rw-r--r--   0        0        0     3203 2024-05-15 08:16:43.453630 continuedfractions-0.12.4/README.md
+-rw-r--r--   0        0        0     3203 2024-05-15 08:16:43.453630 continuedfractions-0.12.4/README.md
+-rw-r--r--   0        0        0     3506 2024-05-15 08:51:10.901697 continuedfractions-0.12.4/pyproject.toml
+-rw-r--r--   0        0        0    31312 2024-03-28 15:58:08.840824 continuedfractions-0.12.4/src/continuedfractions/continuedfraction.py
+-rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.4/src/continuedfractions/lib.py
+-rw-r--r--   0        0        0    40745 2024-05-15 08:31:34.637882 continuedfractions-0.12.4/src/continuedfractions/sequences.py
+-rw-r--r--   0        0        0     2077 2024-05-14 16:54:10.659103 continuedfractions-0.12.4/src/continuedfractions/utils.py
+-rw-r--r--   0        0        0       23 2024-05-15 06:39:57.156955 continuedfractions-0.12.4/src/continuedfractions/version.py
+-rw-r--r--   0        0        0    24187 1970-01-01 00:00:00.000000 continuedfractions-0.12.4/PKG-INFO
```

### Comparing `continuedfractions-0.12.3/LICENSE` & `continuedfractions-0.12.4/LICENSE`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.3/README.md` & `continuedfractions-0.12.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm-project.org)
 [![License: MPL
 2.0](https://img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](https://opensource.org/licenses/MPL-2.0)
 [![Docs](https://readthedocs.org/projects/continuedfractions/badge/?version=latest)](https://continuedfractions.readthedocs.io/en/latest/?badge=latest)
 <a href="https://trackgit.com">
 <img src="https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lsudelfvcxb7f1xm6i4l" alt="trackgit-views" />
 </a>
-[![PyPI version](https://badge.fury.io/py/continuedfractions.svg)](https://badge.fury.io/py/continuedfractions)
+[![PyPI version](https://img.shields.io/pypi/v/continuedfractions?logo=python&color=41bb13)](https://pypi.org/project/continuedfractions)
 [![Downloads](https://static.pepy.tech/badge/continuedfractions/week)](https://pepy.tech/project/continuedfractions)
 
 </div>
 
 # continuedfractions
 
 A simple extension of the Python [`fractions`](https://docs.python.org/3/library/fractions.html) standard library for working with [continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) as Python objects.
 
-The [PyPI package](https://pypi.org/project/continuedfractions/) only uses standard libraries and can be installed on any **Linux**, **Mac OS** or **Windows** system supporting **Python 3.10**, **3.11**, or **3.12**.
+The [PyPI package](https://pypi.org/project/continuedfractions/) is here. Only standard libraries are used, and the package can be installed on any **Linux**, **Mac OS** or **Windows** system supporting **Python 3.10**, **3.11**, or **3.12**.
 ```shell
 pip install continuedfractions
 ```
 
 See the [project docs](https://continuedfractions.readthedocs.io/en/latest/) for more details, which includes the [API reference](https://continuedfractions.readthedocs.io/en/latest/sources/api-reference.html).
 
 [Continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) are beautiful and interesting mathematical objects, with many connections in [number theory](https://en.wikipedia.org/wiki/Number_theory) and also very useful practical applications, including the [rational approximation of real numbers](https://en.wikipedia.org/wiki/Continued_fraction#Best_rational_approximations).
 
 The `continuedfractions` package is designed for:
 
 * working with (finite) continued fractions as Python objects
 * exploring their key properties, such as elements/coefficients, convergents, segments, remainders, and others
 * operating on them as rationals and instances of the standard library [`fractions.Fraction`](https://docs.python.org/3/library/fractions.html#fractions.Fraction) class
 * supporting approximations and experimental computations for irrational numbers
-* exploring other objects related to continued fractions, such as mediants, sequences of coprime integers, and Farey sequences
+* exploring other related objects, such as mediants, and special sequences of rational numbers such as Farey sequences
 
 The project is [licensed](LICENSE) under the [Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
```

#### html2text {}

```diff
@@ -6,35 +6,36 @@
      [![Codecov](https://codecov.io/gh/sr-murthy/continuedfractions/graph/
          badge.svg?token=GWQ08T4P5J)](https://codecov.io/gh/sr-murthy/
  continuedfractions) [![pdm-managed](https://img.shields.io/badge/pdm-managed-
       blueviolet)](https://pdm-project.org) [![License: MPL 2.0](https://
 img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](https://opensource.org/
 licenses/MPL-2.0) [![Docs](https://readthedocs.org/projects/continuedfractions/
  badge/?version=latest)](https://continuedfractions.readthedocs.io/en/latest/
-   ?badge=latest) _[_t_r_a_c_k_g_i_t_-_v_i_e_w_s_][![PyPI version](https://badge.fury.io/py/
-   continuedfractions.svg)](https://badge.fury.io/py/continuedfractions) [!
- [Downloads](https://static.pepy.tech/badge/continuedfractions/week)](https://
-                     pepy.tech/project/continuedfractions)
+?badge=latest) _[_t_r_a_c_k_g_i_t_-_v_i_e_w_s_][![PyPI version](https://img.shields.io/pypi/v/
+    continuedfractions?logo=python&color=41bb13)](https://pypi.org/project/
+       continuedfractions) [![Downloads](https://static.pepy.tech/badge/
+    continuedfractions/week)](https://pepy.tech/project/continuedfractions)
 # continuedfractions A simple extension of the Python [`fractions`](https://
 docs.python.org/3/library/fractions.html) standard library for working with
 [continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) as
 Python objects. The [PyPI package](https://pypi.org/project/continuedfractions/
-) only uses standard libraries and can be installed on any **Linux**, **Mac
-OS** or **Windows** system supporting **Python 3.10**, **3.11**, or **3.12**.
-```shell pip install continuedfractions ``` See the [project docs](https://
-continuedfractions.readthedocs.io/en/latest/) for more details, which includes
-the [API reference](https://continuedfractions.readthedocs.io/en/latest/
-sources/api-reference.html). [Continued fractions](https://en.wikipedia.org/
-wiki/Continued_fraction) are beautiful and interesting mathematical objects,
-with many connections in [number theory](https://en.wikipedia.org/wiki/
-Number_theory) and also very useful practical applications, including the
-[rational approximation of real numbers](https://en.wikipedia.org/wiki/
+) is here. Only standard libraries are used, and the package can be installed
+on any **Linux**, **Mac OS** or **Windows** system supporting **Python 3.10**,
+**3.11**, or **3.12**. ```shell pip install continuedfractions ``` See the
+[project docs](https://continuedfractions.readthedocs.io/en/latest/) for more
+details, which includes the [API reference](https://
+continuedfractions.readthedocs.io/en/latest/sources/api-reference.html).
+[Continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) are
+beautiful and interesting mathematical objects, with many connections in
+[number theory](https://en.wikipedia.org/wiki/Number_theory) and also very
+useful practical applications, including the [rational approximation of real
+numbers](https://en.wikipedia.org/wiki/
 Continued_fraction#Best_rational_approximations). The `continuedfractions`
 package is designed for: * working with (finite) continued fractions as Python
 objects * exploring their key properties, such as elements/coefficients,
 convergents, segments, remainders, and others * operating on them as rationals
 and instances of the standard library [`fractions.Fraction`](https://
 docs.python.org/3/library/fractions.html#fractions.Fraction) class * supporting
 approximations and experimental computations for irrational numbers * exploring
-other objects related to continued fractions, such as mediants, sequences of
-coprime integers, and Farey sequences The project is [licensed](LICENSE) under
-the [Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
+other related objects, such as mediants, and special sequences of rational
+numbers such as Farey sequences The project is [licensed](LICENSE) under the
+[Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
```

### Comparing `continuedfractions-0.12.3/pyproject.toml` & `continuedfractions-0.12.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
-version = "0.12.3"
+version = "0.12.4"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 user = [
     "jupyter",
```

### Comparing `continuedfractions-0.12.3/src/continuedfractions/continuedfraction.py` & `continuedfractions-0.12.4/src/continuedfractions/continuedfraction.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.3/src/continuedfractions/lib.py` & `continuedfractions-0.12.4/src/continuedfractions/lib.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.3/src/continuedfractions/sequences.py` & `continuedfractions-0.12.4/src/continuedfractions/sequences.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.3/src/continuedfractions/utils.py` & `continuedfractions-0.12.4/src/continuedfractions/utils.py`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.12.3/PKG-INFO` & `continuedfractions-0.12.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuedfractions
-Version: 0.12.3
+Version: 0.12.4
 Summary: Object-oriented continued fractions with Python.
 Keywords: computational number theory,coprime integers,continued fractions,farey sequences,irrational numbers,mediants,number theory,rational approximation,rational numbers,real numbers
 Author-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 Maintainer-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
@@ -404,36 +404,36 @@
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm-project.org)
 [![License: MPL
 2.0](https://img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](https://opensource.org/licenses/MPL-2.0)
 [![Docs](https://readthedocs.org/projects/continuedfractions/badge/?version=latest)](https://continuedfractions.readthedocs.io/en/latest/?badge=latest)
 <a href="https://trackgit.com">
 <img src="https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lsudelfvcxb7f1xm6i4l" alt="trackgit-views" />
 </a>
-[![PyPI version](https://badge.fury.io/py/continuedfractions.svg)](https://badge.fury.io/py/continuedfractions)
+[![PyPI version](https://img.shields.io/pypi/v/continuedfractions?logo=python&color=41bb13)](https://pypi.org/project/continuedfractions)
 [![Downloads](https://static.pepy.tech/badge/continuedfractions/week)](https://pepy.tech/project/continuedfractions)
 
 </div>
 
 # continuedfractions
 
 A simple extension of the Python [`fractions`](https://docs.python.org/3/library/fractions.html) standard library for working with [continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) as Python objects.
 
-The [PyPI package](https://pypi.org/project/continuedfractions/) only uses standard libraries and can be installed on any **Linux**, **Mac OS** or **Windows** system supporting **Python 3.10**, **3.11**, or **3.12**.
+The [PyPI package](https://pypi.org/project/continuedfractions/) is here. Only standard libraries are used, and the package can be installed on any **Linux**, **Mac OS** or **Windows** system supporting **Python 3.10**, **3.11**, or **3.12**.
 ```shell
 pip install continuedfractions
 ```
 
 See the [project docs](https://continuedfractions.readthedocs.io/en/latest/) for more details, which includes the [API reference](https://continuedfractions.readthedocs.io/en/latest/sources/api-reference.html).
 
 [Continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) are beautiful and interesting mathematical objects, with many connections in [number theory](https://en.wikipedia.org/wiki/Number_theory) and also very useful practical applications, including the [rational approximation of real numbers](https://en.wikipedia.org/wiki/Continued_fraction#Best_rational_approximations).
 
 The `continuedfractions` package is designed for:
 
 * working with (finite) continued fractions as Python objects
 * exploring their key properties, such as elements/coefficients, convergents, segments, remainders, and others
 * operating on them as rationals and instances of the standard library [`fractions.Fraction`](https://docs.python.org/3/library/fractions.html#fractions.Fraction) class
 * supporting approximations and experimental computations for irrational numbers
-* exploring other objects related to continued fractions, such as mediants, sequences of coprime integers, and Farey sequences
+* exploring other related objects, such as mediants, and special sequences of rational numbers such as Farey sequences
 
 The project is [licensed](LICENSE) under the [Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
```

