# Comparing `tmp/visualgo-2024.5.13.tar.gz` & `tmp/visualgo-2024.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visualgo-2024.5.13.tar", last modified: Mon May 13 20:19:07 2024, max compression
+gzip compressed data, was "visualgo-2024.5.15.tar", last modified: Wed May 15 06:02:09 2024, max compression
```

## Comparing `visualgo-2024.5.13.tar` & `visualgo-2024.5.15.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.530128 visualgo-2024.5.13/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 20:19:01.000000 visualgo-2024.5.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 20:19:01.000000 visualgo-2024.5.13/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-13 20:19:07.530128 visualgo-2024.5.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-13 20:19:01.000000 visualgo-2024.5.13/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-13 20:19:01.000000 visualgo-2024.5.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:19:07.530128 visualgo-2024.5.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-13 20:19:01.000000 visualgo-2024.5.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.518128 visualgo-2024.5.13/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.522128 visualgo-2024.5.13/src/visualgo/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.522128 visualgo-2024.5.13/src/visualgo/logic/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24875 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/controller_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.522128 visualgo-2024.5.13/src/visualgo/logic/debugger/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.522128 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/bdb_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.522128 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_api/from_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_api/to_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.526128 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_impl/python_process_from_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_impl/python_process_to_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/py_debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/debugger/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.526128 visualgo-2024.5.13/src/visualgo/logic/static/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/static/static_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/static/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.526128 visualgo-2024.5.13/src/visualgo/logic/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/ui/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/logic/ui/ui_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.526128 visualgo-2024.5.13/src/visualgo/structures/
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/BinaryTreeNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/BinaryTreeNodeBack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/DoublyLinkedList.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/LinkedList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/List.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/Tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/TreeNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/TwoWayNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-13 20:19:01.000000 visualgo-2024.5.13/src/visualgo/structures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:19:07.530128 visualgo-2024.5.13/src/visualgo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-13 20:19:07.000000 visualgo-2024.5.13/src/visualgo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-13 20:19:07.000000 visualgo-2024.5.13/src/visualgo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:19:07.000000 visualgo-2024.5.13/src/visualgo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 20:19:07.000000 visualgo-2024.5.13/src/visualgo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 20:19:07.000000 visualgo-2024.5.13/src/visualgo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.363858 visualgo-2024.5.15/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 06:02:01.000000 visualgo-2024.5.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 06:02:01.000000 visualgo-2024.5.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-15 06:02:09.363858 visualgo-2024.5.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-15 06:02:01.000000 visualgo-2024.5.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-15 06:02:01.000000 visualgo-2024.5.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:02:09.363858 visualgo-2024.5.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 06:02:01.000000 visualgo-2024.5.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.351858 visualgo-2024.5.15/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.355858 visualgo-2024.5.15/src/visualgo/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.355858 visualgo-2024.5.15/src/visualgo/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25627 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/controller_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.355858 visualgo-2024.5.15/src/visualgo/logic/debugger/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.355858 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/bdb_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.359858 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_api/from_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_api/to_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.359858 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_impl/python_process_from_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_impl/python_process_to_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/py_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/debugger/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.359858 visualgo-2024.5.15/src/visualgo/logic/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/static/static_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/static/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.359858 visualgo-2024.5.15/src/visualgo/logic/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/ui/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/logic/ui/ui_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.363858 visualgo-2024.5.15/src/visualgo/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/BinaryTreeNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/BinaryTreeNodeBack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/DoublyLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/LinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/List.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/Tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/TreeNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/TwoWayNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-15 06:02:01.000000 visualgo-2024.5.15/src/visualgo/structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:02:09.363858 visualgo-2024.5.15/src/visualgo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-15 06:02:09.000000 visualgo-2024.5.15/src/visualgo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-15 06:02:09.000000 visualgo-2024.5.15/src/visualgo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:02:09.000000 visualgo-2024.5.15/src/visualgo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 06:02:09.000000 visualgo-2024.5.15/src/visualgo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 06:02:09.000000 visualgo-2024.5.15/src/visualgo.egg-info/top_level.txt
```

### Comparing `visualgo-2024.5.13/LICENSE` & `visualgo-2024.5.15/LICENSE`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.13/PKG-INFO` & `visualgo-2024.5.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualgo
-Version: 2024.5.13
+Version: 2024.5.15
 Summary: Enjoy classic datatypes and debug user python code
 Author: PFA-Visualgo
 License: MIT License
         
         Copyright (c) 2024 PFA-Visualgo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `visualgo-2024.5.13/pyproject.toml` & `visualgo-2024.5.15/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "visualgo"
