# Comparing `tmp/lca_algebraic_dev-1.1.1753145.dev0.tar.gz` & `tmp/lca_algebraic_dev-1.1.1772272.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lca_algebraic_dev-1.1.1753145.dev0.tar", last modified: Thu May  2 09:05:42 2024, max compression
+gzip compressed data, was "lca_algebraic_dev-1.1.1772272.dev0.tar", last modified: Wed May 15 15:52:56 2024, max compression
```

## Comparing `lca_algebraic_dev-1.1.1753145.dev0.tar` & `lca_algebraic_dev-1.1.1772272.dev0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      199 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/.gitignore
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1331 2020-03-30 15:19:57.000000 lca_algebraic_dev-1.1.1753145.dev0/LICENSE
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      693 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/Makefile
--rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     2916 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/PKG-INFO
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2118 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/README.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5509 2024-05-02 09:02:10.000000 lca_algebraic_dev-1.1.1753145.dev0/RELEASE_NOTES.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        3 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/VERSION
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1147 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    26296 2024-04-30 11:37:51.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/activity.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2224 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/axis_dict.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4736 2024-04-29 09:36:57.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/base_utils.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3015 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/cache.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     6009 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/database.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3600 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/interpolation.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2043 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/io.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    28054 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/lca.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      547 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/log.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1760 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/methods.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    41317 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/params.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      103 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/settings.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    39547 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/stats.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     8202 2024-05-02 08:57:26.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/units.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/
--rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     2916 2024-05-02 09:05:42.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/PKG-INFO
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      757 2024-05-02 09:05:42.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        1 2024-05-02 09:05:42.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      122 2024-05-02 09:05:42.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/requires.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       14 2024-05-02 09:05:42.000000 lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/top_level.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      167 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/requirements.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      338 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/setup.cfg
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2132 2024-05-02 09:05:24.000000 lca_algebraic_dev-1.1.1753145.dev0/setup.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/test/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2021-06-23 08:53:38.000000 lca_algebraic_dev-1.1.1753145.dev0/test/__init__.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-02 09:05:42.386756 lca_algebraic_dev-1.1.1753145.dev0/test/fixtures/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1016 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/test/fixtures/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      777 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1753145.dev0/test/test_axis_dict.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3877 2024-04-29 08:23:09.000000 lca_algebraic_dev-1.1.1753145.dev0/test/test_units.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-15 15:52:56.915981 lca_algebraic_dev-1.1.1772272.dev0/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      199 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1772272.dev0/.gitignore
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1331 2020-03-30 15:19:57.000000 lca_algebraic_dev-1.1.1772272.dev0/LICENSE
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      693 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1772272.dev0/Makefile
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2618 2024-05-15 15:52:56.915981 lca_algebraic_dev-1.1.1772272.dev0/PKG-INFO
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2118 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/README.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5509 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/RELEASE_NOTES.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        3 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/VERSION
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-15 15:52:56.911981 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1147 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    26296 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/activity.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2224 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/axis_dict.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4736 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/base_utils.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3015 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/cache.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     6009 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/database.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3600 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/interpolation.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2043 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/io.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    28075 2024-05-15 15:52:32.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/lca.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      547 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/log.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1760 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/methods.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    41456 2024-05-15 09:17:31.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/params.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      103 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/settings.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    39547 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/stats.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     8313 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/units.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-15 15:52:56.915981 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic_dev.egg-info/
+-rw-r--r--   0 rjolivet  (1000) rjolivet  (1000)     2618 2024-05-15 15:52:56.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      757 2024-05-15 15:52:56.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        1 2024-05-15 15:52:56.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      122 2024-05-15 15:52:56.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic_dev.egg-info/requires.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       14 2024-05-15 15:52:56.000000 lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic_dev.egg-info/top_level.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      167 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/requirements.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      338 2024-05-15 15:52:56.915981 lca_algebraic_dev-1.1.1772272.dev0/setup.cfg
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2132 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/setup.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-15 15:52:56.915981 lca_algebraic_dev-1.1.1772272.dev0/test/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2021-06-23 08:53:38.000000 lca_algebraic_dev-1.1.1772272.dev0/test/__init__.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2024-05-15 15:52:56.915981 lca_algebraic_dev-1.1.1772272.dev0/test/fixtures/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1016 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/test/fixtures/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      777 2024-04-29 08:05:36.000000 lca_algebraic_dev-1.1.1772272.dev0/test/test_axis_dict.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3877 2024-05-14 15:15:47.000000 lca_algebraic_dev-1.1.1772272.dev0/test/test_units.py
```

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/LICENSE` & `lca_algebraic_dev-1.1.1772272.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/Makefile` & `lca_algebraic_dev-1.1.1772272.dev0/Makefile`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/PKG-INFO` & `lca_algebraic_dev-1.1.1772272.dev0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: lca_algebraic_dev
-Version: 1.1.1753145.dev0
-Summary: This library provides a layer above brightway2 for defining parametric models and running super fast LCA for monte carlo analysis.
-Home-page: https://github.com/oie-mines-paristech/lca_algebraic/
-Author: OIE - Mines ParisTech
-Author-email: raphael.jolivet@mines-paristech.fr
-License: BSD
-Keywords: LCA brightway2 monte-carlo parametric
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: tabulate
-Requires-Dist: ipywidgets
-Requires-Dist: pandas
-Requires-Dist: pyarrow
-Requires-Dist: seaborn
-Requires-Dist: sympy
-Requires-Dist: matplotlib
-Requires-Dist: deprecation
-Requires-Dist: brightway2
-Requires-Dist: SALib
-Requires-Dist: pint
-Requires-Dist: typing-extensions
-Requires-Dist: pypardiso
-
 # Introduction
 
 This library is a layer above [**brightway2**](https://brightway.dev/) designed for the definition of **parametric inventories** 
 with fast computation of LCA impacts, suitable for **monte-carlo** / global sensitivity analysis 
 
 It integrates the magic of [Sympy](https://www.sympy.org/en/index.html) in order to write parametric formulas as regular Python expressions.
 
@@ -80,8 +55,8 @@
 Please register to this dedicated mailing list to discuss the evolutions of this library and be informed of future releases :
 
 [lca_algebraic@groupes.mines-paristech.fr](https://groupes.minesparis.psl.eu/wws/subscribe/lca_algebraic)
 
 
 # Documentation
 
-Full documentation and example notebooks are [hosted on **readthedocs**](https://lca-algebraic.readthedocs.io/)
+Full documentation and example notebooks are [hosted on **readthedocs**](https://lca-algebraic.readthedocs.io/)
```

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/README.md` & `lca_algebraic_dev-1.1.1772272.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: lca_algebraic_dev
+Version: 1.1.1772272.dev0
+Summary: This library provides a layer above brightway2 for defining parametric models and running super fast LCA for monte carlo analysis.
+Home-page: https://github.com/oie-mines-paristech/lca_algebraic/
+Author: OIE - Mines ParisTech
+Author-email: raphael.jolivet@mines-paristech.fr
+License: BSD
+Keywords: LCA brightway2 monte-carlo parametric
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Introduction
 
 This library is a layer above [**brightway2**](https://brightway.dev/) designed for the definition of **parametric inventories** 
 with fast computation of LCA impacts, suitable for **monte-carlo** / global sensitivity analysis 
 
 It integrates the magic of [Sympy](https://www.sympy.org/en/index.html) in order to write parametric formulas as regular Python expressions.
 
@@ -55,8 +68,9 @@
 Please register to this dedicated mailing list to discuss the evolutions of this library and be informed of future releases :
 
 [lca_algebraic@groupes.mines-paristech.fr](https://groupes.minesparis.psl.eu/wws/subscribe/lca_algebraic)
 
 
 # Documentation
 
-Full documentation and example notebooks are [hosted on **readthedocs**](https://lca-algebraic.readthedocs.io/)
+Full documentation and example notebooks are [hosted on **readthedocs**](https://lca-algebraic.readthedocs.io/)
+
```

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/RELEASE_NOTES.md` & `lca_algebraic_dev-1.1.1772272.dev0/RELEASE_NOTES.md`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/__init__.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/__init__.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/activity.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/activity.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/axis_dict.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/axis_dict.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/base_utils.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/base_utils.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/cache.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/cache.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/database.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/database.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/interpolation.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/interpolation.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/io.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/io.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/lca.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/lca.py`

 * *Files 0% similar despite different names*

```diff
@@ -718,15 +718,15 @@
             # Already created ?
             return _getDb(target_db).get(code_to_find)
         except DoesNotExist:
             name = act["name"] + " # asTech"
 
             # Create biosphere proxy in User Db
             res = newActivity(
-                target_db, name, act["unit"], {act: 1}, code=code_to_find, isProxy=True
+                target_db, name, act["unit"], {act: 1}, code=code_to_find, switchActivity=True, isProxy=True
             )  # add a this flag to distinguish this dummy activity from others
             return res
     else:
         return act
 
 
 def _replace_fixed_params(expr, fixed_params, fixed_mode=FixedParamMode.DEFAULT):
```

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/log.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/log.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/methods.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/methods.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/params.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -881,14 +881,19 @@
 
     def __len__(self):
         return len(self.params)
 
     def __getitem__(self, key):
         try:
             params_per_db = self.params[key]
+
+            if len(params_per_db) == 0:
+                # Param not found
+                raise KeyError("Parameter %s not found" % key)
+
             if len(params_per_db) == 1:
                 return list(params_per_db.values())[0]
 
             if DbContext.current_db() is None:
                 dbs = [key or "<project>" for key in params_per_db.keys()]
                 raise DuplicateParamsAndNoContextException(
                     """
```

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/stats.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/stats.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic/units.py` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 
 # The global Unit registry
 unit_registry = UnitRegistry()
 
 
 def check_unit_consistency(db_name: str):
-    """Check units of exchanges VS units of target activities in a single database"""
+    """
+    Check units of exchanges VS units of target activities in a single database.
+    This check is done statically. The purpose is to run this on a background, non parametric, database."""
     db = bw.Database(db_name)
 
     errors = list()
     for act in db:
         for ex in act.exchanges():
             sub_act = getActByCode(*ex["input"])
```

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/PKG-INFO` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic_dev.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,19 @@
 Metadata-Version: 2.1
-Name: lca_algebraic_dev
-Version: 1.1.1753145.dev0
+Name: lca-algebraic-dev
+Version: 1.1.1772272.dev0
 Summary: This library provides a layer above brightway2 for defining parametric models and running super fast LCA for monte carlo analysis.
 Home-page: https://github.com/oie-mines-paristech/lca_algebraic/
 Author: OIE - Mines ParisTech
 Author-email: raphael.jolivet@mines-paristech.fr
 License: BSD
 Keywords: LCA brightway2 monte-carlo parametric
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tabulate
-Requires-Dist: ipywidgets
-Requires-Dist: pandas
-Requires-Dist: pyarrow
-Requires-Dist: seaborn
-Requires-Dist: sympy
-Requires-Dist: matplotlib
-Requires-Dist: deprecation
-Requires-Dist: brightway2
-Requires-Dist: SALib
-Requires-Dist: pint
-Requires-Dist: typing-extensions
-Requires-Dist: pypardiso
 
 # Introduction
 
 This library is a layer above [**brightway2**](https://brightway.dev/) designed for the definition of **parametric inventories** 
 with fast computation of LCA impacts, suitable for **monte-carlo** / global sensitivity analysis 
 
 It integrates the magic of [Sympy](https://www.sympy.org/en/index.html) in order to write parametric formulas as regular Python expressions.
@@ -81,7 +69,8 @@
 
 [lca_algebraic@groupes.mines-paristech.fr](https://groupes.minesparis.psl.eu/wws/subscribe/lca_algebraic)
 
 
 # Documentation
 
 Full documentation and example notebooks are [hosted on **readthedocs**](https://lca-algebraic.readthedocs.io/)
+
```

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/lca_algebraic_dev.egg-info/SOURCES.txt` & `lca_algebraic_dev-1.1.1772272.dev0/lca_algebraic_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/setup.py` & `lca_algebraic_dev-1.1.1772272.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/test/fixtures/__init__.py` & `lca_algebraic_dev-1.1.1772272.dev0/test/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/test/test_axis_dict.py` & `lca_algebraic_dev-1.1.1772272.dev0/test/test_axis_dict.py`

 * *Files identical despite different names*

### Comparing `lca_algebraic_dev-1.1.1753145.dev0/test/test_units.py` & `lca_algebraic_dev-1.1.1772272.dev0/test/test_units.py`

 * *Files identical despite different names*

