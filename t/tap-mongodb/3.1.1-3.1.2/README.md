# Comparing `tmp/tap-mongodb-3.1.1.tar.gz` & `tmp/tap-mongodb-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-mongodb-3.1.1.tar", last modified: Wed Feb 14 17:26:44 2024, max compression
+gzip compressed data, was "tap-mongodb-3.1.2.tar", last modified: Wed May 15 05:37:18 2024, max compression
```

## Comparing `tap-mongodb-3.1.1.tar` & `tap-mongodb-3.1.2.tar`

### file list

```diff
@@ -1,20 +1,43 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-14 17:26:44.216521 tap-mongodb-3.1.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32386 2022-12-13 20:00:05.000000 tap-mongodb-3.1.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      287 2024-02-14 17:26:44.216521 tap-mongodb-3.1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3667 2022-12-13 20:00:05.000000 tap-mongodb-3.1.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-02-14 17:26:44.216521 tap-mongodb-3.1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      782 2024-02-14 14:26:55.000000 tap-mongodb-3.1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-14 17:26:44.216521 tap-mongodb-3.1.1/tap_mongodb/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14942 2023-12-19 10:50:08.000000 tap-mongodb-3.1.1/tap_mongodb/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-14 17:26:44.216521 tap-mongodb-3.1.1/tap_mongodb/sync_strategies/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14170 2023-12-19 10:50:08.000000 tap-mongodb-3.1.1/tap_mongodb/sync_strategies/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6988 2023-12-19 10:50:08.000000 tap-mongodb-3.1.1/tap_mongodb/sync_strategies/full_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5170 2022-12-13 20:00:05.000000 tap-mongodb-3.1.1/tap_mongodb/sync_strategies/incremental.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12530 2024-02-14 14:26:55.000000 tap-mongodb-3.1.1/tap_mongodb/sync_strategies/oplog.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-02-14 17:26:44.216521 tap-mongodb-3.1.1/tap_mongodb.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      287 2024-02-14 17:26:44.000000 tap-mongodb-3.1.1/tap_mongodb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      422 2024-02-14 17:26:44.000000 tap-mongodb-3.1.1/tap_mongodb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-02-14 17:26:44.000000 tap-mongodb-3.1.1/tap_mongodb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2024-02-14 17:26:44.000000 tap-mongodb-3.1.1/tap_mongodb.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       98 2024-02-14 17:26:44.000000 tap-mongodb-3.1.1/tap_mongodb.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2024-02-14 17:26:44.000000 tap-mongodb-3.1.1/tap_mongodb.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-15 05:37:18.440009 tap-mongodb-3.1.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32386 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      497 2024-05-15 05:37:18.440009 tap-mongodb-3.1.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3667 2024-04-05 07:31:15.000000 tap-mongodb-3.1.2/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-15 05:37:18.440009 tap-mongodb-3.1.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      782 2024-05-15 05:35:06.000000 tap-mongodb-3.1.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-15 05:37:18.436009 tap-mongodb-3.1.2/tap_mongodb/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14942 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tap_mongodb/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-15 05:37:18.436009 tap-mongodb-3.1.2/tap_mongodb/sync_strategies/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14170 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tap_mongodb/sync_strategies/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6988 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tap_mongodb/sync_strategies/full_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5170 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tap_mongodb/sync_strategies/incremental.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12702 2024-05-14 12:27:10.000000 tap-mongodb-3.1.2/tap_mongodb/sync_strategies/oplog.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-15 05:37:18.440009 tap-mongodb-3.1.2/tap_mongodb.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      497 2024-05-15 05:37:18.000000 tap-mongodb-3.1.2/tap_mongodb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1253 2024-05-15 05:37:18.000000 tap-mongodb-3.1.2/tap_mongodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-15 05:37:18.000000 tap-mongodb-3.1.2/tap_mongodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2024-05-15 05:37:18.000000 tap-mongodb-3.1.2/tap_mongodb.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       98 2024-05-15 05:37:18.000000 tap-mongodb-3.1.2/tap_mongodb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2024-05-15 05:37:18.000000 tap-mongodb-3.1.2/tap_mongodb.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-15 05:37:18.440009 tap-mongodb-3.1.2/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11307 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_cname_restrictions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6918 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_configurable_properties.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10544 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_datatype.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11497 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19377 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_fname_restrictions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12712 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_full_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10542 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_full_table_id.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10412 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_full_table_interruptible.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10648 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_id_pk_variations.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25201 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_incremental.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14765 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_incremental_open_transactions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6285 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_index.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14615 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_log_based_interruptible.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12687 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_name_restrictions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13351 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_namespace_restrictions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11010 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_oplog.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6753 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_oplog_aged_out.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9714 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_oplog_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10154 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_projection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12827 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_table_reset_inc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8070 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_table_reset_log.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5635 2024-04-05 07:25:57.000000 tap-mongodb-3.1.2/tests/test_mongodb_views.py
```

### Comparing `tap-mongodb-3.1.1/LICENSE` & `tap-mongodb-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-mongodb-3.1.1/README.md` & `tap-mongodb-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tap-mongodb-3.1.1/setup.py` & `tap-mongodb-3.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-mongodb',
-      version='3.1.1',
+      version='3.1.2',
       description='Singer.io tap for extracting data from MongoDB',
       author='Stitch',
       url='https://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_mongodb'],
       install_requires=[
           'singer-python==6.0.0',
```

### Comparing `tap-mongodb-3.1.1/tap_mongodb/__init__.py` & `tap-mongodb-3.1.2/tap_mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-3.1.1/tap_mongodb/sync_strategies/common.py` & `tap-mongodb-3.1.2/tap_mongodb/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-3.1.1/tap_mongodb/sync_strategies/full_table.py` & `tap-mongodb-3.1.2/tap_mongodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-3.1.1/tap_mongodb/sync_strategies/incremental.py` & `tap-mongodb-3.1.2/tap_mongodb/sync_strategies/incremental.py`

 * *Files identical despite different names*

### Comparing `tap-mongodb-3.1.1/tap_mongodb/sync_strategies/oplog.py` & `tap-mongodb-3.1.2/tap_mongodb/sync_strategies/oplog.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,17 @@
     # If no projection was provided, return base_projection with 'o' whitelisted
     if projection is None:
         new_projection = base_projection
         new_projection['o'] = 1
         return new_projection
 
     temp_projection = {k:v for k, v in projection.items() if k != '_id'}
-    is_whitelist = sum([v for k, v in temp_projection.items()]) > 0
+    # int(bool(v)) will return 1 if v is any of non empty string, True or number > 0
+    # To avoid errors when v is a string or boolean, it is converted to int
+    is_whitelist = sum([int(bool(v)) for k, v in temp_projection.items()]) > 0
 
     # If only '_id' is included in projection
     if not temp_projection:
         # If only '_id' is whitelisted, return base projection with 'o._id' whitelisted
         new_projection = base_projection
         new_projection['o._id'] = 1
         return new_projection
```

