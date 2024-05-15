# Comparing `tmp/argparse_decorations-0.0.1.tar.gz` & `tmp/argparse_decorations-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse_decorations-0.0.1.tar", last modified: Wed Sep 20 21:11:40 2023, max compression
+gzip compressed data, was "argparse_decorations-0.0.2.tar", last modified: Wed May 15 15:01:05 2024, max compression
```

## Comparing `argparse_decorations-0.0.1.tar` & `argparse_decorations-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rmonico   (1000) users      (985)        0 2023-09-20 21:11:40.718876 argparse_decorations-0.0.1/
--rw-r--r--   0 rmonico   (1000) users      (985)      240 2023-09-20 21:11:40.718876 argparse_decorations-0.0.1/PKG-INFO
-drwxr-xr-x   0 rmonico   (1000) users      (985)        0 2023-09-20 21:11:40.718876 argparse_decorations-0.0.1/argparse_decorations/
--rwxr-xr-x   0 rmonico   (1000) users      (985)     4073 2023-09-11 14:36:18.000000 argparse_decorations-0.0.1/argparse_decorations/__init__.py
-drwxr-xr-x   0 rmonico   (1000) users      (985)        0 2023-09-20 21:11:40.718876 argparse_decorations-0.0.1/argparse_decorations.egg-info/
--rw-r--r--   0 rmonico   (1000) users      (985)      240 2023-09-20 21:11:40.000000 argparse_decorations-0.0.1/argparse_decorations.egg-info/PKG-INFO
--rw-r--r--   0 rmonico   (1000) users      (985)      295 2023-09-20 21:11:40.000000 argparse_decorations-0.0.1/argparse_decorations.egg-info/SOURCES.txt
--rw-r--r--   0 rmonico   (1000) users      (985)        1 2023-09-20 21:11:40.000000 argparse_decorations-0.0.1/argparse_decorations.egg-info/dependency_links.txt
--rw-r--r--   0 rmonico   (1000) users      (985)        1 2023-09-20 21:11:40.000000 argparse_decorations-0.0.1/argparse_decorations.egg-info/not-zip-safe
--rw-r--r--   0 rmonico   (1000) users      (985)       21 2023-09-20 21:11:40.000000 argparse_decorations-0.0.1/argparse_decorations.egg-info/top_level.txt
--rw-r--r--   0 rmonico   (1000) users      (985)       38 2023-09-20 21:11:40.718876 argparse_decorations-0.0.1/setup.cfg
--rw-r--r--   0 rmonico   (1000) users      (985)      467 2023-09-11 14:36:18.000000 argparse_decorations-0.0.1/setup.py
-drwxr-xr-x   0 rmonico   (1000) users      (985)        0 2023-09-20 21:11:40.718876 argparse_decorations-0.0.1/tests/
--rw-r--r--   0 rmonico   (1000) users      (985)     1862 2023-09-11 14:36:18.000000 argparse_decorations-0.0.1/tests/test_argparse_decorations.py
+drwxr-xr-x   0 rmonico   (1000) users      (985)        0 2024-05-15 15:01:05.010083 argparse_decorations-0.0.2/
+-rw-r--r--   0 rmonico   (1000) users      (985)      240 2024-05-15 15:01:05.010083 argparse_decorations-0.0.2/PKG-INFO
+drwxr-xr-x   0 rmonico   (1000) users      (985)        0 2024-05-15 15:01:05.000083 argparse_decorations-0.0.2/argparse_decorations/
+-rwxr-xr-x   0 rmonico   (1000) users      (985)     4670 2024-05-15 14:52:18.000000 argparse_decorations-0.0.2/argparse_decorations/__init__.py
+drwxr-xr-x   0 rmonico   (1000) users      (985)        0 2024-05-15 15:01:05.010083 argparse_decorations-0.0.2/argparse_decorations.egg-info/
+-rw-r--r--   0 rmonico   (1000) users      (985)      240 2024-05-15 15:01:04.000000 argparse_decorations-0.0.2/argparse_decorations.egg-info/PKG-INFO
+-rw-r--r--   0 rmonico   (1000) users      (985)      295 2024-05-15 15:01:05.000000 argparse_decorations-0.0.2/argparse_decorations.egg-info/SOURCES.txt
+-rw-r--r--   0 rmonico   (1000) users      (985)        1 2024-05-15 15:01:04.000000 argparse_decorations-0.0.2/argparse_decorations.egg-info/dependency_links.txt
+-rw-r--r--   0 rmonico   (1000) users      (985)        1 2024-05-15 15:01:04.000000 argparse_decorations-0.0.2/argparse_decorations.egg-info/not-zip-safe
+-rw-r--r--   0 rmonico   (1000) users      (985)       21 2024-05-15 15:01:04.000000 argparse_decorations-0.0.2/argparse_decorations.egg-info/top_level.txt
+-rw-r--r--   0 rmonico   (1000) users      (985)       38 2024-05-15 15:01:05.010083 argparse_decorations-0.0.2/setup.cfg
+-rw-r--r--   0 rmonico   (1000) users      (985)      467 2024-05-15 14:02:28.000000 argparse_decorations-0.0.2/setup.py
+drwxr-xr-x   0 rmonico   (1000) users      (985)        0 2024-05-15 15:01:05.010083 argparse_decorations-0.0.2/tests/
+-rw-r--r--   0 rmonico   (1000) users      (985)     2058 2024-05-15 14:51:08.000000 argparse_decorations-0.0.2/tests/test_argparse_decorations.py
```

### Comparing `argparse_decorations-0.0.1/argparse_decorations/__init__.py` & `argparse_decorations-0.0.2/argparse_decorations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 # -*- coding: utf-8 -*-
 
 from argparse import ArgumentParser
 import logging
 
 
