# Comparing `tmp/livemetrics-0.6.tar.gz` & `tmp/livemetrics-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/livemetrics-0.6.tar", last modified: Fri Jul  3 17:34:24 2020, max compression
+gzip compressed data, was "livemetrics-0.7.tar", last modified: Wed May 15 13:26:12 2024, max compression
```

## Comparing `livemetrics-0.6.tar` & `livemetrics-0.7.tar`

### file list

```diff
@@ -1,47 +1,41 @@
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2020-07-03 17:34:24.113970 livemetrics-0.6/
--rw-r--r--   0 olivier   (1000) olivier   (1000)      151 2020-03-21 18:51:23.000000 livemetrics-0.6/MANIFEST.in
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2520 2020-07-03 17:34:24.113970 livemetrics-0.6/PKG-INFO
--rw-r--r--   0 olivier   (1000) olivier   (1000)     1439 2019-07-22 19:29:49.000000 livemetrics-0.6/README.rst
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2020-07-03 17:34:24.109970 livemetrics-0.6/docs/
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2020-07-03 17:34:24.109970 livemetrics-0.6/docs/_static/
--rw-r--r--   0 olivier   (1000) olivier   (1000)      785 2019-07-22 19:29:49.000000 livemetrics-0.6/docs/_static/custom.css
--rw-r--r--   0 olivier   (1000) olivier   (1000)      442 2019-07-22 19:29:49.000000 livemetrics-0.6/docs/conf.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     1407 2019-07-22 19:29:49.000000 livemetrics-0.6/docs/index.rst
--rw-r--r--   0 olivier   (1000) olivier   (1000)     1017 2019-07-22 19:29:49.000000 livemetrics-0.6/docs/modules.rst
--rw-r--r--   0 olivier   (1000) olivier   (1000)       82 2019-07-22 19:29:49.000000 livemetrics-0.6/docs/requirements.txt
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2020-07-03 17:34:24.109970 livemetrics-0.6/livemetrics/
--rw-r--r--   0 olivier   (1000) olivier   (1000)    15808 2020-06-10 20:05:25.000000 livemetrics-0.6/livemetrics/__init__.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2020-07-03 17:34:24.109970 livemetrics-0.6/livemetrics/dashboard/
--rw-r--r--   0 olivier   (1000) olivier   (1000)    12384 2020-06-10 20:32:52.000000 livemetrics-0.6/livemetrics/dashboard/dashboard.html
--rw-r--r--   0 olivier   (1000) olivier   (1000)    10052 2020-04-14 17:16:38.000000 livemetrics-0.6/livemetrics/dashboard/dashboard.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)    17523 2019-07-25 03:40:42.000000 livemetrics-0.6/livemetrics/metrics.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2020-07-03 17:34:24.109970 livemetrics-0.6/livemetrics/publishers/
--rw-r--r--   0 olivier   (1000) olivier   (1000)     7874 2019-07-22 19:29:49.000000 livemetrics-0.6/livemetrics/publishers/aiohttp.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     7220 2019-07-22 19:29:49.000000 livemetrics-0.6/livemetrics/publishers/django.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     7462 2019-07-22 19:29:49.000000 livemetrics-0.6/livemetrics/publishers/flask.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     7560 2019-07-22 19:29:49.000000 livemetrics-0.6/livemetrics/publishers/http.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2020-07-03 17:34:24.109970 livemetrics-0.6/livemetrics.egg-info/
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2520 2020-07-03 17:34:24.000000 livemetrics-0.6/livemetrics.egg-info/PKG-INFO
--rw-r--r--   0 olivier   (1000) olivier   (1000)      938 2020-07-03 17:34:24.000000 livemetrics-0.6/livemetrics.egg-info/SOURCES.txt
--rw-r--r--   0 olivier   (1000) olivier   (1000)        1 2020-07-03 17:34:24.000000 livemetrics-0.6/livemetrics.egg-info/dependency_links.txt
--rw-r--r--   0 olivier   (1000) olivier   (1000)       80 2020-07-03 17:34:24.000000 livemetrics-0.6/livemetrics.egg-info/entry_points.txt
--rw-r--r--   0 olivier   (1000) olivier   (1000)      110 2020-07-03 17:34:24.000000 livemetrics-0.6/livemetrics.egg-info/requires.txt
--rw-r--r--   0 olivier   (1000) olivier   (1000)       12 2020-07-03 17:34:24.000000 livemetrics-0.6/livemetrics.egg-info/top_level.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2020-07-03 17:34:24.113970 livemetrics-0.6/setup.cfg
--rw-r--r--   0 olivier   (1000) olivier   (1000)     1690 2020-03-22 11:48:42.000000 livemetrics-0.6/setup.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2020-07-03 17:34:24.109970 livemetrics-0.6/tests/
--rw-r--r--   0 olivier   (1000) olivier   (1000)        0 2019-07-22 19:29:49.000000 livemetrics-0.6/tests/__init__.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2020-07-03 17:34:24.109970 livemetrics-0.6/tests/dashboard/
--rw-r--r--   0 olivier   (1000) olivier   (1000)        0 2019-07-22 19:29:49.000000 livemetrics-0.6/tests/dashboard/__init__.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)      588 2020-04-12 12:42:54.000000 livemetrics-0.6/tests/dashboard/client.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2305 2020-06-10 20:37:15.000000 livemetrics-0.6/tests/dashboard/sample.yaml
--rw-r--r--   0 olivier   (1000) olivier   (1000)     1282 2020-04-12 12:45:06.000000 livemetrics-0.6/tests/dashboard/server.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2271 2019-08-12 11:33:58.000000 livemetrics-0.6/tests/dashboard/test_dashboard.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2020-07-03 17:34:24.113970 livemetrics-0.6/tests/publishers/
--rw-r--r--   0 olivier   (1000) olivier   (1000)     6259 2020-03-22 11:04:24.000000 livemetrics-0.6/tests/publishers/__init__.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2444 2020-03-22 11:45:31.000000 livemetrics-0.6/tests/publishers/test_aiohttp.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2601 2019-07-22 19:29:49.000000 livemetrics-0.6/tests/publishers/test_django.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2316 2019-07-22 19:29:49.000000 livemetrics-0.6/tests/publishers/test_flask.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2534 2019-07-22 19:29:49.000000 livemetrics-0.6/tests/publishers/test_http.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)      387 2019-07-22 19:29:49.000000 livemetrics-0.6/tests/test_doc.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2608 2019-07-22 19:29:49.000000 livemetrics-0.6/tests/test_metrics.py
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.615226 livemetrics-0.7/
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      210 2024-05-15 11:50:56.000000 livemetrics-0.7/AUTHORS.rst
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)    21863 2024-05-15 11:50:56.000000 livemetrics-0.7/LICENSE
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      151 2024-05-15 11:50:56.000000 livemetrics-0.7/MANIFEST.in
+-rw-r--r--   0 heurtier  (1000) heurtier  (1000)     2561 2024-05-15 13:26:12.615226 livemetrics-0.7/PKG-INFO
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1470 2024-05-15 11:50:56.000000 livemetrics-0.7/README.rst
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.611226 livemetrics-0.7/docs/
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.611226 livemetrics-0.7/docs/_static/
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      785 2024-05-15 11:50:56.000000 livemetrics-0.7/docs/_static/custom.css
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      442 2024-05-15 11:50:56.000000 livemetrics-0.7/docs/conf.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1407 2024-05-15 11:50:56.000000 livemetrics-0.7/docs/index.rst
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1017 2024-05-15 11:50:56.000000 livemetrics-0.7/docs/modules.rst
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      102 2024-05-15 11:50:56.000000 livemetrics-0.7/docs/requirements.txt
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.611226 livemetrics-0.7/livemetrics/
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)    16181 2024-05-15 13:25:18.000000 livemetrics-0.7/livemetrics/__init__.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)    17523 2024-05-15 11:50:56.000000 livemetrics-0.7/livemetrics/metrics.py
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.615226 livemetrics-0.7/livemetrics.egg-info/
+-rw-r--r--   0 heurtier  (1000) heurtier  (1000)     2561 2024-05-15 13:26:12.000000 livemetrics-0.7/livemetrics.egg-info/PKG-INFO
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      763 2024-05-15 13:26:12.000000 livemetrics-0.7/livemetrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)        1 2024-05-15 13:26:12.000000 livemetrics-0.7/livemetrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       79 2024-05-15 13:26:12.000000 livemetrics-0.7/livemetrics.egg-info/entry_points.txt
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       93 2024-05-15 13:26:12.000000 livemetrics-0.7/livemetrics.egg-info/requires.txt
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       12 2024-05-15 13:26:12.000000 livemetrics-0.7/livemetrics.egg-info/top_level.txt
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       90 2024-05-15 11:50:56.000000 livemetrics-0.7/pyproject.toml
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1025 2024-05-15 13:26:12.615226 livemetrics-0.7/setup.cfg
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)       37 2024-05-15 11:50:56.000000 livemetrics-0.7/setup.py
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.615226 livemetrics-0.7/tests/
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.615226 livemetrics-0.7/tests/dashboard/
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/dashboard/__init__.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      588 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/dashboard/client.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2311 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/dashboard/sample.yaml
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     1282 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/dashboard/server.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2860 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/dashboard/test_dashboard.py
+drwxrwxr-x   0 heurtier  (1000) heurtier  (1000)        0 2024-05-15 13:26:12.615226 livemetrics-0.7/tests/publishers/
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     6368 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/publishers/__init__.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2490 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/publishers/test_aiohttp.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2900 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/publishers/test_django.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2315 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/publishers/test_flask.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2574 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/publishers/test_http.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)      387 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/test_doc.py
+-rw-rw-r--   0 heurtier  (1000) heurtier  (1000)     2608 2024-05-15 11:50:56.000000 livemetrics-0.7/tests/test_metrics.py
```

### Comparing `livemetrics-0.6/PKG-INFO` & `livemetrics-0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,77 @@
 Metadata-Version: 2.1
 Name: livemetrics
