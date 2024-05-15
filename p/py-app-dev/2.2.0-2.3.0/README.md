# Comparing `tmp/py_app_dev-2.2.0.tar.gz` & `tmp/py_app_dev-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_app_dev-2.2.0.tar", max compression
+gzip compressed data, was "py_app_dev-2.3.0.tar", max compression
```

## Comparing `py_app_dev-2.2.0.tar` & `py_app_dev-2.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-04-13 19:30:55.142812 py_app_dev-2.2.0/LICENSE
--rw-r--r--   0        0        0     4583 2024-04-13 19:30:55.142812 py_app_dev-2.2.0/README.md
--rw-r--r--   0        0        0     3787 2024-04-13 19:30:55.958811 py_app_dev-2.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-13 19:30:55.958811 py_app_dev-2.2.0/src/py_app_dev/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/__init__.py
--rw-r--r--   0        0        0     6103 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/cmd_line.py
--rw-r--r--   0        0        0     1007 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/docs_utils.py
--rw-r--r--   0        0        0      279 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/exceptions.py
--rw-r--r--   0        0        0     2235 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/logging.py
--rw-r--r--   0        0        0     4450 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/pipeline.py
--rw-r--r--   0        0        0     4906 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/runnable.py
--rw-r--r--   0        0        0     9967 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/scoop_wrapper.py
--rw-r--r--   0        0        0     2258 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/core/subprocess.py
--rw-r--r--   0        0        0        0 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/mvp/__init__.py
--rw-r--r--   0        0        0     1837 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/mvp/event_manager.py
--rw-r--r--   0        0        0      258 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/mvp/presenter.py
--rw-r--r--   0        0        0      174 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/mvp/view.py
--rw-r--r--   0        0        0        0 2024-04-13 19:30:55.146812 py_app_dev-2.2.0/src/py_app_dev/py.typed
--rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 py_app_dev-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-15 10:15:44.847331 py_app_dev-2.3.0/LICENSE
+-rw-r--r--   0        0        0     4583 2024-05-15 10:15:44.847331 py_app_dev-2.3.0/README.md
+-rw-r--r--   0        0        0     3787 2024-05-15 10:15:45.659331 py_app_dev-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-15 10:15:45.659331 py_app_dev-2.3.0/src/py_app_dev/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/core/__init__.py
+-rw-r--r--   0        0        0     6103 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/core/cmd_line.py
+-rw-r--r--   0        0        0     1007 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/core/docs_utils.py
+-rw-r--r--   0        0        0      279 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/core/exceptions.py
+-rw-r--r--   0        0        0     2235 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/core/logging.py
+-rw-r--r--   0        0        0     4450 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/core/pipeline.py
+-rw-r--r--   0        0        0     5321 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/core/runnable.py
+-rw-r--r--   0        0        0     9967 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/core/scoop_wrapper.py
+-rw-r--r--   0        0        0     2258 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/core/subprocess.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/mvp/__init__.py
+-rw-r--r--   0        0        0     1837 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/mvp/event_manager.py
+-rw-r--r--   0        0        0      258 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/mvp/presenter.py
+-rw-r--r--   0        0        0      174 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/mvp/view.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:15:44.851331 py_app_dev-2.3.0/src/py_app_dev/py.typed
+-rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 py_app_dev-2.3.0/PKG-INFO
```

### Comparing `py_app_dev-2.2.0/LICENSE` & `py_app_dev-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.2.0/README.md` & `py_app_dev-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.2.0/pyproject.toml` & `py_app_dev-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-app-dev"
-version = "2.2.0"
+version = "2.3.0"
 description = "My application development modules."
 authors = ["cuinixam <me@cuinixam.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuinixam/python-app-dev"
 documentation = "https://python-app-dev.readthedocs.io"
 classifiers = [
```

### Comparing `py_app_dev-2.2.0/src/py_app_dev/core/cmd_line.py` & `py_app_dev-2.3.0/src/py_app_dev/core/cmd_line.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.2.0/src/py_app_dev/core/docs_utils.py` & `py_app_dev-2.3.0/src/py_app_dev/core/docs_utils.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.2.0/src/py_app_dev/core/logging.py` & `py_app_dev-2.3.0/src/py_app_dev/core/logging.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.2.0/src/py_app_dev/core/pipeline.py` & `py_app_dev-2.3.0/src/py_app_dev/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.2.0/src/py_app_dev/core/runnable.py` & `py_app_dev-2.3.0/src/py_app_dev/core/runnable.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from pathlib import Path
 from typing import List, Optional
 
 from .logging import logger
 
 
 class Runnable(ABC):
+    def __init__(self, needs_dependency_management: bool = True) -> None:
+        self.needs_dependency_management = needs_dependency_management
+
     @abstractmethod
     def run(self) -> int:
         """Run and return exit code."""
 
     @abstractmethod
     def get_name(self) -> str:
         """Get runnable name."""
@@ -111,14 +114,20 @@
                         return RunInfoStatus.FILE_CHANGED
         # If there is nothing to be checked, assume it shall always run
         else:
             return RunInfoStatus.NOTHING_TO_CHECK
         return RunInfoStatus.MATCH
 
     def execute(self, runnable: Runnable) -> int:
+        if not runnable.needs_dependency_management:
+            logger.info(f"Runnable '{runnable.get_name()}' does not need dependency management. Executing directly.")
+            if self.dry_run:
+                return 0
+            return runnable.run()
+
         run_info_status = self.previous_run_info_matches(runnable)
         if run_info_status.should_run:
             logger.info(f"Runnable '{runnable.get_name()}' must run. {run_info_status.message}")
             if self.dry_run:
                 return 0
             exit_code = runnable.run()
             self.store_run_info(runnable)
```

### Comparing `py_app_dev-2.2.0/src/py_app_dev/core/scoop_wrapper.py` & `py_app_dev-2.3.0/src/py_app_dev/core/scoop_wrapper.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.2.0/src/py_app_dev/core/subprocess.py` & `py_app_dev-2.3.0/src/py_app_dev/core/subprocess.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.2.0/src/py_app_dev/mvp/event_manager.py` & `py_app_dev-2.3.0/src/py_app_dev/mvp/event_manager.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.2.0/PKG-INFO` & `py_app_dev-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-app-dev
-Version: 2.2.0
+Version: 2.3.0
 Summary: My application development modules.
 Home-page: https://github.com/cuinixam/python-app-dev
 License: MIT
 Author: cuinixam
 Author-email: me@cuinixam.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-app-dev Version: 2.2.0 Summary: My application
+Metadata-Version: 2.1 Name: py-app-dev Version: 2.3.0 Summary: My application
 development modules. Home-page: https://github.com/cuinixam/python-app-dev
 License: MIT Author: cuinixam Author-email: me@cuinixam.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