+# logging.basicConfig(level='DEBUG')
+
+_initialized = False
+
 def init(*args, **kwargs):
-    global _parser, _subparsers
+    global _initialized, _parser, _subparsers
+
+    if not _initialized:
+        _parser = ArgumentParser(*args, **kwargs)
+        _subparsers = _parser.add_subparsers()
 
-    _parser = ArgumentParser(*args, **kwargs)
-    _subparsers = _parser.add_subparsers()
+        _initialized = True
 
     return _parser
 
 
 _first_level_commands = list()
 
 
@@ -28,14 +35,19 @@
     def __repr__(self):
         return self.name
 
 
 class _AbstractDecoration(object):
 
     def __init__(self):
+        global _initialized
+
+        if not _initialized:
+            init()
+
         self._handler = None
 
 
     def _class(self):
         return self.__class__.__name__
 
 
@@ -60,22 +72,26 @@
 
 class Command(_AbstractDecoration):
 
     def __init__(self, name, *args, **kwargs):
         super().__init__()
 
         logging.debug('in {self._class()} __init__')
-        logging.debug('name: ' + name)
+        logging.debug('name: ' + (name or '<root command>'))
 
         global _first_level_commands
         global current_command
         pre_existing, current_command = self._get_leaf_by_name(name)
 
         if not pre_existing:
-            current_command.parser = _subparsers.add_parser(name, *args, **kwargs)
+            if name:
+                current_command.parser = _subparsers.add_parser(name, *args, **kwargs)
+            else:
+                global _parser
+                current_command.parser = _parser
 
         self.name = name
 
 
     def _get_leaf_by_name(self, name):
         global _first_level_commands
         for command in _first_level_commands:
@@ -83,14 +99,24 @@
                 return True, command
 
         newCommand = _CommandTreeLeaf(name)
         _first_level_commands.append(newCommand)
         return False, newCommand
 
 
+class RootCommand(Command):
+
+    def __init__(self, *args, **kwargs):
+        logging.debug('in {self._class()} __init__')
+
+        super().__init__(None)
+
+        super().__call__(*args, **kwargs)
+
+
 class SubCommand(_AbstractDecoration):
 
     def __init__(self, name, *args, **kwargs):
         super().__init__()
 
         logging.debug(f'in {self._class()} __init__')
         logging.debug(f'name: {name}')
@@ -160,15 +186,15 @@
     return run()
 
 
 def finish():
     """
     No need to call this in production code, created for tests
     """
-    global _first_level_commands, _parser, _subparsers, current_command, _handler, _args
+    global _first_level_commands, _initialized, _parser, _subparsers, current_command, _handler, _args
     _first_level_commands = list()
+    _initialized = False
     _parser = None
     _subparsers = None
     current_command = None
     _handler = None
     _args = None
-
```

### Comparing `argparse_decorations-0.0.1/tests/test_argparse_decorations.py` & `argparse_decorations-0.0.2/tests/test_argparse_decorations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 from unittest import TestCase
-from argparse_decorations import Command, SubCommand, Argument, init, parse, run, finish
+from argparse_decorations import RootCommand, Command, SubCommand, Argument, init, parse, run, finish
 
 
 class TestDecorations(TestCase):
 
-    def setUp(self):
-        init()
-
-
     def tearDown(self):
         finish()
 
 
     def test_tests(self):
         self.assertTrue(True)
 
 
+    def test_RootCommand(self):
+        called = False
+
+        @RootCommand
+        def handler():
+            nonlocal called
+            called = True
+
+        parse()
+
+        run()
+
+        self.assertTrue(called)
+
+
     def test_Command(self):
         called = False
 
         @Command('command')
         def handler():
             nonlocal called
             called = True
```

