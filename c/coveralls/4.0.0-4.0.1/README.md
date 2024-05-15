# Comparing `tmp/coveralls-4.0.0.tar.gz` & `tmp/coveralls-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coveralls-4.0.0.tar", max compression
+gzip compressed data, was "coveralls-4.0.1.tar", max compression
```

## Comparing `coveralls-4.0.0.tar` & `coveralls-4.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1080 2024-04-29 14:26:08.785074 coveralls-4.0.0/LICENSE.rst
--rw-r--r--   0        0        0     3880 2024-04-29 14:26:08.785074 coveralls-4.0.0/README.rst
--rw-r--r--   0        0        0      134 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/__init__.py
--rw-r--r--   0        0        0       62 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/__main__.py
--rw-r--r--   0        0        0    16403 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/api.py
--rw-r--r--   0        0        0     3434 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/cli.py
--rw-r--r--   0        0        0      336 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/exception.py
--rw-r--r--   0        0        0     4086 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/git.py
--rw-r--r--   0        0        0     4367 2024-04-29 14:26:08.785074 coveralls-4.0.0/coveralls/reporter.py
--rw-r--r--   0        0        0     1720 2024-04-29 14:26:08.789074 coveralls-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 coveralls-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-15 12:55:52.314638 coveralls-4.0.1/LICENSE.rst
+-rw-r--r--   0        0        0     3880 2024-05-15 12:55:52.318638 coveralls-4.0.1/README.rst
+-rw-r--r--   0        0        0      134 2024-05-15 12:55:52.318638 coveralls-4.0.1/coveralls/__init__.py
+-rw-r--r--   0        0        0       62 2024-05-15 12:55:52.318638 coveralls-4.0.1/coveralls/__main__.py
+-rw-r--r--   0        0        0    16403 2024-05-15 12:55:52.318638 coveralls-4.0.1/coveralls/api.py
+-rw-r--r--   0        0        0     3434 2024-05-15 12:55:52.318638 coveralls-4.0.1/coveralls/cli.py
+-rw-r--r--   0        0        0      336 2024-05-15 12:55:52.318638 coveralls-4.0.1/coveralls/exception.py
+-rw-r--r--   0        0        0     4086 2024-05-15 12:55:52.318638 coveralls-4.0.1/coveralls/git.py
+-rw-r--r--   0        0        0     4505 2024-05-15 12:55:52.318638 coveralls-4.0.1/coveralls/reporter.py
+-rw-r--r--   0        0        0     1720 2024-05-15 12:55:52.318638 coveralls-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 coveralls-4.0.1/PKG-INFO
```

### Comparing `coveralls-4.0.0/LICENSE.rst` & `coveralls-4.0.1/LICENSE.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MIT License
 ===========
 
-Copyright (c) 2023 Kevin James
+Copyright (c) 2017 Kevin James
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `coveralls-4.0.0/README.rst` & `coveralls-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `coveralls-4.0.0/coveralls/api.py` & `coveralls-4.0.1/coveralls/api.py`

 * *Files identical despite different names*

### Comparing `coveralls-4.0.0/coveralls/cli.py` & `coveralls-4.0.1/coveralls/cli.py`

 * *Files identical despite different names*

### Comparing `coveralls-4.0.0/coveralls/git.py` & `coveralls-4.0.1/coveralls/git.py`

 * *Files identical despite different names*

### Comparing `coveralls-4.0.0/coveralls/reporter.py` & `coveralls-4.0.1/coveralls/reporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,15 +76,23 @@
 
         Returns a flat list where every four values represent a branch:
         1. line-number
         2. block-number (not used)
         3. branch-number
         4. hits (we only get 1/0 from coverage.py)
         """
-        if not analysis.has_arcs():
+        # pylint: disable=too-complex
+        has_arcs: bool
+        try:
+            has_arcs = analysis.has_arcs()
+        except TypeError:
+            # coverage v7.5+
+            has_arcs = analysis.has_arcs
+
+        if not has_arcs:
             return []
 
         missing_arcs: Dict[int, List[int]] = analysis.missing_branch_arcs()
         try:
             # coverage v6.3+
             executed_arcs = analysis.executed_branch_arcs()
         except AttributeError:
@@ -116,25 +124,23 @@
         # ensure results are properly merged between platforms
         posix_filename = filename.replace(os.path.sep, '/')
 
         if self.base_dir and posix_filename.startswith(self.base_dir):
             posix_filename = posix_filename[len(self.base_dir):]
         posix_filename = self.src_dir + posix_filename
 
-        source = analysis.file_reporter.source()
-
-        token_lines = analysis.file_reporter.source_token_lines()
+        token_lines = cu.source_token_lines()
         coverage_lines = [
             self.get_hits(i, analysis)
             for i, _ in enumerate(token_lines, 1)
         ]
 
         results = {
             'name': posix_filename,
-            'source': source,
+            'source': cu.source(),
             'coverage': coverage_lines,
         }
 
         branches = self.get_arcs(analysis)
         if branches:
             results['branches'] = branches
```

### Comparing `coveralls-4.0.0/pyproject.toml` & `coveralls-4.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coveralls"
-version = "4.0.0"
+version = "4.0.1"
 description = "Show coverage stats online via coveralls.io"
 readme = "README.rst"
 
 repository = "http://github.com/TheKevJames/coveralls-python"
 authors = ["Kevin James <coveralls-python@thekev.in>"]
 license = "MIT"
 
@@ -28,15 +28,15 @@
 
 [tool.poetry.scripts]
 coveralls = "coveralls.cli:main"
 python-coveralls = "coveralls.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
-coverage = { version = ">=5.0,<7.5,!=6.0.*,!=6.1,!=6.1.1", extras = ["toml"] }
+coverage = { version = ">=5.0,<8.0,!=6.0.*,!=6.1,!=6.1.1", extras = ["toml"] }
 docopt = ">=0.6.1,<0.7.0"
 requests = ">=1.0.0,<3.0.0"
 
 pyyaml = { version = ">=3.10,<7.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "8.2.0"
```

### Comparing `coveralls-4.0.0/PKG-INFO` & `coveralls-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coveralls
-Version: 4.0.0
+Version: 4.0.1
 Summary: Show coverage stats online via coveralls.io
 Home-page: http://github.com/TheKevJames/coveralls-python
 License: MIT
 Author: Kevin James
 Author-email: coveralls-python@thekev.in
 Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: yaml
-Requires-Dist: coverage[toml] (>=5.0,<7.5,!=6.0.*,!=6.1,!=6.1.1)
+Requires-Dist: coverage[toml] (>=5.0,<8.0,!=6.0.*,!=6.1,!=6.1.1)
 Requires-Dist: docopt (>=0.6.1,<0.7.0)
 Requires-Dist: pyyaml (>=3.10,<7.0) ; extra == "yaml"
 Requires-Dist: requests (>=1.0.0,<3.0.0)
 Project-URL: Changelog, https://github.com/TheKevJames/coveralls-python/blob/master/CHANGELOG.md
 Project-URL: Docs, https://coveralls-python.rtfd.io/
 Project-URL: Repository, http://github.com/TheKevJames/coveralls-python
 Description-Content-Type: text/x-rst
```

