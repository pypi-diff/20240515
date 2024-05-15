# Comparing `tmp/openbb_biztoc-1.1.5.tar.gz` & `tmp/openbb_biztoc-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_biztoc-1.1.5.tar", max compression
+gzip compressed data, was "openbb_biztoc-1.2.0.tar", max compression
```

## Comparing `openbb_biztoc-1.1.5.tar` & `openbb_biztoc-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      216 2024-04-17 12:33:20.553645 openbb_biztoc-1.1.5/README.md
--rw-r--r--   0        0        0      779 2024-04-17 12:33:20.553645 openbb_biztoc-1.1.5/openbb_biztoc/__init__.py
--rw-r--r--   0        0        0       30 2024-04-17 12:33:20.553645 openbb_biztoc-1.1.5/openbb_biztoc/models/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-19 13:10:31.744034 openbb_biztoc-1.1.5/openbb_biztoc/models/world_news.py
--rw-r--r--   0        0        0       20 2024-04-17 12:33:20.553645 openbb_biztoc-1.1.5/openbb_biztoc/utils/__init__.py
--rw-r--r--   0        0        0     3916 2024-04-17 12:33:20.553645 openbb_biztoc-1.1.5/openbb_biztoc/utils/helpers.py
--rw-r--r--   0        0        0      450 2024-04-19 16:40:51.999177 openbb_biztoc-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 openbb_biztoc-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      319 2024-05-15 14:26:14.052690 openbb_biztoc-1.2.0/README.md
+-rw-r--r--   0        0        0     1559 2024-05-14 15:30:05.610553 openbb_biztoc-1.2.0/openbb_biztoc/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-23 10:22:39.653849 openbb_biztoc-1.2.0/openbb_biztoc/models/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-08 12:02:16.580761 openbb_biztoc-1.2.0/openbb_biztoc/models/world_news.py
+-rw-r--r--   0        0        0       20 2024-04-23 10:22:39.653933 openbb_biztoc-1.2.0/openbb_biztoc/utils/__init__.py
+-rw-r--r--   0        0        0     3916 2024-04-23 10:22:39.654037 openbb_biztoc-1.2.0/openbb_biztoc/utils/helpers.py
+-rw-r--r--   0        0        0      476 2024-05-15 16:06:31.748997 openbb_biztoc-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 openbb_biztoc-1.2.0/PKG-INFO
```

### Comparing `openbb_biztoc-1.1.5/openbb_biztoc/models/world_news.py` & `openbb_biztoc-1.2.0/openbb_biztoc/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_biztoc-1.1.5/openbb_biztoc/utils/helpers.py` & `openbb_biztoc-1.2.0/openbb_biztoc/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_biztoc-1.1.5/PKG-INFO` & `openbb_biztoc-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: openbb-biztoc
-Version: 1.1.5
+Version: 1.2.0
 Summary: 
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
 Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Biztoc Provider
 
 This extension integrates the Biztoc data provider
 into the OpenBB Platform.
 
 ## Installation
 
 To install the extension, run the following command in this folder:
 
 ```bash
-pip install .
+pip install openbb-biztoc
 ```
 
+Documentation available [here](https://docs.openbb.co/platform/development/contributing).
+
```

