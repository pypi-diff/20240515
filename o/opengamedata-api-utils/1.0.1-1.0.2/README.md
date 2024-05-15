# Comparing `tmp/opengamedata_api_utils-1.0.1.tar.gz` & `tmp/opengamedata_api_utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengamedata_api_utils-1.0.1.tar", last modified: Tue May 14 20:45:58 2024, max compression
+gzip compressed data, was "opengamedata_api_utils-1.0.2.tar", last modified: Wed May 15 00:00:28 2024, max compression
```

## Comparing `opengamedata_api_utils-1.0.1.tar` & `opengamedata_api_utils-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:45:58.727874 opengamedata_api_utils-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 20:45:45.000000 opengamedata_api_utils-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-14 20:45:58.727874 opengamedata_api_utils-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-14 20:45:45.000000 opengamedata_api_utils-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-14 20:45:45.000000 opengamedata_api_utils-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:45:58.727874 opengamedata_api_utils-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:45:58.727874 opengamedata_api_utils-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:45:58.723874 opengamedata_api_utils-1.0.1/src/ogd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:45:58.727874 opengamedata_api_utils-1.0.1/src/ogd/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 20:45:45.000000 opengamedata_api_utils-1.0.1/src/ogd/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:45:58.727874 opengamedata_api_utils-1.0.1/src/ogd/apis/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-14 20:45:45.000000 opengamedata_api_utils-1.0.1/src/ogd/apis/schemas/ServerConfigSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:45:45.000000 opengamedata_api_utils-1.0.1/src/ogd/apis/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:45:58.727874 opengamedata_api_utils-1.0.1/src/ogd/apis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-14 20:45:45.000000 opengamedata_api_utils-1.0.1/src/ogd/apis/utils/APIResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-14 20:45:45.000000 opengamedata_api_utils-1.0.1/src/ogd/apis/utils/APIUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-14 20:45:45.000000 opengamedata_api_utils-1.0.1/src/ogd/apis/utils/HelloAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:45:45.000000 opengamedata_api_utils-1.0.1/src/ogd/apis/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:45:58.727874 opengamedata_api_utils-1.0.1/src/opengamedata_api_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-14 20:45:58.000000 opengamedata_api_utils-1.0.1/src/opengamedata_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 20:45:58.000000 opengamedata_api_utils-1.0.1/src/opengamedata_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:45:58.000000 opengamedata_api_utils-1.0.1/src/opengamedata_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 20:45:58.000000 opengamedata_api_utils-1.0.1/src/opengamedata_api_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.364100 opengamedata_api_utils-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.364100 opengamedata_api_utils-1.0.2/src/ogd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/src/ogd/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/src/ogd/apis/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/schemas/ServerConfigSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/src/ogd/apis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/utils/APIResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/utils/APIUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/utils/HelloAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/src/opengamedata_api_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 00:00:28.000000 opengamedata_api_utils-1.0.2/src/opengamedata_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 00:00:28.000000 opengamedata_api_utils-1.0.2/src/opengamedata_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:00:28.000000 opengamedata_api_utils-1.0.2/src/opengamedata_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 00:00:28.000000 opengamedata_api_utils-1.0.2/src/opengamedata_api_utils.egg-info/top_level.txt
```

### Comparing `opengamedata_api_utils-1.0.1/LICENSE` & `opengamedata_api_utils-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.1/PKG-INFO` & `opengamedata_api_utils-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-api-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package of utilities for server-side scripts in OpenGameData.
 Author: Ryan Wilkinson, Glenn Palmer, Daus Husaini
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-api-utils
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-api-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_api_utils-1.0.1/README.md` & `opengamedata_api_utils-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.1/pyproject.toml` & `opengamedata_api_utils-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.1/src/ogd/apis/schemas/ServerConfigSchema.py` & `opengamedata_api_utils-1.0.2/src/ogd/apis/schemas/ServerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.1/src/ogd/apis/utils/APIResponse.py` & `opengamedata_api_utils-1.0.2/src/ogd/apis/utils/APIResponse.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.1/src/ogd/apis/utils/APIUtils.py` & `opengamedata_api_utils-1.0.2/src/ogd/apis/utils/APIUtils.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.1/src/ogd/apis/utils/HelloAPI.py` & `opengamedata_api_utils-1.0.2/src/ogd/apis/utils/HelloAPI.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.1/src/opengamedata_api_utils.egg-info/PKG-INFO` & `opengamedata_api_utils-1.0.2/src/opengamedata_api_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-api-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package of utilities for server-side scripts in OpenGameData.
 Author: Ryan Wilkinson, Glenn Palmer, Daus Husaini
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-api-utils
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-api-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

