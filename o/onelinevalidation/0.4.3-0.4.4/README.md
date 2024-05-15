# Comparing `tmp/onelinevalidation-0.4.3.tar.gz` & `tmp/onelinevalidation-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onelinevalidation-0.4.3.tar", last modified: Sun Feb 25 19:54:30 2024, max compression
+gzip compressed data, was "onelinevalidation-0.4.4.tar", last modified: Sun Feb 25 20:29:53 2024, max compression
```

## Comparing `onelinevalidation-0.4.3.tar` & `onelinevalidation-0.4.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-25 19:54:30.589586 onelinevalidation-0.4.3/
--rw-rw-rw-   0        0        0     1092 2023-03-08 14:21:18.000000 onelinevalidation-0.4.3/LICENSE
--rw-rw-rw-   0        0        0     4608 2024-02-25 19:54:30.589586 onelinevalidation-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     3837 2024-02-25 19:30:35.000000 onelinevalidation-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-25 19:54:30.495851 onelinevalidation-0.4.3/onelinevalidation/
--rw-rw-rw-   0        0        0      323 2024-02-25 19:54:07.000000 onelinevalidation-0.4.3/onelinevalidation/__init__.py
--rw-rw-rw-   0        0        0     3935 2024-02-25 19:10:44.000000 onelinevalidation-0.4.3/onelinevalidation/onelinevalidation.py
-drwxrwxrwx   0        0        0        0 2024-02-25 19:54:30.573962 onelinevalidation-0.4.3/onelinevalidation.egg-info/
--rw-rw-rw-   0        0        0     4608 2024-02-25 19:54:30.000000 onelinevalidation-0.4.3/onelinevalidation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-02-25 19:54:30.000000 onelinevalidation-0.4.3/onelinevalidation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-25 19:54:30.000000 onelinevalidation-0.4.3/onelinevalidation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-02-25 19:54:30.000000 onelinevalidation-0.4.3/onelinevalidation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-02-25 19:54:30.000000 onelinevalidation-0.4.3/onelinevalidation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-25 19:54:30.589586 onelinevalidation-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     4025 2024-02-25 19:44:13.000000 onelinevalidation-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-25 20:29:53.087264 onelinevalidation-0.4.4/
+-rw-rw-rw-   0        0        0     1092 2023-03-08 14:21:18.000000 onelinevalidation-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0     4608 2024-02-25 20:29:53.082267 onelinevalidation-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3837 2024-02-25 19:30:35.000000 onelinevalidation-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-02-25 20:29:52.962065 onelinevalidation-0.4.4/onelinevalidation/
+-rw-rw-rw-   0        0        0      268 2024-02-25 20:29:25.000000 onelinevalidation-0.4.4/onelinevalidation/__init__.py
+-rw-rw-rw-   0        0        0     3935 2024-02-25 20:29:29.000000 onelinevalidation-0.4.4/onelinevalidation/onelinevalidation.py
+-rw-rw-rw-   0        0        0     4025 2024-02-25 20:26:56.000000 onelinevalidation-0.4.4/onelinevalidation/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-25 20:29:53.072879 onelinevalidation-0.4.4/onelinevalidation.egg-info/
+-rw-rw-rw-   0        0        0     4608 2024-02-25 20:29:52.000000 onelinevalidation-0.4.4/onelinevalidation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-02-25 20:29:52.000000 onelinevalidation-0.4.4/onelinevalidation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-25 20:29:52.000000 onelinevalidation-0.4.4/onelinevalidation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-02-25 20:29:52.000000 onelinevalidation-0.4.4/onelinevalidation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-02-25 20:29:52.000000 onelinevalidation-0.4.4/onelinevalidation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-25 20:29:53.088260 onelinevalidation-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     4025 2024-02-25 20:29:15.000000 onelinevalidation-0.4.4/setup.py
```

### Comparing `onelinevalidation-0.4.3/LICENSE` & `onelinevalidation-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onelinevalidation-0.4.3/PKG-INFO` & `onelinevalidation-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onelinevalidation
-Version: 0.4.3
+Version: 0.4.4
 Summary: onelinevalidation It is a simple library in the Python language that performs validate in an easy and simple way
 Home-page: https://github.com/amr2018/onelinevalidation
 Author: Amr Elgarhy
 Author-email: amr.ee@yahoo.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `onelinevalidation-0.4.3/README.md` & `onelinevalidation-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `onelinevalidation-0.4.3/onelinevalidation/onelinevalidation.py` & `onelinevalidation-0.4.4/onelinevalidation/onelinevalidation.py`

 * *Files identical despite different names*

### Comparing `onelinevalidation-0.4.3/onelinevalidation.egg-info/PKG-INFO` & `onelinevalidation-0.4.4/onelinevalidation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onelinevalidation
-Version: 0.4.3
+Version: 0.4.4
 Summary: onelinevalidation It is a simple library in the Python language that performs validate in an easy and simple way
 Home-page: https://github.com/amr2018/onelinevalidation
 Author: Amr Elgarhy
 Author-email: amr.ee@yahoo.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `onelinevalidation-0.4.3/setup.py` & `onelinevalidation-0.4.4/onelinevalidation/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'onelinevalidation'
 DESCRIPTION = 'onelinevalidation It is a simple library in the Python language that performs validate in an easy and simple way'
 URL = 'https://github.com/amr2018/onelinevalidation'
 EMAIL = 'amr.ee@yahoo.com'
 AUTHOR = 'Amr Elgarhy'
 REQUIRES_PYTHON = '>=3.1.0'
-VERSION = '0.4.3'
+VERSION = '0.4.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'validators'
     # 'requests', 'maya', 'records',
 ]
```

