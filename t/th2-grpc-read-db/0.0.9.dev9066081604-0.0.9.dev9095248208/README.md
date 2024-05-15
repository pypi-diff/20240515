# Comparing `tmp/th2_grpc_read_db-0.0.9.dev9066081604.tar.gz` & `tmp/th2_grpc_read_db-0.0.9.dev9095248208.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_read_db-0.0.9.dev9066081604.tar", last modified: Mon May 13 16:03:35 2024, max compression
+gzip compressed data, was "dist/th2_grpc_read_db-0.0.9.dev9095248208.tar", last modified: Wed May 15 12:03:22 2024, max compression
```

## Comparing `th2_grpc_read_db-0.0.9.dev9066081604.tar` & `th2_grpc_read_db-0.0.9.dev9095248208.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-13 16:02:02.000000 th2_grpc_read_db-0.0.9.dev9066081604/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-13 16:02:02.000000 th2_grpc_read_db-0.0.9.dev9066081604/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-13 16:02:02.000000 th2_grpc_read_db-0.0.9.dev9066081604/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:03:34.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:03:34.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-13 16:02:02.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-05-13 16:03:34.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-05-13 16:03:34.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-13 16:03:34.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-13 16:03:17.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-15 12:01:36.000000 th2_grpc_read_db-0.0.9.dev9095248208/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 12:01:36.000000 th2_grpc_read_db-0.0.9.dev9095248208/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-15 12:01:36.000000 th2_grpc_read_db-0.0.9.dev9095248208/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-15 12:01:36.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/read_db.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/read_db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/read_db_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/read_db_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-15 12:03:00.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/read_db_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 12:03:22.000000 th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db.egg-info/top_level.txt
```

### Comparing `th2_grpc_read_db-0.0.9.dev9066081604/PKG-INFO` & `th2_grpc_read_db-0.0.9.dev9095248208/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_read_db
-Version: 0.0.9.dev9066081604
+Version: 0.0.9.dev9095248208
 Summary: th2_grpc_read_db
 Home-page: https://github.com/th2-net/th2-read-db
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # gRPC for read-db (0.0.8)
```

### Comparing `th2_grpc_read_db-0.0.9.dev9066081604/README.md` & `th2_grpc_read_db-0.0.9.dev9095248208/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.9.dev9066081604/setup.py` & `th2_grpc_read_db-0.0.9.dev9095248208/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db.proto` & `th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/read_db.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_pb2.py` & `th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/read_db_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_pb2.pyi` & `th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/read_db_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_pb2_grpc.py` & `th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/read_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_service.py` & `th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db/read_db_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/PKG-INFO` & `th2_grpc_read_db-0.0.9.dev9095248208/th2_grpc_read_db.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-read-db
-Version: 0.0.9.dev9066081604
+Version: 0.0.9.dev9095248208
 Summary: th2_grpc_read_db
 Home-page: https://github.com/th2-net/th2-read-db
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # gRPC for read-db (0.0.8)
```

