# Comparing `tmp/openbb_fixedincome-1.1.5.tar.gz` & `tmp/openbb_fixedincome-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_fixedincome-1.1.5.tar", max compression
+gzip compressed data, was "openbb_fixedincome-1.2.0.tar", max compression
```

## Comparing `openbb_fixedincome-1.1.5.tar` & `openbb_fixedincome-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      552 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/README.md
--rw-r--r--   0        0        0       32 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/__init__.py
--rw-r--r--   0        0        0       52 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/corporate/__init__.py
--rw-r--r--   0        0        0     4950 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/corporate/corporate_router.py
--rw-r--r--   0        0        0     1582 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/fixedincome_router.py
--rw-r--r--   0        0        0       53 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/government/__init__.py
--rw-r--r--   0        0        0     4485 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/government/government_router.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/py.typed
--rw-r--r--   0        0        0       43 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/rate/__init__.py
--rw-r--r--   0        0        0     6955 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/rate/rate_router.py
--rw-r--r--   0        0        0       50 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/spreads/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-17 12:33:20.501645 openbb_fixedincome-1.1.5/openbb_fixedincome/spreads/spreads_router.py
--rw-r--r--   0        0        0      483 2024-04-19 16:39:15.718977 openbb_fixedincome-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 openbb_fixedincome-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      425 2024-05-15 14:28:02.311514 openbb_fixedincome-1.2.0/README.md
+-rw-r--r--   0        0        0       32 2024-02-29 11:03:36.738645 openbb_fixedincome-1.2.0/openbb_fixedincome/__init__.py
+-rw-r--r--   0        0        0       52 2024-02-29 11:03:36.738725 openbb_fixedincome-1.2.0/openbb_fixedincome/corporate/__init__.py
+-rw-r--r--   0        0        0     4950 2024-04-08 12:02:16.529389 openbb_fixedincome-1.2.0/openbb_fixedincome/corporate/corporate_router.py
+-rw-r--r--   0        0        0     1582 2024-04-23 10:22:39.604538 openbb_fixedincome-1.2.0/openbb_fixedincome/fixedincome_router.py
+-rw-r--r--   0        0        0       53 2024-02-29 11:03:36.738953 openbb_fixedincome-1.2.0/openbb_fixedincome/government/__init__.py
+-rw-r--r--   0        0        0     4485 2024-04-08 12:02:16.529631 openbb_fixedincome-1.2.0/openbb_fixedincome/government/government_router.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.739091 openbb_fixedincome-1.2.0/openbb_fixedincome/py.typed
+-rw-r--r--   0        0        0       43 2024-02-29 11:03:36.739181 openbb_fixedincome-1.2.0/openbb_fixedincome/rate/__init__.py
+-rw-r--r--   0        0        0     6955 2024-04-08 12:02:16.529749 openbb_fixedincome-1.2.0/openbb_fixedincome/rate/rate_router.py
+-rw-r--r--   0        0        0       50 2024-02-29 11:03:36.739375 openbb_fixedincome-1.2.0/openbb_fixedincome/spreads/__init__.py
+-rw-r--r--   0        0        0     3076 2024-04-08 12:02:16.529856 openbb_fixedincome-1.2.0/openbb_fixedincome/spreads/spreads_router.py
+-rw-r--r--   0        0        0      509 2024-05-15 16:04:32.741103 openbb_fixedincome-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 openbb_fixedincome-1.2.0/PKG-INFO
```

### Comparing `openbb_fixedincome-1.1.5/openbb_fixedincome/corporate/corporate_router.py` & `openbb_fixedincome-1.2.0/openbb_fixedincome/corporate/corporate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.1.5/openbb_fixedincome/fixedincome_router.py` & `openbb_fixedincome-1.2.0/openbb_fixedincome/fixedincome_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.1.5/openbb_fixedincome/government/government_router.py` & `openbb_fixedincome-1.2.0/openbb_fixedincome/government/government_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.1.5/openbb_fixedincome/rate/rate_router.py` & `openbb_fixedincome-1.2.0/openbb_fixedincome/rate/rate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.1.5/openbb_fixedincome/spreads/spreads_router.py` & `openbb_fixedincome-1.2.0/openbb_fixedincome/spreads/spreads_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.1.5/PKG-INFO` & `openbb_fixedincome-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-fixedincome
-Version: 1.1.5
+Version: 1.2.0
 Summary: Fixed income extension for OpenBB
+License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Fixed Income Extension
 
 This extension provides fixed income data for the OpenBB Platform.
 
 Features of the Fixed Income extension include information on government bonds and central bank rates.
@@ -24,11 +26,9 @@
 
 To install the extension, run the following command in this folder:
 
 ```bash
 pip install openbb-fixedincome
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

