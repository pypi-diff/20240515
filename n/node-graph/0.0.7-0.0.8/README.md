# Comparing `tmp/node_graph-0.0.7.tar.gz` & `tmp/node_graph-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "node_graph-0.0.7.tar", last modified: Sat May  4 08:37:54 2024, max compression
+gzip compressed data, was "node_graph-0.0.8.tar", last modified: Wed May 15 05:39:10 2024, max compression
```

## Comparing `node_graph-0.0.7.tar` & `node_graph-0.0.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.311802 node_graph-0.0.7/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1064 2023-12-03 08:36:19.000000 node_graph-0.0.7/LICENSE
--rw-r--r--   0 xing      (1000) xing      (1000)     1468 2024-05-04 08:37:54.311802 node_graph-0.0.7/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     1027 2024-04-22 09:09:57.000000 node_graph-0.0.7/README.md
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.307802 node_graph-0.0.7/node_graph/
--rw-rw-r--   0 xing      (1000) xing      (1000)       34 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    13105 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/analysis.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    13072 2024-04-26 12:04:23.000000 node_graph-0.0.7/node_graph/collection.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    10339 2024-05-04 08:37:08.000000 node_graph-0.0.7/node_graph/decorator.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3473 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/link.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    18403 2024-04-22 09:09:57.000000 node_graph-0.0.7/node_graph/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11430 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/node_graph.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.307802 node_graph-0.0.7/node_graph/nodes/
--rw-rw-r--   0 xing      (1000) xing      (1000)       85 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/nodes/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4600 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/nodes/test_nodes.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.307802 node_graph-0.0.7/node_graph/properties/
--rw-rw-r--   0 xing      (1000) xing      (1000)       93 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/properties/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11956 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/properties/builtin.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3331 2024-04-22 09:09:57.000000 node_graph-0.0.7/node_graph/property.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1541 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/serializer.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4066 2024-04-15 12:06:25.000000 node_graph-0.0.7/node_graph/socket.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.307802 node_graph-0.0.7/node_graph/sockets/
--rw-rw-r--   0 xing      (1000) xing      (1000)       89 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/sockets/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3332 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/sockets/builtin.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2550 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/utils.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      103 2023-12-03 08:36:19.000000 node_graph-0.0.7/node_graph/version.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.307802 node_graph-0.0.7/node_graph.egg-info/
--rw-r--r--   0 xing      (1000) xing      (1000)     1468 2024-05-04 08:37:54.000000 node_graph-0.0.7/node_graph.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)      889 2024-05-04 08:37:54.000000 node_graph-0.0.7/node_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-05-04 08:37:54.000000 node_graph-0.0.7/node_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      212 2024-05-04 08:37:54.000000 node_graph-0.0.7/node_graph.egg-info/entry_points.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       50 2024-05-04 08:37:54.000000 node_graph-0.0.7/node_graph.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       11 2024-05-04 08:37:54.000000 node_graph-0.0.7/node_graph.egg-info/top_level.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-05-04 08:37:54.311802 node_graph-0.0.7/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)     1361 2024-05-04 08:37:17.000000 node_graph-0.0.7/setup.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-04 08:37:54.307802 node_graph-0.0.7/tests/
--rw-rw-r--   0 xing      (1000) xing      (1000)      597 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_collection.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2231 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_decorator.py
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_entry_point.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      632 2024-04-15 12:06:25.000000 node_graph-0.0.7/tests/test_hooks.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1731 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      616 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2506 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_property.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2152 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_socket.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      378 2023-12-03 08:36:19.000000 node_graph-0.0.7/tests/test_yaml.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1064 2023-12-03 08:36:19.000000 node_graph-0.0.8/LICENSE
+-rw-r--r--   0 xing      (1000) xing      (1000)     1572 2024-05-15 05:39:10.672942 node_graph-0.0.8/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1131 2024-05-15 05:38:38.000000 node_graph-0.0.8/README.md
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/node_graph/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       34 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    13105 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/analysis.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    13072 2024-04-26 12:04:23.000000 node_graph-0.0.8/node_graph/collection.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    10230 2024-05-15 05:38:38.000000 node_graph-0.0.8/node_graph/decorator.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3473 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/link.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    18403 2024-04-22 09:09:57.000000 node_graph-0.0.8/node_graph/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11430 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/node_graph.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/node_graph/nodes/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       85 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/nodes/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4600 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/nodes/test_nodes.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/node_graph/properties/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       93 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/properties/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11956 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/properties/builtin.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3331 2024-04-22 09:09:57.000000 node_graph-0.0.8/node_graph/property.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1541 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/serializer.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4066 2024-04-15 12:06:25.000000 node_graph-0.0.8/node_graph/socket.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/node_graph/sockets/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       89 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/sockets/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3332 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/sockets/builtin.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2550 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/utils.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      103 2023-12-03 08:36:19.000000 node_graph-0.0.8/node_graph/version.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/node_graph.egg-info/
+-rw-r--r--   0 xing      (1000) xing      (1000)     1572 2024-05-15 05:39:10.000000 node_graph-0.0.8/node_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)      889 2024-05-15 05:39:10.000000 node_graph-0.0.8/node_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-05-15 05:39:10.000000 node_graph-0.0.8/node_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      212 2024-05-15 05:39:10.000000 node_graph-0.0.8/node_graph.egg-info/entry_points.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       50 2024-05-15 05:39:10.000000 node_graph-0.0.8/node_graph.egg-info/requires.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       11 2024-05-15 05:39:10.000000 node_graph-0.0.8/node_graph.egg-info/top_level.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-05-15 05:39:10.672942 node_graph-0.0.8/setup.cfg
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1361 2024-05-15 05:38:55.000000 node_graph-0.0.8/setup.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-05-15 05:39:10.672942 node_graph-0.0.8/tests/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      597 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_collection.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2465 2024-05-15 05:38:38.000000 node_graph-0.0.8/tests/test_decorator.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_entry_point.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      632 2024-04-15 12:06:25.000000 node_graph-0.0.8/tests/test_hooks.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1731 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      616 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2506 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_property.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2152 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_socket.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      378 2023-12-03 08:36:19.000000 node_graph-0.0.8/tests/test_yaml.py
```

### Comparing `node_graph-0.0.7/LICENSE` & `node_graph-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/PKG-INFO` & `node_graph-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: node_graph
-Version: 0.0.7
+Version: 0.0.8
 Summary: Create node-based workflow
 Home-page: https://github.com/scinode/node-graph
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -14,15 +14,16 @@
 Requires-Dist: pyyaml
 Requires-Dist: colorama
 Requires-Dist: termcolor
 Requires-Dist: cloudpickle
 
 # NodeGraph
 [![PyPI version](https://badge.fury.io/py/node-graph.svg)](https://badge.fury.io/py/node-graph)
-[![Unit test](https://github.com/scinode/node-graph/actions/workflows/unit_test.yaml/badge.svg)](https://github.com/scinode/node-graph/actions/workflows/unit_test.yaml)
+[![CI](https://github.com/scinode/node-graph/actions/workflows/ci.yaml/badge.svg)](https://github.com/scinode/node-graph/actions/workflows/ci.yaml)
+[![codecov](https://codecov.io/gh/scinode/node-graph/branch/main/graph/badge.svg)](https://codecov.io/gh/scinode/node-graph)
 [![Docs status](https://readthedocs.org/projects/node-graph/badge)](http://node-graph.readthedocs.io/)
 
 
 
 A platform for designing node-based workflows.
```

### Comparing `node_graph-0.0.7/README.md` & `node_graph-0.0.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # NodeGraph
 [![PyPI version](https://badge.fury.io/py/node-graph.svg)](https://badge.fury.io/py/node-graph)
-[![Unit test](https://github.com/scinode/node-graph/actions/workflows/unit_test.yaml/badge.svg)](https://github.com/scinode/node-graph/actions/workflows/unit_test.yaml)
+[![CI](https://github.com/scinode/node-graph/actions/workflows/ci.yaml/badge.svg)](https://github.com/scinode/node-graph/actions/workflows/ci.yaml)
+[![codecov](https://codecov.io/gh/scinode/node-graph/branch/main/graph/badge.svg)](https://codecov.io/gh/scinode/node-graph)
 [![Docs status](https://readthedocs.org/projects/node-graph/badge)](http://node-graph.readthedocs.io/)
 
 
 
 A platform for designing node-based workflows.
```

### Comparing `node_graph-0.0.7/node_graph/analysis.py` & `node_graph-0.0.8/node_graph/analysis.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/node_graph/collection.py` & `node_graph-0.0.8/node_graph/collection.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/node_graph/decorator.py` & `node_graph-0.0.8/node_graph/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,27 +23,24 @@
     # Iterate over the parameters
     args = []
     kwargs = {}
     var_args = None
     var_kwargs = None
     for name, parameter in parameters.items():
         if parameter.kind == inspect.Parameter.POSITIONAL_ONLY:
-            if parameter.annotation is not inspect.Parameter.empty:
-                arg = [name, parameter.annotation]
-            else:
-                arg = [name, None]
+            arg = [name, parameter.annotation]
             args.append(arg)
         elif parameter.kind == inspect.Parameter.POSITIONAL_OR_KEYWORD:
             if parameter.default is not inspect.Parameter.empty:
                 kwargs[name] = {
                     "type": parameter.annotation,
                     "default": parameter.default,
                 }
             else:
-                args.append([name, None])
+                args.append([name, parameter.annotation])
         elif parameter.kind == inspect.Parameter.VAR_POSITIONAL:
             var_args = name
         elif parameter.kind == inspect.Parameter.VAR_KEYWORD:
             var_kwargs = name
 
     return args, kwargs, var_args, var_kwargs
```

### Comparing `node_graph-0.0.7/node_graph/link.py` & `node_graph-0.0.8/node_graph/link.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/node_graph/node.py` & `node_graph-0.0.8/node_graph/node.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/node_graph/node_graph.py` & `node_graph-0.0.8/node_graph/node_graph.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/node_graph/nodes/test_nodes.py` & `node_graph-0.0.8/node_graph/nodes/test_nodes.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/node_graph/properties/builtin.py` & `node_graph-0.0.8/node_graph/properties/builtin.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/node_graph/property.py` & `node_graph-0.0.8/node_graph/property.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/node_graph/serializer.py` & `node_graph-0.0.8/node_graph/serializer.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/node_graph/socket.py` & `node_graph-0.0.8/node_graph/socket.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/node_graph/sockets/builtin.py` & `node_graph-0.0.8/node_graph/sockets/builtin.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/node_graph/utils.py` & `node_graph-0.0.8/node_graph/utils.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/node_graph.egg-info/PKG-INFO` & `node_graph-0.0.8/node_graph.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: node_graph
-Version: 0.0.7
+Version: 0.0.8
 Summary: Create node-based workflow
 Home-page: https://github.com/scinode/node-graph
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -14,15 +14,16 @@
 Requires-Dist: pyyaml
 Requires-Dist: colorama
 Requires-Dist: termcolor
 Requires-Dist: cloudpickle
 
 # NodeGraph
 [![PyPI version](https://badge.fury.io/py/node-graph.svg)](https://badge.fury.io/py/node-graph)
-[![Unit test](https://github.com/scinode/node-graph/actions/workflows/unit_test.yaml/badge.svg)](https://github.com/scinode/node-graph/actions/workflows/unit_test.yaml)
+[![CI](https://github.com/scinode/node-graph/actions/workflows/ci.yaml/badge.svg)](https://github.com/scinode/node-graph/actions/workflows/ci.yaml)
+[![codecov](https://codecov.io/gh/scinode/node-graph/branch/main/graph/badge.svg)](https://codecov.io/gh/scinode/node-graph)
 [![Docs status](https://readthedocs.org/projects/node-graph/badge)](http://node-graph.readthedocs.io/)
 
 
 
 A platform for designing node-based workflows.
```

### Comparing `node_graph-0.0.7/node_graph.egg-info/SOURCES.txt` & `node_graph-0.0.8/node_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/setup.py` & `node_graph-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="node_graph",
-    version="0.0.7",
+    version="0.0.8",
     description="Create node-based workflow",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/scinode/node-graph",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="MIT License",
```

### Comparing `node_graph-0.0.7/tests/test_collection.py` & `node_graph-0.0.8/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/tests/test_decorator.py` & `node_graph-0.0.8/tests/test_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     "properties": [["Float", "x", {"default": 3}]],
     "inputs": [["Float", "y", {"property": ["Float", {"default": 10}]}]],
     "outputs": [["General", "result"]],
     "executor": {"path": "numpy.add"},
 }
 MyNumpyAdd = create_node(ndata)
 
-
 def create_test_node_group():
     nt = NodeGraph()
     add1 = nt.nodes.new("TestAdd", "add1")
     add2 = nt.nodes.new("TestAdd", "add2")
     add3 = nt.nodes.new("TestAdd", "add3")
     nt.links.new(add1.outputs[0], add3.inputs[0])
     nt.links.new(add2.outputs[0], add3.inputs[1])
@@ -31,14 +30,21 @@
 MyTestAddGroup = create_node_group(
     {
         "identifier": "MyTestAddGroup",
         "nt": create_test_node_group(),
     }
 )
 
+def test_socket(decorated_myadd):
+    """Test simple math."""
+    n = decorated_myadd.node()
+    assert n.inputs["x"].identifier == "Float"
+    assert n.inputs["y"].identifier == "Float"
+    assert n.inputs["t"].property.default == 1
+
 
 def test_create_node():
     """Build node on-the-fly."""
 
     nt = NodeGraph(name="test_create_node")
     nt.nodes.new(MyNumpyAdd, "add1")
     assert len(nt.nodes) == 1
```

### Comparing `node_graph-0.0.7/tests/test_hooks.py` & `node_graph-0.0.8/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/tests/test_node.py` & `node_graph-0.0.8/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/tests/test_nodetree.py` & `node_graph-0.0.8/tests/test_nodetree.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/tests/test_property.py` & `node_graph-0.0.8/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.7/tests/test_socket.py` & `node_graph-0.0.8/tests/test_socket.py`

 * *Files identical despite different names*

