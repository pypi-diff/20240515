# Comparing `tmp/volue-insight-timeseries-1.0.4.tar.gz` & `tmp/volue-insight-timeseries-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volue-insight-timeseries-1.0.4.tar", last modified: Mon Dec 11 10:05:14 2023, max compression
+gzip compressed data, was "volue-insight-timeseries-1.0.5.tar", last modified: Fri Jan 26 13:51:06 2024, max compression
```

## Comparing `volue-insight-timeseries-1.0.4.tar` & `volue-insight-timeseries-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 10:05:14.719100 volue-insight-timeseries-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-11 10:05:08.000000 volue-insight-timeseries-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-11 10:05:08.000000 volue-insight-timeseries-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-12-11 10:05:14.719100 volue-insight-timeseries-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2023-12-11 10:05:08.000000 volue-insight-timeseries-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-11 10:05:14.719100 volue-insight-timeseries-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-12-11 10:05:08.000000 volue-insight-timeseries-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 10:05:14.719100 volue-insight-timeseries-1.0.4/volue_insight_timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-11 10:05:08.000000 volue-insight-timeseries-1.0.4/volue_insight_timeseries/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-11 10:05:08.000000 volue-insight-timeseries-1.0.4/volue_insight_timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2023-12-11 10:05:08.000000 volue-insight-timeseries-1.0.4/volue_insight_timeseries/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    65949 2023-12-11 10:05:08.000000 volue-insight-timeseries-1.0.4/volue_insight_timeseries/curves.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2023-12-11 10:05:08.000000 volue-insight-timeseries-1.0.4/volue_insight_timeseries/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    20124 2023-12-11 10:05:08.000000 volue-insight-timeseries-1.0.4/volue_insight_timeseries/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9301 2023-12-11 10:05:08.000000 volue-insight-timeseries-1.0.4/volue_insight_timeseries/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 10:05:14.719100 volue-insight-timeseries-1.0.4/volue_insight_timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-12-11 10:05:14.000000 volue-insight-timeseries-1.0.4/volue_insight_timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-11 10:05:14.000000 volue-insight-timeseries-1.0.4/volue_insight_timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 10:05:14.000000 volue-insight-timeseries-1.0.4/volue_insight_timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-11 10:05:14.000000 volue-insight-timeseries-1.0.4/volue_insight_timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-11 10:05:14.000000 volue-insight-timeseries-1.0.4/volue_insight_timeseries.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:51:06.187474 volue-insight-timeseries-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-26 13:50:58.000000 volue-insight-timeseries-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-26 13:50:58.000000 volue-insight-timeseries-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-26 13:51:06.187474 volue-insight-timeseries-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-01-26 13:50:58.000000 volue-insight-timeseries-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-26 13:51:06.187474 volue-insight-timeseries-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-01-26 13:50:58.000000 volue-insight-timeseries-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:51:06.187474 volue-insight-timeseries-1.0.5/volue_insight_timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-26 13:50:58.000000 volue-insight-timeseries-1.0.5/volue_insight_timeseries/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-26 13:50:58.000000 volue-insight-timeseries-1.0.5/volue_insight_timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-01-26 13:50:58.000000 volue-insight-timeseries-1.0.5/volue_insight_timeseries/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65949 2024-01-26 13:50:58.000000 volue-insight-timeseries-1.0.5/volue_insight_timeseries/curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-01-26 13:50:58.000000 volue-insight-timeseries-1.0.5/volue_insight_timeseries/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20124 2024-01-26 13:50:58.000000 volue-insight-timeseries-1.0.5/volue_insight_timeseries/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-01-26 13:50:58.000000 volue-insight-timeseries-1.0.5/volue_insight_timeseries/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:51:06.187474 volue-insight-timeseries-1.0.5/volue_insight_timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-26 13:51:06.000000 volue-insight-timeseries-1.0.5/volue_insight_timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-26 13:51:06.000000 volue-insight-timeseries-1.0.5/volue_insight_timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 13:51:06.000000 volue-insight-timeseries-1.0.5/volue_insight_timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-26 13:51:06.000000 volue-insight-timeseries-1.0.5/volue_insight_timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-26 13:51:06.000000 volue-insight-timeseries-1.0.5/volue_insight_timeseries.egg-info/top_level.txt
```

### Comparing `volue-insight-timeseries-1.0.4/LICENSE` & `volue-insight-timeseries-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.4/PKG-INFO` & `volue-insight-timeseries-1.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volue-insight-timeseries
-Version: 1.0.4
+Version: 1.0.5
 Summary: Volue Insight API python library
 Home-page: https://www.volueinsight.com
 Author: Volue Insight
 Author-email: support.insight@volue.com
 Requires-Python: >=3.9, <3.12a0
 License-File: LICENSE
```

### Comparing `volue-insight-timeseries-1.0.4/README.md` & `volue-insight-timeseries-1.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 The library is tested against Python 3.9, 3.10 and 3.11 - we recommend using 
 the latest Python version.
 
 
 ## Documentation
 
 The 
-[documentation](https://wattsight-volue-insight-timeseries.readthedocs-hosted.com/en/latest/ 
+[documentation](https://wattsight-volue-insight-timeseries.readthedocs-hosted.com/en/master/) 
 with various 
-[examples](https://wattsight-volue-insight-timeseries.readthedocs-hosted.com/en/latest/examples.html)
+[examples](https://wattsight-volue-insight-timeseries.readthedocs-hosted.com/en/master/examples.html)
 is hosted on Read the Docs.
 
 ## Installation
 
 You can simply install/update the latest version of Volue Insight API python
 library with pip.
 Start a terminal (a shell) and use the following command
```

### Comparing `volue-insight-timeseries-1.0.4/setup.py` & `volue-insight-timeseries-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.4/volue_insight_timeseries/auth.py` & `volue-insight-timeseries-1.0.5/volue_insight_timeseries/auth.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.4/volue_insight_timeseries/curves.py` & `volue-insight-timeseries-1.0.5/volue_insight_timeseries/curves.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.4/volue_insight_timeseries/events.py` & `volue-insight-timeseries-1.0.5/volue_insight_timeseries/events.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.4/volue_insight_timeseries/session.py` & `volue-insight-timeseries-1.0.5/volue_insight_timeseries/session.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.4/volue_insight_timeseries/util.py` & `volue-insight-timeseries-1.0.5/volue_insight_timeseries/util.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.4/volue_insight_timeseries.egg-info/PKG-INFO` & `volue-insight-timeseries-1.0.5/volue_insight_timeseries.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volue-insight-timeseries
-Version: 1.0.4
+Version: 1.0.5
 Summary: Volue Insight API python library
 Home-page: https://www.volueinsight.com
 Author: Volue Insight
 Author-email: support.insight@volue.com
 Requires-Python: >=3.9, <3.12a0
 License-File: LICENSE
```

### Comparing `volue-insight-timeseries-1.0.4/volue_insight_timeseries.egg-info/SOURCES.txt` & `volue-insight-timeseries-1.0.5/volue_insight_timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

