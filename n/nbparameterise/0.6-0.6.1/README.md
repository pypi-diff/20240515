# Comparing `tmp/nbparameterise-0.6.tar.gz` & `tmp/nbparameterise-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbparameterise-0.6.tar", last modified: Tue Feb 28 11:06:06 2023, max compression
+gzip compressed data, was "nbparameterise-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nbparameterise-0.6.tar` & `nbparameterise-0.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      858 2023-02-28 10:59:45.262802 nbparameterise-0.6/.github/workflows/test.yml
--rw-r--r--   0        0        0       45 2016-03-04 10:32:05.652057 nbparameterise-0.6/.gitignore
--rw-r--r--   0        0        0     1081 2016-03-04 10:32:05.652057 nbparameterise-0.6/LICENSE
--rw-r--r--   0        0        0     2849 2023-02-28 11:03:35.360041 nbparameterise-0.6/README.rst
--rw-r--r--   0        0        0     2131 2021-04-23 13:52:58.669272 nbparameterise-0.6/examples/Fibonacci.ipynb
--rw-r--r--   0        0        0     2160 2021-08-17 14:29:33.906099 nbparameterise-0.6/examples/Stock display.ipynb
--rwxr-xr-x   0        0        0      717 2021-08-17 14:29:33.906099 nbparameterise-0.6/examples/batch.py
--rw-r--r--   0        0        0     3058 2023-02-27 17:03:48.303435 nbparameterise-0.6/examples/htmlform.py
--rw-r--r--   0        0        0      504 2016-03-04 10:32:05.654057 nbparameterise-0.6/examples/static/README.rst
--rw-r--r--   0        0        0      261 2016-03-04 10:32:05.654057 nbparameterise-0.6/examples/static/styles.css
--rwxr-xr-x   0        0        0     2194 2023-02-27 17:03:48.263435 nbparameterise-0.6/examples/webapp.py
--rw-r--r--   0        0        0      211 2023-02-28 11:04:33.063851 nbparameterise-0.6/nbparameterise/__init__.py
--rw-r--r--   0        0        0     6932 2023-02-27 18:51:09.542099 nbparameterise-0.6/nbparameterise/code.py
--rw-r--r--   0        0        0        1 2016-03-04 10:32:05.655057 nbparameterise-0.6/nbparameterise/code_drivers/__init__.py
--rw-r--r--   0        0        0     5241 2023-02-28 10:59:11.560913 nbparameterise-0.6/nbparameterise/code_drivers/python.py
--rw-r--r--   0        0        0      504 2023-02-28 10:59:19.719886 nbparameterise-0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2016-03-04 10:32:05.655057 nbparameterise-0.6/tests/__init__.py
--rw-r--r--   0        0        0     1699 2023-02-27 16:06:49.027029 nbparameterise-0.6/tests/sample.ipynb
--rw-r--r--   0        0        0     1262 2023-02-27 18:53:31.978870 nbparameterise-0.6/tests/sample_parameters_tag.ipynb
--rw-r--r--   0        0        0     5129 2023-02-27 18:51:07.268087 nbparameterise-0.6/tests/test_basic.py
--rw-r--r--   0        0        0     1615 2023-02-27 18:51:07.268087 nbparameterise-0.6/tests/test_parameters_tag.py
--rw-r--r--   0        0        0     3299 1970-01-01 00:00:00.000000 nbparameterise-0.6/PKG-INFO
+-rw-r--r--   0        0        0      858 2023-02-28 10:59:45.262802 nbparameterise-0.6.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0       45 2016-03-04 10:32:05.652057 nbparameterise-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1081 2016-03-04 10:32:05.652057 nbparameterise-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3035 2024-05-15 12:44:23.578967 nbparameterise-0.6.1/README.rst
+-rw-r--r--   0        0        0     2131 2021-04-23 13:52:58.669272 nbparameterise-0.6.1/examples/Fibonacci.ipynb
+-rw-r--r--   0        0        0     2160 2021-08-17 14:29:33.906099 nbparameterise-0.6.1/examples/Stock display.ipynb
+-rwxr-xr-x   0        0        0      717 2021-08-17 14:29:33.906099 nbparameterise-0.6.1/examples/batch.py
+-rw-r--r--   0        0        0     3058 2023-02-27 17:03:48.303435 nbparameterise-0.6.1/examples/htmlform.py
+-rw-r--r--   0        0        0      504 2016-03-04 10:32:05.654057 nbparameterise-0.6.1/examples/static/README.rst
+-rw-r--r--   0        0        0      261 2016-03-04 10:32:05.654057 nbparameterise-0.6.1/examples/static/styles.css
+-rwxr-xr-x   0        0        0     2194 2023-02-27 17:03:48.263435 nbparameterise-0.6.1/examples/webapp.py
+-rw-r--r--   0        0        0      213 2024-05-15 12:42:35.490431 nbparameterise-0.6.1/nbparameterise/__init__.py
+-rw-r--r--   0        0        0     6940 2024-05-15 12:40:49.471919 nbparameterise-0.6.1/nbparameterise/code.py
+-rw-r--r--   0        0        0        1 2016-03-04 10:32:05.655057 nbparameterise-0.6.1/nbparameterise/code_drivers/__init__.py
+-rw-r--r--   0        0        0     5241 2023-02-28 10:59:11.560913 nbparameterise-0.6.1/nbparameterise/code_drivers/python.py
+-rw-r--r--   0        0        0      503 2024-05-15 12:40:49.472919 nbparameterise-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2016-03-04 10:32:05.655057 nbparameterise-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     1699 2023-02-27 16:06:49.027029 nbparameterise-0.6.1/tests/sample.ipynb
+-rw-r--r--   0        0        0     1262 2023-02-27 18:53:31.978870 nbparameterise-0.6.1/tests/sample_parameters_tag.ipynb
+-rw-r--r--   0        0        0     5129 2023-02-27 18:51:07.268087 nbparameterise-0.6.1/tests/test_basic.py
+-rw-r--r--   0        0        0     1615 2023-02-27 18:51:07.268087 nbparameterise-0.6.1/tests/test_parameters_tag.py
+-rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 nbparameterise-0.6.1/PKG-INFO
```

### Comparing `nbparameterise-0.6/.github/workflows/test.yml` & `nbparameterise-0.6.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nbparameterise-0.6/LICENSE` & `nbparameterise-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nbparameterise-0.6/README.rst` & `nbparameterise-0.6.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,22 @@
     nbclient.execute(new_nb)
 
 If you are interested in using your parameterized Jupyter notebooks through a command line interface, have a look at `nbclick <https://github.com/ssciwr/nbclick>`_.
 
 Changes
 -------
 