-Version: 0.6
+Version: 0.7
 Summary: LiveMetrics collector and publisher for Python applications
 Home-page: https://github.com/idemia/python-livemetrics
-Author: Olivier Heurtier
+Author: attr: livemetrics.__author__
 Author-email: olivier.heurtier@idemia.com
 License: CeCILL-C
-Description: ===========
-        livemetrics
-        ===========
-        
-        .. image:: https://readthedocs.org/projects/livemetrics/badge/?version=latest
-            :target: https://livemetrics.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/pypi/l/livemetrics.svg
-            :target: https://pypi.org/project/livemetrics/
-            :alt: CeCILL-C
-        
-        .. image:: https://img.shields.io/pypi/v/livemetrics.svg
-            :target: https://pypi.org/project/livemetrics/
-            :alt: v?.?
-        
-        .. image:: https://img.shields.io/pypi/pyversions/livemetrics.svg
-            :target: https://pypi.org/project/livemetrics/
-            :alt: Python 3.x
-        
-        .. image:: https://travis-ci.org/idemia/python-livemetrics.svg?branch=master
-            :target: https://travis-ci.org/idemia/python-livemetrics
-            :alt: Build Status (Travis CI)
-        
-        .. image:: https://codecov.io/gh/idemia/python-livemetrics/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/idemia/python-livemetrics
-            :alt: Code Coverage Status (Codecov)
-        
-        A Python library for building and publishing live business metrics used to have insights
-        about the behavior of applications.
-        
-        It is based on the Dropwizard `metrics <https://metrics.dropwizard.io/>`_ library for Java.
-        
-        Installation
-        ============
-        
-        ``livemetrics`` is published on PyPI and can be installed from there::
-        
-            pip install -U livemetrics
-        
-        Quick Start
-        ===========
-        
-        
-        See `the full documentation <http://livemetrics.readthedocs.io/>`_ for more details.
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: CeCILL-C Free Software License Agreement (CECILL-C)
-Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+License-File: LICENSE
+License-File: AUTHORS.rst
+Requires-Dist: Pillow
 Provides-Extra: aiohttp
