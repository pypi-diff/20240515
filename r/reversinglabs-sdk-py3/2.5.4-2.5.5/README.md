# Comparing `tmp/reversinglabs_sdk_py3-2.5.4.tar.gz` & `tmp/reversinglabs_sdk_py3-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reversinglabs_sdk_py3-2.5.4.tar", last modified: Thu May  9 13:04:02 2024, max compression
+gzip compressed data, was "reversinglabs_sdk_py3-2.5.5.tar", last modified: Wed May 15 12:28:01 2024, max compression
```

## Comparing `reversinglabs_sdk_py3-2.5.4.tar` & `reversinglabs_sdk_py3-2.5.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:02.631045 reversinglabs_sdk_py3-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    46144 2024-05-09 13:04:02.631045 reversinglabs_sdk_py3-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    44788 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:02.627045 reversinglabs_sdk_py3-2.5.4/ReversingLabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:02.627045 reversinglabs_sdk_py3-2.5.4/ReversingLabs/SDK/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/ReversingLabs/SDK/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    96422 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/ReversingLabs/SDK/a1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/ReversingLabs/SDK/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)   250906 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/ReversingLabs/SDK/ticloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/ReversingLabs/SDK/tiscale.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/ReversingLabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:02.627045 reversinglabs_sdk_py3-2.5.4/reversinglabs_sdk_py3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46144 2024-05-09 13:04:02.000000 reversinglabs_sdk_py3-2.5.4/reversinglabs_sdk_py3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-09 13:04:02.000000 reversinglabs_sdk_py3-2.5.4/reversinglabs_sdk_py3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:04:02.000000 reversinglabs_sdk_py3-2.5.4/reversinglabs_sdk_py3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:04:02.000000 reversinglabs_sdk_py3-2.5.4/reversinglabs_sdk_py3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 13:04:02.000000 reversinglabs_sdk_py3-2.5.4/reversinglabs_sdk_py3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 13:04:02.000000 reversinglabs_sdk_py3-2.5.4/reversinglabs_sdk_py3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-09 13:04:02.631045 reversinglabs_sdk_py3-2.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:02.627045 reversinglabs_sdk_py3-2.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/tests/test_a1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/tests/test_ticloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-09 13:03:58.000000 reversinglabs_sdk_py3-2.5.4/tests/test_tiscale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:28:01.767688 reversinglabs_sdk_py3-2.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11004 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    46144 2024-05-15 12:28:01.767688 reversinglabs_sdk_py3-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    44788 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:28:01.763688 reversinglabs_sdk_py3-2.5.5/ReversingLabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:28:01.763688 reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96422 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/a1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)   250906 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/ticloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/tiscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/ReversingLabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:28:01.767688 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46144 2024-05-15 12:28:01.000000 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-15 12:28:01.000000 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:28:01.000000 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:28:01.000000 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 12:28:01.000000 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 12:28:01.000000 reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 12:28:01.767688 reversinglabs_sdk_py3-2.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:28:01.767688 reversinglabs_sdk_py3-2.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/tests/test_a1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/tests/test_ticloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-15 12:27:57.000000 reversinglabs_sdk_py3-2.5.5/tests/test_tiscale.py
```

### Comparing `reversinglabs_sdk_py3-2.5.4/CHANGELOG.md` & `reversinglabs_sdk_py3-2.5.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -258,8 +258,16 @@
 
 2.5.4 (2024-05-09)
 -------------------
 
 #### Improvements
 - Updated the Python package dependencies to:
   - `requests>=2.31.0`
-  - `urllib3>=2.0.7`
+  - `urllib3>=2.0.7`
+
+
+2.5.5 (2024-05-15)
+-------------------
+
+#### Bugfixes
+- **a1000** module:
+  - Changed the `risk_score` parameter's type hint from `str` to `int` in `set_classification` method's docstring.
```

### Comparing `reversinglabs_sdk_py3-2.5.4/LICENSE` & `reversinglabs_sdk_py3-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.4/PKG-INFO` & `reversinglabs_sdk_py3-2.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.5.4
+Version: 2.5.5
 Summary: Python SDK for using ReversingLabs services.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
```

### Comparing `reversinglabs_sdk_py3-2.5.4/README.md` & `reversinglabs_sdk_py3-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.4/ReversingLabs/SDK/a1000.py` & `reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/a1000.py`

 * *Files 1% similar despite different names*

```diff
@@ -1120,15 +1120,15 @@
             :type sample_hash: str
             :param system: 'local' or 'ticloud'
             :type system: str
             :param classification: 'goodware', 'suspicious' or 'malicious'
             :type classification: str
             :param risk_score: If specified, it must be within range for the specified classification. If not specified,
             a default value is used: Goodware: 0, Suspicious: 6, Malicious: 10
-            :type risk_score: str
+            :type risk_score: int
             :param threat_platform: if specified, it must be on the supported list (platforms and subplatforms - see
             official API docs). If not specified, the default value is 'Win32'.
             :type threat_platform: str
             :param threat_type: If specified, it must be on the supported list (malware types - see official API docs).
             If not specified, the default value is 'Malware'.
             :type threat_type: str
             :param threat_name: If specified, must be an alphanumeric string not longer than 32 characters. If not
@@ -2110,15 +2110,15 @@
             :type comment: str
             :param cloud_analysis: use cloud analysis
             :type cloud_analysis: bool
             :param classification: 'goodware', 'suspicious' or 'malicious'
             :type classification: str
             :param risk_score: If specified, it must be within range for the specified classification. If not specified,
             a default value is used: Goodware: 0, Suspicious: 6, Malicious: 10
-            :type risk_score: str
+            :type risk_score: int
             :param threat_platform: if specified, it must be on the supported list (platforms and subplatforms - see
             official API docs). If not specified, the default value is 'Win32'.
             :type threat_platform: str
             :param threat_type: If specified, it must be on the supported list (malware types - see pfficial API docs).
             If not specified, the default value is 'Malware'.
             :type threat_type: str
             :param threat_name: If specified, must be an alphanumeric string not longer than 32 characters. If not
```

### Comparing `reversinglabs_sdk_py3-2.5.4/ReversingLabs/SDK/helper.py` & `reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/helper.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.4/ReversingLabs/SDK/ticloud.py` & `reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/ticloud.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.4/ReversingLabs/SDK/tiscale.py` & `reversinglabs_sdk_py3-2.5.5/ReversingLabs/SDK/tiscale.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.4/logo.png` & `reversinglabs_sdk_py3-2.5.5/logo.png`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.4/reversinglabs_sdk_py3.egg-info/PKG-INFO` & `reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.5.4
+Version: 2.5.5
 Summary: Python SDK for using ReversingLabs services.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
```

### Comparing `reversinglabs_sdk_py3-2.5.4/reversinglabs_sdk_py3.egg-info/SOURCES.txt` & `reversinglabs_sdk_py3-2.5.5/reversinglabs_sdk_py3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.4/setup.py` & `reversinglabs_sdk_py3-2.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.4/tests/test_a1000.py` & `reversinglabs_sdk_py3-2.5.5/tests/test_a1000.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.4/tests/test_helper.py` & `reversinglabs_sdk_py3-2.5.5/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.4/tests/test_ticloud.py` & `reversinglabs_sdk_py3-2.5.5/tests/test_ticloud.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.4/tests/test_tiscale.py` & `reversinglabs_sdk_py3-2.5.5/tests/test_tiscale.py`

 * *Files identical despite different names*

