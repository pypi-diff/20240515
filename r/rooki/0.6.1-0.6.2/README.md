# Comparing `tmp/rooki-0.6.1.tar.gz` & `tmp/rooki-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rooki-0.6.1.tar", last modified: Fri Nov 10 15:38:58 2023, max compression
+gzip compressed data, was "rooki-0.6.2.tar", last modified: Wed May 15 11:20:00 2024, max compression
```

## Comparing `rooki-0.6.1.tar` & `rooki-0.6.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-10 15:38:58.110549 rooki-0.6.1/
--rw-r--r--   0 pingu      (501) staff       (20)      190 2021-08-10 15:47:01.000000 rooki-0.6.1/AUTHORS.rst
--rw-r--r--   0 pingu      (501) staff       (20)     2840 2023-11-10 15:25:30.000000 rooki-0.6.1/HISTORY.rst
--rw-r--r--   0 pingu      (501) staff       (20)     1537 2021-08-10 15:47:01.000000 rooki-0.6.1/LICENSE
--rw-r--r--   0 pingu      (501) staff       (20)      192 2021-08-10 15:47:01.000000 rooki-0.6.1/MANIFEST.in
--rw-r--r--   0 pingu      (501) staff       (20)     2453 2021-08-10 15:47:01.000000 rooki-0.6.1/Makefile
--rw-r--r--   0 pingu      (501) staff       (20)     3446 2023-11-10 15:38:58.110267 rooki-0.6.1/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)     1885 2023-11-10 15:20:10.000000 rooki-0.6.1/README.rst
--rw-r--r--   0 pingu      (501) staff       (20)      115 2023-11-08 18:20:48.000000 rooki-0.6.1/requirements.txt
--rw-r--r--   0 pingu      (501) staff       (20)      222 2021-08-10 15:47:01.000000 rooki-0.6.1/requirements_dev.txt
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-10 15:38:58.103958 rooki-0.6.1/rooki/
--rw-r--r--   0 pingu      (501) staff       (20)      269 2021-08-10 15:47:01.000000 rooki-0.6.1/rooki/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)     2367 2021-08-10 15:47:01.000000 rooki-0.6.1/rooki/client.py
--rw-r--r--   0 pingu      (501) staff       (20)     2563 2021-08-10 15:47:01.000000 rooki-0.6.1/rooki/config.py
--rw-r--r--   0 pingu      (501) staff       (20)      132 2021-08-10 15:47:01.000000 rooki-0.6.1/rooki/default.cfg
--rw-r--r--   0 pingu      (501) staff       (20)     3291 2023-09-29 13:37:15.000000 rooki-0.6.1/rooki/operators.py
--rw-r--r--   0 pingu      (501) staff       (20)     3221 2023-11-08 18:20:48.000000 rooki-0.6.1/rooki/results.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-10 15:38:58.108045 rooki-0.6.1/rooki.egg-info/
--rw-r--r--   0 pingu      (501) staff       (20)     3446 2023-11-10 15:38:58.000000 rooki-0.6.1/rooki.egg-info/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)      439 2023-11-10 15:38:58.000000 rooki-0.6.1/rooki.egg-info/SOURCES.txt
--rw-r--r--   0 pingu      (501) staff       (20)        1 2023-11-10 15:38:58.000000 rooki-0.6.1/rooki.egg-info/dependency_links.txt
--rw-r--r--   0 pingu      (501) staff       (20)        1 2021-11-08 12:37:27.000000 rooki-0.6.1/rooki.egg-info/not-zip-safe
--rw-r--r--   0 pingu      (501) staff       (20)      115 2023-11-10 15:38:58.000000 rooki-0.6.1/rooki.egg-info/requires.txt
--rw-r--r--   0 pingu      (501) staff       (20)        6 2023-11-10 15:38:58.000000 rooki-0.6.1/rooki.egg-info/top_level.txt
--rw-r--r--   0 pingu      (501) staff       (20)      475 2023-11-10 15:38:58.111491 rooki-0.6.1/setup.cfg
--rw-r--r--   0 pingu      (501) staff       (20)     2623 2023-11-10 15:25:30.000000 rooki-0.6.1/setup.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-11-10 15:38:58.109172 rooki-0.6.1/tests/
--rw-r--r--   0 pingu      (501) staff       (20)     1895 2023-09-26 13:14:06.000000 rooki-0.6.1/tests/test_rooki.py
--rw-r--r--   0 pingu      (501) staff       (20)     2617 2023-09-26 13:14:06.000000 rooki-0.6.1/tests/test_workflow.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-05-15 11:20:00.011844 rooki-0.6.2/
+-rw-r--r--   0 pingu      (501) staff       (20)      190 2021-08-12 11:51:52.000000 rooki-0.6.2/AUTHORS.rst
+-rw-r--r--   0 pingu      (501) staff       (20)     2967 2024-05-15 11:19:27.000000 rooki-0.6.2/HISTORY.rst
+-rw-r--r--   0 pingu      (501) staff       (20)     1537 2021-08-12 11:51:52.000000 rooki-0.6.2/LICENSE
+-rw-r--r--   0 pingu      (501) staff       (20)      192 2021-08-12 11:51:52.000000 rooki-0.6.2/MANIFEST.in
+-rw-r--r--   0 pingu      (501) staff       (20)     2453 2021-08-12 11:51:52.000000 rooki-0.6.2/Makefile
+-rw-r--r--   0 pingu      (501) staff       (20)     3226 2024-05-15 11:20:00.012200 rooki-0.6.2/PKG-INFO
+-rw-r--r--   0 pingu      (501) staff       (20)     1885 2023-11-20 10:13:59.000000 rooki-0.6.2/README.rst
+-rw-r--r--   0 pingu      (501) staff       (20)      115 2023-11-03 11:15:49.000000 rooki-0.6.2/requirements.txt
+-rw-r--r--   0 pingu      (501) staff       (20)      222 2021-08-12 11:51:52.000000 rooki-0.6.2/requirements_dev.txt
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-05-15 11:19:59.999666 rooki-0.6.2/rooki/
+-rw-r--r--   0 pingu      (501) staff       (20)      269 2021-08-12 11:51:52.000000 rooki-0.6.2/rooki/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)     3254 2024-05-15 10:42:36.000000 rooki-0.6.2/rooki/client.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2563 2021-08-12 11:51:52.000000 rooki-0.6.2/rooki/config.py
+-rw-r--r--   0 pingu      (501) staff       (20)      132 2021-08-12 11:51:52.000000 rooki-0.6.2/rooki/default.cfg
+-rw-r--r--   0 pingu      (501) staff       (20)     3291 2023-09-28 15:48:58.000000 rooki-0.6.2/rooki/operators.py
+-rw-r--r--   0 pingu      (501) staff       (20)     3221 2023-11-03 11:15:49.000000 rooki-0.6.2/rooki/results.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-05-15 11:20:00.007397 rooki-0.6.2/rooki.egg-info/
+-rw-r--r--   0 pingu      (501) staff       (20)     3226 2024-05-15 11:19:59.000000 rooki-0.6.2/rooki.egg-info/PKG-INFO
+-rw-r--r--   0 pingu      (501) staff       (20)      439 2024-05-15 11:19:59.000000 rooki-0.6.2/rooki.egg-info/SOURCES.txt
+-rw-r--r--   0 pingu      (501) staff       (20)        1 2024-05-15 11:19:59.000000 rooki-0.6.2/rooki.egg-info/dependency_links.txt
+-rw-r--r--   0 pingu      (501) staff       (20)        1 2021-08-12 12:20:49.000000 rooki-0.6.2/rooki.egg-info/not-zip-safe
+-rw-r--r--   0 pingu      (501) staff       (20)      115 2024-05-15 11:19:59.000000 rooki-0.6.2/rooki.egg-info/requires.txt
+-rw-r--r--   0 pingu      (501) staff       (20)        6 2024-05-15 11:19:59.000000 rooki-0.6.2/rooki.egg-info/top_level.txt
+-rw-r--r--   0 pingu      (501) staff       (20)      475 2024-05-15 11:20:00.013703 rooki-0.6.2/setup.cfg
+-rw-r--r--   0 pingu      (501) staff       (20)     2623 2024-05-15 11:19:27.000000 rooki-0.6.2/setup.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-05-15 11:20:00.010586 rooki-0.6.2/tests/
+-rw-r--r--   0 pingu      (501) staff       (20)     1895 2023-05-04 16:45:52.000000 rooki-0.6.2/tests/test_rooki.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2617 2023-05-04 16:45:52.000000 rooki-0.6.2/tests/test_workflow.py
```

### Comparing `rooki-0.6.1/HISTORY.rst` & `rooki-0.6.2/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Version History
 ===============
 