-Provides-Extra: dashboard
+Requires-Dist: aiohttp; extra == "aiohttp"
 Provides-Extra: django
+Requires-Dist: django; extra == "django"
 Provides-Extra: flask
+Requires-Dist: flask; extra == "flask"
+Provides-Extra: dashboard
+Requires-Dist: jinja2; extra == "dashboard"
+Requires-Dist: PyYAML; extra == "dashboard"
+Requires-Dist: aiohttp; extra == "dashboard"
+
+===========
+livemetrics
+===========
+
+.. image:: https://readthedocs.org/projects/livemetrics/badge/?version=latest
+    :target: https://livemetrics.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/l/livemetrics.svg
+    :target: https://pypi.org/project/livemetrics/
+    :alt: CeCILL-C
+
+.. image:: https://img.shields.io/pypi/v/livemetrics.svg
+    :target: https://pypi.org/project/livemetrics/
+    :alt: v?.?
+
+.. image:: https://img.shields.io/pypi/pyversions/livemetrics.svg
+    :target: https://pypi.org/project/livemetrics/
+    :alt: Python 3.x
+
+.. image:: https://github.com/idemia/python-livemetrics/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/idemia/python-livemetrics/actions/workflows/tests.yml
+    :alt: Github action
+
+.. image:: https://codecov.io/gh/idemia/python-livemetrics/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/idemia/python-livemetrics
+    :alt: Code Coverage Status (Codecov)
+
+A Python library for building and publishing live business metrics used to have insights
+about the behavior of applications.
+
+It is based on the Dropwizard `metrics <https://metrics.dropwizard.io/>`_ library for Java.
+
+Installation
+============
+
+``livemetrics`` is published on PyPI and can be installed from there::
+
+    pip install -U livemetrics
+
+Quick Start
+===========
+
+
+See `the full documentation <http://livemetrics.readthedocs.io/>`_ for more details.
+
+
```

### Comparing `livemetrics-0.6/README.rst` & `livemetrics-0.7/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     :target: https://pypi.org/project/livemetrics/
     :alt: v?.?
 
 .. image:: https://img.shields.io/pypi/pyversions/livemetrics.svg
     :target: https://pypi.org/project/livemetrics/
     :alt: Python 3.x
 
