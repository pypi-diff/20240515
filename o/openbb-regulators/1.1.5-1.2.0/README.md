# Comparing `tmp/openbb_regulators-1.1.5.tar.gz` & `tmp/openbb_regulators-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_regulators-1.1.5.tar", max compression
+gzip compressed data, was "openbb_regulators-1.2.0.tar", max compression
```

## Comparing `openbb_regulators-1.1.5.tar` & `openbb_regulators-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      470 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/README.md
--rw-r--r--   0        0        0       35 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/openbb_regulators/__init__.py
--rw-r--r--   0        0        0       51 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/openbb_regulators/cftc/__init__.py
--rw-r--r--   0        0        0     1889 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/openbb_regulators/cftc/cftc_router.py
--rw-r--r--   0        0        0      419 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/openbb_regulators/regulators_router.py
--rw-r--r--   0        0        0       35 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/openbb_regulators/sec/__init__.py
--rw-r--r--   0        0        0     4215 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/openbb_regulators/sec/sec_router.py
--rw-r--r--   0        0        0      502 2024-04-19 16:39:42.707029 openbb_regulators-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1006 1970-01-01 00:00:00.000000 openbb_regulators-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      343 2024-05-15 14:26:33.043720 openbb_regulators-1.2.0/README.md
+-rw-r--r--   0        0        0       35 2024-04-23 10:22:39.608891 openbb_regulators-1.2.0/openbb_regulators/__init__.py
+-rw-r--r--   0        0        0       51 2024-02-29 11:03:36.742976 openbb_regulators-1.2.0/openbb_regulators/cftc/__init__.py
+-rw-r--r--   0        0        0     1889 2024-04-23 10:22:39.609012 openbb_regulators-1.2.0/openbb_regulators/cftc/cftc_router.py
+-rw-r--r--   0        0        0      419 2024-04-23 10:22:39.609108 openbb_regulators-1.2.0/openbb_regulators/regulators_router.py
+-rw-r--r--   0        0        0       35 2024-04-23 10:22:39.609201 openbb_regulators-1.2.0/openbb_regulators/sec/__init__.py
+-rw-r--r--   0        0        0     4215 2024-04-23 10:22:39.609308 openbb_regulators-1.2.0/openbb_regulators/sec/sec_router.py
+-rw-r--r--   0        0        0      528 2024-05-15 16:05:00.871422 openbb_regulators-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 openbb_regulators-1.2.0/PKG-INFO
```

### Comparing `openbb_regulators-1.1.5/openbb_regulators/cftc/cftc_router.py` & `openbb_regulators-1.2.0/openbb_regulators/cftc/cftc_router.py`

 * *Files identical despite different names*

### Comparing `openbb_regulators-1.1.5/openbb_regulators/sec/sec_router.py` & `openbb_regulators-1.2.0/openbb_regulators/sec/sec_router.py`

 * *Files identical despite different names*

### Comparing `openbb_regulators-1.1.5/PKG-INFO` & `openbb_regulators-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: openbb-regulators
-Version: 1.1.5
+Version: 1.2.0
 Summary: Markets and Agency Regulators extension for OpenBB
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
 
 # OpenBB Regulators Extension
 
 This extension provides a structure for data sourced from various global market regulators.
 
 ## Installation
 
 To install the extension, run the following command in this folder:
 
 ```bash
 pip install openbb-regulators
 ```
 
-For development please check [Contribution Guidelines](https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/openbb_platform/CONTRIBUTING.md).
-
-Documentation available [here](https://docs.openbb.co/platform).
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
```

