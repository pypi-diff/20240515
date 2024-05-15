# Comparing `tmp/aiidalab_widgets_base-2.2.1.tar.gz` & `tmp/aiidalab_widgets_base-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiidalab_widgets_base-2.2.1.tar", last modified: Mon May  6 09:16:49 2024, max compression
+gzip compressed data, was "aiidalab_widgets_base-2.2.2.tar", last modified: Wed May 15 15:02:25 2024, max compression
```

## Comparing `aiidalab_widgets_base-2.2.1.tar` & `aiidalab_widgets_base-2.2.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:16:49.167941 aiidalab_widgets_base-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-06 09:16:49.167941 aiidalab_widgets_base-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:16:49.159941 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    70960 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/computational_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:16:49.159941 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15852 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/elns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    29520 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/process.py
--rw-r--r--   0 runner    (1001) docker     (127)    60005 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:16:49.159941 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    60452 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:16:49.163941 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-06 09:16:49.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-06 09:16:49.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:16:49.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:16:48.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-06 09:16:49.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 09:16:49.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-06 09:16:49.167941 aiidalab_widgets_base-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:16:49.163941 aiidalab_widgets_base-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    30474 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_computational_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_elns.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:02:25.298485 aiidalab_widgets_base-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-15 15:02:25.298485 aiidalab_widgets_base-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:02:25.294485 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70960 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/computational_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:02:25.294485 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15832 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/elns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29520 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60005 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:02:25.294485 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60452 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:02:25.294485 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-15 15:02:25.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-15 15:02:25.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:02:25.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:02:25.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 15:02:25.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 15:02:25.000000 aiidalab_widgets_base-2.2.2/aiidalab_widgets_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-15 15:02:25.298485 aiidalab_widgets_base-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:02:25.294485 aiidalab_widgets_base-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/tests/test_bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30474 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/tests/test_computational_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/tests/test_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/tests/test_elns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/tests/test_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-15 15:02:21.000000 aiidalab_widgets_base-2.2.2/tests/test_wizard.py
```

### Comparing `aiidalab_widgets_base-2.2.1/LICENSE.txt` & `aiidalab_widgets_base-2.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/PKG-INFO` & `aiidalab_widgets_base-2.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiidalab_widgets_base
-Version: 2.2.1
+Version: 2.2.2
 Summary: Reusable widgets for AiiDAlab applications.
 Home-page: https://github.com/aiidalab/aiidalab-widgets-base
 Author: The AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
```

### Comparing `aiidalab_widgets_base-2.2.1/README.md` & `aiidalab_widgets_base-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/__init__.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,8 +113,8 @@
     "SubmitButtonWidget",
     "WizardAppWidget",
     "WizardAppWidgetStep",
     "register_viewer_widget",
     "viewer",
 ]
 
-__version__ = "2.2.1"
+__version__ = "2.2.2"
```

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/bug_report.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/bug_report.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/computational_resources.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/computational_resources.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/data/__init__.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/databases.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/databases.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,17 +349,15 @@
                     if domain_value.get("default") == computer:
                         # also remove default computer from domain
                         del domain_value["default"]
 
             if len(domain_value) == 0:
                 # remove domain since no computers with required codes defined in this domain source
                 del database[domain]
-                continue
-
-            if domain_value["default"] not in domain_value:
+            elif domain_value.get("default") not in domain_value:
                 # make sure default computer is still points to existing computer
                 domain_value["default"] = sorted(domain_value.keys() - {"default"})[0]
 
         return database
 
     def _domain_changed(self, change=None):
         """callback when new domain selected"""
```

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/dicts.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/dicts.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/elns.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/elns.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/export.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/export.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/misc.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/misc.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/nodes.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/nodes.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/process.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/process.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/structures.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/structures.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/utils/__init__.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/viewers.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/viewers.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/wizard.py` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base/wizard.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/PKG-INFO` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiidalab_widgets_base
-Version: 2.2.1
+Version: 2.2.2
 Summary: Reusable widgets for AiiDAlab applications.
 Home-page: https://github.com/aiidalab/aiidalab-widgets-base
 Author: The AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
```

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/SOURCES.txt` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/requires.txt` & `aiidalab_widgets_base-2.2.2/aiidalab_widgets_base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/pyproject.toml` & `aiidalab_widgets_base-2.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/setup.cfg` & `aiidalab_widgets_base-2.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 docs = 
 	sphinx
 	sphinx-design
 	pydata-sphinx-theme
 	myst-nb
 
 [bumpver]
-current_version = "v2.2.1"
+current_version = "v2.2.2"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
```

### Comparing `aiidalab_widgets_base-2.2.1/tests/test_bug_report.py` & `aiidalab_widgets_base-2.2.2/tests/test_bug_report.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/tests/test_computational_resources.py` & `aiidalab_widgets_base-2.2.2/tests/test_computational_resources.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/tests/test_databases.py` & `aiidalab_widgets_base-2.2.2/tests/test_databases.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/tests/test_elns.py` & `aiidalab_widgets_base-2.2.2/tests/test_elns.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/tests/test_export.py` & `aiidalab_widgets_base-2.2.2/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/tests/test_nodes.py` & `aiidalab_widgets_base-2.2.2/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/tests/test_process.py` & `aiidalab_widgets_base-2.2.2/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/tests/test_structures.py` & `aiidalab_widgets_base-2.2.2/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/tests/test_viewers.py` & `aiidalab_widgets_base-2.2.2/tests/test_viewers.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.1/tests/test_wizard.py` & `aiidalab_widgets_base-2.2.2/tests/test_wizard.py`

 * *Files identical despite different names*