-.. image:: https://travis-ci.org/idemia/python-livemetrics.svg?branch=master
-    :target: https://travis-ci.org/idemia/python-livemetrics
-    :alt: Build Status (Travis CI)
+.. image:: https://github.com/idemia/python-livemetrics/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/idemia/python-livemetrics/actions/workflows/tests.yml
+    :alt: Github action
 
 .. image:: https://codecov.io/gh/idemia/python-livemetrics/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/idemia/python-livemetrics
     :alt: Code Coverage Status (Codecov)
 
 A Python library for building and publishing live business metrics used to have insights
 about the behavior of applications.
```

### Comparing `livemetrics-0.6/docs/_static/custom.css` & `livemetrics-0.7/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `livemetrics-0.6/docs/index.rst` & `livemetrics-0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `livemetrics-0.6/docs/modules.rst` & `livemetrics-0.7/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `livemetrics-0.6/livemetrics/__init__.py` & `livemetrics-0.7/livemetrics/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 import time
 import collections
 from functools import wraps
 import asyncio
 
 from livemetrics.metrics import *
 
-__version__ = '0.6'
+__version__ = '0.7'
 __author__ = "Olivier Heurtier"
 __copyright__ = "IDEMIA"
 __license__ = "CeCILL-C"
 
 if os.name=='posix':
     # XXX make it 2 values (one with data+stack only)
     def get_memory():
@@ -218,34 +218,36 @@
             return 0
 
 #______________________________________________________________________________
 class LiveMetrics(object):
     """
     An object to be used as a singleton to aggregate all live metrics of an application.
 
-    """
+    *version*: a string giving the version of the application
 
-    def __init__(self,version,about,is_healthy,is_ready=None,memory_and_cpu=True):
-        """
-        Contructor.
+    *about*: a string describing the application
 
-        *version*: a string giving the version of the application
+    *is_healthy*: a function called to know if the application is healthy or not.
+    Function must have no parameter and return a boolean.
 
-        *about*: a string describing the application
+    *is_ready*: a function called to know if the application is ready to process requests or not.
+    Function must have no parameter and return a boolean.
+    If None is provided, *is_healthy* is used.
+    
+    *memory_and_cpu*: a flag to activate gauges to report the memory (``memory``),
+    number of threads (``num_threads``) and CPU usage (``cpu``) on Linux only. Default is True.
+    
+    .. versionadded:: 0.7
+        *is_healthy* and *is_ready* can be coroutine if the publisher is ``aiohttp``.
 
-        *is_healthy*: a function called to know if the application is healthy or not.
-        Function must have no parameter and return a boolean.
+    """
 
-        *is_ready*: a function called to know if the application is ready to process requests or not.
-        Function must have no parameter and return a boolean.
-        If None is provided, *is_healthy* is used.
-        
-        *memory_and_cpu*: a flag to activate gauges to report the memory (``memory``),
-        number of threads (``num_threads``) and CPU usage (``cpu``) on Linux only. Default is True.
-        
+    def __init__(self,version,about,is_healthy,is_ready=None,memory_and_cpu=True):
+        """
+        Contructor.
         """
         self.version = version
         self.about = about
         self.is_healthy = is_healthy
         if not callable(self.is_healthy):
             self.is_healthy = lambda: is_healthy
 
@@ -271,22 +273,33 @@
         """
         self._meters[event][result].mark()
 
     def gauge(self,name,value):
         """
         Register a new gauge for this **name**. If **value** is a callable,
         it will be called everytime the gauge value is accessed.
+
+        Return the Gauge object.
+
+        .. versionadded:: 0.7
+            The Gauge object is returned.
         """
-        self._gauges[name].mark(value)
+        g = self._gauges.setdefault(name, Gauge(value))
+        return g
 
     def histogram(self,name,value):
         """
-        Register a new value in a histogram.
+        Register a new value in a histogram and return the Histogram object.
+
+        .. versionadded:: 0.7
+            The Histogram object is returned.
         """
-        self._histograms[name].update(value)
+        h = self._histograms.setdefault(name, Histogram())
+        h.update(value)
+        return h
 
     def timer(self,event,ok,error):
         """
         Decorator to automate meter and histogram on one event.
 
         *event*: the name of the event
```

