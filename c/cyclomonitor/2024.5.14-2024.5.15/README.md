# Comparing `tmp/cyclomonitor-2024.5.14.tar.gz` & `tmp/cyclomonitor-2024.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclomonitor-2024.5.14.tar", last modified: Tue May 14 00:21:02 2024, max compression
+gzip compressed data, was "cyclomonitor-2024.5.15.tar", last modified: Wed May 15 12:38:09 2024, max compression
```

## Comparing `cyclomonitor-2024.5.14.tar` & `cyclomonitor-2024.5.15.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.307294 cyclomonitor-2024.5.14/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    34523 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.14/LICENSE
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      263 2024-04-14 18:11:55.000000 cyclomonitor-2024.5.14/MANIFEST.in
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    43427 2024-05-14 00:21:02.307294 cyclomonitor-2024.5.14/PKG-INFO
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     2069 2024-05-13 03:01:31.000000 cyclomonitor-2024.5.14/README.md
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      640 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.14/privacy-policy.md
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     1574 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.14/pyproject.toml
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)       15 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.14/requirements.txt
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)       38 2024-05-14 00:21:02.311294 cyclomonitor-2024.5.14/setup.cfg
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     1834 2024-05-14 00:11:33.000000 cyclomonitor-2024.5.14/setup.py
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.299294 cyclomonitor-2024.5.14/src/
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.303294 cyclomonitor-2024.5.14/src/cyclomonitor/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      189 2024-04-15 00:43:27.000000 cyclomonitor-2024.5.14/src/cyclomonitor/__init__.py
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     4713 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.14/src/cyclomonitor/__main__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    10835 2024-05-13 02:20:38.000000 cyclomonitor-2024.5.14/src/cyclomonitor/atcf.py
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    12462 2024-05-13 23:49:46.000000 cyclomonitor-2024.5.14/src/cyclomonitor/cli.py
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    35681 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.14/src/cyclomonitor/cyclomonitor.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1050 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.14/src/cyclomonitor/dir_calc.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      239 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.14/src/cyclomonitor/errors.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      801 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/global_vars.py
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.303294 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    13524 2024-05-13 23:52:17.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      185 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/__main__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5008 2024-05-13 23:49:26.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/ibtracs_ALL.sql
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5012 2024-05-13 23:49:25.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.307294 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/C.json
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1945 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/en_US.json
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.307294 cyclomonitor-2024.5.14/src/cyclomonitor/locales/
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    14230 2024-05-13 22:53:22.000000 cyclomonitor-2024.5.14/src/cyclomonitor/locales/C.json
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     7862 2024-05-13 22:50:42.000000 cyclomonitor-2024.5.14/src/cyclomonitor/locales/__init__.py
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    14230 2024-05-13 22:53:22.000000 cyclomonitor-2024.5.14/src/cyclomonitor/locales/en_US.json
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1794 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/server_vars.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1192 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.14/src/cyclomonitor/uptime.py
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-14 00:21:02.307294 cyclomonitor-2024.5.14/src/cyclomonitor.egg-info/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      767 2024-05-14 00:21:02.000000 cyclomonitor-2024.5.14/src/cyclomonitor.egg-info/SOURCES.txt
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.638745 cyclomonitor-2024.5.15/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    34523 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.15/LICENSE
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      263 2024-04-14 18:11:55.000000 cyclomonitor-2024.5.15/MANIFEST.in
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    43427 2024-05-15 12:38:09.638745 cyclomonitor-2024.5.15/PKG-INFO
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     2069 2024-05-13 03:01:31.000000 cyclomonitor-2024.5.15/README.md
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      640 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.15/privacy-policy.md
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     1574 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.15/pyproject.toml
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)       15 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.15/requirements.txt
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)       38 2024-05-15 12:38:09.638745 cyclomonitor-2024.5.15/setup.cfg
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     1834 2024-05-15 12:35:47.000000 cyclomonitor-2024.5.15/setup.py
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.630746 cyclomonitor-2024.5.15/src/
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.634745 cyclomonitor-2024.5.15/src/cyclomonitor/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      189 2024-04-15 00:43:27.000000 cyclomonitor-2024.5.15/src/cyclomonitor/__init__.py
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     4713 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.15/src/cyclomonitor/__main__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    10874 2024-05-15 12:28:39.000000 cyclomonitor-2024.5.15/src/cyclomonitor/atcf.py
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    12462 2024-05-15 12:29:29.000000 cyclomonitor-2024.5.15/src/cyclomonitor/cli.py
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    35681 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.15/src/cyclomonitor/cyclomonitor.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1050 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.15/src/cyclomonitor/dir_calc.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      239 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.15/src/cyclomonitor/errors.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      801 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/global_vars.py
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.634745 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    13524 2024-05-13 23:52:17.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      185 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/__main__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5008 2024-05-13 23:49:26.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/ibtracs_ALL.sql
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5012 2024-05-13 23:49:25.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.638745 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/C.json
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1945 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/en_US.json
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.638745 cyclomonitor-2024.5.15/src/cyclomonitor/locales/
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    14230 2024-05-13 22:53:22.000000 cyclomonitor-2024.5.15/src/cyclomonitor/locales/C.json
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     7862 2024-05-13 22:50:42.000000 cyclomonitor-2024.5.15/src/cyclomonitor/locales/__init__.py
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    14230 2024-05-13 22:53:22.000000 cyclomonitor-2024.5.15/src/cyclomonitor/locales/en_US.json
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1794 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/server_vars.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1192 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/uptime.py
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.638745 cyclomonitor-2024.5.15/src/cyclomonitor.egg-info/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      767 2024-05-15 12:38:09.000000 cyclomonitor-2024.5.15/src/cyclomonitor.egg-info/SOURCES.txt
```

### Comparing `cyclomonitor-2024.5.14/LICENSE` & `cyclomonitor-2024.5.15/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/PKG-INFO` & `cyclomonitor-2024.5.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclomonitor
-Version: 2024.5.14
+Version: 2024.5.15
 Summary: Discord bot that helps you keep tabs on tropical cyclones.
 Home-page: https://github.com/ntvmb/cyclomonitor
 Author: Nathaniel Greenwell
 Author-email: Nathaniel Greenwell <nategreenwell@live.com>
 Maintainer-email: Nathaniel Greenwell <nategreenwell@live.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

