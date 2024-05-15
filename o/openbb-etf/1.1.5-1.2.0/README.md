# Comparing `tmp/openbb_etf-1.1.5.tar.gz` & `tmp/openbb_etf-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_etf-1.1.5.tar", max compression
+gzip compressed data, was "openbb_etf-1.2.0.tar", max compression
```

## Comparing `openbb_etf-1.1.5.tar` & `openbb_etf-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      216 2024-04-17 12:33:20.501645 openbb_etf-1.1.5/README.md
--rw-r--r--   0        0        0       28 2024-04-17 12:33:20.501645 openbb_etf-1.1.5/openbb_etf/__init__.py
--rw-r--r--   0        0        0       21 2024-04-17 12:33:20.501645 openbb_etf-1.1.5/openbb_etf/discovery/__init__.py
--rw-r--r--   0        0        0     1770 2024-04-17 12:33:20.501645 openbb_etf-1.1.5/openbb_etf/discovery/discovery_router.py
--rw-r--r--   0        0        0     6392 2024-04-19 13:09:31.715183 openbb_etf-1.1.5/openbb_etf/etf_router.py
--rw-r--r--   0        0        0        0 2024-04-17 12:33:20.501645 openbb_etf-1.1.5/openbb_etf/py.typed
--rw-r--r--   0        0        0      441 2024-04-19 16:39:36.851018 openbb_etf-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 openbb_etf-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      225 2024-05-15 14:34:21.677648 openbb_etf-1.2.0/README.md
+-rw-r--r--   0        0        0       28 2024-02-29 11:03:36.737607 openbb_etf-1.2.0/openbb_etf/__init__.py
+-rw-r--r--   0        0        0       21 2024-02-29 11:03:36.737701 openbb_etf-1.2.0/openbb_etf/discovery/__init__.py
+-rw-r--r--   0        0        0     1770 2024-04-08 12:02:16.528487 openbb_etf-1.2.0/openbb_etf/discovery/discovery_router.py
+-rw-r--r--   0        0        0     6392 2024-04-23 10:22:39.603236 openbb_etf-1.2.0/openbb_etf/etf_router.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.737920 openbb_etf-1.2.0/openbb_etf/py.typed
+-rw-r--r--   0        0        0      467 2024-05-15 16:04:50.102434 openbb_etf-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 openbb_etf-1.2.0/PKG-INFO
```

### Comparing `openbb_etf-1.1.5/openbb_etf/discovery/discovery_router.py` & `openbb_etf-1.2.0/openbb_etf/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_etf-1.1.5/openbb_etf/etf_router.py` & `openbb_etf-1.2.0/openbb_etf/etf_router.py`

 * *Files identical despite different names*

### Comparing `openbb_etf-1.1.5/PKG-INFO` & `openbb_etf-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: openbb-etf
-Version: 1.1.5
+Version: 1.2.0
 Summary: ETF extension for OpenBB
+License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # ETF data extension for OpenBB SDK
 
 This extension provides a set of commands for ETF data retrieval.
 
 ## Installation
 
 To install the extension, run the following command in this folder:
 
 ```bash
-pip install .
+pip install openbb-etf
 ```
```