### Comparing `livemetrics-0.6/livemetrics/metrics.py` & `livemetrics-0.7/livemetrics/metrics.py`

 * *Files identical despite different names*

### Comparing `livemetrics-0.6/livemetrics.egg-info/PKG-INFO` & `livemetrics-0.7/livemetrics.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,77 @@
 Metadata-Version: 2.1
 Name: livemetrics
-Version: 0.6
+Version: 0.7
 Summary: LiveMetrics collector and publisher for Python applications
 Home-page: https://github.com/idemia/python-livemetrics
-Author: Olivier Heurtier
+Author: attr: livemetrics.__author__
 Author-email: olivier.heurtier@idemia.com
 License: CeCILL-C
-Description: ===========
-        livemetrics
-        ===========
-        
-        .. image:: https://readthedocs.org/projects/livemetrics/badge/?version=latest
-            :target: https://livemetrics.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/pypi/l/livemetrics.svg
-            :target: https://pypi.org/project/livemetrics/
-            :alt: CeCILL-C
-        
-        .. image:: https://img.shields.io/pypi/v/livemetrics.svg
-            :target: https://pypi.org/project/livemetrics/
-            :alt: v?.?
-        
-        .. image:: https://img.shields.io/pypi/pyversions/livemetrics.svg
-            :target: https://pypi.org/project/livemetrics/
-            :alt: Python 3.x
-        
-        .. image:: https://travis-ci.org/idemia/python-livemetrics.svg?branch=master
-            :target: https://travis-ci.org/idemia/python-livemetrics
-            :alt: Build Status (Travis CI)
-        
-        .. image:: https://codecov.io/gh/idemia/python-livemetrics/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/idemia/python-livemetrics
-            :alt: Code Coverage Status (Codecov)
-        
-        A Python library for building and publishing live business metrics used to have insights
-        about the behavior of applications.
-        
-        It is based on the Dropwizard `metrics <https://metrics.dropwizard.io/>`_ library for Java.
-        
-        Installation
-        ============
-        
-        ``livemetrics`` is published on PyPI and can be installed from there::
-        
-            pip install -U livemetrics
-        
-        Quick Start
-        ===========
-        
-        
-        See `the full documentation <http://livemetrics.readthedocs.io/>`_ for more details.
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: CeCILL-C Free Software License Agreement (CECILL-C)
-Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+License-File: LICENSE
+License-File: AUTHORS.rst
+Requires-Dist: Pillow
 Provides-Extra: aiohttp
-Provides-Extra: dashboard
+Requires-Dist: aiohttp; extra == "aiohttp"
 Provides-Extra: django
+Requires-Dist: django; extra == "django"
 Provides-Extra: flask