+0.6.1
+~~~~~
+
+2024-05-15
+
+- nbparameterise no longer requires `nbconvert <https://pypi.org/project/nbconvert/>`_,
+  and loads it only if you pass the deprecated ``execute=True`` option.
+
 0.6
 ~~~
 
 2023-02-28
 
 - The parameters cell no longer needs to be the first code cell: if you add a cell tag
   'parameters' to another cell, parameters will be extracted from and replaced in that
```

### Comparing `nbparameterise-0.6/examples/Fibonacci.ipynb` & `nbparameterise-0.6.1/examples/Fibonacci.ipynb`

 * *Files identical despite different names*

### Comparing `nbparameterise-0.6/examples/Stock display.ipynb` & `nbparameterise-0.6.1/examples/Stock display.ipynb`

 * *Files identical despite different names*

### Comparing `nbparameterise-0.6/examples/batch.py` & `nbparameterise-0.6.1/examples/batch.py`

 * *Files identical despite different names*

### Comparing `nbparameterise-0.6/examples/htmlform.py` & `nbparameterise-0.6.1/examples/htmlform.py`

 * *Files identical despite different names*

### Comparing `nbparameterise-0.6/examples/webapp.py` & `nbparameterise-0.6.1/examples/webapp.py`

 * *Files identical despite different names*

### Comparing `nbparameterise-0.6/nbparameterise/code.py` & `nbparameterise-0.6.1/nbparameterise/code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import copy
 import importlib
 import re
 from warnings import warn
 
-from nbconvert.preprocessors import ExecutePreprocessor
 
 class Parameter(object):
     def __init__(self, name, vtype, value=None, metadata=None, comment=None):
         self.name = name
         self.type = vtype
         self.value = value
         self.metadata = metadata or {}
@@ -179,10 +178,11 @@
     nb = copy.deepcopy(nb)
 
     drv = get_driver_module(nb, override=lang)
     cell = get_parameter_cell(nb, tag)
     cell.source = drv.build_definitions(values, prev_code=cell.source)
     if execute:
         warn("execute=True is deprecated, use nbclient instead", stacklevel=2)
+        from nbconvert.preprocessors import ExecutePreprocessor
         resources = execute_resources or {}
         nb, resources = ExecutePreprocessor().preprocess(nb, resources)
     return nb
```

### Comparing `nbparameterise-0.6/nbparameterise/code_drivers/python.py` & `nbparameterise-0.6.1/nbparameterise/code_drivers/python.py`

 * *Files identical despite different names*

### Comparing `nbparameterise-0.6/tests/sample.ipynb` & `nbparameterise-0.6.1/tests/sample.ipynb`

 * *Files identical despite different names*

### Comparing `nbparameterise-0.6/tests/sample_parameters_tag.ipynb` & `nbparameterise-0.6.1/tests/sample_parameters_tag.ipynb`

 * *Files identical despite different names*

### Comparing `nbparameterise-0.6/tests/test_basic.py` & `nbparameterise-0.6.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nbparameterise-0.6/tests/test_parameters_tag.py` & `nbparameterise-0.6.1/tests/test_parameters_tag.py`

 * *Files identical despite different names*

### Comparing `nbparameterise-0.6/PKG-INFO` & `nbparameterise-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: nbparameterise
-Version: 0.6
+Version: 0.6.1
 Summary: Re-run a notebook substituting input parameters in the first cell.
 Author-email: Thomas Kluyver <thomas@kluyver.me.uk>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Jupyter
-Requires-Dist: nbconvert
+Requires-Dist: nbformat
 Requires-Dist: astcheck >=0.3
 Project-URL: Source, https://github.com/takluyver/nbparameterise
 
 This is a tool to run notebooks with input values. When you write the notebook,
 these are defined in the first code cell - or a cell with a 'parameters' cell
 tag - with regular assignments like this:
 
@@ -67,14 +67,22 @@
     nbclient.execute(new_nb)
 
 If you are interested in using your parameterized Jupyter notebooks through a command line interface, have a look at `nbclick <https://github.com/ssciwr/nbclick>`_.
 
 Changes
 -------
 
+0.6.1
+~~~~~
+
+2024-05-15
+
+- nbparameterise no longer requires `nbconvert <https://pypi.org/project/nbconvert/>`_,
+  and loads it only if you pass the deprecated ``execute=True`` option.
+
 0.6
 ~~~
 
 2023-02-28
 
 - The parameters cell no longer needs to be the first code cell: if you add a cell tag
   'parameters' to another cell, parameters will be extracted from and replaced in that
```