### Comparing `cyclomonitor-2024.5.14/README.md` & `cyclomonitor-2024.5.15/README.md`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/privacy-policy.md` & `cyclomonitor-2024.5.15/privacy-policy.md`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/pyproject.toml` & `cyclomonitor-2024.5.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/setup.py` & `cyclomonitor-2024.5.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import pathlib
 
-__version__ = "2024.5.14"
+__version__ = "2024.5.15"
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
```

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/__main__.py` & `cyclomonitor-2024.5.15/src/cyclomonitor/__main__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/atcf.py` & `cyclomonitor-2024.5.15/src/cyclomonitor/atcf.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,27 +75,27 @@
     print("CLI coming soon")
 
 
 def reset():
     """Reset ATCF data."""
     global cyclones, names, timestamps, lats, longs, basins, winds, pressures
     global tc_classes, lats_real, longs_real, movement_speeds, movement_dirs
-    cyclones = []
-    names = []
-    timestamps = []
-    lats = []
-    longs = []
-    basins = []
-    winds = []
-    pressures = []
-    tc_classes = []
-    lats_real = []
-    longs_real = []
-    movement_speeds = []
-    movement_dirs = []
+    cyclones.clear()
+    names.clear()
+    timestamps.clear()
+    lats.clear()
+    longs.clear()
+    basins.clear()
+    winds.clear()
+    pressures.clear()
+    tc_classes.clear()
+    lats_real.clear()
+    longs_real.clear()
+    movement_speeds.clear()
+    movement_dirs.clear()
 
 
 def parse_storm(line: str, *, mode="std"):
     """Parse ATCF data.
 
     Arguments:
     line -- the data to be parsed
```

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/cli.py` & `cyclomonitor-2024.5.15/src/cyclomonitor/cli.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/cyclomonitor.py` & `cyclomonitor-2024.5.15/src/cyclomonitor/cyclomonitor.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/dir_calc.py` & `cyclomonitor-2024.5.15/src/cyclomonitor/dir_calc.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/global_vars.py` & `cyclomonitor-2024.5.15/src/cyclomonitor/global_vars.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/__init__.py` & `cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/ibtracs_ALL.sql` & `cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/ibtracs_ALL.sql`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql` & `cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/C.json` & `cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/C.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/__init__.py` & `cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/ibtracs/locales/en_US.json` & `cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/en_US.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/locales/C.json` & `cyclomonitor-2024.5.15/src/cyclomonitor/locales/C.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/locales/__init__.py` & `cyclomonitor-2024.5.15/src/cyclomonitor/locales/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/locales/en_US.json` & `cyclomonitor-2024.5.15/src/cyclomonitor/locales/en_US.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/server_vars.py` & `cyclomonitor-2024.5.15/src/cyclomonitor/server_vars.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor/uptime.py` & `cyclomonitor-2024.5.15/src/cyclomonitor/uptime.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.14/src/cyclomonitor.egg-info/SOURCES.txt` & `cyclomonitor-2024.5.15/src/cyclomonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

