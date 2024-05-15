# Comparing `tmp/opengamedata_api_utils-1.0.2.tar.gz` & `tmp/opengamedata_api_utils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengamedata_api_utils-1.0.2.tar", last modified: Wed May 15 00:00:28 2024, max compression
+gzip compressed data, was "opengamedata_api_utils-1.0.3.tar", last modified: Wed May 15 00:13:03 2024, max compression
```

## Comparing `opengamedata_api_utils-1.0.2.tar` & `opengamedata_api_utils-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.364100 opengamedata_api_utils-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.364100 opengamedata_api_utils-1.0.2/src/ogd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/src/ogd/apis/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/src/ogd/apis/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/schemas/ServerConfigSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/src/ogd/apis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/utils/APIResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/utils/APIUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/utils/HelloAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:14.000000 opengamedata_api_utils-1.0.2/src/ogd/apis/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:00:28.368100 opengamedata_api_utils-1.0.2/src/opengamedata_api_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 00:00:28.000000 opengamedata_api_utils-1.0.2/src/opengamedata_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 00:00:28.000000 opengamedata_api_utils-1.0.2/src/opengamedata_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:00:28.000000 opengamedata_api_utils-1.0.2/src/opengamedata_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 00:00:28.000000 opengamedata_api_utils-1.0.2/src/opengamedata_api_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.746476 opengamedata_api_utils-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 00:13:03.746476 opengamedata_api_utils-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:13:03.746476 opengamedata_api_utils-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.742476 opengamedata_api_utils-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.742476 opengamedata_api_utils-1.0.3/src/ogd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.742476 opengamedata_api_utils-1.0.3/src/ogd/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.742476 opengamedata_api_utils-1.0.3/src/ogd/apis/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/schemas/ServerConfigSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.746476 opengamedata_api_utils-1.0.3/src/ogd/apis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/utils/APIResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/utils/APIUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/utils/HelloAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.746476 opengamedata_api_utils-1.0.3/src/opengamedata_api_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 00:13:03.000000 opengamedata_api_utils-1.0.3/src/opengamedata_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 00:13:03.000000 opengamedata_api_utils-1.0.3/src/opengamedata_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:13:03.000000 opengamedata_api_utils-1.0.3/src/opengamedata_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 00:13:03.000000 opengamedata_api_utils-1.0.3/src/opengamedata_api_utils.egg-info/top_level.txt
```

### Comparing `opengamedata_api_utils-1.0.2/LICENSE` & `opengamedata_api_utils-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.2/PKG-INFO` & `opengamedata_api_utils-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-api-utils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package of utilities for server-side scripts in OpenGameData.
 Author: Ryan Wilkinson, Glenn Palmer, Daus Husaini
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-api-utils
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-api-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_api_utils-1.0.2/README.md` & `opengamedata_api_utils-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.2/pyproject.toml` & `opengamedata_api_utils-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.2/src/ogd/apis/schemas/ServerConfigSchema.py` & `opengamedata_api_utils-1.0.3/src/ogd/apis/schemas/ServerConfigSchema.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,37 +14,37 @@
 from ogd.core.schemas.Schema import Schema
 
 # import local files
 
 class ServerConfigSchema(Schema):
     def __init__(self, name:str, all_elements:Dict[str, Any], logger:logging.Logger):
         self._dbg_level        : int
-        self._version          : int
+        self._version          : str
 
         if "DEBUG_LEVEL" in all_elements.keys():
             self._dbg_level = ServerConfigSchema._parseDebugLevel(all_elements["DEBUG_LEVEL"], logger=logger)
         else:
             self._dbg_level = logging.INFO
             logger.warn(f"{name} config does not have a 'DEBUG_LEVEL' element; defaulting to dbg_level={self._dbg_level}", logging.WARN)
         if "VER" in all_elements.keys():
             self._version = ServerConfigSchema._parseVersion(all_elements["VER"], logger=logger)
         else:
-            self._version = -1
+            self._version = "UNKNOWN VERSION"
             logger.warn(f"{name} config does not have a 'VER' element; defaulting to version={self._version}", logging.WARN)
 
         _used = {"DB_CONFIG", "OGD_CORE_PATH", "GOOGLE_CLIENT_ID", "DEBUG_LEVEL", "VER"}
         _leftovers = { key : val for key,val in all_elements.items() if key not in _used }
         super().__init__(name=name, other_elements=_leftovers)
 
     @property
     def DebugLevel(self) -> int:
         return self._dbg_level
 
     @property
-    def Version(self) -> int:
+    def Version(self) -> str:
         return self._version
 
     @property
     def AsMarkdown(self) -> str:
         ret_val : str
 
         ret_val = f"{self.Name}"
@@ -68,17 +68,17 @@
                     logger.warn(f"Config debug level had unexpected value {level}, defaulting to logging.INFO.", logging.WARN)
         else:
             ret_val = logging.INFO
             logger.warn(f"Config debug level was unexpected type {type(level)}, defaulting to logging.INFO.", logging.WARN)
         return ret_val
 
     @staticmethod
-    def _parseVersion(version, logger:logging.Logger) -> int:
-        ret_val : int
+    def _parseVersion(version, logger:logging.Logger) -> str:
+        ret_val : str
         if isinstance(version, int):
-            ret_val = version
+            ret_val = str(version)
         elif isinstance(version, str):
-            ret_val = int(version)
+            ret_val = version
         else:
-            ret_val = int(str(version))
-            logger.warn(f"Config version was unexpected type {type(version)}, defaulting to int(str(version))={ret_val}.", logging.WARN)
+            ret_val = str(version)
+            logger.warn(f"Config version was unexpected type {type(version)}, defaulting to str(version)={ret_val}.", logging.WARN)
         return ret_val
```

### Comparing `opengamedata_api_utils-1.0.2/src/ogd/apis/utils/APIResponse.py` & `opengamedata_api_utils-1.0.3/src/ogd/apis/utils/APIResponse.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.2/src/ogd/apis/utils/APIUtils.py` & `opengamedata_api_utils-1.0.3/src/ogd/apis/utils/APIUtils.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.2/src/ogd/apis/utils/HelloAPI.py` & `opengamedata_api_utils-1.0.3/src/ogd/apis/utils/HelloAPI.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.2/src/opengamedata_api_utils.egg-info/PKG-INFO` & `opengamedata_api_utils-1.0.3/src/opengamedata_api_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-api-utils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package of utilities for server-side scripts in OpenGameData.
 Author: Ryan Wilkinson, Glenn Palmer, Daus Husaini
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-api-utils
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-api-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