+v0.6.2 (2024-05-15)
+-------------------
+
+Changes
+^^^^^^^
+
+* Fix usage of signal in birdy (#163).
+* Added notebooks for atlas.
+
 v0.6.1 (2023-11-10)
 -------------------
 
 Changes
 ^^^^^^^
 
 * Clean up setup (#146).
```

### Comparing `rooki-0.6.1/LICENSE` & `rooki-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rooki-0.6.1/Makefile` & `rooki-0.6.2/Makefile`

 * *Files identical despite different names*

### Comparing `rooki-0.6.1/PKG-INFO` & `rooki-0.6.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rooki
-Version: 0.6.1
+Version: 0.6.2
 Summary: A client for roocs climate data operations service.
 Home-page: https://github.com/roocs/rooki
 Author: Carsten Ehbrecht
 Author-email: ehbrecht@dkrz.de
 License: BSD - see LICENSE file in top-level package directory
 Keywords: rooki
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,21 +27,14 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: Click>=6.0
-Requires-Dist: birdhouse-birdy<0.9.0,>=0.8.2
-Requires-Dist: netCDF4>=1.5
-Requires-Dist: xarray>=0.16
-Requires-Dist: cf-xarray
-Requires-Dist: beautifulsoup4>=4.9.1
-Requires-Dist: pymetalink>=6.2
 
 rooki
 =====
 
 |pypi| |conda| |build| |black|
```

### Comparing `rooki-0.6.1/README.rst` & `rooki-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `rooki-0.6.1/rooki/client.py` & `rooki-0.6.2/rooki/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -78,7 +78,34 @@
 
     def _execute(self, pid, **kwargs):
         try:
             resp = super(Rooki, self)._execute(pid, **kwargs)
         except Exception:
             raise RuntimeError("execution failed")
         return Result(resp, output_dir=self.output_dir)
+
+    def _console_monitor(self, execution, sleep=3):
+        """
+        TODO: overwrites birdy method to avoid conflict with usage of signal and dask.
+        """
+        # import signal
+
+        # # Intercept CTRL-C
+        # def sigint_handler(signum, frame):
+        #     self.cancel()
+
+        # signal.signal(signal.SIGINT, sigint_handler)
+
+        while not execution.isComplete():
+            execution.checkStatus(sleepSecs=sleep)
+            self.logger.info(
+                "{} [{}/100] - {} ".format(
+                    execution.process.identifier,
+                    execution.percentCompleted,
+                    execution.statusMessage[:50],
+                )
+            )
+
+        if execution.isSucceded():
+            self.logger.info(f"{execution.process.identifier} done.")
+        else:
+            self.logger.info(f"{execution.process.identifier} failed.")
```

### Comparing `rooki-0.6.1/rooki/config.py` & `rooki-0.6.2/rooki/config.py`

 * *Files identical despite different names*

### Comparing `rooki-0.6.1/rooki/operators.py` & `rooki-0.6.2/rooki/operators.py`

 * *Files identical despite different names*

### Comparing `rooki-0.6.1/rooki/results.py` & `rooki-0.6.2/rooki/results.py`

 * *Files identical despite different names*

### Comparing `rooki-0.6.1/rooki.egg-info/PKG-INFO` & `rooki-0.6.2/rooki.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rooki
-Version: 0.6.1
+Version: 0.6.2
 Summary: A client for roocs climate data operations service.
 Home-page: https://github.com/roocs/rooki
 Author: Carsten Ehbrecht
 Author-email: ehbrecht@dkrz.de
 License: BSD - see LICENSE file in top-level package directory
 Keywords: rooki
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,21 +27,14 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: Click>=6.0
-Requires-Dist: birdhouse-birdy<0.9.0,>=0.8.2
-Requires-Dist: netCDF4>=1.5
-Requires-Dist: xarray>=0.16
-Requires-Dist: cf-xarray
-Requires-Dist: beautifulsoup4>=4.9.1
-Requires-Dist: pymetalink>=6.2
 
 rooki
 =====
 
 |pypi| |conda| |build| |black|
```

### Comparing `rooki-0.6.1/setup.py` & `rooki-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import setup, find_packages
 
 __author__ = "Carsten Ehbrecht"
 __contact__ = "ehbrecht@dkrz.de"
 __copyright__ = "Copyright 2023 United Kingdom Research and Innovation"
 __license__ = "BSD - see LICENSE file in top-level package directory"
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 # One strategy for storing the overall version is to put it in the top-level
 # package's __init__ but Nb. __init__.py files are not needed to declare
 # packages in Python 3
 # from rooki import __version__ as _package_version
 
 # Populate long description setting with content of README
```

### Comparing `rooki-0.6.1/tests/test_rooki.py` & `rooki-0.6.2/tests/test_rooki.py`

 * *Files identical despite different names*

### Comparing `rooki-0.6.1/tests/test_workflow.py` & `rooki-0.6.2/tests/test_workflow.py`

 * *Files identical despite different names*

