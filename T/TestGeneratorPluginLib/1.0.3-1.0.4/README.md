# Comparing `tmp/TestGeneratorPluginLib-1.0.3.tar.gz` & `tmp/TestGeneratorPluginLib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TestGeneratorPluginLib-1.0.3.tar", last modified: Tue May 14 17:48:49 2024, max compression
+gzip compressed data, was "TestGeneratorPluginLib-1.0.4.tar", last modified: Wed May 15 08:02:38 2024, max compression
```

## Comparing `TestGeneratorPluginLib-1.0.3.tar` & `TestGeneratorPluginLib-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 17:48:49.746217 TestGeneratorPluginLib-1.0.3/
--rw-rw-rw-   0        0        0     1090 2024-05-14 17:47:56.000000 TestGeneratorPluginLib-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1569 2024-05-14 17:48:49.746217 TestGeneratorPluginLib-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 17:48:49.746217 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib/
--rw-rw-rw-   0        0        0      191 2024-05-14 17:47:56.000000 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib/__init__.py
--rw-rw-rw-   0        0        0      994 2024-05-14 17:47:56.000000 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib/_built_plugin.py
--rw-rw-rw-   0        0        0       19 2024-05-14 17:47:56.000000 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib/_config.py
--rw-rw-rw-   0        0        0      965 2024-05-14 17:47:56.000000 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib/_managers.py
--rw-rw-rw-   0        0        0     2760 2024-05-14 17:47:56.000000 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib/_plugin.py
--rw-rw-rw-   0        0        0     3344 2024-05-14 17:47:56.000000 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib/_widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:48:49.746217 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib.egg-info/
--rw-rw-rw-   0        0        0     1569 2024-05-14 17:48:49.000000 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2024-05-14 17:48:49.000000 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 17:48:49.000000 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-14 17:48:49.000000 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-14 17:48:49.000000 TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 17:48:49.746217 TestGeneratorPluginLib-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-05-14 17:47:56.000000 TestGeneratorPluginLib-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:02:38.537877 TestGeneratorPluginLib-1.0.4/
+-rw-rw-rw-   0        0        0     1090 2024-05-15 08:01:40.000000 TestGeneratorPluginLib-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1569 2024-05-15 08:02:38.537877 TestGeneratorPluginLib-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 08:02:38.537877 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib/
+-rw-rw-rw-   0        0        0      288 2024-05-15 08:01:40.000000 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib/__init__.py
+-rw-rw-rw-   0        0        0     1707 2024-05-15 08:01:40.000000 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib/_built_plugin.py
+-rw-rw-rw-   0        0        0       19 2024-05-15 08:01:40.000000 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib/_config.py
+-rw-rw-rw-   0        0        0     1684 2024-05-15 08:01:40.000000 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib/_language.py
+-rw-rw-rw-   0        0        0     1219 2024-05-15 08:01:40.000000 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib/_managers.py
+-rw-rw-rw-   0        0        0     3093 2024-05-15 08:01:40.000000 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib/_plugin.py
+-rw-rw-rw-   0        0        0     3344 2024-05-15 08:01:40.000000 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib/_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-15 08:02:38.537877 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib.egg-info/
+-rw-rw-rw-   0        0        0     1569 2024-05-15 08:02:38.000000 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2024-05-15 08:02:38.000000 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 08:02:38.000000 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-15 08:02:38.000000 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-15 08:02:38.000000 TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 08:02:38.537877 TestGeneratorPluginLib-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-05-15 08:01:40.000000 TestGeneratorPluginLib-1.0.4/setup.py
```

### Comparing `TestGeneratorPluginLib-1.0.3/LICENSE` & `TestGeneratorPluginLib-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.3/PKG-INFO` & `TestGeneratorPluginLib-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.0.3
+Version: 1.0.4
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib/_managers.py` & `TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib/_managers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable, Any
 
-from PyQt6.QtCore import QThread
+from PyQt6.QtCore import QThread, QObject
 
 
 class BackendManager:
     def __init__(self):
         self.sm = _SettingsManager()
         self.processes = _ProcessesManager()
         self.projects = _ProjectsManager()
@@ -29,7 +29,23 @@
     async def run_async(self, thread: Callable[[], Any] | QThread, group: str, name: str): ...
 
 
 class _ProjectsManager:
     @property
     def current(self):
         return None
+
+
+class Manager(QObject):
+    def __init__(self, bm):
+        super().__init__()
+        self._bm = bm
+
+    async def load(self):
+        pass
+
+    async def close(self):
+        pass
+
+    async def indexing(self):
+        pass
+
```

### Comparing `TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib/_plugin.py` & `TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib/_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import os
 import shutil
 import subprocess
 import sys
 from sys import argv
 from typing import Iterable, Callable
 
-from TestGeneratorPluginLib import BackendManager
+from TestGeneratorPluginLib import BackendManager, Manager
+from TestGeneratorPluginLib._language import _FastRunOption
 from TestGeneratorPluginLib._widgets import MainTab, SideTab
 
 
 class Plugin:
     def __init__(self,
                  name: str,
                  description: str,
@@ -22,14 +23,16 @@
                  conflicts: Iterable[str] = tuple(),
 
                  directories: Iterable[str] = tuple(),
                  requirements: Iterable[str] = tuple(),
 
                  main_tabs: dict[str: Callable[[BackendManager], MainTab]] = None,
                  side_tabs: dict[str: Callable[[BackendManager], SideTab]] = None,
+                 managers: dict[str: Callable[[BackendManager], Manager]] = None,
+                 fast_run_options: dict[str, list[_FastRunOption]] = None,
                  ):
         self.name = name
         self.description = description
         self.version = version
         self.author = author
         self.url = url
         self.platform_specific = bool(requirements) if platform_specific is None else platform_specific
@@ -37,14 +40,16 @@
         self.conflicts = list(conflicts)
 
         self._directories = list(directories)
         self._requirements = list(requirements)
 
         self.main_tabs = main_tabs or dict()
         self.side_tabs = side_tabs or dict()
+        self.managers = managers or dict()
+        self.fast_run_options = fast_run_options or dict()
 
         self._parse_args()
 
     def _parse_args(self):
         _parser = argparse.ArgumentParser()
         _parser.add_argument('-b', '--build', action='store_true')
         _parser.add_argument('-u', '--upload', action='store_true')
```

### Comparing `TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib/_widgets.py` & `TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib/_widgets.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.3/TestGeneratorPluginLib.egg-info/PKG-INFO` & `TestGeneratorPluginLib-1.0.4/TestGeneratorPluginLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.0.3
+Version: 1.0.4
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.0.3/setup.py` & `TestGeneratorPluginLib-1.0.4/setup.py`

 * *Files identical despite different names*