+Requires-Dist: flask; extra == "flask"
+Provides-Extra: dashboard
+Requires-Dist: jinja2; extra == "dashboard"
+Requires-Dist: PyYAML; extra == "dashboard"
+Requires-Dist: aiohttp; extra == "dashboard"
+
+===========
+livemetrics
+===========
+
+.. image:: https://readthedocs.org/projects/livemetrics/badge/?version=latest
+    :target: https://livemetrics.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/l/livemetrics.svg
+    :target: https://pypi.org/project/livemetrics/
+    :alt: CeCILL-C
+
+.. image:: https://img.shields.io/pypi/v/livemetrics.svg
+    :target: https://pypi.org/project/livemetrics/
+    :alt: v?.?
+
+.. image:: https://img.shields.io/pypi/pyversions/livemetrics.svg
+    :target: https://pypi.org/project/livemetrics/
+    :alt: Python 3.x
+
+.. image:: https://github.com/idemia/python-livemetrics/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/idemia/python-livemetrics/actions/workflows/tests.yml
+    :alt: Github action
+
+.. image:: https://codecov.io/gh/idemia/python-livemetrics/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/idemia/python-livemetrics
+    :alt: Code Coverage Status (Codecov)
+
+A Python library for building and publishing live business metrics used to have insights
+about the behavior of applications.
+
+It is based on the Dropwizard `metrics <https://metrics.dropwizard.io/>`_ library for Java.
+
+Installation
+============
+
+``livemetrics`` is published on PyPI and can be installed from there::
+
+    pip install -U livemetrics
+
+Quick Start
+===========
+
+
+See `the full documentation <http://livemetrics.readthedocs.io/>`_ for more details.
+
+
```

### Comparing `livemetrics-0.6/livemetrics.egg-info/SOURCES.txt` & `livemetrics-0.7/livemetrics.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,27 @@
+AUTHORS.rst
+LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
+setup.cfg
 setup.py
 docs/conf.py
 docs/index.rst
 docs/modules.rst
 docs/requirements.txt
 docs/_static/custom.css
 livemetrics/__init__.py
 livemetrics/metrics.py
 livemetrics.egg-info/PKG-INFO
 livemetrics.egg-info/SOURCES.txt
 livemetrics.egg-info/dependency_links.txt
 livemetrics.egg-info/entry_points.txt
 livemetrics.egg-info/requires.txt
 livemetrics.egg-info/top_level.txt
-livemetrics/dashboard/dashboard.html
-livemetrics/dashboard/dashboard.py
-livemetrics/publishers/aiohttp.py
-livemetrics/publishers/django.py
-livemetrics/publishers/flask.py
-livemetrics/publishers/http.py
-tests/__init__.py
 tests/test_doc.py
 tests/test_metrics.py
 tests/dashboard/__init__.py
 tests/dashboard/client.py
 tests/dashboard/sample.yaml
 tests/dashboard/server.py
 tests/dashboard/test_dashboard.py
```

### Comparing `livemetrics-0.6/tests/dashboard/client.py` & `livemetrics-0.7/tests/dashboard/client.py`

 * *Files identical despite different names*

### Comparing `livemetrics-0.6/tests/dashboard/sample.yaml` & `livemetrics-0.7/tests/dashboard/sample.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   - type: empty
   - label: Time
     server: "{{server}}/metrics/histograms/time"
     type: histogram
     unit: ms
     factor: "*1000"
     color: "#ff000080"
-    median_color: green
+    median_color: "#00ff0080"
   - label: Test OK
     server: "{{server}}/metrics/meters/test/ok/rate1"
     type: gauge
     unit: "/h"
     factor: "*3600"
     gauge_color: green
     color: "#C0F0C0"
```

### Comparing `livemetrics-0.6/tests/dashboard/server.py` & `livemetrics-0.7/tests/dashboard/server.py`

 * *Files identical despite different names*

### Comparing `livemetrics-0.6/tests/dashboard/test_dashboard.py` & `livemetrics-0.7/tests/dashboard/test_dashboard.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,76 @@
 
 import os
 import unittest
 import time
 import threading
+import asyncio
 import http.server
 import requests
+import aiohttp
 
 from livemetrics.dashboard import dashboard
 
-def _serve_dashboard():
-    dashboard.main(['-i',os.path.join(os.path.dirname(__file__),'sample.yaml')])
+async def runner():
+    app = dashboard.get_app()
+    runner = aiohttp.web.AppRunner(app)
+    await runner.setup()
+
+    site = aiohttp.web.TCPSite(runner, '0.0.0.0', 9000,reuse_address=True)
+    await site.start()
+
+def run_server(handler):
+    global LOOP
+    loop = asyncio.new_event_loop()
+    LOOP = loop
+    asyncio.set_event_loop(loop)
+    loop.run_until_complete(handler)
+
+    try:
+        loop.run_forever()
+    finally:
+        loop.run_until_complete(loop.shutdown_asyncgens())
+        loop.close()
 
 from . import server
 from . import client
 
 #_______________________________________________________________________________
 class TestDashboard(unittest.TestCase):
     
     def setUp(self):
