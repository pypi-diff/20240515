# Comparing `tmp/flake8-fill-one-line-0.4.0.tar.gz` & `tmp/flake8_fill_one_line-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-fill-one-line-0.4.0.tar", last modified: Mon Sep 25 13:57:55 2023, max compression
+gzip compressed data, was "flake8_fill_one_line-0.4.1.tar", last modified: Wed May 15 10:13:45 2024, max compression
```

## Comparing `flake8-fill-one-line-0.4.0.tar` & `flake8_fill_one_line-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 13:57:55.160778 flake8-fill-one-line-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2023-09-25 13:57:55.160778 flake8-fill-one-line-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 13:57:55.152778 flake8-fill-one-line-0.4.0/flake8_fill_one_line/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 13:57:55.160778 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/call_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/def_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/if_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/if_exp_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/import_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/with_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 13:57:55.156778 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2023-09-25 13:57:55.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-09-25 13:57:55.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 13:57:55.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-09-25 13:57:55.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-25 13:57:55.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-25 13:57:55.000000 flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-09-25 13:57:55.160778 flake8-fill-one-line-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-09-25 13:57:40.000000 flake8-fill-one-line-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:13:45.058148 flake8_fill_one_line-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-15 10:13:45.058148 flake8_fill_one_line-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-15 10:13:37.000000 flake8_fill_one_line-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:13:45.054149 flake8_fill_one_line-0.4.1/flake8_fill_one_line/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 10:13:37.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:13:45.054149 flake8_fill_one_line-0.4.1/flake8_fill_one_line/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-15 10:13:37.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line/analyzers/call_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-15 10:13:37.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line/analyzers/def_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-15 10:13:37.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line/analyzers/if_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-15 10:13:37.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line/analyzers/if_exp_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 10:13:37.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line/analyzers/import_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-15 10:13:37.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line/analyzers/with_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-15 10:13:37.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 10:13:37.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:13:45.058148 flake8_fill_one_line-0.4.1/flake8_fill_one_line.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-15 10:13:45.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-15 10:13:45.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:13:45.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 10:13:45.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 10:13:45.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 10:13:45.000000 flake8_fill_one_line-0.4.1/flake8_fill_one_line.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-15 10:13:45.058148 flake8_fill_one_line-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 10:13:37.000000 flake8_fill_one_line-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:13:45.054149 flake8_fill_one_line-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-15 10:13:37.000000 flake8_fill_one_line-0.4.1/tests/test_flake8_fill_one_line.py
```

### Comparing `flake8-fill-one-line-0.4.0/PKG-INFO` & `flake8_fill_one_line-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: flake8-fill-one-line
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Flake8 plugin to ensure an expression can be written in one line without exceeding the maximum length limit
 Home-page: https://github.com/dronperminov/flake8-fill-one-line
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Requires-Dist: flake8>=3.7
+Requires-Dist: astunparse>=1.6
 
 ====================
 flake8-fill-one-line
 ====================
 
 A Flake8 plugin to ensure an expression can be written in one line without exceeding the maximum length (``160`` characters by default) limit.
```

### Comparing `flake8-fill-one-line-0.4.0/README.rst` & `flake8_fill_one_line-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/call_analyzer.py` & `flake8_fill_one_line-0.4.1/flake8_fill_one_line/analyzers/call_analyzer.py`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/def_analyzer.py` & `flake8_fill_one_line-0.4.1/flake8_fill_one_line/analyzers/def_analyzer.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,26 +10,40 @@
         args_lengths = []
         end_line = node.lineno
 
         for arg in node.args.args:
             args_lengths.append(get_node_length(arg))
             end_line = max(end_line, arg.end_lineno)
 
+        if node.args.kwonlyargs:
+            length += 3  # ", *"
+
+        for arg in node.args.kwonlyargs:
+            args_lengths.append(get_node_length(arg))
+            end_line = max(end_line, arg.end_lineno)
+
         if node.args.vararg is not None:
             args_lengths.append(get_node_length(node.args.vararg) + 1)  # *vararg
             end_line = max(end_line, node.args.vararg.end_lineno)
 
         if node.args.kwarg is not None:
             args_lengths.append(get_node_length(node.args.kwarg) + 2)  # **kvarg
             end_line = max(end_line, node.args.kwarg.end_lineno)
 
         length += sum(args_lengths) + (len(args_lengths) - 1) * 2
 
         for i, default in enumerate(node.args.defaults):
-            offset = 1 if node.args.args[-(i + 1)].annotation is None else 3
+            offset = 1 if node.args.args[i].annotation is None else 3
+            length += default.end_col_offset - default.col_offset + offset
+
+        for i, default in enumerate(node.args.kw_defaults):
+            if default is None:
+                continue
+
+            offset = 1 if node.args.kwonlyargs[i].annotation is None else 3
             length += default.end_col_offset - default.col_offset + offset
 
         if node.returns is not None:
             length += get_node_length(node.returns) + 4  # " -> "
             end_line = max(end_line, node.returns.end_lineno)
 
         if end_line == node.lineno:
```

### Comparing `flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/import_analyzer.py` & `flake8_fill_one_line-0.4.1/flake8_fill_one_line/analyzers/import_analyzer.py`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.4.0/flake8_fill_one_line/analyzers/with_analyzer.py` & `flake8_fill_one_line-0.4.1/flake8_fill_one_line/analyzers/with_analyzer.py`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.4.0/flake8_fill_one_line/check.py` & `flake8_fill_one_line-0.4.1/flake8_fill_one_line/check.py`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.4.0/flake8_fill_one_line/utils.py` & `flake8_fill_one_line-0.4.1/flake8_fill_one_line/utils.py`

 * *Files identical despite different names*

### Comparing `flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/PKG-INFO` & `flake8_fill_one_line-0.4.1/flake8_fill_one_line.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: flake8-fill-one-line
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Flake8 plugin to ensure an expression can be written in one line without exceeding the maximum length limit
 Home-page: https://github.com/dronperminov/flake8-fill-one-line
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Requires-Dist: flake8>=3.7
+Requires-Dist: astunparse>=1.6
 
 ====================
 flake8-fill-one-line
 ====================
 
 A Flake8 plugin to ensure an expression can be written in one line without exceeding the maximum length (``160`` characters by default) limit.
```

### Comparing `flake8-fill-one-line-0.4.0/flake8_fill_one_line.egg-info/SOURCES.txt` & `flake8_fill_one_line-0.4.1/flake8_fill_one_line.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 flake8_fill_one_line.egg-info/requires.txt
 flake8_fill_one_line.egg-info/top_level.txt
 flake8_fill_one_line/analyzers/call_analyzer.py
 flake8_fill_one_line/analyzers/def_analyzer.py
 flake8_fill_one_line/analyzers/if_analyzer.py
 flake8_fill_one_line/analyzers/if_exp_analyzer.py
 flake8_fill_one_line/analyzers/import_analyzer.py
-flake8_fill_one_line/analyzers/with_analyzer.py
+flake8_fill_one_line/analyzers/with_analyzer.py
+tests/test_flake8_fill_one_line.py
```

### Comparing `flake8-fill-one-line-0.4.0/setup.cfg` & `flake8_fill_one_line-0.4.1/setup.cfg`

 * *Files identical despite different names*

