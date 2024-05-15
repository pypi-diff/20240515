# Comparing `tmp/simplelens-1.1.0.tar.gz` & `tmp/simplelens-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplelens-1.1.0.tar", last modified: Fri May 10 17:05:14 2024, max compression
+gzip compressed data, was "simplelens-1.1.1.tar", last modified: Wed May 15 14:14:04 2024, max compression
```

## Comparing `simplelens-1.1.0.tar` & `simplelens-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:05:14.398829 simplelens-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-10 17:05:14.398829 simplelens-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-10 17:05:05.000000 simplelens-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:05:14.394829 simplelens-1.1.0/lens/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 17:05:05.000000 simplelens-1.1.0/lens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-10 17:05:05.000000 simplelens-1.1.0/lens/lens.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-10 17:05:05.000000 simplelens-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:05:14.398829 simplelens-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:05:14.398829 simplelens-1.1.0/simplelens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-10 17:05:14.000000 simplelens-1.1.0/simplelens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-10 17:05:14.000000 simplelens-1.1.0/simplelens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:05:14.000000 simplelens-1.1.0/simplelens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 17:05:14.000000 simplelens-1.1.0/simplelens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 17:05:14.000000 simplelens-1.1.0/simplelens.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:05:14.398829 simplelens-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-10 17:05:05.000000 simplelens-1.1.0/tests/test_focus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-10 17:05:05.000000 simplelens-1.1.0/tests/test_lens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:14:04.902652 simplelens-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-15 14:14:04.902652 simplelens-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-15 14:13:56.000000 simplelens-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:14:04.902652 simplelens-1.1.1/lens/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 14:13:56.000000 simplelens-1.1.1/lens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-15 14:13:56.000000 simplelens-1.1.1/lens/lens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-15 14:13:56.000000 simplelens-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:14:04.902652 simplelens-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:14:04.902652 simplelens-1.1.1/simplelens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-15 14:14:04.000000 simplelens-1.1.1/simplelens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-15 14:14:04.000000 simplelens-1.1.1/simplelens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:14:04.000000 simplelens-1.1.1/simplelens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 14:14:04.000000 simplelens-1.1.1/simplelens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 14:14:04.000000 simplelens-1.1.1/simplelens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:14:04.902652 simplelens-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-15 14:13:56.000000 simplelens-1.1.1/tests/test_focus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-15 14:13:56.000000 simplelens-1.1.1/tests/test_lens.py
```

### Comparing `simplelens-1.1.0/PKG-INFO` & `simplelens-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: simplelens
-Version: 1.1.0
+Version: 1.1.1
 Summary: Implementation of the lens functional pattern
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: build==1.2.1
 
-# Lens v1.1.0
+# Lens v1.1.1
 
 ## Purpose
 
 The purpose of this project is to implement the "Lens" functional pattern in Python and supply that implementation as a package that can be imported into any other python project.
 
 
 ## Install
@@ -18,22 +18,22 @@
     pip install simplelens
 
 ## Uninstall
 
     pip uninstall simplelens
 
 ## Usage
-Install the package from PyPi via pip install
-`from lens import focus`
+Install the package from PyPi via pip install  
+`import lens`
 
 The lens function expects a collection of some form, as well as a list of keys and/or indexes to use to extract data 
 from the collection.
 
     collection = {'a': {'b': [{'a': 1}, {'b': 2}, {'c': 3}]
-    focus(collection, ['a', 'b', 2, 'c'])
+    lens.focus(collection, ['a', 'b', 2, 'c'])
     #=> 3
 
 
 ## Changelog
   See changelog here: [Changelog.md](changelog.md)
```

### Comparing `simplelens-1.1.0/README.md` & `simplelens-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Lens v1.1.0
+# Lens v1.1.1
 
 ## Purpose
 
 The purpose of this project is to implement the "Lens" functional pattern in Python and supply that implementation as a package that can be imported into any other python project.
 
 
 ## Install
@@ -10,22 +10,22 @@
     pip install simplelens
 
 ## Uninstall
 
     pip uninstall simplelens
 
 ## Usage
-Install the package from PyPi via pip install
-`from lens import focus`
+Install the package from PyPi via pip install  
+`import lens`
 
 The lens function expects a collection of some form, as well as a list of keys and/or indexes to use to extract data 
 from the collection.
 
     collection = {'a': {'b': [{'a': 1}, {'b': 2}, {'c': 3}]
-    focus(collection, ['a', 'b', 2, 'c'])
+    lens.focus(collection, ['a', 'b', 2, 'c'])
     #=> 3
 
 
 ## Changelog
   See changelog here: [Changelog.md](changelog.md)
```

### Comparing `simplelens-1.1.0/lens/lens.py` & `simplelens-1.1.1/lens/lens.py`

 * *Files identical despite different names*

### Comparing `simplelens-1.1.0/simplelens.egg-info/PKG-INFO` & `simplelens-1.1.1/simplelens.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: simplelens
-Version: 1.1.0
+Version: 1.1.1
 Summary: Implementation of the lens functional pattern
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: build==1.2.1
 
-# Lens v1.1.0
+# Lens v1.1.1
 
 ## Purpose
 
 The purpose of this project is to implement the "Lens" functional pattern in Python and supply that implementation as a package that can be imported into any other python project.
 
 
 ## Install
@@ -18,22 +18,22 @@
     pip install simplelens
 
 ## Uninstall
 
     pip uninstall simplelens
 
 ## Usage
-Install the package from PyPi via pip install
-`from lens import focus`
+Install the package from PyPi via pip install  
+`import lens`
 
 The lens function expects a collection of some form, as well as a list of keys and/or indexes to use to extract data 
 from the collection.
 
     collection = {'a': {'b': [{'a': 1}, {'b': 2}, {'c': 3}]
-    focus(collection, ['a', 'b', 2, 'c'])
+    lens.focus(collection, ['a', 'b', 2, 'c'])
     #=> 3
 
 
 ## Changelog
   See changelog here: [Changelog.md](changelog.md)
```

### Comparing `simplelens-1.1.0/tests/test_lens.py` & `simplelens-1.1.1/tests/test_lens.py`

 * *Files identical despite different names*

