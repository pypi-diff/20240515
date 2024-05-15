# Comparing `tmp/missing_mga-1.1.0.tar.gz` & `tmp/missing_mga-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "missing_mga-1.1.0.tar", last modified: Sun May 12 19:15:19 2024, max compression
+gzip compressed data, was "missing_mga-1.1.1.tar", last modified: Wed May 15 15:15:43 2024, max compression
```

## Comparing `missing_mga-1.1.0.tar` & `missing_mga-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:15:19.409920 missing_mga-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-12 19:15:11.000000 missing_mga-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-12 19:15:19.405920 missing_mga-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-12 19:15:11.000000 missing_mga-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:15:19.405920 missing_mga-1.1.0/missing_mga/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-12 19:15:11.000000 missing_mga-1.1.0/missing_mga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18433 2024-05-12 19:15:11.000000 missing_mga-1.1.0/missing_mga/missing_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:15:19.405920 missing_mga-1.1.0/missing_mga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-12 19:15:19.000000 missing_mga-1.1.0/missing_mga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-12 19:15:19.000000 missing_mga-1.1.0/missing_mga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:15:19.000000 missing_mga-1.1.0/missing_mga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-12 19:15:19.000000 missing_mga-1.1.0/missing_mga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-12 19:15:19.000000 missing_mga-1.1.0/missing_mga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:15:19.409920 missing_mga-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-12 19:15:11.000000 missing_mga-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:15:19.405920 missing_mga-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-12 19:15:11.000000 missing_mga-1.1.0/tests/test_missing_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:43.130848 missing_mga-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 15:15:37.000000 missing_mga-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-15 15:15:43.130848 missing_mga-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-15 15:15:37.000000 missing_mga-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:43.126848 missing_mga-1.1.1/missing_mga/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 15:15:37.000000 missing_mga-1.1.1/missing_mga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18433 2024-05-15 15:15:37.000000 missing_mga-1.1.1/missing_mga/missing_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:43.130848 missing_mga-1.1.1/missing_mga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-15 15:15:43.000000 missing_mga-1.1.1/missing_mga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-15 15:15:43.000000 missing_mga-1.1.1/missing_mga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:15:43.000000 missing_mga-1.1.1/missing_mga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 15:15:43.000000 missing_mga-1.1.1/missing_mga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 15:15:43.000000 missing_mga-1.1.1/missing_mga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:15:43.130848 missing_mga-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-15 15:15:37.000000 missing_mga-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:15:43.130848 missing_mga-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-15 15:15:37.000000 missing_mga-1.1.1/tests/test_missing_methods.py
```

### Comparing `missing_mga-1.1.0/LICENSE` & `missing_mga-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `missing_mga-1.1.0/PKG-INFO` & `missing_mga-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missing_mga
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package for handling missing values in datasets.
 Home-page: https://github.com/Mgobeaalcoba/missing_mga
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -102,10 +102,14 @@
 
 ## References
 
 - [naniar: Data Structures, Summaries, and Visualisations for Missing Data](https://naniar.njtierney.com/)
 - [Handling Missing Data in Pandas](https://towardsdatascience.com/handling-missing-data-in-pandas-ba0b2ee0f4e4)
 - [Working with Missing Data in Pandas](https://pandas.pydata.org/pandas-docs/stable/user_guide/missing_data.html)
 
+## Metrics
+
+You can find the metrics of this package in the following link: [Metrics](https://lookerstudio.google.com/s/m-3EH05N9W8)
+
 ## Contact
 
 If you have any questions or need further assistance, please contact the package maintainer: gobeamariano@gmail.com
```

### Comparing `missing_mga-1.1.0/README.md` & `missing_mga-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,10 +85,14 @@
 
 ## References
 
 - [naniar: Data Structures, Summaries, and Visualisations for Missing Data](https://naniar.njtierney.com/)
 - [Handling Missing Data in Pandas](https://towardsdatascience.com/handling-missing-data-in-pandas-ba0b2ee0f4e4)
 - [Working with Missing Data in Pandas](https://pandas.pydata.org/pandas-docs/stable/user_guide/missing_data.html)
 
+## Metrics
+
+You can find the metrics of this package in the following link: [Metrics](https://lookerstudio.google.com/s/m-3EH05N9W8)
+
 ## Contact
 
 If you have any questions or need further assistance, please contact the package maintainer: gobeamariano@gmail.com
```

### Comparing `missing_mga-1.1.0/missing_mga/missing_methods.py` & `missing_mga-1.1.1/missing_mga/missing_methods.py`

 * *Files identical despite different names*

### Comparing `missing_mga-1.1.0/missing_mga.egg-info/PKG-INFO` & `missing_mga-1.1.1/missing_mga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missing_mga
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package for handling missing values in datasets.
 Home-page: https://github.com/Mgobeaalcoba/missing_mga
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -102,10 +102,14 @@
 
 ## References
 
 - [naniar: Data Structures, Summaries, and Visualisations for Missing Data](https://naniar.njtierney.com/)
 - [Handling Missing Data in Pandas](https://towardsdatascience.com/handling-missing-data-in-pandas-ba0b2ee0f4e4)
 - [Working with Missing Data in Pandas](https://pandas.pydata.org/pandas-docs/stable/user_guide/missing_data.html)
 
+## Metrics
+
+You can find the metrics of this package in the following link: [Metrics](https://lookerstudio.google.com/s/m-3EH05N9W8)
+
 ## Contact
 
 If you have any questions or need further assistance, please contact the package maintainer: gobeamariano@gmail.com
```

### Comparing `missing_mga-1.1.0/setup.py` & `missing_mga-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='missing_mga',
-    version='1.1.0',
+    version='1.1.1',
     packages=find_packages(),
     install_requires=['pandas', 'numpy', 'matplotlib', 'seaborn', 'upsetplot', 'scikit-learn'],
     author='Mariano Gobea Alcoba',
     author_email='gobeamariano@gmail.com',
     description='A package for handling missing values in datasets.',
     long_description=long_description,  # Usa el contenido del README.md como descripción larga
     long_description_content_type="text/markdown",  # Especifica el tipo de contenido como markdown
```

### Comparing `missing_mga-1.1.0/tests/test_missing_methods.py` & `missing_mga-1.1.1/tests/test_missing_methods.py`

 * *Files identical despite different names*

