# Comparing `tmp/flake8-fill-one-line-0.3.5.tar.gz` & `tmp/flake8-fill-one-line-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-fill-one-line-0.3.5.tar", last modified: Mon Sep 25 11:23:46 2023, max compression
+gzip compressed data, was "flake8-fill-one-line-0.4.0.tar", last modified: Mon Sep 25 13:57:55 2023, max compression
```

## Comparing `flake8-fill-one-line-0.3.5.tar` & `flake8-fill-one-line-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 11:23:46.659535 flake8-fill-one-line-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2023-09-25 11:23:46.659535 flake8-fill-one-line-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2023-09-25 11:23:34.000000 flake8-fill-one-line-0.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 11:23:46.659535 flake8-fill-one-line-0.3.5/flake8_fill_one_line/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-25 11:23:34.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 11:23:46.659535 flake8-fill-one-line-0.3.5/flake8_fill_one_line/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-09-25 11:23:34.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line/analyzers/call_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-09-25 11:23:34.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line/analyzers/def_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-09-25 11:23:34.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line/analyzers/if_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-09-25 11:23:34.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line/analyzers/if_exp_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-09-25 11:23:34.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line/analyzers/import_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-09-25 11:23:34.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line/analyzers/with_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2023-09-25 11:23:34.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-09-25 11:23:34.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 11:23:46.659535 flake8-fill-one-line-0.3.5/flake8_fill_one_line.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2023-09-25 11:23:46.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-09-25 11:23:46.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 11:23:46.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-09-25 11:23:46.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-25 11:23:46.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-25 11:23:46.000000 flake8-fill-one-line-0.3.5/flake8_fill_one_line.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-09-25 11:23:46.663534 flake8-fill-one-line-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-09-25 11:23:34.000000 flake8-fill-one-line-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 13:57:55.160778 flake8-fill-one-line-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2023-09-25 13:57:55.160778 flake8-fill-one-line-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 13:57:55.152778 flake8-fill-one-line-0.4.0/flake8_fill_one_line/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 13:57:55.160778 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/call_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/def_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/if_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/if_exp_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/import_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/with_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 13:57:55.156778 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2023-09-25 13:57:55.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2023-09-25 13:57:55.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 13:57:55.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2023-09-25 13:57:55.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-25 13:57:55.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-25 13:57:55.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-09-25 13:57:55.160778 flake8-fill-one-line-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/setup.py
```

### Comparing `flake8-fill-one-line-0.3.5/PKG-INFO` & `flake8-fill-one-line-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: flake8-fill-one-line
-Version: 0.3.5
+Version: 0.4.0
 Summary: A Flake8 plugin to ensure an expression can be written in one line without exceeding the maximum length limit
 Home-page: https://github.com/dronperminov/flake8-fill-one-line
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 
 ====================
 flake8-fill-one-line
 ====================
 
 A Flake8 plugin to ensure an expression can be written in one line without exceeding the maximum length (``160`` characters by default) limit.
```

### Comparing `flake8-fill-one-line-0.3.5/README.rst` & `flake8-fill-one-line-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.3.5/flake8_fill_one_line/analyzers/call_analyzer.py` & `flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/call_analyzer.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,17 @@
         for arg in node.args:
             if self.skip_multiline_arguments and not is_one_line(arg):
                 return None
 
             args_lengths.append(get_node_length(arg))
 
         for keyword in node.keywords:
+            if not hasattr(keyword, "lineno"):
+                return None
+
             if self.skip_multiline_arguments and not is_one_line(keyword):
                 return None
 
             args_lengths.append(get_node_length(keyword))
 
         length = node.func.col_offset + get_node_length(node.func) + 2
         length += sum(args_lengths) + (len(args_lengths) - 1) * 2
```

### Comparing `flake8-fill-one-line-0.3.5/flake8_fill_one_line/analyzers/def_analyzer.py` & `flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/def_analyzer.py`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.3.5/flake8_fill_one_line/analyzers/import_analyzer.py` & `flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/import_analyzer.py`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.3.5/flake8_fill_one_line/analyzers/with_analyzer.py` & `flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/with_analyzer.py`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.3.5/flake8_fill_one_line/check.py` & `flake8-fill-one-line-0.4.0/flake8_fill_one_line/check.py`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.3.5/flake8_fill_one_line/utils.py` & `flake8-fill-one-line-0.4.0/flake8_fill_one_line/utils.py`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.3.5/flake8_fill_one_line.egg-info/PKG-INFO` & `flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: flake8-fill-one-line
-Version: 0.3.5
+Version: 0.4.0
 Summary: A Flake8 plugin to ensure an expression can be written in one line without exceeding the maximum length limit
 Home-page: https://github.com/dronperminov/flake8-fill-one-line
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 
 ====================
 flake8-fill-one-line
 ====================
 
 A Flake8 plugin to ensure an expression can be written in one line without exceeding the maximum length (``160`` characters by default) limit.
```

### Comparing `flake8-fill-one-line-0.3.5/flake8_fill_one_line.egg-info/SOURCES.txt` & `flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.3.5/setup.cfg` & `flake8-fill-one-line-0.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 	flake8_fill_one_line.analyzers.if_analyzer
 	flake8_fill_one_line.analyzers.if_exp_analyzer
 	flake8_fill_one_line.analyzers.import_analyzer
 	flake8_fill_one_line.analyzers.with_analyzer
 install_requires = 
 	flake8>=3.7
 	astunparse>=1.6
-python_requires = >=3.9
+python_requires = >=3.8
 
 [options.entry_points]
 flake8.extension = 
 	FOL=flake8_fill_one_line.check:FillOneLineChecker
 
 [egg_info]
 tag_build =
```

