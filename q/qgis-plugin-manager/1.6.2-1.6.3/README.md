# Comparing `tmp/qgis-plugin-manager-1.6.2.tar.gz` & `tmp/qgis-plugin-manager-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgis-plugin-manager-1.6.2.tar", last modified: Wed May 15 08:48:59 2024, max compression
+gzip compressed data, was "qgis-plugin-manager-1.6.3.tar", last modified: Wed May 15 10:19:26 2024, max compression
```

## Comparing `qgis-plugin-manager-1.6.2.tar` & `qgis-plugin-manager-1.6.3.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:48:59.836010 qgis-plugin-manager-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-15 08:48:59.832010 qgis-plugin-manager-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-15 08:48:57.000000 qgis-plugin-manager-1.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:48:59.832010 qgis-plugin-manager-1.6.2/qgis_plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-15 08:48:57.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6653 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19417 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:48:59.832010 qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-15 08:48:59.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-15 08:48:59.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:48:59.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 08:48:59.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 08:48:59.000000 qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:48:59.836010 qgis-plugin-manager-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-15 08:48:57.000000 qgis-plugin-manager-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:48:59.832010 qgis-plugin-manager-1.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/test/test_full_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/test/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/test/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-15 08:48:55.000000 qgis-plugin-manager-1.6.2/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:19:26.560993 qgis-plugin-manager-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-15 10:19:26.560993 qgis-plugin-manager-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:19:26.560993 qgis-plugin-manager-1.6.3/qgis_plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-15 10:19:25.000000 qgis-plugin-manager-1.6.3/qgis_plugin_manager/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/qgis_plugin_manager/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6653 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/qgis_plugin_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/qgis_plugin_manager/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/qgis_plugin_manager/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19417 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/qgis_plugin_manager/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/qgis_plugin_manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:19:26.560993 qgis-plugin-manager-1.6.3/qgis_plugin_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-15 10:19:26.000000 qgis-plugin-manager-1.6.3/qgis_plugin_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-15 10:19:26.000000 qgis-plugin-manager-1.6.3/qgis_plugin_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:19:26.000000 qgis-plugin-manager-1.6.3/qgis_plugin_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 10:19:26.000000 qgis-plugin-manager-1.6.3/qgis_plugin_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 10:19:26.000000 qgis-plugin-manager-1.6.3/qgis_plugin_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 10:19:26.560993 qgis-plugin-manager-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-15 10:19:24.000000 qgis-plugin-manager-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:19:26.560993 qgis-plugin-manager-1.6.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/test/test_full_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/test/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/test/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-15 10:19:22.000000 qgis-plugin-manager-1.6.3/test/test_utils.py
```

### Comparing `qgis-plugin-manager-1.6.2/LICENSE` & `qgis-plugin-manager-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.2/PKG-INFO` & `qgis-plugin-manager-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qgis-plugin-manager
-Version: 1.6.2
+Version: 1.6.3
 Summary: Tool for downloading/managing QGIS plugins from CLI.
 Home-page: https://github.com/3liz/qgis-plugin-manager
-Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.2.tar.gz
+Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.3.tar.gz
 Author: Étienne Trimaille
 Author-email: etrimaille@3liz.com
 Project-URL: Docs, https://github.com/3liz/qgis-plugin-manager/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/3liz/qgis-plugin-manager/issues/
 Project-URL: Source, https://github.com/3liz/qgis-plugin-manager
 Keywords: QGIS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qgis-plugin-manager-1.6.2/README.md` & `qgis-plugin-manager-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.2/qgis_plugin_manager/__about__.py` & `qgis-plugin-manager-1.6.3/qgis_plugin_manager/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 __license__ = "GNU General Public License v3.0"
 __summary__ = "Tool for downloading/managing QGIS plugins from CLI."
 __title__ = "QGIS Plugin Manager"
 __title_clean__ = "".join(e for e in __title__ if e.isalnum())
 __uri__ = "https://github.com/3liz/qgis-plugin-manager"
 
 # This string might be updated on CI on runtime with a proper semantic version name with X.Y.Z
-__version__ = "1.6.2"
+__version__ = "1.6.3"
 
 if "." not in __version__:
     # If __version__ is still not a proper semantic versioning with X.Y.Z
     # let's hardcode 0.0.0
     __version__ = "0.0.0"
 
 __version_info__ = tuple(
```

### Comparing `qgis-plugin-manager-1.6.2/qgis_plugin_manager/__main__.py` & `qgis-plugin-manager-1.6.3/qgis_plugin_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.2/qgis_plugin_manager/definitions.py` & `qgis-plugin-manager-1.6.3/qgis_plugin_manager/definitions.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.2/qgis_plugin_manager/local_directory.py` & `qgis-plugin-manager-1.6.3/qgis_plugin_manager/local_directory.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.2/qgis_plugin_manager/remote.py` & `qgis-plugin-manager-1.6.3/qgis_plugin_manager/remote.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.2/qgis_plugin_manager/utils.py` & `qgis-plugin-manager-1.6.3/qgis_plugin_manager/utils.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/PKG-INFO` & `qgis-plugin-manager-1.6.3/qgis_plugin_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qgis-plugin-manager
-Version: 1.6.2
+Version: 1.6.3
 Summary: Tool for downloading/managing QGIS plugins from CLI.
 Home-page: https://github.com/3liz/qgis-plugin-manager
-Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.2.tar.gz
+Download-URL: https://github.com/3liz/qgis-plugin-manager/archive/1.6.3.tar.gz
 Author: Étienne Trimaille
 Author-email: etrimaille@3liz.com
 Project-URL: Docs, https://github.com/3liz/qgis-plugin-manager/blob/master/README.md
 Project-URL: Bug Reports, https://github.com/3liz/qgis-plugin-manager/issues/
 Project-URL: Source, https://github.com/3liz/qgis-plugin-manager
 Keywords: QGIS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qgis-plugin-manager-1.6.2/qgis_plugin_manager.egg-info/SOURCES.txt` & `qgis-plugin-manager-1.6.3/qgis_plugin_manager.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 setup.py
 qgis_plugin_manager/__about__.py
 qgis_plugin_manager/__init__.py
 qgis_plugin_manager/__main__.py
 qgis_plugin_manager/definitions.py
 qgis_plugin_manager/local_directory.py
 qgis_plugin_manager/remote.py
```

### Comparing `qgis-plugin-manager-1.6.2/setup.py` & `qgis-plugin-manager-1.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     sys.exit(
         "qgis-plugin-manager requires at least Python version "
         f"{python_min_version[0]}.{python_min_version[1]}.\n"
         f"You are currently running this installation with\n\n{sys.version}",
     )
 
 # This string might be updated on CI on runtime with a proper semantic version name with X.Y.Z
-VERSION = "1.6.2"
+VERSION = "1.6.3"
 
 if "." not in VERSION:
     # If VERSION is still not a proper semantic versioning with X.Y.Z
     # let's hardcode 0.0.0
     VERSION = "0.0.0"
 
 read_me = Path(__file__).parent.joinpath("README.md").read_text(encoding='utf8')
```

### Comparing `qgis-plugin-manager-1.6.2/test/test_full_install.py` & `qgis-plugin-manager-1.6.3/test/test_full_install.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.2/test/test_local.py` & `qgis-plugin-manager-1.6.3/test/test_local.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.2/test/test_remote.py` & `qgis-plugin-manager-1.6.3/test/test_remote.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-manager-1.6.2/test/test_utils.py` & `qgis-plugin-manager-1.6.3/test/test_utils.py`

 * *Files identical despite different names*