-        t = threading.Thread(target=_serve_dashboard, daemon=True)
-        t.start()
-        time.sleep(0.2)
+        self.t = threading.Thread(target=run_server,args=(runner(),) , daemon=True)
+        self.t.start()
+        time.sleep(1.0)
 
         t = threading.Thread(target=server._serve, daemon=True)
         t.start()
-        time.sleep(0.2)
+        time.sleep(1.0)
 
         t = threading.Thread(target=client.inject, daemon=True)
         t.start()
         time.sleep(1.0)
 
+    def tearDown(self):
+        # Clean up to release the socket address for the other tests
+        global LOOP
+        LOOP.stop()
+
     def test_all(self):
         # Send some events
         with requests.get('http://localhost:9000/') as r:
             self.assertEqual(200,r.status_code)
 
         payload = {'server': 'http://localhost:7070/monitoring/v1/is_healthy'}
         with requests.get('http://localhost:9000/all', params=payload) as r:
             self.assertEqual(200,r.status_code)
 
         payload = {'server': 'http://localhost:7070/monitoring/missing'}
         with requests.get('http://localhost:9000/all', params=payload) as r:
-            self.assertEqual(500,r.status_code)
+            self.assertEqual(404,r.status_code)
 
         payload = {'server': 'http://localhost:7070/monitoring/v1/metrics/meters/test/ok'}
         with requests.get('http://localhost:9000/all', params=payload) as r:
             self.assertEqual(200,r.status_code)
             self.assertGreater(r.json()['count'],2)
 
         payload = {'server': 'http://localhost:7070/monitoring/v1/metrics/histograms'}
```

### Comparing `livemetrics-0.6/tests/publishers/__init__.py` & `livemetrics-0.7/tests/publishers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,33 +91,36 @@
 
         # Test with a bad status
         backup_ih = self.LM.is_healthy
         self.LM.is_healthy = lambda: False
 
         backup_ir = self.LM.is_ready
         self.LM.is_ready = lambda: False
+        requests.get('http://'+IP+':'+PORT+'/switch')
 
         with requests.get('http://'+IP+':'+PORT+'/monitoring/v1/is_healthy') as r:
             self.assertEqual(500,r.status_code)
         with requests.get('http://'+IP+':'+PORT+'/monitoring/v1/is_ready') as r:
             self.assertEqual(500,r.status_code)
 
         self.LM.is_healthy = backup_ih
         self.LM.is_ready = backup_ir
+        requests.get('http://'+IP+':'+PORT+'/switch')
 
         # Test memory & CPU
         if not os.name=='posix':
             return
 
         with requests.get('http://'+IP+':'+PORT+'/monitoring/v1/metrics/gauges/memory/count') as r:
             self.assertGreater(r.json(),20000000)
 
         with requests.get('http://'+IP+':'+PORT+'/monitoring/v1/metrics/gauges/num_threads/count') as r:
             self.assertGreater(r.json(),2)
-            self.assertLess(r.json(),10)
+            self.assertLess(r.json(),15)
 
         with requests.get('http://'+IP+':'+PORT+'/monitoring/v1/metrics/gauges/cpu/count') as r:
             cpu = r.json()
         with requests.get('http://'+IP+':'+PORT+'/monitoring/v1/metrics/gauges/cpu/count') as r:
             self.assertEqual(cpu,r.json())
         time.sleep(0.5)
         requests.get('http://'+IP+':'+PORT+'/monitoring/v1/metrics/gauges/cpu/count')
+
```

### Comparing `livemetrics-0.6/tests/publishers/test_aiohttp.py` & `livemetrics-0.7/tests/publishers/test_aiohttp.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 routes = web.RouteTableDef()
 
 import livemetrics
 import livemetrics.publishers.aiohttp
 
 import tests.publishers
 
-LM = livemetrics.LiveMetrics('{"version":"1.0"}',"Test server",True, True)
+async def is_healthy():
+    return True
+
+LM = livemetrics.LiveMetrics('{"version":"1.0"}',"Test server",is_healthy, True)
 
 # Sample of gauges
 LM.gauge('fixed',10)
 LM.gauge('test',10)
 LM.gauge('call',lambda: random.randrange(100,1000))
 
 #______________________________________________________________________________