-version = "2024.5.13"
+version = "2024.5.15"
 description = "Enjoy classic datatypes and debug user python code"
 readme = "README.md"
 authors = [{ name = "PFA-Visualgo" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `visualgo-2024.5.13/src/visualgo/logic/controller.py` & `visualgo-2024.5.15/src/visualgo/logic/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from enum import Enum
 from dataclasses import dataclass
 from abc import ABC, abstractmethod
 from functools import wraps
 import asyncio
-import time
 from typing import Union
 
 from .types import Statistics, SymbolDescription
 from .controller_callbacks import ControllerCallbacksInterface
 
 from .debugger.types import DebugContext, DebugVariables
 from .debugger.debugger import AbstractDebugger
 
-from .static.types import CodeVariablesAndUserFunctions, StaticSymbolDescription, StaticBasicDescription
+from .static.types import CodeVariablesAndUserFunctions, StaticSymbolDescription
 from .static.static_analysis import StaticAnalyser
 
 from .ui.types import TransferVariable, TransferVariables
 from .ui.ui_callbacks import UICallbacksInterface
 
 
 @dataclass
@@ -167,29 +166,31 @@
 
         :param line_number: int
         :return: None
         """
         pass
 
     @abstractmethod
-    def new_tracker(self, line_number: int) -> None:
+    def new_tracker(self, name: str, line_number: int) -> None:
         """
         Add a new tracker at the given `line_number`.
 
-        :param line_number: int
+        :param name: str the name of the tracker
+        :param line_number: int the line where the tracker will be put
         :return: None
         """
         pass
 
     @abstractmethod
-    def del_tracker(self, line_number: int) -> None:
+    def del_tracker(self, name: str, line_number: int) -> None:
         """
         Delete the tracker at the given `line_number`.
 
-        :param line_number: int
+        :param name: str the name of the tracker
+        :param line_number: int the line where the tracker will be deleted
         :return: None
         """
         pass
 
     # Tracking for drawings
     @abstractmethod
     def hide_variable(self, variable: SymbolDescription) -> None:
@@ -326,34 +327,35 @@
         Initializes the debugger with the given `code`.
 
         :param code: str
         :return: None
         """
         self.__debugger.add_breakpoints(self.__breakpoints)
         self.__debugger.add_breakpoints([(lineno, None) for lineno in self.__checkpoints])
+        self.__debugger.add_breakpoints(
+            [(lineno, None) for tracker in self.__trackers.values() for lineno in tracker.lines])
         self.__debugger.set_code(code)
         self.__execution_state = ExecutionState.RUNNING
 
     def __get_ui_stats(self, stats: Statistics) -> Statistics:
         """
         Returns the statistics of the execution given the debugger `stats`
         and the user parameters `tracked_types` and `tracked_funs`.
 
         :demand: F.1.5
         :param stats: Statistics
-        :param tracked_types: list[SymbolDescription]
-        :param tracked_funs: list[SymbolDescription]
         :return: Statistics
         """
         tracked_types = self.__hidden_types
         tracked_funs = self.__tracked_funs
-        pass
+        return Statistics({})  # For now
 
+    # noinspection PyMethodMayBeStatic
     def __transform_in_transfer_vars(
-            self, vars: DebugVariables, function_name: str, depth: int) -> TransferVariables:
+            self, vars: DebugVariables, function_name: str, depth: int) -> list[TransferVariable]:
         """
         Returns the variables of the execution given the `frame`.
 
         :param vars: DebugVariables
         :param function_name: str
         :param depth: int
         :return: TransferVariables
@@ -363,21 +365,20 @@
         for name, value in vars.locals.items():
             desc = SymbolDescription(name, function_name, depth)
             ui_var = TransferVariable(desc, value)
             res.append(ui_var)
         return res
 
     def __get_ui_vars(
-            self, context: DebugContext) -> TransferVariables:
+            self, context: list[DebugContext]) -> TransferVariables:
         """
         Returns the variables of the execution given the debugger
         `variables` and the user parameters `tracked_vars`.
 
         :param context: DebugContext
-        :param tracked_vars: typing.List[SymbolDescription]
         :return: TransferVariables
         """
         hidden_vars = self.__hidden_vars
         hidden_fun_vars = self.__hidden_fun_vars
         res = []
         depth = 0
         # iterate frame by frame
@@ -397,15 +398,15 @@
             if var.description in hidden:
                 res.remove(var)
             elif var.description.name in hidden_fun.name and var.description.depth in hidden_fun.depth:
                 res.remove(var)
 
         return TransferVariables(res)
 
-    def __update_ui(self, context: DebugContext) -> None:
+    def __update_ui(self, context: list[DebugContext]) -> None:
         """
         Updates the UI with the given `context`.
 
         :param context: DebugContext
         :return: None
         """
         vars = self.__get_ui_vars(context)
@@ -485,65 +486,71 @@
         self.__ui_callbacks.set_current_line(current_line_number)
 
         # At every execution stop we update the UI
         self.__update_ui(contexts)
         if self.__execution_state != ExecutionState.RUNNING:
             self.__ui_callbacks.execution_paused()
 
-    def execution_paused(self, context: DebugContext) -> None:
+    def execution_paused(self, context: list[DebugContext]) -> None:
         """
         Update the visualisation once the debugger has finished executing some part of a code
         and is awaiting further instructions.
         Occurs on steps, next and continues.
-        TODO: Update statistics here.
 
         :param context: DebugContext
         :return: None
         """
         # print("in controller execution_paused, line:", context[0].lineno)
 
         line_number = context[0].lineno
+        hasTracker = self.__update_trackers(line_number)  # We always want to update trackers!
         for lineno, _ in self.__breakpoints:
             if line_number == lineno:
                 self.pause()
                 self.__update_full_ui(line_number, context)
-                self.__update_trackers(line_number)  # Update tracker on the same line
                 return
-        if self.__execution_state == ExecutionState.RUNNING_IGNORE_CHECKPOINTS:
-            for lineno in self.__checkpoints:
-                if line_number == lineno:
-                    self.__update_trackers(line_number)  # Update tracker on the same line
-                    self.do_continue()
-                    return
-        if self.__update_trackers(line_number):  # No breakpoint here, but we still check if there's a tracker
+        # Breakpoints have been checked for. From this line on, we know there's no breakpoint at this line
+        hasCheckpoint = False
+        for lineno in self.__checkpoints:
+            if line_number == lineno:
+                hasCheckpoint = True
+                break
+        if self.__execution_state == ExecutionState.RUNNING_IGNORE_CHECKPOINTS and hasCheckpoint:
+            # We're supposed to ignore checkpoints but we were called on a checkpoint. GET OUT
+            self.do_continue()
+            return
+        if hasTracker:
             if self.__execution_state == ExecutionState.RUNNING_IGNORE_CHECKPOINTS:
+                # If we stopped on a tracker, but we're running w/o checkpoints, then just continue till next cp/tp/bp
                 self.do_continue()
                 return
-            if self.__autoplay:
-                if len(self.__checkpoints) == 0 and len(self.__breakpoints) == 0:
-                    self.forward_step()
-                else:
-                    self.__debugger.do_continue()
+            if self.__autoplay and not hasCheckpoint and (len(self.__checkpoints) > 0 or len(self.__breakpoints) > 0):
+                # If we're on autoplay, on a tracker but not on a checkpoint, but we need to only stop at checkpoints,
+                # then make the debugger instantly continue w/o updating UI. Otherwise then we're supposed to stop
+                # here
+                self.__debugger.do_continue()
                 return
+        # If we're here, we're supposed to update UI, yay :D
         # print("No trackers nor breakpoints nor ignored checkpoints found")
         self.__update_full_ui(line_number, context)
         if self.__autoplay:
             asyncio.create_task(self.__call_debugger_later())
 
-    def execution_done(self, context: DebugContext) -> None:
+    def execution_done(self, context: list[DebugContext]) -> None:
         # print("in execution_done")
         line_number = context[0].lineno
         self.__update_ui(context)
         self.__ui_callbacks.set_current_line(line_number)  # Could be 0 too
         self.__ui_callbacks.code_is_over()
         self.__execution_state = ExecutionState.CODE_NOT_INITIALIZED
         self.__autoplay = False
 
-    def on_error(self, error: str) -> None:
-        self.__execution_state = ExecutionState.WAITING_DEBUGGER_INITIALIZATION
+    def on_error(self, error: BaseException) -> None:
+        self.__ui_callbacks.code_is_over()
+        self.__execution_state = ExecutionState.CODE_NOT_INITIALIZED
         self.__ui_callbacks.show_error(error)
 
     def on_message(self, message: str) -> None:
         self.__ui_callbacks.show_message(message)
 
     def on_initialized(self) -> None:
         self.__execution_state = ExecutionState.CODE_NOT_INITIALIZED
@@ -561,15 +568,15 @@
         # print("initialize")
         if self.__execution_state == ExecutionState.CODE_NOT_INITIALIZED:
             code = self.__ui_callbacks.get_code()
             self.__initialize_debugger(code)
             self.__reset_trackers()
             self.__execution_state = ExecutionState.PAUSED
         # else:
-            # print("Did nothing in initialize")
+        # print("Did nothing in initialize")
 
     async def step_forward_automatic(self) -> None:
         # print("step_forward_automatic")
         if self.__execution_state == ExecutionState.PAUSED:
 
             self.__recursion_depth = 0
             self.__execution_state = ExecutionState.RUNNING
@@ -603,15 +610,15 @@
         """
         self.__autoplay = False
         self.__debugger.stop()
         self.__execution_state = ExecutionState.WAITING_DEBUGGER_INITIALIZATION
 
     def set_step_time(self, time: int) -> None:
         if time <= 0:
-            self.__ui_callbacks.show_error("Time must be greater than 0")
+            self.__ui_callbacks.show_error(Exception("Time must be greater than 0"))
         else:
             self.__step_time = time
 
     @needs_initialization
     def forward_step(self) -> None:
         self.__ui_callbacks.set_running_code()
         self.__debugger.forward_step()
@@ -665,15 +672,15 @@
         self.__debugger.add_breakpoints([(line_number, None)])
         if name in self.__trackers:
             self.__trackers[name].lines.append(line_number)
         else:
             self.__trackers[name] = Tracker(0, [line_number])
 
     def del_tracker(self, name: str, line_number: int) -> None:
-        self.__debugger.del_breakpoints(line_number)
+        self.__debugger.del_breakpoints([line_number])
         if name in self.__trackers.keys():
             self.__trackers[name].lines.remove(line_number)
             if len(self.__trackers[name].lines) == 0:
                 del self.__trackers[name]
 
     # Tracking for drawings
     def hide_variable(self, variable: SymbolDescription) -> None:
@@ -709,15 +716,15 @@
             if fun.description in self.__hidden_fun_vars:
                 fun_state = False
             new_funcs.append(StaticSymbolDescription(fun.description, fun_state))
 
         self.__ui_callbacks.set_static_variables_and_user_fun(CodeVariablesAndUserFunctions(new_vars, new_funcs))
 
     # Statistics
-    def get_csv(self) -> str:
+    def get_csv(self) -> dict[str, Tracker]:
         return self.__trackers
 
     # -- Other public methods -- #
 
     @property
     def recursion_depth(self) -> int:
         return self.__recursion_depth
```

### Comparing `visualgo-2024.5.13/src/visualgo/logic/controller_callbacks.py` & `visualgo-2024.5.15/src/visualgo/logic/controller_callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 from abc import ABC, abstractmethod
 
 from .debugger.types import DebugContext
 
+
 class ControllerCallbacksInterface(ABC):
     """
     Interface so that the debugger can call when it has finished an action asked by the controller.
     """
 
     @abstractmethod
-    def execution_paused(self, frames: DebugContext) -> None:
+    def execution_paused(self, frames: list[DebugContext]) -> None:
         """
         Update the visualisation once the debugger has finished executing code and is awaiting
         further instructions. Occurs on steps, next and continues.
-        :param context:
+        :param frames: list[DebugContext] the stack of debug frames.
         :return:
         """
         ...
 
     @abstractmethod
-    def execution_done(self, frames: DebugContext) -> None:
+    def execution_done(self, frames: list[DebugContext]) -> None:
         """
         Update the visualisation once the end of the code has been reached in the debugger.
 
-        :param context: DebugContext
+        :param frames: list[DebugContext] the stack of debug frames.
         :return: None
         """
         pass
 
     @abstractmethod
-    def on_error(self, error: str) -> None:
+    def on_error(self, error: BaseException) -> None:
         """
         Show an error in the visualisation when the debugged code throws an un-caught exception
 
-        :param error: str
+        :param error: BaseException
         :return: None
         """
         pass
 
     @abstractmethod
     def on_message(self, message: str) -> None:
         """
@@ -48,21 +49,20 @@
         pass
 
     @abstractmethod
     def on_initialized(self) -> None:
         """
         Tell the controller that the debugger has been initialized and is ready to receive the code.
 
-        :param message: str
         :return: None
         """
         pass
 
     @abstractmethod
     def on_interrupted(self) -> None:
         """
         Tell the controller that the debugger has been interrupted and is no longer running.
         It needs to be re-initialized before it can be used again.
 
         :return: None
         """
-        pass
+        pass
```

### Comparing `visualgo-2024.5.13/src/visualgo/logic/debugger/__private/bdb_layer.py` & `visualgo-2024.5.15/src/visualgo/logic/debugger/__private/bdb_layer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import bdb
-import linecache
 import re
 import sys
 from pkgutil import iter_modules
 from sys import stderr
 from types import FrameType
-from typing import Any
 
 from ..types import DebugContext
 from .comm_api import from_worker
 
 _FILE_NAME = "__visualgo_code.py"
 
 _MESSAGE_QUEUE = []
@@ -35,19 +33,21 @@
 
 
 def _run_bdb_task():
     from_worker.get_implementation().send_message("INITIALIZED", None)
     # print("BDB initialized, waiting for SET_CODE message")
     code = ""
     dbg = BdbLayer()
+    CANONIC_FILE_NAME = dbg.canonic(_FILE_NAME)
     while True:
         breakpoints = []
-        # print("debugger has been reset")
         dbg.reset()
         dbg.reset_internal()
+        dbg.clear_all_file_breaks(CANONIC_FILE_NAME)
+        # print("debugger has been reset")
         while True:
             mes_queue = from_worker.get_implementation().wait_for_main_messages()
             _append_to_message_queue(mes_queue)
             contains_code = False
             while not _is_message_queue_empty():  # This time, just consume all the message queue...
                 # print(_MESSAGE_QUEUE)
                 mes_id, mes_data = _pop_first_message()
@@ -64,34 +64,42 @@
                     # print("after :", breakpoints)
                 if mes_id == "CONT":
                     # _append_to_message_queue([(mes_id, mes_data)])
                     dbg.set_continue()
                     break
             if contains_code:
                 break
-        CANONIC_FILE_NAME = dbg.canonic(_FILE_NAME)
         with open(CANONIC_FILE_NAME, "w") as f:
             f.write(code)
             f.flush()
+            import linecache
+            linecache.checkcache(CANONIC_FILE_NAME)  # Force update cache to reflect changes to file.
             try:
                 cmd = compile(code, CANONIC_FILE_NAME, "exec")
                 dbg.set_source(code)
-                # print("bdb_layer: set code")
-                dbg.set_break(CANONIC_FILE_NAME, len(dbg.lines))
+                # print(f"bdb_layer: set code '{code}'")
+                # print("Setting breakpoint...")
+                # noinspection PyNoneFunctionAssignment
+                err_code = dbg.set_break(CANONIC_FILE_NAME, len(dbg.code_running))
+                if err_code is not None:
+                    print(err_code)
+                    exit(1)  # kms. However, this should never happen :)
                 # print(breakpoints)
                 dbg.do_add_breakpoints(breakpoints)
                 # print("bdb_layer: running code")
                 dbg.run(cmd)
                 # print("bdb_layer: Code ran")
             except SyntaxError as e:
-                print("Invalid code.")
+                print("Invalid code.", file=sys.stderr)
+                from_worker.get_implementation().send_message("EXEC_THROWED", (e, []))
 
 
 def _should_skip_frame(frame: FrameType):
     globs = frame.f_globals if frame else None
+    import linecache
     cur_line = linecache.getline(_FILE_NAME, frame.f_lineno, globs).strip()
     if (_ANNOTATION_REGEX.fullmatch(cur_line)
             or _FUNCTION_DEFINITION_REGEX.fullmatch(cur_line)
             or _IMPORT_NAME_REGEX.fullmatch(cur_line)
             or _IMPORT_FROM_REGEX.fullmatch(cur_line)):
         return True
     return False
@@ -99,30 +107,32 @@
 
 class BdbLayer(bdb.Bdb):
     def __init__(self, skip=None):
         # super().__init__(["visualgo.*", "importlib", "importlib.*", "zipimport", "typing"])
         self.continue_state = False
         modules_to_skip = {x.name for x in iter_modules()}
         modules_to_skip.update({x.name + ".*" for x in iter_modules()})
+        if skip is not None:
+            modules_to_skip.update(skip)
         # print("SKIP:", modules_to_skip)
         super().__init__(modules_to_skip)
         self.curframe = None
-        self.lines = None
+        self.code_running = None
         self.actions = {
             "SET_CODE": self.do_set_code,
             "CONT": self.do_continue,
             "ADD_BP": self.do_add_breakpoints,
             "DEL_BP": self.do_del_breakpoints,
             "FW_S": self.do_forward_step,
             "BW_S": self.do_backwards_step,
             "FW_N": self.do_forward_next
         }
 
     def reset_internal(self):  # Have to do this stupid thing because self.reset() is called whenever run() is called :)
-        self.lines = None
+        self.code_running = None
         self.curframe = None
         self.continue_state = False
 
     def set_continue(self):
         self.continue_state = True
         super().set_continue()
 
@@ -134,41 +144,41 @@
         :returns: the continue state before being consumed.
         """
         prev = self.continue_state
         self.continue_state = False
         return prev
 
     def do_add_breakpoints(self, data):
-        global _FILE_NAME
         for lineno, cond in data:
             # print("bdb_layer: Adding breakpoint at line", lineno)
             self.set_break(self.canonic(_FILE_NAME), lineno, cond=cond)
             # print("bdb_layer: Breakpoint added at line", lineno)
         return False
 
     def do_del_breakpoints(self, data):
-        global _FILE_NAME
         for lineno in data:
             # print("bdb_layer: Removing breakpoint at line", lineno)
             self.clear_break(self.canonic(_FILE_NAME), lineno)
             # print("bdb_layer: Removed breakpoint at line", lineno)
         return False
 
     def do_forward_step(self, data):
         self.set_step()
         return True
 
+    # noinspection PyMethodMayBeStatic
     def do_backwards_step(self, data):
         print("Call to backwards step. It is NOT implemented!", file=stderr)
         return True
 
     def do_forward_next(self, data):
         self.set_next(self.curframe)
         return True
 
+    # noinspection PyMethodMayBeStatic
     def do_set_code(self, data):
         print("Call to set_code. It is NOT implemented!", file=stderr)
         return True
 
     def do_continue(self, data):
         self.set_continue()
         return True
@@ -190,43 +200,45 @@
         if self.get_continue_state() and not self.break_here(frame):
             self.set_continue()
             return
         # print("FRAME MODULE", ctx[0].variables.globals["__name__"])
         # print("DBG CONTEXT GLOBALS:", ctx[0].variables.globals.keys())
         # print("DBG CONTEXT LOCALS:", ctx[0].variables.locals.keys())
         # print("LENGTH DBG CONTEXT:", len(ctx))
-        if frame.f_lineno == len(self.lines):
+
+        if frame.f_lineno == len(self.code_running):
             from_worker.get_implementation().send_message("EXEC_DONE", ctx)
         else:
             from_worker.get_implementation().send_message("EXEC_PAUSED", ctx)
             self._cmdloop()
 
     def user_return(self, frame, return_value):
         pass
 
     def user_call(self, frame, argument_list):
         pass
 
     def user_exception(self, frame, exc_info):
         from_worker.get_implementation().send_message("EXEC_THROWED",
-                                                      (exc_info[0], DebugContext.list_from_frame(frame, self.botframe)))
+                                                      (exc_info[1], DebugContext.list_from_frame(frame, self.botframe)))
 
     def set_source(self, code: str):
-        self.lines = code.split("\n")
+        self.code_running = code.split("\n")
 
     def run(self, cmd, _globals=None, _locals=None):
         import __main__
         __main__.__dict__.clear()
         __main__.__dict__.update({"__name__": "__main__",
                                   "__file__": _FILE_NAME,
                                   "__builtins__": __builtins__,
                                   })
+        # noinspection PyBroadException
         try:
             super().run(cmd, _globals, _locals)
-        except SystemExit as e:
+        except SystemExit:
             pass
         except:
             ex_type, ex, t = sys.exc_info()
             while t.tb_next:
                 t = t.tb_next
             frame = t.tb_frame
             from_worker.get_implementation().send_message("EXEC_THROWED",
```

### Comparing `visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_api/from_worker.py` & `visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_api/from_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Any, Callable
+from typing import Any
 
 
 class FromWorker(ABC):
     @abstractmethod
     def send_message(self, mes_id: str, data: Any):
         """
         Send a message to the main program. This will interrupt the main to handle the message as soon as possible
```

### Comparing `visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_api/to_worker.py` & `visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_api/to_worker.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_impl/python_process_from_worker.py` & `visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_impl/python_process_from_worker.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
             try:
                 res.append(self.queue.get_nowait())
                 has_at_least_one = True
             except Empty:
                 if has_at_least_one:
                     return res
                 else:
-                    return [self.queue.get()]
+                    return [self.queue.get()]
```

### Comparing `visualgo-2024.5.13/src/visualgo/logic/debugger/__private/comm_impl/python_process_to_worker.py` & `visualgo-2024.5.15/src/visualgo/logic/debugger/__private/comm_impl/python_process_to_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     """
     An implementation of the communication API for the CPython engine for the main side.
     This will start the worker in another process and use a shared Queue to communicate with it and a simplex Pipe for
     the worker to send messages to us.
 
     This implementation uses the signal `SIGUSR1` so the worker can interrupt us whenever it needs to send us a message.
     """
+
     def __init__(self, task: Callable[[], None], message_handler: Callable[[str, Any], None]):
         self.message_value: [str, Any] = None
         self.task: Callable[[], None] = task
         self.worker_message_queue = Queue()
         self.recv_conn, send_conn = Pipe(False)  # no duplex
         self.worker_process = Process(target=_wrapper_task,
                                       args=(task, self.worker_message_queue, send_conn, os.getpid()))
```

### Comparing `visualgo-2024.5.13/src/visualgo/logic/debugger/debugger.py` & `visualgo-2024.5.15/src/visualgo/logic/debugger/debugger.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 class AbstractDebugger(ABC):
     """
     Interface for the Debugger class.
 
     :call: callbacks.on_initialized() once it is fully initialized.
     :call: callbacks.on_interrupted() when it is fully stopped and don't want to receive any more messages.
     """
+
     @abstractmethod
     def __init__(self, callbacks: ControllerCallbacksInterface) -> None:
         """
         Constructor of the debugger.
         Initializes debugger with the corresponding callbacks
 
         :param callbacks: ControllerCallbacksInterface
@@ -49,15 +50,14 @@
         Or update the condition of the breakpoint at the given `line_number`.
 
         :param breakpoints: list[[int, str]]
         :return: None
         """
         pass
 
-
     @abstractmethod
     def del_breakpoints(self, line_numbers: list[int]) -> None:
         """
         Remove the breakpoint at the given `line_number`.
 
         :param line_numbers: list[int]
         :return: None
```

### Comparing `visualgo-2024.5.13/src/visualgo/logic/debugger/py_debugger.py` & `visualgo-2024.5.15/src/visualgo/logic/debugger/py_debugger.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,13 @@
         to_worker.get_implementation().send_message("DEL_BP", line_numbers)
 
     def backward_step(self) -> None:
         to_worker.get_implementation().send_message("BW_S", None)
 
     def forward_step(self) -> None:
         to_worker.get_implementation().send_message("FW_S", None)
-    
+
     def step_into(self) -> None:
         to_worker.get_implementation().send_message("FW_N", None)
 
     def do_continue(self) -> None:
         to_worker.get_implementation().send_message("CONT", None)
-
```

### Comparing `visualgo-2024.5.13/src/visualgo/logic/debugger/types.py` & `visualgo-2024.5.15/src/visualgo/logic/debugger/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pickle
 from dataclasses import dataclass
 from inspect import isfunction, ismodule
 from types import FrameType
 import re
 from typing import Any
 
 _builtin_pattern = re.compile('__.*__')
@@ -46,15 +45,15 @@
         while cur_frame is not None and cur_frame is not botframe:  # Dirty hack to remove all the nasty bdb clutter
             lst.append(cls(cur_frame))
             cur_frame = cur_frame.f_back
         return lst
 
     def __init__(self, frame: FrameType):
         self.filepath = frame.f_globals["__file__"]
-        self.lineno = frame.f_lineno
+        self.lineno: int = frame.f_lineno
         self.variables = DebugVariables(_remove_unpickable(_remove_builtins(frame.f_globals)),
                                         _remove_unpickable(_remove_builtins(frame.f_locals)))
         self.function_name = frame.f_code.co_name if frame.f_code.co_name else "<lambda>"
 
     def __str__(self):
         return str(self.__dict__)
```

### Comparing `visualgo-2024.5.13/src/visualgo/logic/static/static_analysis.py` & `visualgo-2024.5.15/src/visualgo/logic/static/static_analysis.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 import ast
 from dataclasses import dataclass
 
-from .types import StaticSymbolDescription, StaticSymbolDescription, StaticBasicDescription, CodeVariablesAndUserFunctions
+from .types import StaticSymbolDescription, \
+    CodeVariablesAndUserFunctions
 from ..types import SymbolDescription
 
 import importlib
 
+
 @dataclass
 class StaticAnalysisRes:
     variables_user_functions: CodeVariablesAndUserFunctions
 
+
 class StaticAnalyser:
-    
+
     def __init__(self):
         self._visualgo_types = self._get_structure_types()
 
+    # noinspection PyMethodMayBeStatic
     def _get_structure_types(self):
         try:
             structure_module = importlib.import_module('visualgo.structures')
             structure_types = set()
             for name in dir(structure_module):
                 attr = getattr(structure_module, name)
                 if "class 'visualgo.structures." in str(attr):
                     structure_types.add(name)
             return structure_types
         except ImportError:
             print("Error: Could not import visualgo.structures module")
             return set()
-    
+
+    # noinspection PyMethodMayBeStatic
     def __analyse_code_types(self, code: str) -> StaticAnalysisRes:
         tree = ast.parse(code)
 
         variables = []
         functions = []
 
-
         def traverse(node, level=-1, current_function='<module>'):
             if isinstance(node, ast.Assign):
                 for target in node.targets:
                     if isinstance(target, ast.Name):
-                        variables.append(StaticSymbolDescription(SymbolDescription(target.id, current_function, level), True))
+                        variables.append(
+                            StaticSymbolDescription(SymbolDescription(target.id, current_function, level), True))
             elif isinstance(node, ast.FunctionDef):
                 functions.append(StaticSymbolDescription(SymbolDescription(node.name, node.name, level), True))
                 current_function = node.name  # Update current function name
 
             for child_node in ast.iter_child_nodes(node):
                 traverse(child_node, level + 1, current_function)  # Pass current function name
 
         traverse(tree)
 
-
         user_functions = [f for f in functions]
 
         return StaticAnalysisRes(CodeVariablesAndUserFunctions(variables, user_functions))
 
     def get_code_variables_and_user_functions(self, code: str) -> CodeVariablesAndUserFunctions:
         """
         :demand: F.2.7
         """
         return self.__analyse_code_types(code).variables_user_functions
-
```

### Comparing `visualgo-2024.5.13/src/visualgo/logic/ui/ui_callbacks.py` & `visualgo-2024.5.15/src/visualgo/logic/ui/ui_callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from abc import ABC, abstractmethod
 
 from .types import TransferVariables
 from ..types import Statistics
 
 from ..static.types import CodeVariablesAndUserFunctions
 
+
 class UICallbacksInterface(ABC):
     """
     Interface for the UI Callbacks in order to communicate with the UI.
 
     :demand: F.1.7
     """
 
     @abstractmethod
     def set_current_line(self, line: int) -> None:
         """
         Update the UI to show that the last executed line is `line`.
 
-        :param variables: TransferVariables
+        :param line: the current line
         :return: None
         """
         pass
 
     @abstractmethod
     def update_variables(self, variables: TransferVariables) -> None:
         """
@@ -48,31 +49,30 @@
         """
         Tells the UI that the execution has been paused and all interaction should be enabled.
 
         :return: None
         """
         pass
 
-
     @abstractmethod
-    def show_error(self, error: str) -> None:
+    def show_error(self, error: BaseException) -> None:
         """
         Shows the error in the UI with the given `error`.
 
         :param error: str
         :return: None
         """
         pass
 
     @abstractmethod
     def show_message(self, message: str) -> None:
         """
         Shows the message in the UI with the given `message`.
 
-        :param error: str
+        :param message: str
         :return: None
         """
         pass
 
     @abstractmethod
     def get_code(self) -> str:
         """
@@ -133,8 +133,8 @@
     @abstractmethod
     def set_running_code(self) -> None:
         """
         Tell the UI that code is being run
 
         :return: None
         """
-        ...
+        ...
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/Array.py` & `visualgo-2024.5.15/src/visualgo/structures/Array.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         :return: int
         """
         try:
             return self.__array.index(v)
         except ValueError:
             raise ValueError(f"{v} is not in array")
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.length == 0:
             return "[]"
         string: str = "[{}".format(self.get(0))
         for i in range(1, self.length):
             string += ", {}".format(self.get(i))
         return string + "]"
 
@@ -68,15 +68,15 @@
             if self[i] != other[i]:
                 return False
         return True
 
     def __len__(self) -> int:
         return self.length
 
-    def __to_visu__(self):
+    def __to_visu__(self) -> str:
         if self.length == 0:
             return ""
         string: str = "{}".format(self.get(0))
         for i in range(1, self.length):
             string += ",{}".format(self.get(i))
         return string
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/BinaryTreeNode.py` & `visualgo-2024.5.15/src/visualgo/structures/BinaryTreeNode.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,16 +80,16 @@
         :return: bool
         """
         return self.left_child is not None or self.right_child is not None
 
     def __str__(self) -> str:
         return "↙{}↘".format(self.value)
 
-    def __to_visu__(self) -> str:
-        return None if self.is_sentinel() else {"data" : self.value, "children" : [child.__to_visu__() for child in filter(lambda c : c is not None and not c.is_sentinel(), self.children)]}
+    def __to_visu__(self) -> Optional[dict]:
+        return None if self.is_sentinel() else {"data": self.value, "children": [child.__to_visu__() for child in filter(lambda c: c is not None and not c.is_sentinel(), self.children)]}
 
 
 def BinaryTreeNode_value(node: BinaryTreeNode) -> T:
     return node.value
 
 
 def BinaryTreeNode_set_value(node: BinaryTreeNode, value: T) -> None:
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/BinaryTreeNodeBack.py` & `visualgo-2024.5.15/src/visualgo/structures/BinaryTreeNodeBack.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.13/src/visualgo/structures/DoublyLinkedList.py` & `visualgo-2024.5.15/src/visualgo/structures/DoublyLinkedList.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,14 @@
 
         :param e: Object
         :return: None
         """
         if self.is_empty():
             return self.insert_head(e)
         new_node = TwoWayNode(e)
-        # last_node = self._get_node(self.__length - 1)
         tmp_sentinel = self.__tail.next
         self.__tail.next = new_node
         new_node.previous = self.__tail
         new_node.next = tmp_sentinel
         self.__tail = new_node
         self.__length += 1
 
@@ -206,15 +205,15 @@
                 current_node = current_node.next
             result += current_node.__to_visu__() + "]"
             return result
 
     def __getitem__(self, index: int) -> T:
         return self.get(index)
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         if not isinstance(other, DoublyLinkedList) or self.__length != other.__length:
             return False
         current = self.__head
         other_current = other.__head
         while not current.is_sentinel():
             if current.value != other_current.value:
                 return False
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/Graph.py` & `visualgo-2024.5.15/src/visualgo/structures/Graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class RestrictedDoublyLinkedList:
     def __init__(self, doubly_linked_list):
         self.__doubly_linked_list: DoublyLinkedList = doubly_linked_list
 
     @property
-    def length(self):
+    def length(self) -> int:
         return self.__doubly_linked_list.length
 
     def is_empty(self) -> bool:
         return self.__doubly_linked_list.length == 0
 
     def get(self, index: int) -> T:
         return self.__doubly_linked_list.get(index)
@@ -27,33 +27,33 @@
 
     def __str__(self) -> str:
         return str(self.__doubly_linked_list)
 
     def __getitem__(self, index: int) -> T:
         return self.__doubly_linked_list[index]
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         return self.__doubly_linked_list == other or (hasattr(other,
                                                               "_RestrictedDoublyLinkedList__doubly_linked_list") and self.__doubly_linked_list == other.__doubly_linked_list)
 
     def __len__(self) -> int:
         return self.__doubly_linked_list.length
 
     def __iter__(self):
         return self.__doubly_linked_list.__iter__()
 
     def __to_visu__(self) -> str:
         return self.__doubly_linked_list.__to_visu__()
 
-    def insert_last(self, value):
+    def insert_last(self, value) -> None:
         if not isinstance(inspect.currentframe().f_back.f_locals.get('self'), Graph):
             raise AttributeError("Method 'insert_last' can only be called from 'Graph'.")
         return self.__doubly_linked_list.insert_last(value)
 
-    def delete(self, index):
+    def delete(self, index) -> None:
         if not isinstance(inspect.currentframe().f_back.f_locals.get('self'), Graph):
             raise AttributeError("Method 'delete' can only be called from 'Graph'.")
         return self.__doubly_linked_list.delete(index)
 
 
 class Graph:
     def __init__(self, it: Iterable[T] = None):
@@ -149,27 +149,27 @@
         for i in range(self.__nb_vertices):
             for j in range(self.__nb_vertices):
                 if self.__edges[i][j] != other.__edges[i][j]:
                     return False
         return True
 
     def __to_visu__(self) -> str:
-        if self.__nb_vertices == 0 :
+        if self.__nb_vertices == 0:
             return "&"
-        
+
         edges = ""
         for i in self.__edges:
             for j in i:
                 edges += str(j)
                 edges += ","
             edges = edges[:-1]
             edges += ";"
         edges = edges[:-1]
 
-        return  self.__vertices.__to_visu__() + "&" + edges
+        return self.__vertices.__to_visu__() + "&" + edges
 
 
 def Graph_add_vertex(graph: Graph, v: T) -> None:
     return graph.add_vertex(v)
 
 
 def Graph_remove_vertex(graph: Graph, index: int) -> None:
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/LinkedList.py` & `visualgo-2024.5.15/src/visualgo/structures/LinkedList.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             raise IndexError('Index out of range')
         new_node = Node(e)
         current_node = self._get_node(index)
         new_node.next = current_node.next
         current_node.next = new_node
         self.__length += 1
 
-    def insert(self, index: int, e: T):
+    def insert(self, index: int, e: T) -> None:
         if index == 0:
             return self.insert_head(e)
         self.insert_after(index - 1, e)
 
     def delete(self, index: int) -> None:
         """
         Deletes the element at the given `index`.
@@ -143,15 +143,15 @@
         while not current_node.is_sentinel() and current_node.value != v:
             current_node = current_node.next
             i += 1
         if current_node.is_sentinel():
             raise ValueError(f'No such element in the list :{v}')
         return i
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.is_empty():
             return "[]"
         current_node = self.__head
         string: str = "[{}".format(current_node.value)
 
         while current_node.has_next():
             current_node = current_node.next
@@ -173,15 +173,15 @@
     def __len__(self) -> int:
         return self.length
 
     def __iter__(self):
         for i in range(self.length):
             yield self[i]
 
-    def __to_visu__(self):
+    def __to_visu__(self) -> str:
         if self.is_empty():
             return ""
         current_node = self.__head
         string: str = "{}".format(current_node.value)
 
         while current_node.has_next():
             current_node = current_node.next
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/List.py` & `visualgo-2024.5.15/src/visualgo/structures/List.py`

 * *Files identical despite different names*

### Comparing `visualgo-2024.5.13/src/visualgo/structures/Node.py` & `visualgo-2024.5.15/src/visualgo/structures/Node.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         """
         Creates a sentinel Node.
 
         :return: Node
         """
         return Node()
 
-    def is_sentinel(self):
+    def is_sentinel(self) -> bool:
         """
         Checks if the node is a sentinel.
 
         :return: bool
         """
         return self.next is None and self.value is None
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/Queue.py` & `visualgo-2024.5.15/src/visualgo/structures/Queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         :return: str
         """
         return self.__dll.__str__()
 
     def __eq__(self, other):
         return self.__dll == other.__dll
 
-    def __to_visu__(self):
+    def __to_visu__(self) -> str:
         return self.__dll.__to_visu__()
 
 
 def Queue_is_empty(queue: Queue) -> bool:
     return queue.is_empty()
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/Set.py` & `visualgo-2024.5.15/src/visualgo/structures/Set.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             return "{}"
         return repr(self.__set)
 
     def __eq__(self, o: object) -> bool:
         if isinstance(o, Set):
             return self.__set == o.__set
 
-    def __to_visu__(self):
+    def __to_visu__(self) -> str:
         if self.is_empty():
             return ""
         string = ""
         for e in self.__set:
             string += "{},".format(e)
         return string[:-1]
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/Stack.py` & `visualgo-2024.5.15/src/visualgo/structures/Stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         :return: A boolean
         """
         return self.__ll.is_empty()
 
     def __str__(self) -> str:
         return str(self.__ll)
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         return self.__ll == other.__ll
 
     def __to_visu__(self) -> str:
         return self.__ll.__to_visu__()
 
 
 def Stack_top(stack: Stack) -> T:
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/Tree.py` & `visualgo-2024.5.15/src/visualgo/structures/Tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,18 +63,18 @@
     def __depth_first_postorder_recursive(self, node: TreeNode, result: List[TreeNode]) -> None:
         if node.is_sentinel():
             return
         for child in node.children:
             self.__depth_first_postorder_recursive(child, result)
         result.append(node)
 
-    def __str__(self):
+    def __str__(self) -> None:
         return ""
 
-    def __to_visu__(self):
+    def __to_visu__(self) -> Optional[dict]:
         return self.__root.__to_visu__()
 
 
 def Tree_root(tree: Tree) -> TreeNode:
     return tree.root
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/TreeNode.py` & `visualgo-2024.5.15/src/visualgo/structures/TreeNode.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class TreeNode(Node):
     def __init__(self, value: T = None, children: Iterable = None) -> None:
         super().__init__(value)
         self.__children = DoublyLinkedList(children)
 
     @property
-    def children(self):
+    def children(self) -> DoublyLinkedList:
         """
         Returns the children of this TreeNode.
 
         :return: List[TreeNode]
         """
         return self.__children
 
@@ -60,20 +60,20 @@
         """
         Checks if the node is a sentinel.
 
         :return: bool
         """
         return self.children.is_empty() and self.value is None
 
-    def __str__(self):
+    def __str__(self) -> str:
         # return "{}→[{}]".format(self.value, ", ".join(map(str, self.children)))
         return "{}→".format(self.value)
 
-    def __to_visu__(self):
-        return None if self.is_sentinel() else {"data" : self.value, "children" : [child.__to_visu__() for child in filter(lambda c : c is not None and not c.is_sentinel(), self.children)]}
+    def __to_visu__(self) -> Optional[dict]:
+        return None if self.is_sentinel() else {"data": self.value, "children": [child.__to_visu__() for child in filter(lambda c: c is not None and not c.is_sentinel(), self.children)]}
 
 
 def TreeNode_value(node: TreeNode) -> T:
     return node.value
 
 
 def TreeNode_set_value(node: TreeNode, value: T) -> None:
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/TwoWayNode.py` & `visualgo-2024.5.15/src/visualgo/structures/TwoWayNode.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,26 +48,26 @@
         """
         Creates a sentinel Node.
 
         :return: Node
         """
         return TwoWayNode()
 
-    def is_sentinel(self):
+    def is_sentinel(self) -> bool:
         """
         Checks if the node is a sentinel.
 
         :return: bool
         """
         return self.value is None and self.next is None
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "←{}→".format(self.value)
 
-    def __to_visu__(self):
+    def __to_visu__(self) -> str:
         return str(self._value)
 
 
 def TwoWayNode_value(node: TwoWayNode) -> T:
     return node.value
```

### Comparing `visualgo-2024.5.13/src/visualgo/structures/__init__.py` & `visualgo-2024.5.15/src/visualgo/structures/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 """:demand: F1.8"""
 
-from .Set import ( Set, Set_is_empty, is_in_Set, Set_add, Set_delete )
+from .Set import (Set, Set_is_empty, is_in_Set, Set_add, Set_delete)
 
-from .Array import ( Array, Array_length, Array_get, Array_set )
+from .Array import (Array, Array_length, Array_get, Array_set)
 
-from .BinaryTreeNode import ( BinaryTreeNode, BinaryTreeNode_value, BinaryTreeNode_set_value, 
-    BinaryTreeNode_next, BinaryTreeNode_set_next, BinaryTreeNode_has_next, BinaryTreeNode_sentinel, 
-    BinaryTreeNode_is_sentinel, BinaryTreeNode_left_child, BinaryTreeNode_set_left_child, 
-    BinaryTreeNode_right_child, BinaryTreeNode_set_right_child, BinaryTreeNode_has_child )
+from .BinaryTreeNode import (BinaryTreeNode, BinaryTreeNode_value, BinaryTreeNode_set_value,
+                             BinaryTreeNode_next, BinaryTreeNode_set_next, BinaryTreeNode_has_next,
+                             BinaryTreeNode_sentinel,
+                             BinaryTreeNode_is_sentinel, BinaryTreeNode_left_child, BinaryTreeNode_set_left_child,
+                             BinaryTreeNode_right_child, BinaryTreeNode_set_right_child, BinaryTreeNode_has_child)
 
-from .Stack import ( Stack, Stack_top, Stack_is_empty, Stack_push, Stack_pop )
+from .Stack import (Stack, Stack_top, Stack_is_empty, Stack_push, Stack_pop)
 
-from .Queue import ( Queue, Queue_is_empty, Queue_enqueue, Queue_dequeue )
+from .Queue import (Queue, Queue_is_empty, Queue_enqueue, Queue_dequeue)
 
 # from .List import List
 
-from .Node import ( Node, Node_value, Node_set_value, Node_next, Node_set_next, Node_has_next, 
-    Node_sentinel, Node_is_sentinel )
-
-from .TwoWayNode import ( TwoWayNode, TwoWayNode_value, TwoWayNode_set_value, TwoWayNode_next,
-    TwoWayNode_set_next, TwoWayNode_has_next, TwoWayNode_sentinel, TwoWayNode_is_sentinel,
-    TwoWayNode_previous, TwoWayNode_set_previous, TwoWayNode_has_previous )
- 
-from .LinkedList import ( LinkedList, LinkedList_length, LinkedList_get, LinkedList_insert, LinkedList_delete,
-    LinkedList_is_empty, LinkedList_set, LinkedList_insert_head, LinkedList_insert_after, LinkedList__get_node )
+from .Node import (Node, Node_value, Node_set_value, Node_next, Node_set_next, Node_has_next,
+                   Node_sentinel, Node_is_sentinel)
 
+from .TwoWayNode import (TwoWayNode, TwoWayNode_value, TwoWayNode_set_value, TwoWayNode_next,
+                         TwoWayNode_set_next, TwoWayNode_has_next, TwoWayNode_sentinel, TwoWayNode_is_sentinel,
+                         TwoWayNode_previous, TwoWayNode_set_previous, TwoWayNode_has_previous)
+
+from .LinkedList import (LinkedList, LinkedList_length, LinkedList_get, LinkedList_insert, LinkedList_delete,
+                         LinkedList_is_empty, LinkedList_set, LinkedList_insert_head, LinkedList_insert_after,
+                         LinkedList__get_node)
 
 from .DoublyLinkedList import (DoublyLinkedList, DoublyLinkedList_length, DoublyLinkedList_get,
-    DoublyLinkedList_insert, DoublyLinkedList_delete, DoublyLinkedList_is_empty, DoublyLinkedList_set,
-    DoublyLinkedList_insert_head, DoublyLinkedList_insert_last, DoublyLinkedList_insert_after,
-    DoublyLinkedList__get_node)
-
-from .TreeNode import ( TreeNode, TreeNode_value, TreeNode_set_value, TreeNode_next, TreeNode_set_next,
-    TreeNode_has_next, TreeNode_sentinel, TreeNode_is_sentinel, TreeNode_children, TreeNode_has_child,
-    TreeNode_add_child, TreeNode_delete_child )
-
-from .Graph import ( Graph, Graph_add_vertex, Graph_remove_vertex, Graph_get_vertex, Graph_add_edge,
-    Graph_remove_edge, Graph_has_edge )
+                               DoublyLinkedList_insert, DoublyLinkedList_delete, DoublyLinkedList_is_empty,
+                               DoublyLinkedList_set,
+                               DoublyLinkedList_insert_head, DoublyLinkedList_insert_last,
+                               DoublyLinkedList_insert_after,
+                               DoublyLinkedList__get_node)
+
+from .TreeNode import (TreeNode, TreeNode_value, TreeNode_set_value, TreeNode_next, TreeNode_set_next,
+                       TreeNode_has_next, TreeNode_sentinel, TreeNode_is_sentinel, TreeNode_children,
+                       TreeNode_has_child,
+                       TreeNode_add_child, TreeNode_delete_child)
 
+from .Graph import (Graph, Graph_add_vertex, Graph_remove_vertex, Graph_get_vertex, Graph_add_edge,
+                    Graph_remove_edge, Graph_has_edge)
```

### Comparing `visualgo-2024.5.13/src/visualgo.egg-info/PKG-INFO` & `visualgo-2024.5.15/src/visualgo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualgo
-Version: 2024.5.13
+Version: 2024.5.15
 Summary: Enjoy classic datatypes and debug user python code
 Author: PFA-Visualgo
 License: MIT License
         
         Copyright (c) 2024 PFA-Visualgo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `visualgo-2024.5.13/src/visualgo.egg-info/SOURCES.txt` & `visualgo-2024.5.15/src/visualgo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

