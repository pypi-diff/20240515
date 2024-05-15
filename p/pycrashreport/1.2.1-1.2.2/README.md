# Comparing `tmp/pycrashreport-1.2.1.tar.gz` & `tmp/pycrashreport-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrashreport-1.2.1.tar", last modified: Wed Oct 25 05:49:39 2023, max compression
+gzip compressed data, was "pycrashreport-1.2.2.tar", last modified: Thu Nov 16 16:52:08 2023, max compression
```

## Comparing `pycrashreport-1.2.1.tar` & `pycrashreport-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 05:49:39.839583 pycrashreport-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-10-25 05:49:23.000000 pycrashreport-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    45317 2023-10-25 05:49:39.839583 pycrashreport-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2023-10-25 05:49:23.000000 pycrashreport-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 05:49:39.839583 pycrashreport-1.2.1/pycrashreport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 05:49:23.000000 pycrashreport-1.2.1/pycrashreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-10-25 05:49:23.000000 pycrashreport-1.2.1/pycrashreport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14066 2023-10-25 05:49:23.000000 pycrashreport-1.2.1/pycrashreport/crash_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 05:49:39.839583 pycrashreport-1.2.1/pycrashreport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45317 2023-10-25 05:49:39.000000 pycrashreport-1.2.1/pycrashreport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-10-25 05:49:39.000000 pycrashreport-1.2.1/pycrashreport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 05:49:39.000000 pycrashreport-1.2.1/pycrashreport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-25 05:49:39.000000 pycrashreport-1.2.1/pycrashreport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-25 05:49:39.000000 pycrashreport-1.2.1/pycrashreport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-10-25 05:49:39.000000 pycrashreport-1.2.1/pycrashreport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-10-25 05:49:23.000000 pycrashreport-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 05:49:23.000000 pycrashreport-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 05:49:39.839583 pycrashreport-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 05:49:39.839583 pycrashreport-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11390 2023-10-25 05:49:23.000000 pycrashreport-1.2.1/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 16:52:08.543232 pycrashreport-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-11-16 16:51:49.000000 pycrashreport-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    45317 2023-11-16 16:52:08.543232 pycrashreport-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2023-11-16 16:51:49.000000 pycrashreport-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 16:52:08.543232 pycrashreport-1.2.2/pycrashreport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 16:51:49.000000 pycrashreport-1.2.2/pycrashreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-11-16 16:51:49.000000 pycrashreport-1.2.2/pycrashreport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14312 2023-11-16 16:51:49.000000 pycrashreport-1.2.2/pycrashreport/crash_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 16:52:08.543232 pycrashreport-1.2.2/pycrashreport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45317 2023-11-16 16:52:08.000000 pycrashreport-1.2.2/pycrashreport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2023-11-16 16:52:08.000000 pycrashreport-1.2.2/pycrashreport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 16:52:08.000000 pycrashreport-1.2.2/pycrashreport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-16 16:52:08.000000 pycrashreport-1.2.2/pycrashreport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-16 16:52:08.000000 pycrashreport-1.2.2/pycrashreport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-16 16:52:08.000000 pycrashreport-1.2.2/pycrashreport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-11-16 16:51:49.000000 pycrashreport-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 16:51:49.000000 pycrashreport-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 16:52:08.543232 pycrashreport-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 16:52:08.543232 pycrashreport-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2023-11-16 16:51:49.000000 pycrashreport-1.2.2/tests/test_parse.py
```

### Comparing `pycrashreport-1.2.1/LICENSE` & `pycrashreport-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrashreport-1.2.1/PKG-INFO` & `pycrashreport-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrashreport
-Version: 1.2.1
+Version: 1.2.2
 Summary: Pure python3 for parsing Apple's crash reports
 Author-email: doronz88 <doron88@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `pycrashreport-1.2.1/README.md` & `pycrashreport-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pycrashreport-1.2.1/pycrashreport/crash_report.py` & `pycrashreport-1.2.2/pycrashreport/crash_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import posixpath
 from collections import namedtuple
 from datetime import datetime
 from enum import Enum
 from io import StringIO
-from typing import List, Optional, Mapping, IO
+from typing import IO, List, Mapping, Optional
 
 import click
 from cached_property import cached_property
 from la_panic.panic_parser.kernel_panic import KernelPanic
 
 Frame = namedtuple('Frame', 'image_name image_base image_offset symbol symbol_offset')
 Register = namedtuple('Register', 'name value')
@@ -188,15 +188,20 @@
         self._metadata = metadata
         self._data = data
         self._parse()
 
     def _parse(self):
         self._is_json = False
         try:
-            self._data = json.loads(self._data)
+            modified_data = self._data
+            if '\n  \n' in modified_data:
+                modified_data, rest = modified_data.split('\n  \n', 1)
+                rest = '",' + rest.split('",', 1)[1]
+                modified_data += rest
+            self._data = json.loads(modified_data)
             self._is_json = True
         except json.decoder.JSONDecodeError:
             pass
 
     @cached_property
     def bug_type(self) -> BugType:
         return BugType(self.bug_type_str)
```

### Comparing `pycrashreport-1.2.1/pycrashreport.egg-info/PKG-INFO` & `pycrashreport-1.2.2/pycrashreport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrashreport
-Version: 1.2.1
+Version: 1.2.2
 Summary: Pure python3 for parsing Apple's crash reports
 Author-email: doronz88 <doron88@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `pycrashreport-1.2.1/pyproject.toml` & `pycrashreport-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pycrashreport"
-version = "1.2.1"
+version = "1.2.2"
 description = "Pure python3 for parsing Apple's crash reports"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["ios", "cli", "macos", "parser", "crash"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" }
```

### Comparing `pycrashreport-1.2.1/tests/test_parse.py` & `pycrashreport-1.2.2/tests/test_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 from pathlib import Path
 
-from pycrashreport.crash_report import Frame, Register, get_crash_report_from_file, BugType
+from pycrashreport.crash_report import BugType, Frame, Register, get_crash_report_from_file
 
 
 def test_non_symbolicated_ios14():
     filename = Path(__file__).parent / 'user_mode_crash_report_ios14_non_symbolicated_abort.ips'
     crash_report = get_crash_report_from_file(open(filename, 'rt'))
     assert crash_report.bug_type == BugType.Crash_109
     assert crash_report.incident_id == '13917FF0-E1B1-4652-84C2-85516D101DFE'
```