@@ -75,17 +78,17 @@
         loop.run_until_complete(loop.shutdown_asyncgens())
         loop.close()
 
 #_______________________________________________________________________________
 class TestAioHttp(tests.publishers.TestPublisher):
     
     def setUp(self):
-        self.t = threading.Thread(target=run_server,args=(runner(),) , daemon=False)
+        self.t = threading.Thread(target=run_server,args=(runner(),) , daemon=True)
         self.t.start()
-        time.sleep(0.2)
+        time.sleep(1.0)
         self.LM = LM
 
     def tearDown(self):
         # Clean up to release the socket address for the other tests
         global LOOP
         LOOP.stop()
```

### Comparing `livemetrics-0.6/tests/publishers/test_django.py` & `livemetrics-0.7/tests/publishers/test_django.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,16 +44,28 @@
     LM.histogram("histo",random.random()*20)
     global COUNT
     COUNT += 1
     if COUNT % 3 ==0:
         raise Exception("false-alert")
     return HttpResponse("OK")
 
+def switchview(request):
+    global LM
+    if LM.is_healthy():
+        LM.is_healthy = lambda: False
+    else:
+        LM.is_healthy = lambda: True
+    if LM.is_ready():
+        LM.is_ready = lambda: False
+    else:
+        LM.is_ready = lambda: True
+
 urlpatterns = [
     path('test', myview, name='test'),
+    path('switch', switchview, name='switch'),
 ]
 
 urlpatterns += livemetrics.publishers.django.urlpatterns(LM)
 
 def _serve():
     from django.conf import settings
 
@@ -88,13 +100,13 @@
 #_______________________________________________________________________________
 class TestDjango(tests.publishers.TestPublisher):
     
     def setUp(self):
         global LM
         self.t = threading.Thread(target=_serve , daemon=True)
         self.t.start()
-        time.sleep(0.2)
+        time.sleep(1.0)
         self.LM = LM
 
 # ______________________________________________________________________________
 if __name__=='__main__':
     unittest.main(argv=['-v'])
```

### Comparing `livemetrics-0.6/tests/publishers/test_flask.py` & `livemetrics-0.7/tests/publishers/test_flask.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,17 @@
     app.register_blueprint(livemetrics.publishers.flask.blueprint(LM))
     app.run(host=tests.publishers.IP, port=int(tests.publishers.PORT))
 
 #_______________________________________________________________________________
 class TestFlask(tests.publishers.TestPublisher):
     
     def setUp(self):
-        self.t = threading.Thread(target=_serve , daemon=False)
+        self.t = threading.Thread(target=_serve , daemon=True)
         self.t.start()
-        time.sleep(0.2)
+        time.sleep(1.0)
         self.LM = LM
 
     def tearDown(self):
         # Clean up to release the socket address for the other tests
         requests.post('http://'+tests.publishers.IP+':'+tests.publishers.PORT+'/shutdown')
```

### Comparing `livemetrics-0.6/tests/publishers/test_http.py` & `livemetrics-0.7/tests/publishers/test_http.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,31 +59,33 @@
                 self.end_headers()
         else:
             return super().do_GET()
 
     def log_message(self, format, *args):
         pass
         
+TestHTTPRequestHandler.__test__ = False
+
 def _serve():
     global LM
     tests.publishers.PORT = '8765'
     server_address = (tests.publishers.IP, int(tests.publishers.PORT))
     httpd = http.server.HTTPServer(server_address, lambda r,a,s: TestHTTPRequestHandler(LM,r,a,s))
     global HTTPD
     HTTPD = httpd
     httpd.allow_reuse_address = True
     httpd.serve_forever()
 
 #_______________________________________________________________________________
 class TestHttp(tests.publishers.TestPublisher):
     
     def setUp(self):
-        t = threading.Thread(target=_serve, daemon=False)
+        t = threading.Thread(target=_serve, daemon=True)
         t.start()
-        time.sleep(0.2)
+        time.sleep(1.0)
         self.LM = LM
 
     def tearDown(self):
         # Clean up to release the socket address for the other tests
         global HTTPD
         HTTPD.shutdown()
```

### Comparing `livemetrics-0.6/tests/test_metrics.py` & `livemetrics-0.7/tests/test_metrics.py`

 * *Files identical despite different names*

