# Comparing `tmp/aerospike-vector-search-0.5.1.tar.gz` & `tmp/aerospike-vector-search-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerospike-vector-search-0.5.1.tar", last modified: Mon May  6 23:33:23 2024, max compression
+gzip compressed data, was "aerospike-vector-search-0.6.0.tar", last modified: Tue May 14 19:33:21 2024, max compression
```

## Comparing `aerospike-vector-search-0.5.1.tar` & `aerospike-vector-search-0.6.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11357 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/LICENSE
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2271 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/PKG-INFO
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1431 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/README.md
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1291 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/pyproject.toml
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       38 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/setup.cfg
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.263811 aerospike-vector-search-0.5.1/src/
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.263811 aerospike-vector-search-0.5.1/src/aerospike_vector_search/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      197 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/__init__.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11145 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/admin.py
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      198 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/__init__.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11671 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/admin.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    12289 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/client.py
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/internal/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     4463 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/internal/channel_provider.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11830 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/client.py
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/src/aerospike_vector_search/internal/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/internal/__init__.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     3757 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/internal/channel_provider.py
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/__init__.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     5147 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/admin_helpers.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     4337 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/base_channel_provider.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     6090 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/client_helpers.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     3861 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/conversions.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      775 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/helpers.py
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1735 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/auth_pb2.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2308 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/auth_pb2_grpc.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2063 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/index_pb2.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     8361 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/index_pb2_grpc.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     3588 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/transact_pb2.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     8310 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/transact_pb2_grpc.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     7941 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/types_pb2.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      159 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/types_pb2_grpc.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     4790 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     9503 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2_grpc.py
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     8729 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search/types.py
-drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-06 23:33:23.267812 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2271 2024-05-06 23:33:23.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/PKG-INFO
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1767 2024-05-06 23:33:23.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/SOURCES.txt
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        1 2024-05-06 23:33:23.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/dependency_links.txt
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        1 2024-05-06 23:32:30.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/not-zip-safe
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       16 2024-05-06 23:33:23.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/requires.txt
--rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       24 2024-05-06 23:33:23.000000 aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/top_level.txt
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-14 19:33:21.617906 aerospike-vector-search-0.6.0/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11357 2024-04-24 15:28:08.000000 aerospike-vector-search-0.6.0/LICENSE
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2271 2024-05-14 19:33:21.617906 aerospike-vector-search-0.6.0/PKG-INFO
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1431 2024-04-30 14:24:15.000000 aerospike-vector-search-0.6.0/README.md
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1776 2024-05-14 17:34:00.000000 aerospike-vector-search-0.6.0/pyproject.toml
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       38 2024-05-14 19:33:21.617906 aerospike-vector-search-0.6.0/setup.cfg
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-14 19:33:21.617906 aerospike-vector-search-0.6.0/src/
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-14 19:33:21.617906 aerospike-vector-search-0.6.0/src/aerospike_vector_search/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      269 2024-05-14 17:15:41.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/__init__.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    11717 2024-05-14 19:17:08.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/admin.py
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-14 19:33:21.617906 aerospike-vector-search-0.6.0/src/aerospike_vector_search/aio/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      236 2024-05-14 17:15:41.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/aio/__init__.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    12241 2024-05-14 19:22:26.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/aio/admin.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    16917 2024-05-14 17:15:41.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/aio/client.py
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-14 19:33:21.617906 aerospike-vector-search-0.6.0/src/aerospike_vector_search/aio/internal/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     4639 2024-05-14 19:27:26.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/aio/internal/channel_provider.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)    16324 2024-05-14 17:15:41.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/client.py
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-14 19:33:21.617906 aerospike-vector-search-0.6.0/src/aerospike_vector_search/internal/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        0 2024-04-24 15:28:08.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/internal/__init__.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     3950 2024-05-14 17:15:41.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/internal/channel_provider.py
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-14 19:33:21.617906 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        0 2024-04-24 15:28:08.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/__init__.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     5227 2024-05-14 17:15:41.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/admin_helpers.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     4359 2024-05-14 17:15:41.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/base_channel_provider.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     8748 2024-05-14 17:15:41.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/client_helpers.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     3929 2024-05-14 17:15:41.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/conversions.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      854 2024-05-14 17:15:41.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/helpers.py
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-14 19:33:21.617906 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1735 2024-05-14 17:29:07.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/auth_pb2.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2308 2024-05-14 17:29:08.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/auth_pb2_grpc.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2063 2024-05-14 17:29:09.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/index_pb2.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     8361 2024-05-14 17:29:10.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/index_pb2_grpc.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     4637 2024-05-14 17:29:10.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/transact_pb2.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     9734 2024-05-14 17:29:11.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/transact_pb2_grpc.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     8214 2024-05-14 17:29:12.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/types_pb2.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)      159 2024-05-14 17:29:13.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/types_pb2_grpc.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     4790 2024-05-14 17:29:14.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     9503 2024-05-14 17:29:15.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2_grpc.py
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     9366 2024-05-14 17:15:41.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search/types.py
+drwxrwxr-x   0 dpelini   (1001) dpelini   (1001)        0 2024-05-14 19:33:21.617906 aerospike-vector-search-0.6.0/src/aerospike_vector_search.egg-info/
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     2271 2024-05-14 19:33:21.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search.egg-info/PKG-INFO
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)     1767 2024-05-14 19:33:21.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        1 2024-05-14 19:33:21.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)        1 2024-04-30 14:44:08.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search.egg-info/not-zip-safe
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       16 2024-05-14 19:33:21.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search.egg-info/requires.txt
+-rw-rw-r--   0 dpelini   (1001) dpelini   (1001)       24 2024-05-14 19:33:21.000000 aerospike-vector-search-0.6.0/src/aerospike_vector_search.egg-info/top_level.txt
```

### Comparing `aerospike-vector-search-0.5.1/LICENSE` & `aerospike-vector-search-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.1/PKG-INFO` & `aerospike-vector-search-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerospike-vector-search
-Version: 0.5.1
+Version: 0.6.0
 Summary: Aerospike Proximus Client Library for Python
 Author-email: "Aerospike, Inc." <info@aerospike.com>
 License: Apache Software License
 Project-URL: Homepage, https://aerospike.com
 Keywords: aerospike,vector,database,ANN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `aerospike-vector-search-0.5.1/README.md` & `aerospike-vector-search-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.1/pyproject.toml` & `aerospike-vector-search-0.6.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -18,22 +18,37 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Database"
 ]
-version = "0.5.1"
+version = "0.6.0"
 requires-python = ">3.8"
 dependencies = [
     "grpcio",
     "protobuf"
 ]
 
 [project.urls]
 "Homepage" = "https://aerospike.com"
 
 [tool.setuptools]
 zip-safe = false
 include-package-data = true
 packages = ["aerospike_vector_search", "aerospike_vector_search.aio", "aerospike_vector_search.shared", "aerospike_vector_search.shared.proto_generated", "aerospike_vector_search.internal", "aerospike_vector_search.aio.internal"]
 package-dir={"" = "src"}
+
+[tool.black]
+include = 'src'
+exclude = '''
+/(
+    src/aerospike_vector_search/shared/proto_generated/*
+  | src/aerospike_vector_search/aio/internal/__pycache__/*
+  | src/aerospike_vector_search/aio/__pycache__/*
+  | src/aerospike_vector_search/internal/__pycache__/*
+  | src/aerospike_vector_search/shared/__pycache__/*
+  | src/aerospike_vector_search/shared/proto_generated/__pycache__/*
+  | src/aerospike_vector_search/__pycache__/*
+  | src/aerospike_vector_search.egg-info/*
+)/
+'''
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/admin.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from . import types
 from .internal import channel_provider
 from .shared.admin_helpers import BaseClient
 
 logger = logging.getLogger(__name__)
 
+
 class Client(BaseClient):
     """
     Aerospike Vector Search Admin Client
 
     This client is designed to conduct Aerospike Vector Search administrative operation such as creating indexes, querying index information, and dropping indexes.
     """
 
@@ -38,15 +39,14 @@
         """
         seeds = self._prepare_seeds(seeds)
 
         self._channel_provider = channel_provider.ChannelProvider(
             seeds, listener_name, is_loadbalancer
         )
 
-
     def index_create(
         self,
         *,
         namespace: str,
         name: str,
         vector_field: str,
         dimensions: int,
@@ -62,43 +62,53 @@
 
         Args:
             namespace (str): The namespace for the index.
             name (str): The name of the index.
             vector_field (str): The name of the field containing vector data.
             dimensions (int): The number of dimensions in the vector data.
             vector_distance_metric (Optional[types.VectorDistanceMetric], optional):
-                The distance metric used to compare when performing a vector search.
-                Defaults to VectorDistanceMetric.SQUARED_EUCLIDEAN.
+            The distance metric used to compare when performing a vector search.
+            Defaults to VectorDistanceMetric.SQUARED_EUCLIDEAN.
             sets (Optional[str], optional): The set used for the index. Defaults to None.
             index_params (Optional[types.HnswParams], optional):
-                Parameters used for tuning vector search. Defaults to None. If index_params is None, then the default values specified for
-                types.HnswParams will be used.
+            Parameters used for tuning vector search. Defaults to None. If index_params is None, then the default values specified for
+            types.HnswParams will be used.
             index_meta_data (Optional[dict[str, str]], optional): Meta data associated with the index. Defaults to None.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         Note:
             This method creates an index with the specified parameters and waits for the index creation to complete.
             It waits for up to 100,000 seconds for the index creation to complete.
         """
-        (index_stub, index_create_request) = self._prepare_index_create(namespace, name, vector_field, dimensions, vector_distance_metric, sets, index_params, index_meta_data, logger)
+        (index_stub, index_create_request) = self._prepare_index_create(
+            namespace,
+            name,
+            vector_field,
+            dimensions,
+            vector_distance_metric,
+            sets,
+            index_params,
+            index_meta_data,
+            logger,
+        )
         try:
             index_stub.Create(index_create_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
         try:
             self._wait_for_index_creation(
                 namespace=namespace, name=name, timeout=100_000
             )
         except grpc.RpcError as e:
             logger.error("Failed waiting for creation with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
 
     def index_drop(self, *, namespace: str, name: str) -> None:
         """
         Drop an index.
 
         Args:
             namespace (str): The namespace of the index.
@@ -108,27 +118,29 @@
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         Note:
             This method drops an index with the specified parameters and waits for the index deletion to complete.
             It waits for up to 100,000 seconds for the index deletion to complete.
         """
-        (index_stub, index_drop_request) = self._prepare_index_drop(namespace, name, logger)
+        (index_stub, index_drop_request) = self._prepare_index_drop(
+            namespace, name, logger
+        )
         try:
             index_stub.Drop(index_drop_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
         try:
             self._wait_for_index_deletion(
                 namespace=namespace, name=name, timeout=100_000
             )
         except grpc.RpcError as e:
             logger.error("Failed waiting for deletion with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
 
     def index_list(self) -> list[dict]:
         """
         List all indices.
 
         Returns:
             list[dict]: A list of indices.
@@ -138,20 +150,18 @@
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
         (index_stub, index_list_request) = self._prepare_index_list(logger)
         try:
             response = index_stub.List(index_list_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
         return self._respond_index_list(response)
 
-    def index_get(
-        self, *, namespace: str, name: str
-    ) -> dict[str, Union[int, str]]:
+    def index_get(self, *, namespace: str, name: str) -> dict[str, Union[int, str]]:
         """
         Retrieve the information related with an index.
 
         Args:
             namespace (str): The namespace of the index.
             name (str): The name of the index.
 
@@ -159,23 +169,24 @@
             dict[str, Union[int, str]: Information about an index.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         """
-        (index_stub, index_get_request) = self._prepare_index_get(namespace, name, logger)
+        (index_stub, index_get_request) = self._prepare_index_get(
+            namespace, name, logger
+        )
         try:
             response = index_stub.Get(index_get_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
         return self._respond_index_get(response)
 
-
     def index_get_status(self, *, namespace: str, name: str) -> int:
         """
         Retrieve the number of records queued to be merged into an index.
 
         Args:
             namespace (str): The namespace of the index.
             name (str): The name of the index.
@@ -189,70 +200,86 @@
 
         Note:
             This method retrieves the status of the specified index. If index_get_status is called the vector client puts some records into Aerospike Vector Search,
             the records may not immediately begin to merge into the index. To wait for all records to be merged into an index, use vector_client.wait_for_index_completion.
 
             Warning: This API is subject to change.
         """
-        (index_stub, index_get_status_request) = self._prepare_index_get_status(namespace, name, logger)
+        (index_stub, index_get_status_request) = self._prepare_index_get_status(
+            namespace, name, logger
+        )
         try:
             response = index_stub.GetStatus(index_get_status_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
 
         return self._respond_index_get_status(response)
 
     def _wait_for_index_creation(
-        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize, wait_interval: Optional[int] = 0.1
+        self,
+        *,
+        namespace: str,
+        name: str,
+        timeout: Optional[int] = sys.maxsize,
+        wait_interval: Optional[int] = 0.1,
     ) -> None:
         """
         Wait for the index to be created.
         """
-        (index_stub, wait_interval, start_time, _, _, index_creation_request) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
+        (index_stub, wait_interval, start_time, _, _, index_creation_request) = (
+            self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
+        )
         while True:
             self._check_timeout(start_time, timeout)
             try:
                 index_stub.GetStatus(index_creation_request)
                 logger.debug("Index created succesfully")
                 # Index has been created
                 return
             except grpc.RpcError as e:
                 if e.code() in (grpc.StatusCode.UNAVAILABLE, grpc.StatusCode.NOT_FOUND):
 
                     # Wait for some more time.
                     time.sleep(wait_interval)
                 else:
                     logger.error("Failed with error: %s", e)
-                    raise e
+                    raise types.AVSServerError(rpc_error=e)
 
     def _wait_for_index_deletion(
-        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize, wait_interval: Optional[int] = 0.1
+        self,
+        *,
+        namespace: str,
+        name: str,
+        timeout: Optional[int] = sys.maxsize,
+        wait_interval: Optional[int] = 0.1,
     ) -> None:
         """
         Wait for the index to be deleted.
         """
 
         # Wait interval between polling
-        (index_stub, wait_interval, start_time, _, _, index_deletion_request) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
+        (index_stub, wait_interval, start_time, _, _, index_deletion_request) = (
+            self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
+        )
 
         while True:
             self._check_timeout(start_time, timeout)
 
             try:
                 index_stub.GetStatus(index_deletion_request)
                 # Wait for some more time.
                 time.sleep(wait_interval)
             except grpc.RpcError as e:
                 if e.code() in (grpc.StatusCode.UNAVAILABLE, grpc.StatusCode.NOT_FOUND):
                     logger.debug("Index deleted succesfully")
                     # Index has been created
                     return
                 else:
-                    raise e
+                    raise types.AVSServerError(rpc_error=e)
 
     def close(self):
         """
         Close the Aerospike Vector Search Admin Client.
 
         This method closes gRPC channels connected to Aerospike Vector Search.
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/admin.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/aio/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from .. import types
 from .internal import channel_provider
 from ..shared.admin_helpers import BaseClient
 
 logger = logging.getLogger(__name__)
 
+
 class Client(BaseClient):
     """
     Aerospike Vector Search Asyncio Admin Client
 
     This client is designed to conduct Aerospike Vector Search administrative operation such as creating indexes, querying index information, and dropping indexes.
     """
 
@@ -38,15 +39,14 @@
         """
         seeds = self._prepare_seeds(seeds)
 
         self._channel_provider = channel_provider.ChannelProvider(
             seeds, listener_name, is_loadbalancer
         )
 
-
     async def index_create(
         self,
         *,
         namespace: str,
         name: str,
         vector_field: str,
         dimensions: int,
@@ -62,47 +62,57 @@
 
         Args:
             namespace (str): The namespace for the index.
             name (str): The name of the index.
             vector_field (str): The name of the field containing vector data.
             dimensions (int): The number of dimensions in the vector data.
             vector_distance_metric (Optional[types.VectorDistanceMetric], optional):
-                The distance metric used to compare when performing a vector search.
-                Defaults to VectorDistanceMetric.SQUARED_EUCLIDEAN.
+            The distance metric used to compare when performing a vector search.
+            Defaults to VectorDistanceMetric.SQUARED_EUCLIDEAN.
             sets (Optional[str], optional): The set used for the index. Defaults to None.
             index_params (Optional[types.HnswParams], optional):
-                Parameters used for tuning vector search. Defaults to None. If index_params is None, then the default values specified for
-                types.HnswParams will be used.
+            Parameters used for tuning vector search. Defaults to None. If index_params is None, then the default values specified for
+            types.HnswParams will be used.
             index_meta_data (Optional[dict[str, str]], optional): Meta data associated with the index. Defaults to None.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         Note:
             This method creates an index with the specified parameters and waits for the index creation to complete.
             It waits for up to 100,000 seconds for the index creation to complete.
         """
 
         await self._channel_provider._is_ready()
 
-        (index_stub, index_create_request) = self._prepare_index_create(namespace, name, vector_field, dimensions, vector_distance_metric, sets, index_params, index_meta_data, logger)
-        
+        (index_stub, index_create_request) = self._prepare_index_create(
+            namespace,
+            name,
+            vector_field,
+            dimensions,
+            vector_distance_metric,
+            sets,
+            index_params,
+            index_meta_data,
+            logger,
+        )
+
         try:
             await index_stub.Create(index_create_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
         try:
             await self._wait_for_index_creation(
                 namespace=namespace, name=name, timeout=100_000
             )
         except grpc.RpcError as e:
             logger.error("Failed waiting for creation with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
 
     async def index_drop(self, *, namespace: str, name: str) -> None:
         """
         Drop an index.
 
         Args:
             namespace (str): The namespace of the index.
@@ -114,47 +124,49 @@
 
         Note:
             This method drops an index with the specified parameters and waits for the index deletion to complete.
             It waits for up to 100,000 seconds for the index deletion to complete.
         """
         await self._channel_provider._is_ready()
 
-        (index_stub, index_drop_request) = self._prepare_index_drop(namespace, name, logger)
+        (index_stub, index_drop_request) = self._prepare_index_drop(
+            namespace, name, logger
+        )
         try:
             await index_stub.Drop(index_drop_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
         try:
             await self._wait_for_index_deletion(
                 namespace=namespace, name=name, timeout=100_000
             )
         except grpc.RpcError as e:
             logger.error("Failed waiting for deletion with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
 
     async def index_list(self) -> list[dict]:
         """
         List all indices.
 
         Returns:
             list[dict]: A list of indices.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
         await self._channel_provider._is_ready()
-        
+
         (index_stub, index_list_request) = self._prepare_index_list(logger)
         try:
             response = await index_stub.List(index_list_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
         return self._respond_index_list(response)
 
     async def index_get(
         self, *, namespace: str, name: str
     ) -> dict[str, Union[int, str]]:
         """
         Retrieve the information related with an index.
@@ -169,23 +181,24 @@
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         """
         await self._channel_provider._is_ready()
 
-        (index_stub, index_get_request) = self._prepare_index_get(namespace, name, logger)
+        (index_stub, index_get_request) = self._prepare_index_get(
+            namespace, name, logger
+        )
         try:
             response = await index_stub.Get(index_get_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
         return self._respond_index_get(response)
 
-
     async def index_get_status(self, *, namespace: str, name: str) -> int:
         """
         Retrieve the number of records queued to be merged into an index.
 
         Args:
             namespace (str): The namespace of the index.
             name (str): The name of the index.
@@ -201,73 +214,89 @@
             This method retrieves the status of the specified index. If index_get_status is called the vector client puts some records into Aerospike Vector Search,
             the records may not immediately begin to merge into the index. To wait for all records to be merged into an index, use vector_client.wait_for_index_completion.
 
             Warning: This API is subject to change.
         """
         await self._channel_provider._is_ready()
 
-        (index_stub, index_get_status_request) = self._prepare_index_get_status(namespace, name, logger)
+        (index_stub, index_get_status_request) = self._prepare_index_get_status(
+            namespace, name, logger
+        )
         try:
             response = await index_stub.GetStatus(index_get_status_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
 
         return self._respond_index_get_status(response)
 
     async def _wait_for_index_creation(
-        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize, wait_interval: Optional[int] = 0.1
+        self,
+        *,
+        namespace: str,
+        name: str,
+        timeout: Optional[int] = sys.maxsize,
+        wait_interval: Optional[int] = 0.1,
     ) -> None:
         """
         Wait for the index to be created.
         """
         await self._channel_provider._is_ready()
 
-        (index_stub, wait_interval, start_time, _, _, index_creation_request) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
+        (index_stub, wait_interval, start_time, _, _, index_creation_request) = (
+            self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
+        )
         while True:
             self._check_timeout(start_time, timeout)
             try:
                 await index_stub.GetStatus(index_creation_request)
                 logger.debug("Index created succesfully")
                 # Index has been created
                 return
             except grpc.RpcError as e:
                 if e.code() in (grpc.StatusCode.UNAVAILABLE, grpc.StatusCode.NOT_FOUND):
 
                     # Wait for some more time.
                     await asyncio.sleep(wait_interval)
                 else:
                     logger.error("Failed with error: %s", e)
-                    raise e
+                    raise types.AVSServerError(rpc_error=e)
 
     async def _wait_for_index_deletion(
-        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize, wait_interval: Optional[int] = 0.1
+        self,
+        *,
+        namespace: str,
+        name: str,
+        timeout: Optional[int] = sys.maxsize,
+        wait_interval: Optional[int] = 0.1,
     ) -> None:
         """
         Wait for the index to be deleted.
         """
         await self._channel_provider._is_ready()
 
         # Wait interval between polling
-        (index_stub, wait_interval, start_time, _, _, index_deletion_request) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
+        (index_stub, wait_interval, start_time, _, _, index_deletion_request) = (
+            self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
+        )
 
         while True:
             self._check_timeout(start_time, timeout)
 
             try:
                 await index_stub.GetStatus(index_deletion_request)
                 # Wait for some more time.
                 await asyncio.sleep(wait_interval)
             except grpc.RpcError as e:
                 if e.code() in (grpc.StatusCode.UNAVAILABLE, grpc.StatusCode.NOT_FOUND):
                     logger.debug("Index deleted succesfully")
                     # Index has been created
                     return
                 else:
-                    raise e
+                    raise types.AVSServerError(rpc_error=e)
 
     async def close(self):
         """
         Close the Aerospike Vector Search Admin Client.
 
         This method closes gRPC channels connected to Aerospike Vector Search.
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/client.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/aio/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from .. import types
 from .internal import channel_provider
 from ..shared.client_helpers import BaseClient
 
 logger = logging.getLogger(__name__)
 
+
 class Client(BaseClient):
     """
     Aerospike Vector Search Asyncio Admin Client
 
     This client specializes in performing database operations with vector data.
     Moreover, the client supports Hierarchical Navigable Small World (HNSW) vector searches,
     allowing users to find vectors similar to a given query vector within an index.
@@ -42,24 +43,103 @@
             Exception: Raised when no seed host is provided.
         """
         seeds = self._prepare_seeds(seeds)
         self._channel_provider = channel_provider.ChannelProvider(
             seeds, listener_name, is_loadbalancer
         )
 
-    async def put(
+    async def insert(
+        self,
+        *,
+        namespace: str,
+        key: Union[int, str, bytes, bytearray],
+        record_data: dict[str, Any],
+        set_name: Optional[str] = None,
+    ) -> None:
+        """
+        Insert a record into Aerospike Vector Search.
+
+        If record does exist, an exception is raised.
+        If record doesn't exist, the record is inserted.
+
+        Args:
+            namespace (str): The namespace for the record.
+            key (Union[int, str, bytes, bytearray]): The key for the record.
+            record_data (dict[str, Any]): The data to be stored in the record.
+            set_name (Optional[str], optional): The name of the set to which the record belongs. Defaults to None.
+
+        Raises:
+            grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
+            This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
+
+        """
+
+        await self._channel_provider._is_ready()
+
+        (transact_stub, insert_request) = self._prepare_insert(
+            namespace, key, record_data, set_name, logger
+        )
+
+        try:
+            await transact_stub.Put(insert_request)
+        except grpc.RpcError as e:
+            logger.error("Failed with error: %s", e)
+            raise types.AVSServerError(rpc_error=e)
+
+    async def update(
+        self,
+        *,
+        namespace: str,
+        key: Union[int, str, bytes, bytearray],
+        record_data: dict[str, Any],
+        set_name: Optional[str] = None,
+    ) -> None:
+        """
+        Update a record in Aerospike Vector Search.
+
+        If record does exist, update the record.
+        If record doesn't exist, an exception is raised.
+
+        Args:
+            namespace (str): The namespace for the record.
+            key (Union[int, str, bytes, bytearray]): The key for the record.
+            record_data (dict[str, Any]): The data to be stored in the record.
+            set_name (Optional[str], optional): The name of the set to which the record belongs. Defaults to None.
+
+        Raises:
+            grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
+            This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
+
+        """
+
+        await self._channel_provider._is_ready()
+
+        (transact_stub, update_request) = self._prepare_update(
+            namespace, key, record_data, set_name, logger
+        )
+
+        try:
+            await transact_stub.Put(update_request)
+        except grpc.RpcError as e:
+            logger.error("Failed with error: %s", e)
+            raise types.AVSServerError(rpc_error=e)
+
+    async def upsert(
         self,
         *,
         namespace: str,
         key: Union[int, str, bytes, bytearray],
         record_data: dict[str, Any],
         set_name: Optional[str] = None,
     ) -> None:
         """
-        Write a record to Aerospike Vector Search.
+        Update a record in Aerospike Vector Search.
+
+        If record does exist, update the record.
+        If record doesn't exist, the record is inserted.
 
         Args:
             namespace (str): The namespace for the record.
             key (Union[int, str, bytes, bytearray]): The key for the record.
             record_data (dict[str, Any]): The data to be stored in the record.
             set_name (Optional[str], optional): The name of the set to which the record belongs. Defaults to None.
 
@@ -67,56 +147,60 @@
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         """
 
         await self._channel_provider._is_ready()
 
-        (transact_stub, put_request) = self._prepare_put(namespace, key, record_data, set_name, logger)
+        (transact_stub, upsert_request) = self._prepare_upsert(
+            namespace, key, record_data, set_name, logger
+        )
 
         try:
-            await transact_stub.Put(put_request)
+            await transact_stub.Put(upsert_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
 
     async def get(
         self,
         *,
         namespace: str,
         key: Union[int, str, bytes, bytearray],
-        bin_names: Optional[list[str]] = None,
+        field_names: Optional[list[str]] = None,
         set_name: Optional[str] = None,
     ) -> types.RecordWithKey:
         """
         Read a record from Aerospike Vector Search.
 
         Args:
             namespace (str): The namespace for the record.
             key (Union[int, str, bytes, bytearray]): The key for the record.
-            bin_names (Optional[list[str]], optional): A list of bin names to retrieve from the record.
-            If None, all bins are retrieved. Defaults to None.
+            field_names (Optional[list[str]], optional): A list of field names to retrieve from the record.
+            If None, all fields are retrieved. Defaults to None.
             set_name (Optional[str], optional): The name of the set from which to read the record. Defaults to None.
 
         Returns:
             types.RecordWithKey: A record with its associated key.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
 
         await self._channel_provider._is_ready()
 
-        (transact_stub, key, get_request) = self._prepare_get(namespace, key, bin_names, set_name, logger)
+        (transact_stub, key, get_request) = self._prepare_get(
+            namespace, key, field_names, set_name, logger
+        )
         try:
             response = await transact_stub.Get(get_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
 
         return self._respond_get(response, key)
 
     async def exists(
         self, *, namespace: str, key: Any, set_name: Optional[str] = None
     ) -> bool:
         """
@@ -133,23 +217,54 @@
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
 
         await self._channel_provider._is_ready()
 
-        (transact_stub, key) = self._prepare_exists(namespace, key, set_name, logger)
+        (transact_stub, exists_request) = self._prepare_exists(
+            namespace, key, set_name, logger
+        )
+
         try:
-            response = await transact_stub.Exists(key)
+            response = await transact_stub.Exists(exists_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
 
         return self._respond_exists(response)
 
+    async def delete(
+        self, *, namespace: str, key: Any, set_name: Optional[str] = None
+    ) -> None:
+        """
+        Delete a record from Aerospike Vector Search.
+
+        Args:
+            namespace (str): The namespace for the record.
+            key (Any): The key for the record.
+            set_name (Optional[str], optional): The name of the set to which the record belongs. Defaults to None.
+
+        Raises:
+            grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
+            This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
+        """
+
+        await self._channel_provider._is_ready()
+
+        (transact_stub, delete_request) = self._prepare_delete(
+            namespace, key, set_name, logger
+        )
+
+        try:
+            await transact_stub.Delete(delete_request)
+        except grpc.RpcError as e:
+            logger.error("Failed with error: %s", e)
+            raise types.AVSServerError(rpc_error=e)
+
     async def is_indexed(
         self,
         *,
         namespace: str,
         key: Union[int, str, bytes, bytearray],
         index_name: str,
         index_namespace: Optional[str] = None,
@@ -172,111 +287,130 @@
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
 
         await self._channel_provider._is_ready()
 
-        (transact_stub, is_indexed_request) = self._prepare_is_indexed(namespace, key, index_name, index_namespace, set_name, logger)
+        (transact_stub, is_indexed_request) = self._prepare_is_indexed(
+            namespace, key, index_name, index_namespace, set_name, logger
+        )
         try:
             response = await transact_stub.IsIndexed(is_indexed_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
         return self._respond_is_indexed(response)
 
     async def vector_search(
         self,
         *,
         namespace: str,
         index_name: str,
         query: list[Union[bool, float]],
         limit: int,
         search_params: Optional[types.HnswSearchParams] = None,
-        bin_names: Optional[list[str]] = None,
+        field_names: Optional[list[str]] = None,
     ) -> list[types.Neighbor]:
         """
         Perform a Hierarchical Navigable Small World (HNSW) vector search in Aerospike Vector Search.
 
         Args:
             namespace (str): The namespace for the records.
             index_name (str): The name of the index.
             query (list[Union[bool, float]]): The query vector for the search.
             limit (int): The maximum number of neighbors to return. K value.
             search_params (Optional[types_pb2.HnswSearchParams], optional): Parameters for the HNSW algorithm.
             If None, the default parameters for the index are used. Defaults to None.
-            bin_names (Optional[list[str]], optional): A list of bin names to retrieve from the results.
-            If None, all bins are retrieved. Defaults to None.
+            field_names (Optional[list[str]], optional): A list of field names to retrieve from the results.
+            If None, all fields are retrieved. Defaults to None.
 
         Returns:
             list[types.Neighbor]: A list of neighbors records found by the search.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
         await self._channel_provider._is_ready()
 
-        (transact_stub, vector_search_request) = self._prepare_vector_search(namespace, index_name, query, limit, search_params, bin_names, logger)
+        (transact_stub, vector_search_request) = self._prepare_vector_search(
+            namespace, index_name, query, limit, search_params, field_names, logger
+        )
 
         try:
             results_stream = transact_stub.VectorSearch(vector_search_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
         async_results = []
         async for result in results_stream:
             async_results.append(self._respond_neighbor(result))
 
         return async_results
 
     async def wait_for_index_completion(
-        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize, wait_interval: Optional[int] = 12
+        self,
+        *,
+        namespace: str,
+        name: str,
+        timeout: Optional[int] = sys.maxsize,
+        wait_interval: Optional[int] = 12,
+        validation_threshold: Optional[int] = 2,
     ) -> None:
         """
         Wait for the index to have no pending index update operations.
 
         Args:
             namespace (str): The namespace of the index.
             name (str): The name of the index.
             timeout (int, optional): The maximum time (in seconds) to wait for the index to complete.
             Defaults to sys.maxsize.
             wait_interval (int, optional): The time (in seconds) to wait between index completion status request to the server.
             Lowering this value increases the chance that the index completion status is incorrect, which can result in poor search accuracy.
-            
+
         Raises:
             Exception: Raised when the timeout occurs while waiting for index completion.
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         Note:
             The function polls the index status with a wait interval of 10 seconds until either
             the timeout is reached or the index has no pending index update operations.
         """
         await self._channel_provider._is_ready()
 
         # Wait interval between polling
-        (index_stub, wait_interval, start_time, unmerged_record_initialized, double_check, index_completion_request) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
+        (
+            index_stub,
+            wait_interval,
+            start_time,
+            unmerged_record_initialized,
+            validation_count,
+            index_completion_request,
+        ) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
         while True:
             try:
                 index_status = await index_stub.GetStatus(index_completion_request)
 
             except grpc.RpcError as e:
                 if e.code() == grpc.StatusCode.UNAVAILABLE:
                     continue
                 else:
                     logger.error("Failed with error: %s", e)
-                    raise e
-            if self._check_completion_condition(start_time, timeout, index_status, unmerged_record_initialized):
-                if double_check:
+                    raise types.AVSServerError(rpc_error=e)
+            if self._check_completion_condition(
+                start_time, timeout, index_status, unmerged_record_initialized
+            ):
+                if validation_count == validation_threshold:
                     return
                 else:
-                    double_check = True
+                    validation_count += 1
             else:
-                double_check = False
+                validation_count = 0
             await asyncio.sleep(wait_interval)
 
     async def close(self):
         """
         Close the Aerospike Vector Search Vector Client.
 
         This method closes gRPC channels connected to Aerospike Vector Search.
@@ -295,8 +429,8 @@
         """
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         """
         Exit an asynchronous context manager for the vector client.
         """
-        await self.close()
+        await self.close()
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/aio/internal/channel_provider.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/aio/internal/channel_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 from ...shared import base_channel_provider
 
 empty = google.protobuf.empty_pb2.Empty()
 
 logger = logging.getLogger(__name__)
 
 
-
 class ChannelProvider(base_channel_provider.BaseChannelProvider):
-    """Proximus Channel Provider"""
+    """AVS Channel Provider"""
+
     def __init__(
-        self, seeds: tuple[types.HostPort, ...], listener_name: Optional[str] = None, is_loadbalancer: Optional[bool] = False
+        self,
+        seeds: tuple[types.HostPort, ...],
+        listener_name: Optional[str] = None,
+        is_loadbalancer: Optional[bool] = False,
     ) -> None:
         super().__init__(seeds, listener_name, is_loadbalancer)
         asyncio.create_task(self._tend())
-        self._tend_initalized: asyncio.Event =  asyncio.Event()
+        self._tend_initalized: asyncio.Event = asyncio.Event()
 
-        self._tend_ended: asyncio.Event =  asyncio.Event()
+        self._tend_ended: asyncio.Event = asyncio.Event()
         self._task: Optional[asyncio.Task] = None
 
-
-
     async def close(self):
         self._closed = True
         await self._tend_ended.wait()
 
         for channel in self._seedChannels:
             await channel.close()
 
@@ -63,15 +64,17 @@
 
             stub = vector_db_pb2_grpc.ClusterInfoStub(channel)
             stubs.append(stub)
             try:
                 tasks.append(stub.GetClusterId(empty))
 
             except Exception as e:
-                logger.debug("While tending, failed to get cluster id with error:" + str(e))
+                logger.debug(
+                    "While tending, failed to get cluster id with error:" + str(e)
+                )
 
         new_cluster_ids = await asyncio.gather(*tasks)
 
         for index, value in enumerate(new_cluster_ids):
             if self.check_cluster_id(value.id):
                 update_endpoints_stub = stubs[index]
                 break
@@ -81,51 +84,57 @@
                 response = await update_endpoints_stub.GetClusterEndpoints(
                     vector_db_pb2.ClusterNodeEndpointsRequest(
                         listenerName=self.listener_name
                     )
                 )
                 temp_endpoints = self.update_temp_endpoints(response, temp_endpoints)
             except Exception as e:
-                logger.debug("While tending, failed to get cluster endpoints with error:" + str(e))
+                logger.debug(
+                    "While tending, failed to get cluster endpoints with error:"
+                    + str(e)
+                )
 
             tasks = []
             add_new_channel_info = []
 
             for node, newEndpoints in temp_endpoints.items():
-                (channel_endpoints, add_new_channel) = self.check_for_new_endpoints(node, newEndpoints)
-                
+                (channel_endpoints, add_new_channel) = self.check_for_new_endpoints(
+                    node, newEndpoints
+                )
+
                 if add_new_channel:
                     try:
                         # TODO: Wait for all calls to drain
                         tasks.append(channel_endpoints.channel.close())
                     except Exception as e:
-                        logger.debug("While tending, failed to close GRPC channel:" + str(e))
+                        logger.debug(
+                            "While tending, failed to close GRPC channel:" + str(e)
+                        )
                     add_new_channel_info.append((node, newEndpoints))
 
-
             for node, newEndpoints in add_new_channel_info:
                 self.add_new_channel_to_node_channels(node, newEndpoints)
 
-
-            temp_node_channels = self._node_channels.items()
-            for node, channel_endpoints in temp_node_channels:
-                if not temp_endpoints.get(node):
+            for node, channel_endpoints in list(self._node_channels.items()):
+                if not self._node_channels.get(node):
                     try:
                         # TODO: Wait for all calls to drain
                         tasks.append(channel_endpoints.channel.close())
                         del self._node_channels[node]
-                        
+
                     except Exception as e:
-                        logger.debug("While tending, failed to close GRPC channel:" + str(e))
+                        logger.debug(
+                            "While tending, failed to close GRPC channel:" + str(e)
+                        )
 
             await asyncio.gather(*tasks)
 
         self._tend_initalized.set()
 
         # TODO: check tend interval.
         await asyncio.sleep(1)
         self._task = asyncio.create_task(self._tend())
 
     def _create_channel(self, host: str, port: int, is_tls: bool) -> grpc.aio.Channel:
         # TODO: Take care of TLS
         host = re.sub(r"%.*", "", host)
-        return grpc.aio.insecure_channel(f"{host}:{port}")
+        return grpc.aio.insecure_channel(f"{host}:{port}")
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/client.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from . import types
 from .internal import channel_provider
 from .shared.client_helpers import BaseClient
 
 logger = logging.getLogger(__name__)
 
+
 class Client(BaseClient):
     """
     Aerospike Vector Search Admin Client
 
     This client specializes in performing database operations with vector data.
     Moreover, the client supports Hierarchical Navigable Small World (HNSW) vector searches,
     allowing users to find vectors similar to a given query vector within an index.
@@ -42,75 +43,152 @@
             Exception: Raised when no seed host is provided.
         """
         seeds = self._prepare_seeds(seeds)
         self._channel_provider = channel_provider.ChannelProvider(
             seeds, listener_name, is_loadbalancer
         )
 
-    def put(
+    def insert(
+        self,
+        *,
+        namespace: str,
+        key: Union[int, str, bytes, bytearray],
+        record_data: dict[str, Any],
+        set_name: Optional[str] = None,
+    ) -> None:
+        """
+        Insert a record into Aerospike Vector Search.
+
+        If record does exist, an exception is raised.
+        If record doesn't exist, the record is inserted.
+
+        Args:
+            namespace (str): The namespace for the record.
+            key (Union[int, str, bytes, bytearray]): The key for the record.
+            record_data (dict[str, Any]): The data to be stored in the record.
+            set_name (Optional[str], optional): The name of the set to which the record belongs. Defaults to None.
+
+        Raises:
+            grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
+            This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
+
+        """
+        (transact_stub, insert_request) = self._prepare_insert(
+            namespace, key, record_data, set_name, logger
+        )
+
+        try:
+            transact_stub.Put(insert_request)
+        except grpc.RpcError as e:
+            logger.error("Failed with error: %s", e)
+            raise types.AVSServerError(rpc_error=e)
+
+    def update(
+        self,
+        *,
+        namespace: str,
+        key: Union[int, str, bytes, bytearray],
+        record_data: dict[str, Any],
+        set_name: Optional[str] = None,
+    ) -> None:
+        """
+        Update a record in Aerospike Vector Search.
+
+        If record does exist, update the record.
+        If record doesn't exist, an exception is raised.
+
+        Args:
+            namespace (str): The namespace for the record.
+            key (Union[int, str, bytes, bytearray]): The key for the record.
+            record_data (dict[str, Any]): The data to be stored in the record.
+            set_name (Optional[str], optional): The name of the set to which the record belongs. Defaults to None.
+
+        Raises:
+            grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
+            This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
+
+        """
+        (transact_stub, update_request) = self._prepare_update(
+            namespace, key, record_data, set_name, logger
+        )
+
+        try:
+            transact_stub.Put(update_request)
+        except grpc.RpcError as e:
+            logger.error("Failed with error: %s", e)
+            raise types.AVSServerError(rpc_error=e)
+
+    def upsert(
         self,
         *,
         namespace: str,
         key: Union[int, str, bytes, bytearray],
         record_data: dict[str, Any],
         set_name: Optional[str] = None,
     ) -> None:
         """
-        Write a record to Aerospike Vector Search.
+        Upsert a record in Aerospike Vector Search.
+
+        If record does exist, update the record.
+        If record doesn't exist, the record is inserted.
 
         Args:
             namespace (str): The namespace for the record.
             key (Union[int, str, bytes, bytearray]): The key for the record.
             record_data (dict[str, Any]): The data to be stored in the record.
             set_name (Optional[str], optional): The name of the set to which the record belongs. Defaults to None.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         """
-        (transact_stub, put_request) = self._prepare_put(namespace, key, record_data, set_name, logger)
+        (transact_stub, upsert_request) = self._prepare_upsert(
+            namespace, key, record_data, set_name, logger
+        )
 
         try:
-            transact_stub.Put(put_request)
+            transact_stub.Put(upsert_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
 
     def get(
         self,
         *,
         namespace: str,
         key: Union[int, str, bytes, bytearray],
-        bin_names: Optional[list[str]] = None,
+        field_names: Optional[list[str]] = None,
         set_name: Optional[str] = None,
     ) -> types.RecordWithKey:
         """
         Read a record from Aerospike Vector Search.
 
         Args:
             namespace (str): The namespace for the record.
             key (Union[int, str, bytes, bytearray]): The key for the record.
-            bin_names (Optional[list[str]], optional): A list of bin names to retrieve from the record.
-            If None, all bins are retrieved. Defaults to None.
+            field_names (Optional[list[str]], optional): A list of field names to retrieve from the record.
+            If None, all fields are retrieved. Defaults to None.
             set_name (Optional[str], optional): The name of the set from which to read the record. Defaults to None.
 
         Returns:
             types.RecordWithKey: A record with its associated key.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (transact_stub, key, get_request) = self._prepare_get(namespace, key, bin_names, set_name, logger)
+        (transact_stub, key, get_request) = self._prepare_get(
+            namespace, key, field_names, set_name, logger
+        )
         try:
             response = transact_stub.Get(get_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
 
         return self._respond_get(response, key)
 
     def exists(
         self, *, namespace: str, key: Any, set_name: Optional[str] = None
     ) -> bool:
         """
@@ -124,23 +202,49 @@
         Returns:
             bool: True if the record exists, False otherwise.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (transact_stub, key) = self._prepare_exists(namespace, key, set_name, logger)
+        (transact_stub, exists_request) = self._prepare_exists(
+            namespace, key, set_name, logger
+        )
         try:
-            response = transact_stub.Exists(key)
+            response = transact_stub.Exists(exists_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
 
         return self._respond_exists(response)
 
+    def delete(
+        self, *, namespace: str, key: Any, set_name: Optional[str] = None
+    ) -> None:
+        """
+        Delete a record from Aerospike Vector Search.
+
+        Args:
+            namespace (str): The namespace for the record.
+            key (Any): The key for the record.
+            set_name (Optional[str], optional): The name of the set to which the record belongs. Defaults to None.
+
+        Raises:
+            grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
+            This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
+        """
+        (transact_stub, delete_request) = self._prepare_delete(
+            namespace, key, set_name, logger
+        )
+        try:
+            transact_stub.Delete(delete_request)
+        except grpc.RpcError as e:
+            logger.error("Failed with error: %s", e)
+            raise types.AVSServerError(rpc_error=e)
+
     def is_indexed(
         self,
         *,
         namespace: str,
         key: Union[int, str, bytes, bytearray],
         index_name: str,
         index_namespace: Optional[str] = None,
@@ -160,67 +264,77 @@
         Returns:
             bool: True if the record is indexed, False otherwise.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (transact_stub, is_indexed_request) = self._prepare_is_indexed(namespace, key, index_name, index_namespace, set_name, logger)
+        (transact_stub, is_indexed_request) = self._prepare_is_indexed(
+            namespace, key, index_name, index_namespace, set_name, logger
+        )
         try:
             response = transact_stub.IsIndexed(is_indexed_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
         return self._respond_is_indexed(response)
 
     def vector_search(
         self,
         *,
         namespace: str,
         index_name: str,
         query: list[Union[bool, float]],
         limit: int,
         search_params: Optional[types.HnswSearchParams] = None,
-        bin_names: Optional[list[str]] = None,
+        field_names: Optional[list[str]] = None,
     ) -> list[types.Neighbor]:
         """
-        Perform a Hierarchical Navigable Small World (HNSW) vector search in Aerospike Vector Search. 
+        Perform a Hierarchical Navigable Small World (HNSW) vector search in Aerospike Vector Search.
 
         Args:
             namespace (str): The namespace for the records.
             index_name (str): The name of the index.
             query (list[Union[bool, float]]): The query vector for the search.
             limit (int): The maximum number of neighbors to return. K value.
             search_params (Optional[types_pb2.HnswSearchParams], optional): Parameters for the HNSW algorithm.
             If None, the default parameters for the index are used. Defaults to None.
-            bin_names (Optional[list[str]], optional): A list of bin names to retrieve from the results.
-            If None, all bins are retrieved. Defaults to None.
+            field_names (Optional[list[str]], optional): A list of field names to retrieve from the results.
+            If None, all fields are retrieved. Defaults to None.
 
         Returns:
             list[types.Neighbor]: A list of neighbors records found by the search.
 
         Raises:
             grpc.RpcError: Raised if an error occurs during the RPC communication with the server while attempting to create the index.
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
         """
-        (transact_stub, vector_search_request) = self._prepare_vector_search(namespace, index_name, query, limit, search_params, bin_names, logger)
+        (transact_stub, vector_search_request) = self._prepare_vector_search(
+            namespace, index_name, query, limit, search_params, field_names, logger
+        )
 
         try:
             results_stream = transact_stub.VectorSearch(vector_search_request)
         except grpc.RpcError as e:
             logger.error("Failed with error: %s", e)
-            raise e
+            raise types.AVSServerError(rpc_error=e)
         results = []
         for result in results_stream:
             results.append(self._respond_neighbor(result))
 
         return results
 
     def wait_for_index_completion(
-        self, *, namespace: str, name: str, timeout: Optional[int] = sys.maxsize, wait_interval: Optional[int] = 12
+        self,
+        *,
+        namespace: str,
+        name: str,
+        timeout: Optional[int] = sys.maxsize,
+        wait_interval: Optional[int] = 12,
+        validation_checks: Optional[int] = 2,
     ) -> None:
         """
         Wait for the index to have no pending index update operations.
 
         Args:
             namespace (str): The namespace of the index.
             name (str): The name of the index.
@@ -235,32 +349,41 @@
             This error could occur due to various reasons such as network issues, server-side failures, or invalid request parameters.
 
         Note:
             The function polls the index status with a wait interval of 10 seconds until either
             the timeout is reached or the index has no pending index update operations.
         """
         # Wait interval between polling
-        (index_stub, wait_interval, start_time, unmerged_record_initialized, double_check, index_completion_request) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
+        (
+            index_stub,
+            wait_interval,
+            start_time,
+            unmerged_record_initialized,
+            consecutive_index_validations,
+            index_completion_request,
+        ) = self._prepare_wait_for_index_waiting(namespace, name, wait_interval)
         while True:
             try:
                 index_status = index_stub.GetStatus(index_completion_request)
 
             except grpc.RpcError as e:
                 if e.code() == grpc.StatusCode.UNAVAILABLE:
                     continue
                 else:
                     logger.error("Failed with error: %s", e)
-                    raise e
-            if self._check_completion_condition(start_time, timeout, index_status, unmerged_record_initialized):
-                if double_check:
+                    raise types.AVSServerError(rpc_error=e)
+            if self._check_completion_condition(
+                start_time, timeout, index_status, unmerged_record_initialized
+            ):
+                if consecutive_index_validations == validation_checks:
                     return
                 else:
-                    double_check = True
+                    consecutive_index_validations += 1
             else:
-                double_check = False
+                consecutive_index_validations = 0
             time.sleep(wait_interval)
 
     def close(self):
         """
         Close the Aerospike Vector Search Vector Client.
 
         This method closes gRPC channels connected to Aerospike Vector Search.
@@ -279,8 +402,8 @@
         """
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """
         Exit an asynchronous context manager for the vector client.
         """
-        self.close()
+        self.close()
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/internal/channel_provider.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/internal/channel_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,20 @@
 empty = google.protobuf.empty_pb2.Empty()
 
 logger = logging.getLogger(__name__)
 
 
 class ChannelProvider(base_channel_provider.BaseChannelProvider):
     """Proximus Channel Provider"""
+
     def __init__(
-        self, seeds: tuple[types.HostPort, ...], listener_name: Optional[str] = None, is_loadbalancer: Optional[bool] = False
+        self,
+        seeds: tuple[types.HostPort, ...],
+        listener_name: Optional[str] = None,
+        is_loadbalancer: Optional[bool] = False,
     ) -> None:
         super().__init__(seeds, listener_name, is_loadbalancer)
         self._tend_ended = threading.Event()
         self._timer = None
         self._tend()
 
     def close(self):
@@ -36,71 +40,80 @@
 
         for k, channelEndpoints in self._node_channels.items():
             if channelEndpoints.channel:
                 channelEndpoints.channel.close()
 
         if self._timer != None:
             self._timer.join()
- 
+
     def _tend(self):
         (temp_endpoints, update_endpoints_stub, channels, end_tend) = self.init_tend()
 
         if end_tend:
             self._tend_ended.set()
 
             return
         for channel in channels:
 
             stub = vector_db_pb2_grpc.ClusterInfoStub(channel)
-            
+
             try:
                 new_cluster_id = stub.GetClusterId(empty).id
                 if self.check_cluster_id(new_cluster_id):
                     update_endpoints_stub = stub
                     break
                 else:
                     continue
 
             except Exception as e:
-                logger.debug("While tending, failed to get cluster id with error:" + str(e))
-
+                logger.debug(
+                    "While tending, failed to get cluster id with error:" + str(e)
+                )
 
         if update_endpoints_stub:
             try:
                 response = stub.GetClusterEndpoints(
                     vector_db_pb2.ClusterNodeEndpointsRequest(
                         listenerName=self.listener_name
                     )
                 )
                 temp_endpoints = self.update_temp_endpoints(response, temp_endpoints)
             except Exception as e:
-                logger.debug("While tending, failed to get cluster endpoints with error:" + str(e))
+                logger.debug(
+                    "While tending, failed to get cluster endpoints with error:"
+                    + str(e)
+                )
 
             for node, newEndpoints in temp_endpoints.items():
-                (channel_endpoints, add_new_channel) = self.check_for_new_endpoints(node, newEndpoints)
+                (channel_endpoints, add_new_channel) = self.check_for_new_endpoints(
+                    node, newEndpoints
+                )
 
                 if add_new_channel:
                     try:
                         # TODO: Wait for all calls to drain
                         channel_endpoints.channel.close()
                     except Exception as e:
-                        logger.debug("While tending, failed to close GRPC channel:" + str(e))
+                        logger.debug(
+                            "While tending, failed to close GRPC channel:" + str(e)
+                        )
 
                     self.add_new_channel_to_node_channels(node, newEndpoints)
 
-            temp_node_channels = self._node_channels.items()
-            for node, channel_endpoints in temp_node_channels:
-                if not temp_endpoints.get(node):
-                    # TODO: Wait for all calls to drain
+            for node, channel_endpoints in list(self._node_channels.items()):
+                if not self._node_channels.get(node):
                     try:
+                        # TODO: Wait for all calls to drain
                         channel_endpoints.channel.close()
                         del self._node_channels[node]
-                        
+
                     except Exception as e:
-                        logger.debug("While tending, failed to close GRPC channel:" + str(e))
+                        logger.debug(
+                            "While tending, failed to close GRPC channel:" + str(e)
+                        )
         # TODO: check tend interval.
         self._timer = threading.Timer(1, self._tend).start()
 
     def _create_channel(self, host: str, port: int, is_tls: bool) -> grpc.Channel:
         # TODO: Take care of TLS
         host = re.sub(r"%.*", "", host)
         return grpc.insecure_channel(f"{host}:{port}")
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/admin_helpers.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/admin_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,26 @@
 
 
 class BaseClient(object):
 
     def _prepare_seeds(self, seeds) -> None:
         return helpers._prepare_seeds(seeds)
 
-    def _prepare_index_create(self, namespace, name, vector_field, dimensions, vector_distance_metric, sets, index_params, index_meta_data, logger) -> None:
+    def _prepare_index_create(
+        self,
+        namespace,
+        name,
+        vector_field,
+        dimensions,
+        vector_distance_metric,
+        sets,
+        index_params,
+        index_meta_data,
+        logger,
+    ) -> None:
 
         logger.debug(
             "Creating index: namespace=%s, name=%s, vector_field=%s, dimensions=%d, vector_distance_metric=%s, "
             "sets=%s, index_params=%s, index_meta_data=%s",
             namespace,
             name,
             vector_field,
@@ -47,22 +58,22 @@
         index_stub = self._get_index_stub()
 
         index_create_request = types_pb2.IndexDefinition(
             id=id,
             vectorDistanceMetric=vector_distance_metric,
             setFilter=sets,
             hnswParams=index_params,
-            bin=vector_field,
+            field=vector_field,
             dimensions=dimensions,
             labels=index_meta_data,
         )
         return (index_stub, index_create_request)
 
     def _prepare_index_drop(self, namespace, name, logger) -> None:
-        
+
         logger.debug("Dropping index: namespace=%s, name=%s", namespace, name)
 
         index_stub = self._get_index_stub()
         index_drop_request = self._get_index_id(namespace, name)
 
         return (index_stub, index_drop_request)
 
@@ -89,15 +100,14 @@
     def _prepare_index_get_status(self, namespace, name, logger) -> None:
 
         logger.debug("Getting index status: namespace=%s, name=%s", namespace, name)
 
         index_stub = self._get_index_stub()
         index_get_status_request = self._get_index_id(namespace, name)
 
-
         return (index_stub, index_get_status_request)
 
     def _respond_index_list(self, response) -> None:
         response_list = []
         for index in response.indices:
             response_dict = MessageToDict(index)
 
@@ -137,21 +147,20 @@
         response_dict["hnsw_params"] = hnsw_params_dict
         return response_dict
 
     def _respond_index_get_status(self, response) -> None:
         return response.unmergedRecordCount
 
     def _get_index_stub(self):
-        return index_pb2_grpc.IndexServiceStub(
-            self._channel_provider.get_channel()
-        )
+        return index_pb2_grpc.IndexServiceStub(self._channel_provider.get_channel())
 
     def _get_index_id(self, namespace, name):
         return types_pb2.IndexId(namespace=namespace, name=name)
 
     def _prepare_wait_for_index_waiting(self, namespace, name, wait_interval):
-        return helpers._prepare_wait_for_index_waiting(self, namespace, name, wait_interval)
-
+        return helpers._prepare_wait_for_index_waiting(
+            self, namespace, name, wait_interval
+        )
 
     def _check_timeout(self, start_time, timeout):
         if start_time + timeout < time.monotonic():
-            raise "timed-out waiting for index creation"
+            raise "timed-out waiting for index creation"
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/base_channel_provider.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/base_channel_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,55 +6,63 @@
 import grpc
 
 from .. import types
 from .proto_generated import vector_db_pb2
 
 logger = logging.getLogger(__name__)
 
+
 class ChannelAndEndpoints(object):
     def __init__(
-        self, channel: Union[grpc.Channel, grpc.aio.Channel], endpoints: vector_db_pb2.ServerEndpointList
+        self,
+        channel: Union[grpc.Channel, grpc.aio.Channel],
+        endpoints: vector_db_pb2.ServerEndpointList,
     ) -> None:
         self.channel = channel
         self.endpoints = endpoints
 
 
 class BaseChannelProvider(object):
     """Proximus Channel Provider"""
+
     def __init__(
-        self, seeds: tuple[types.HostPort, ...], listener_name: Optional[str] = None, is_loadbalancer: Optional[bool] = False
+        self,
+        seeds: tuple[types.HostPort, ...],
+        listener_name: Optional[str] = None,
+        is_loadbalancer: Optional[bool] = False,
     ) -> None:
         self.seeds: tuple[types.HostPort, ...] = seeds
         self.listener_name: Optional[str] = listener_name
         self._is_loadbalancer: Optional[bool] = is_loadbalancer
         # dict of Node Number and ChannelAndEndponts object
         self._node_channels: dict[int, ChannelAndEndpoints] = {}
         self._seedChannels: Union[list[grpc.Channel], list[grpc.Channel.aio]] = [
             self._create_channel_from_host_port(seed) for seed in self.seeds
         ]
         self._closed: bool = False
         self._cluster_id: int = 0
 
-
     def get_channel(self) -> Union[grpc.aio.Channel, grpc.Channel]:
         if not self._is_loadbalancer:
             discovered_channels: list[ChannelAndEndpoints] = list(
-                self._node_channels.values())
+                self._node_channels.values()
+            )
             if len(discovered_channels) <= 0:
                 return self._seedChannels[0]
 
-
             # Return a random channel.
             channel = random.choice(discovered_channels).channel
             if channel:
                 return channel
 
         return self._seedChannels[0]
 
-    def _create_channel_from_host_port(self, host: types.HostPort) -> Union[grpc.aio.Channel, grpc.Channel]:
+    def _create_channel_from_host_port(
+        self, host: types.HostPort
+    ) -> Union[grpc.aio.Channel, grpc.Channel]:
         return self._create_channel(host.host, host.port, host.is_tls)
 
     def _create_channel_from_server_endpoint_list(
         self, endpoints: vector_db_pb2.ServerEndpointList
     ) -> Union[grpc.aio.Channel, grpc.Channel]:
         # TODO: Create channel with all endpoints
         for endpoint in endpoints.endpoints:
@@ -67,20 +75,16 @@
                 )
             except Exception as e:
                 logger.debug("failure creating channel: " + str(e))
 
     def add_new_channel_to_node_channels(self, node, newEndpoints):
 
         # We have discovered a new node
-        new_channel = self._create_channel_from_server_endpoint_list(
-            newEndpoints
-        )
-        self._node_channels[node] = ChannelAndEndpoints(
-            new_channel, newEndpoints
-        )
+        new_channel = self._create_channel_from_server_endpoint_list(newEndpoints)
+        self._node_channels[node] = ChannelAndEndpoints(new_channel, newEndpoints)
 
     def init_tend(self) -> None:
         end_tend = False
         if self._is_loadbalancer:
             # Skip tend if we are behind a load-balancer
             end_tend = True
 
@@ -92,15 +96,14 @@
 
         update_endpoints_stub = None
         channels = self._seedChannels + [
             x.channel for x in self._node_channels.values()
         ]
         return (temp_endpoints, update_endpoints_stub, channels, end_tend)
 
-
     def check_cluster_id(self, new_cluster_id) -> None:
         if new_cluster_id == self._cluster_id:
             return False
 
         self._cluster_id = new_cluster_id
 
         return True
@@ -108,23 +111,21 @@
     def update_temp_endpoints(self, response, temp_endpoints):
         endpoints = response.endpoints
         if len(endpoints) > len(temp_endpoints):
             return endpoints
         else:
             return temp_endpoints
 
-
     def check_for_new_endpoints(self, node, newEndpoints):
 
         channel_endpoints = self._node_channels.get(node)
         add_new_channel = True
 
         if channel_endpoints:
             # We have this node. Check if the endpoints changed.
             if channel_endpoints.endpoints == newEndpoints:
                 # Nothing to be done for this node
                 add_new_channel = False
             else:
                 add_new_channel = True
 
         return (channel_endpoints, add_new_channel)
-
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/client_helpers.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/client_helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,99 @@
 from typing import Any, Optional, Union
 import time
+import numpy
 from . import conversions
 
 from .proto_generated import transact_pb2
 from .proto_generated import transact_pb2_grpc
 from .. import types
 from .proto_generated import types_pb2
 from . import helpers
 
+
 class BaseClient(object):
 
     def _prepare_seeds(self, seeds) -> None:
         return helpers._prepare_seeds(seeds)
-        
-    def _prepare_put(self, namespace, key, record_data, set_name, logger) -> None:
+
+    def _prepare_put(
+        self, namespace, key, record_data, set_name, write_type, logger
+    ) -> None:
 
         logger.debug(
             "Putting record: namespace=%s, key=%s, record_data:%s, set_name:%s",
             namespace,
             key,
             record_data,
             set_name,
         )
 
         key = self._get_key(namespace, set_name, key)
-        bin_list = [
-            types_pb2.Bin(name=k, value=conversions.toVectorDbValue(v))
-            for (k, v) in record_data.items()
-        ]
+        field_list = []
+
+        for k, v in record_data.items():
+            if isinstance(v, numpy.ndarray):
+                field_list.append(
+                    types_pb2.Field(
+                        name=k, value=conversions.toVectorDbValue(v.tolist())
+                    )
+                )
+
+            else:
+                field_list.append(
+                    types_pb2.Field(name=k, value=conversions.toVectorDbValue(v))
+                )
 
         transact_stub = self._get_transact_stub()
-        put_request = transact_pb2.PutRequest(key=key, bins=bin_list)
+        put_request = transact_pb2.PutRequest(
+            key=key, writeType=write_type, fields=field_list
+        )
 
         return (transact_stub, put_request)
 
-    def _prepare_get(self, namespace, key, bin_names, set_name, logger) -> None:
+    def _prepare_insert(self, namespace, key, record_data, set_name, logger) -> None:
+        return self._prepare_put(
+            namespace,
+            key,
+            record_data,
+            set_name,
+            transact_pb2.WriteType.INSERT_ONLY,
+            logger,
+        )
 
-        logger.debug(
-            "Getting record: namespace=%s, key=%s, bin_names:%s, set_name:%s",
+    def _prepare_update(self, namespace, key, record_data, set_name, logger) -> None:
+        return self._prepare_put(
             namespace,
             key,
-            bin_names,
+            record_data,
             set_name,
+            transact_pb2.WriteType.UPDATE_ONLY,
+            logger,
         )
 
+    def _prepare_upsert(self, namespace, key, record_data, set_name, logger) -> None:
+        return self._prepare_put(
+            namespace, key, record_data, set_name, transact_pb2.WriteType.UPSERT, logger
+        )
+
+    def _prepare_get(self, namespace, key, field_names, set_name, logger) -> None:
+
+        logger.debug(
+            "Getting record: namespace=%s, key=%s, field_names:%s, set_name:%s",
+            namespace,
+            key,
+            field_names,
+            set_name,
+        )
 
         key = self._get_key(namespace, set_name, key)
-        bin_selector = self._get_bin_selector(bin_names=bin_names)
+        projection_spec = self._get_projection_spec(field_names=field_names)
 
         transact_stub = self._get_transact_stub()
-        get_request = transact_pb2.GetRequest(key=key, binSelector=bin_selector)
+        get_request = transact_pb2.GetRequest(key=key, projectionSpec=projection_spec)
 
         return (transact_stub, key, get_request)
 
     def _prepare_exists(self, namespace, key, set_name, logger) -> None:
 
         logger.debug(
             "Getting record existence: namespace=%s, key=%s, set_name:%s",
@@ -61,18 +101,37 @@
             key,
             set_name,
         )
 
         key = self._get_key(namespace, set_name, key)
 
         transact_stub = self._get_transact_stub()
+        exists_request = transact_pb2.ExistsRequest(key=key)
 
-        return (transact_stub, key)
+        return (transact_stub, exists_request)
 
-    def _prepare_is_indexed(self, namespace, key, index_name, index_namespace, set_name, logger) -> None:
+    def _prepare_delete(self, namespace, key, set_name, logger) -> None:
+
+        logger.debug(
+            "Deleting record: key=%s",
+            namespace,
+            key,
+            set_name,
+        )
+
+        key = self._get_key(namespace, set_name, key)
+
+        transact_stub = self._get_transact_stub()
+        delete_request = transact_pb2.DeleteRequest(key=key)
+
+        return (transact_stub, delete_request)
+
+    def _prepare_is_indexed(
+        self, namespace, key, index_name, index_namespace, set_name, logger
+    ) -> None:
 
         logger.debug(
             "Checking if index exists: namespace=%s, key=%s, index_name=%s, index_namespace=%s, set_name=%s",
             namespace,
             key,
             index_name,
             index_namespace,
@@ -85,96 +144,128 @@
         key = self._get_key(namespace, set_name, key)
 
         transact_stub = self._get_transact_stub()
         is_indexed_request = transact_pb2.IsIndexedRequest(key=key, indexId=index_id)
 
         return (transact_stub, is_indexed_request)
 
-    def _prepare_vector_search(self, namespace, index_name, query, limit, search_params, bin_names, logger) -> None:
+    def _prepare_vector_search(
+        self, namespace, index_name, query, limit, search_params, field_names, logger
+    ) -> None:
 
         logger.debug(
-            "Performing vector search: namespace=%s, index_name=%s, query=%s, limit=%s, search_params=%s, bin_names=%s",
+            "Performing vector search: namespace=%s, index_name=%s, query=%s, limit=%s, search_params=%s, field_names=%s",
             namespace,
             index_name,
             query,
             limit,
             search_params,
-            bin_names,
+            field_names,
         )
 
         if search_params != None:
             search_params = search_params._to_pb2()
-        bin_selector = self._get_bin_selector(bin_names=bin_names)
+
+        projection_spec = self._get_projection_spec(field_names=field_names)
+
         index = types_pb2.IndexId(namespace=namespace, name=index_name)
-        query_vector = conversions.toVectorDbValue(query).vectorValue
 
+        if isinstance(query, numpy.ndarray):
+            query_vector = conversions.toVectorDbValue(query.tolist()).vectorValue
+        else:
+            query_vector = conversions.toVectorDbValue(query).vectorValue
 
         transact_stub = self._get_transact_stub()
 
         vector_search_request = transact_pb2.VectorSearchRequest(
             index=index,
             queryVector=query_vector,
             limit=limit,
             hnswSearchParams=search_params,
-            binSelector=bin_selector,
+            projection=projection_spec,
         )
-        
+
         return (transact_stub, vector_search_request)
 
     def _get_transact_stub(self):
-        return transact_pb2_grpc.TransactStub(
-            self._channel_provider.get_channel()
-        )
+        return transact_pb2_grpc.TransactStub(self._channel_provider.get_channel())
 
     def _respond_get(self, response, key) -> None:
         return types.RecordWithKey(
             key=conversions.fromVectorDbKey(key),
-            bins=conversions.fromVectorDbRecord(response),
+            fields=conversions.fromVectorDbRecord(response),
         )
 
     def _respond_exists(self, response) -> None:
         return response.value
 
     def _respond_is_indexed(self, response) -> None:
         return response.value
 
     def _respond_neighbor(self, response) -> None:
         return conversions.fromVectorDbNeighbor(response)
 
-    def _get_bin_selector(self, *, bin_names: Optional[list] = None):
-
-        if not bin_names:
-            bin_selector = transact_pb2.BinSelector(
-                type=transact_pb2.BinSelectorType.ALL, binNames=bin_names
+    def _get_projection_spec(
+        self,
+        *,
+        field_names: Optional[list] = None,
+        exclude_field_names: Optional[list] = None,
+    ):
+
+        if field_names:
+            include = transact_pb2.ProjectionFilter(
+                type=transact_pb2.ProjectionType.SPECIFIED, fields=field_names
+            )
+            exclude = transact_pb2.ProjectionFilter(
+                type=transact_pb2.ProjectionType.NONE, fields=None
+            )
+        elif exclude_field_names:
+            include = transact_pb2.ProjectionFilter(
+                type=transact_pb2.ProjectionType.NONE, fields=None
+            )
+            exclude = transact_pb2.ProjectionFilter(
+                type=transact_pb2.ProjectionType.SPECIFIED, fields=exclude_field_names
             )
         else:
-            bin_selector = transact_pb2.BinSelector(
-                type=transact_pb2.BinSelectorType.SPECIFIED, binNames=bin_names
+            include = transact_pb2.ProjectionFilter(
+                type=transact_pb2.ProjectionType.ALL, fields=None
             )
-        return bin_selector
+            exclude = transact_pb2.ProjectionFilter(
+                type=transact_pb2.ProjectionType.NONE, fields=None
+            )
+
+        projection_spec = transact_pb2.ProjectionSpec(include=include, exclude=exclude)
+
+        return projection_spec
 
-    def _get_key(self, namespace: str, set: str, key: Union[int, str, bytes, bytearray]):
+    def _get_key(
+        self, namespace: str, set: str, key: Union[int, str, bytes, bytearray]
+    ):
         if isinstance(key, str):
             key = types_pb2.Key(namespace=namespace, set=set, stringValue=key)
         elif isinstance(key, int):
             key = types_pb2.Key(namespace=namespace, set=set, longValue=key)
         elif isinstance(key, (bytes, bytearray)):
             key = types_pb2.Key(namespace=namespace, set=set, bytesValue=key)
         else:
             raise Exception("Invalid key type" + type(key))
         return key
 
     def _prepare_wait_for_index_waiting(self, namespace, name, wait_interval):
-        return helpers._prepare_wait_for_index_waiting(self, namespace, name, wait_interval)
+        return helpers._prepare_wait_for_index_waiting(
+            self, namespace, name, wait_interval
+        )
 
-    def _check_completion_condition(self, start_time, timeout, index_status, unmerged_record_initialized):
+    def _check_completion_condition(
+        self, start_time, timeout, index_status, unmerged_record_initialized
+    ):
 
         if start_time + 10 < time.monotonic():
             unmerged_record_initialized = True
-            
+
         if index_status.unmergedRecordCount > 0:
             unmerged_record_initialized = True
 
         if (
             index_status.unmergedRecordCount == 0
             and unmerged_record_initialized == True
         ):
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/conversions.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/conversions.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,16 @@
         return types_pb2.Value(stringValue=value)
     elif isinstance(value, int):
         return types_pb2.Value(longValue=value)
     elif isinstance(value, float):
         return types_pb2.Value(doubleValue=value)
     elif isinstance(value, (bytes, bytearray)):
         return types_pb2.Value(bytesValue=value)
+    elif isinstance(value, bool):
+        return types_pb2.Value(booleanValue=value)
     elif isinstance(value, list) and value:
         # TODO: Convert every element correctly to destination type.
         if isinstance(value[0], float):
             return types_pb2.Value(
                 vectorValue=types_pb2.Vector(
                     floatData={"value": [float(x) for x in value]}
                 )
@@ -65,31 +67,29 @@
     elif key.HasField("intValue"):
         keyValue = key.intValue
     elif key.HasField("longValue"):
         keyValue = key.longValue
     elif key.HasField("bytesValue"):
         keyValue = key.bytesValue
 
-    return types.Key(
-        namespace=key.namespace, set=key.set, digest=key.digest, key=keyValue
-    )
+    return types.Key(namespace=key.namespace, set=key.set, key=keyValue)
 
 
 def fromVectorDbRecord(record: types_pb2.Record) -> dict[str, Any]:
-    bins = {}
-    for bin in record.bins:
-        bins[bin.name] = fromVectorDbValue(bin.value)
+    fields = {}
+    for field in record.fields:
+        fields[field.name] = fromVectorDbValue(field.value)
 
-    return bins
+    return fields
 
 
 def fromVectorDbNeighbor(input: types_pb2.Neighbor) -> types.Neighbor:
     return types.Neighbor(
         key=fromVectorDbKey(input.key),
-        bins=fromVectorDbRecord(input.record),
+        fields=fromVectorDbRecord(input.record),
         distance=input.distance,
     )
 
 
 def fromVectorDbValue(input: types_pb2.Value) -> Any:
     if input.HasField("stringValue"):
         return input.stringValue
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/helpers.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 from .. import types
 from .proto_generated import types_pb2
 from .proto_generated import index_pb2_grpc
 
+
 def _prepare_seeds(seeds) -> None:
 
     if not seeds:
         raise Exception("at least one seed host needed")
 
     if isinstance(seeds, types.HostPort):
         seeds = (seeds,)
@@ -14,14 +15,19 @@
     return seeds
 
 
 def _prepare_wait_for_index_waiting(self, namespace, name, wait_interval):
 
     unmerged_record_initialized = False
     start_time = time.monotonic()
-    double_check = False
+    consecutive_index_validations = 0
 
-    index_stub = index_pb2_grpc.IndexServiceStub(
-        self._channel_provider.get_channel()
-    )
+    index_stub = index_pb2_grpc.IndexServiceStub(self._channel_provider.get_channel())
     index_wait_request = types_pb2.IndexId(namespace=namespace, name=name)
-    return (index_stub, wait_interval, start_time, unmerged_record_initialized, False, index_wait_request)
+    return (
+        index_stub,
+        wait_interval,
+        start_time,
+        unmerged_record_initialized,
+        consecutive_index_validations,
+        index_wait_request,
+    )
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/auth_pb2.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/auth_pb2_grpc.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/index_pb2.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/index_pb2.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/index_pb2_grpc.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/index_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/transact_pb2.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/transact_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,30 +12,38 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from . import types_pb2 as types__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0etransact.proto\x12\x10\x61\x65rospike.vector\x1a\x1bgoogle/protobuf/empty.proto\x1a\x0btypes.proto\"U\n\nPutRequest\x12\"\n\x03key\x18\x01 \x01(\x0b\x32\x15.aerospike.vector.Key\x12#\n\x04\x62ins\x18\x03 \x03(\x0b\x32\x15.aerospike.vector.Bin\"d\n\nGetRequest\x12\"\n\x03key\x18\x01 \x01(\x0b\x32\x15.aerospike.vector.Key\x12\x32\n\x0b\x62inSelector\x18\x02 \x01(\x0b\x32\x1d.aerospike.vector.BinSelector\"b\n\x10IsIndexedRequest\x12\"\n\x03key\x18\x01 \x01(\x0b\x32\x15.aerospike.vector.Key\x12*\n\x07indexId\x18\x02 \x01(\x0b\x32\x19.aerospike.vector.IndexId\"P\n\x0b\x42inSelector\x12/\n\x04type\x18\x01 \x01(\x0e\x32!.aerospike.vector.BinSelectorType\x12\x10\n\x08\x62inNames\x18\x02 \x03(\t\"\x81\x02\n\x13VectorSearchRequest\x12(\n\x05index\x18\x01 \x01(\x0b\x32\x19.aerospike.vector.IndexId\x12-\n\x0bqueryVector\x18\x02 \x01(\x0b\x32\x18.aerospike.vector.Vector\x12\r\n\x05limit\x18\x03 \x01(\r\x12\x32\n\x0b\x62inSelector\x18\x04 \x01(\x0b\x32\x1d.aerospike.vector.BinSelector\x12>\n\x10hnswSearchParams\x18\x05 \x01(\x0b\x32\".aerospike.vector.HnswSearchParamsH\x00\x42\x0e\n\x0csearchParams*3\n\x0f\x42inSelectorType\x12\x07\n\x03\x41LL\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\r\n\tSPECIFIED\x10\x02\x32\xed\x02\n\x08Transact\x12=\n\x03Put\x12\x1c.aerospike.vector.PutRequest\x1a\x16.google.protobuf.Empty\"\x00\x12?\n\x03Get\x12\x1c.aerospike.vector.GetRequest\x1a\x18.aerospike.vector.Record\"\x00\x12<\n\x06\x45xists\x12\x15.aerospike.vector.Key\x1a\x19.aerospike.vector.Boolean\"\x00\x12L\n\tIsIndexed\x12\".aerospike.vector.IsIndexedRequest\x1a\x19.aerospike.vector.Boolean\"\x00\x12U\n\x0cVectorSearch\x12%.aerospike.vector.VectorSearchRequest\x1a\x1a.aerospike.vector.Neighbor\"\x00\x30\x01\x42=\n\x1b\x63om.aerospike.vector.clientP\x01Z\x1c\x61\x65rospike.com/vector/protos/b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0etransact.proto\x12\x10\x61\x65rospike.vector\x1a\x1bgoogle/protobuf/empty.proto\x1a\x0btypes.proto\"\x89\x01\n\nPutRequest\x12\"\n\x03key\x18\x01 \x01(\x0b\x32\x15.aerospike.vector.Key\x12.\n\twriteType\x18\x02 \x01(\x0e\x32\x1b.aerospike.vector.WriteType\x12\'\n\x06\x66ields\x18\x03 \x03(\x0b\x32\x17.aerospike.vector.Field\"j\n\nGetRequest\x12\"\n\x03key\x18\x01 \x01(\x0b\x32\x15.aerospike.vector.Key\x12\x38\n\x0eprojectionSpec\x18\x02 \x01(\x0b\x32 .aerospike.vector.ProjectionSpec\"3\n\rExistsRequest\x12\"\n\x03key\x18\x01 \x01(\x0b\x32\x15.aerospike.vector.Key\"3\n\rDeleteRequest\x12\"\n\x03key\x18\x01 \x01(\x0b\x32\x15.aerospike.vector.Key\"b\n\x10IsIndexedRequest\x12\"\n\x03key\x18\x01 \x01(\x0b\x32\x15.aerospike.vector.Key\x12*\n\x07indexId\x18\x02 \x01(\x0b\x32\x19.aerospike.vector.IndexId\"R\n\x10ProjectionFilter\x12.\n\x04type\x18\x01 \x01(\x0e\x32 .aerospike.vector.ProjectionType\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"z\n\x0eProjectionSpec\x12\x33\n\x07include\x18\x01 \x01(\x0b\x32\".aerospike.vector.ProjectionFilter\x12\x33\n\x07\x65xclude\x18\x02 \x01(\x0b\x32\".aerospike.vector.ProjectionFilter\"\x83\x02\n\x13VectorSearchRequest\x12(\n\x05index\x18\x01 \x01(\x0b\x32\x19.aerospike.vector.IndexId\x12-\n\x0bqueryVector\x18\x02 \x01(\x0b\x32\x18.aerospike.vector.Vector\x12\r\n\x05limit\x18\x03 \x01(\r\x12\x34\n\nprojection\x18\x04 \x01(\x0b\x32 .aerospike.vector.ProjectionSpec\x12>\n\x10hnswSearchParams\x18\x05 \x01(\x0b\x32\".aerospike.vector.HnswSearchParamsH\x00\x42\x0e\n\x0csearchParams*9\n\tWriteType\x12\n\n\x06UPSERT\x10\x00\x12\x0f\n\x0bUPDATE_ONLY\x10\x01\x12\x0f\n\x0bINSERT_ONLY\x10\x02*2\n\x0eProjectionType\x12\x07\n\x03\x41LL\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\r\n\tSPECIFIED\x10\x02\x32\xbc\x03\n\x08Transact\x12=\n\x03Put\x12\x1c.aerospike.vector.PutRequest\x1a\x16.google.protobuf.Empty\"\x00\x12?\n\x03Get\x12\x1c.aerospike.vector.GetRequest\x1a\x18.aerospike.vector.Record\"\x00\x12\x43\n\x06\x44\x65lete\x12\x1f.aerospike.vector.DeleteRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x06\x45xists\x12\x1f.aerospike.vector.ExistsRequest\x1a\x19.aerospike.vector.Boolean\"\x00\x12L\n\tIsIndexed\x12\".aerospike.vector.IsIndexedRequest\x1a\x19.aerospike.vector.Boolean\"\x00\x12U\n\x0cVectorSearch\x12%.aerospike.vector.VectorSearchRequest\x1a\x1a.aerospike.vector.Neighbor\"\x00\x30\x01\x42=\n\x1b\x63om.aerospike.vector.clientP\x01Z\x1c\x61\x65rospike.com/vector/protos/b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'transact_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\033com.aerospike.vector.clientP\001Z\034aerospike.com/vector/protos/'
-  _globals['_BINSELECTORTYPE']._serialized_start=709
-  _globals['_BINSELECTORTYPE']._serialized_end=760
-  _globals['_PUTREQUEST']._serialized_start=78
-  _globals['_PUTREQUEST']._serialized_end=163
-  _globals['_GETREQUEST']._serialized_start=165
-  _globals['_GETREQUEST']._serialized_end=265
-  _globals['_ISINDEXEDREQUEST']._serialized_start=267
-  _globals['_ISINDEXEDREQUEST']._serialized_end=365
-  _globals['_BINSELECTOR']._serialized_start=367
-  _globals['_BINSELECTOR']._serialized_end=447
-  _globals['_VECTORSEARCHREQUEST']._serialized_start=450
-  _globals['_VECTORSEARCHREQUEST']._serialized_end=707
-  _globals['_TRANSACT']._serialized_start=763
-  _globals['_TRANSACT']._serialized_end=1128
+  _globals['_WRITETYPE']._serialized_start=1002
+  _globals['_WRITETYPE']._serialized_end=1059
+  _globals['_PROJECTIONTYPE']._serialized_start=1061
+  _globals['_PROJECTIONTYPE']._serialized_end=1111
+  _globals['_PUTREQUEST']._serialized_start=79
+  _globals['_PUTREQUEST']._serialized_end=216
+  _globals['_GETREQUEST']._serialized_start=218
+  _globals['_GETREQUEST']._serialized_end=324
+  _globals['_EXISTSREQUEST']._serialized_start=326
+  _globals['_EXISTSREQUEST']._serialized_end=377
+  _globals['_DELETEREQUEST']._serialized_start=379
+  _globals['_DELETEREQUEST']._serialized_end=430
+  _globals['_ISINDEXEDREQUEST']._serialized_start=432
+  _globals['_ISINDEXEDREQUEST']._serialized_end=530
+  _globals['_PROJECTIONFILTER']._serialized_start=532
+  _globals['_PROJECTIONFILTER']._serialized_end=614
+  _globals['_PROJECTIONSPEC']._serialized_start=616
+  _globals['_PROJECTIONSPEC']._serialized_end=738
+  _globals['_VECTORSEARCHREQUEST']._serialized_start=741
+  _globals['_VECTORSEARCHREQUEST']._serialized_end=1000
+  _globals['_TRANSACT']._serialized_start=1114
+  _globals['_TRANSACT']._serialized_end=1558
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/transact_pb2_grpc.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/transact_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,22 @@
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.Get = channel.unary_unary(
                 '/aerospike.vector.Transact/Get',
                 request_serializer=transact__pb2.GetRequest.SerializeToString,
                 response_deserializer=types__pb2.Record.FromString,
                 )
+        self.Delete = channel.unary_unary(
+                '/aerospike.vector.Transact/Delete',
+                request_serializer=transact__pb2.DeleteRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
         self.Exists = channel.unary_unary(
                 '/aerospike.vector.Transact/Exists',
-                request_serializer=types__pb2.Key.SerializeToString,
+                request_serializer=transact__pb2.ExistsRequest.SerializeToString,
                 response_deserializer=types__pb2.Boolean.FromString,
                 )
         self.IsIndexed = channel.unary_unary(
                 '/aerospike.vector.Transact/IsIndexed',
                 request_serializer=transact__pb2.IsIndexedRequest.SerializeToString,
                 response_deserializer=types__pb2.Boolean.FromString,
                 )
@@ -45,39 +50,51 @@
 
 
 class TransactServicer(object):
     """Record transaction services.
     """
 
     def Put(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Update/insert records.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Get(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Get a record.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def Delete(self, request, context):
+        """Delete a record.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Exists(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Check if a record exists.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def IsIndexed(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Check is a record is indexed.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def VectorSearch(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Perform a vector nearest neighbor search.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_TransactServicer_to_server(servicer, server):
     rpc_method_handlers = {
@@ -87,17 +104,22 @@
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'Get': grpc.unary_unary_rpc_method_handler(
                     servicer.Get,
                     request_deserializer=transact__pb2.GetRequest.FromString,
                     response_serializer=types__pb2.Record.SerializeToString,
             ),
+            'Delete': grpc.unary_unary_rpc_method_handler(
+                    servicer.Delete,
+                    request_deserializer=transact__pb2.DeleteRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
             'Exists': grpc.unary_unary_rpc_method_handler(
                     servicer.Exists,
-                    request_deserializer=types__pb2.Key.FromString,
+                    request_deserializer=transact__pb2.ExistsRequest.FromString,
                     response_serializer=types__pb2.Boolean.SerializeToString,
             ),
             'IsIndexed': grpc.unary_unary_rpc_method_handler(
                     servicer.IsIndexed,
                     request_deserializer=transact__pb2.IsIndexedRequest.FromString,
                     response_serializer=types__pb2.Boolean.SerializeToString,
             ),
@@ -148,26 +170,43 @@
         return grpc.experimental.unary_unary(request, target, '/aerospike.vector.Transact/Get',
             transact__pb2.GetRequest.SerializeToString,
             types__pb2.Record.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def Delete(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/aerospike.vector.Transact/Delete',
+            transact__pb2.DeleteRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def Exists(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/aerospike.vector.Transact/Exists',
-            types__pb2.Key.SerializeToString,
+            transact__pb2.ExistsRequest.SerializeToString,
             types__pb2.Boolean.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def IsIndexed(request,
             target,
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/types_pb2.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/types_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,64 +10,66 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btypes.proto\x12\x10\x61\x65rospike.vector\"\xa1\x01\n\x03Key\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x10\n\x03set\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x0e\n\x06\x64igest\x18\x03 \x01(\x0c\x12\x15\n\x0bstringValue\x18\x04 \x01(\tH\x00\x12\x14\n\nbytesValue\x18\x05 \x01(\x0cH\x00\x12\x12\n\x08intValue\x18\x06 \x01(\x05H\x00\x12\x13\n\tlongValue\x18\x07 \x01(\x03H\x00\x42\x07\n\x05valueB\x06\n\x04_set\"\x19\n\x08\x42oolData\x12\r\n\x05value\x18\x01 \x03(\x08\"\x1a\n\tFloatData\x12\r\n\x05value\x18\x01 \x03(\x02\"\x94\x01\n\x06MapKey\x12\x15\n\x0bstringValue\x18\x01 \x01(\tH\x00\x12\x14\n\nbytesValue\x18\x02 \x01(\x0cH\x00\x12\x12\n\x08intValue\x18\x03 \x01(\x05H\x00\x12\x13\n\tlongValue\x18\x04 \x01(\x03H\x00\x12\x14\n\nfloatValue\x18\x05 \x01(\x02H\x00\x12\x15\n\x0b\x64oubleValue\x18\x06 \x01(\x01H\x00\x42\x07\n\x05value\"Y\n\x08MapEntry\x12%\n\x03key\x18\x01 \x01(\x0b\x32\x18.aerospike.vector.MapKey\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.aerospike.vector.Value\"2\n\x03Map\x12+\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x1a.aerospike.vector.MapEntry\"0\n\x04List\x12(\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x17.aerospike.vector.Value\"r\n\x06Vector\x12.\n\x08\x62oolData\x18\x01 \x01(\x0b\x32\x1a.aerospike.vector.BoolDataH\x00\x12\x30\n\tfloatData\x18\x02 \x01(\x0b\x32\x1b.aerospike.vector.FloatDataH\x00\x42\x06\n\x04\x64\x61ta\"\x9c\x02\n\x05Value\x12\x15\n\x0bstringValue\x18\x01 \x01(\tH\x00\x12\x14\n\nbytesValue\x18\x02 \x01(\x0cH\x00\x12\x12\n\x08intValue\x18\x03 \x01(\x05H\x00\x12\x13\n\tlongValue\x18\x04 \x01(\x03H\x00\x12\x14\n\nfloatValue\x18\x05 \x01(\x02H\x00\x12\x15\n\x0b\x64oubleValue\x18\x06 \x01(\x01H\x00\x12)\n\x08mapValue\x18\x07 \x01(\x0b\x32\x15.aerospike.vector.MapH\x00\x12+\n\tlistValue\x18\x08 \x01(\x0b\x32\x16.aerospike.vector.ListH\x00\x12/\n\x0bvectorValue\x18\t \x01(\x0b\x32\x18.aerospike.vector.VectorH\x00\x42\x07\n\x05value\";\n\x03\x42in\x12\x0c\n\x04name\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.aerospike.vector.Value\"U\n\x06Record\x12\x12\n\ngeneration\x18\x01 \x01(\r\x12\x12\n\nexpiration\x18\x02 \x01(\r\x12#\n\x04\x62ins\x18\x03 \x03(\x0b\x32\x15.aerospike.vector.Bin\"z\n\x08Neighbor\x12\"\n\x03key\x18\x01 \x01(\x0b\x32\x15.aerospike.vector.Key\x12-\n\x06record\x18\x02 \x01(\x0b\x32\x18.aerospike.vector.RecordH\x00\x88\x01\x01\x12\x10\n\x08\x64istance\x18\x03 \x01(\x02\x42\t\n\x07_record\"*\n\x07IndexId\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tnamespace\x18\x02 \x01(\t\"\xa8\x01\n\nHnswParams\x12\x0e\n\x01m\x18\x01 \x01(\rH\x00\x88\x01\x01\x12\x1b\n\x0e\x65\x66\x43onstruction\x18\x02 \x01(\rH\x01\x88\x01\x01\x12\x0f\n\x02\x65\x66\x18\x03 \x01(\rH\x02\x88\x01\x01\x12<\n\x0e\x62\x61tchingParams\x18\x04 \x01(\x0b\x32$.aerospike.vector.HnswBatchingParamsB\x04\n\x02_mB\x11\n\x0f_efConstructionB\x05\n\x03_ef\"*\n\x10HnswSearchParams\x12\x0f\n\x02\x65\x66\x18\x01 \x01(\rH\x00\x88\x01\x01\x42\x05\n\x03_ef\"\x84\x01\n\x12HnswBatchingParams\x12\x17\n\nmaxRecords\x18\x01 \x01(\rH\x00\x88\x01\x01\x12\x15\n\x08interval\x18\x02 \x01(\rH\x01\x88\x01\x01\x12\x15\n\x08\x64isabled\x18\x03 \x01(\x08H\x02\x88\x01\x01\x42\r\n\x0b_maxRecordsB\x0b\n\t_intervalB\x0b\n\t_disabled\"W\n\x15\x41\x65rospikeIndexStorage\x12\x16\n\tnamespace\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x10\n\x03set\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x0c\n\n_namespaceB\x06\n\x04_set\"\xec\x03\n\x0fIndexDefinition\x12%\n\x02id\x18\x01 \x01(\x0b\x32\x19.aerospike.vector.IndexId\x12)\n\x04type\x18\x02 \x01(\x0e\x32\x1b.aerospike.vector.IndexType\x12\x12\n\ndimensions\x18\x03 \x01(\r\x12\x44\n\x14vectorDistanceMetric\x18\x04 \x01(\x0e\x32&.aerospike.vector.VectorDistanceMetric\x12\x0b\n\x03\x62in\x18\x05 \x01(\t\x12\x16\n\tsetFilter\x18\x06 \x01(\tH\x02\x88\x01\x01\x12\x32\n\nhnswParams\x18\x07 \x01(\x0b\x32\x1c.aerospike.vector.HnswParamsH\x00\x12\x43\n\x10\x61\x65rospikeStorage\x18\x08 \x01(\x0b\x32\'.aerospike.vector.AerospikeIndexStorageH\x01\x12=\n\x06labels\x18\t \x03(\x0b\x32-.aerospike.vector.IndexDefinition.LabelsEntry\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x08\n\x06paramsB\t\n\x07storageB\x0c\n\n_setFilter\"I\n\x13IndexDefinitionList\x12\x32\n\x07indices\x18\x01 \x03(\x0b\x32!.aerospike.vector.IndexDefinition\"\x18\n\x07\x42oolean\x12\r\n\x05value\x18\x01 \x01(\x08*f\n\x14VectorDistanceMetric\x12\x15\n\x11SQUARED_EUCLIDEAN\x10\x00\x12\n\n\x06\x43OSINE\x10\x01\x12\x0f\n\x0b\x44OT_PRODUCT\x10\x02\x12\r\n\tMANHATTAN\x10\x03\x12\x0b\n\x07HAMMING\x10\x04*\x15\n\tIndexType\x12\x08\n\x04HNSW\x10\x00\x42=\n\x1b\x63om.aerospike.vector.clientP\x01Z\x1c\x61\x65rospike.com/vector/protos/b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btypes.proto\x12\x10\x61\x65rospike.vector\"\x91\x01\n\x03Key\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x10\n\x03set\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x15\n\x0bstringValue\x18\x03 \x01(\tH\x00\x12\x14\n\nbytesValue\x18\x04 \x01(\x0cH\x00\x12\x12\n\x08intValue\x18\x05 \x01(\x05H\x00\x12\x13\n\tlongValue\x18\x06 \x01(\x03H\x00\x42\x07\n\x05valueB\x06\n\x04_set\"\x19\n\x08\x42oolData\x12\r\n\x05value\x18\x01 \x03(\x08\"\x1a\n\tFloatData\x12\r\n\x05value\x18\x01 \x03(\x02\"\x94\x01\n\x06MapKey\x12\x15\n\x0bstringValue\x18\x01 \x01(\tH\x00\x12\x14\n\nbytesValue\x18\x02 \x01(\x0cH\x00\x12\x12\n\x08intValue\x18\x03 \x01(\x05H\x00\x12\x13\n\tlongValue\x18\x04 \x01(\x03H\x00\x12\x14\n\nfloatValue\x18\x05 \x01(\x02H\x00\x12\x15\n\x0b\x64oubleValue\x18\x06 \x01(\x01H\x00\x42\x07\n\x05value\"Y\n\x08MapEntry\x12%\n\x03key\x18\x01 \x01(\x0b\x32\x18.aerospike.vector.MapKey\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.aerospike.vector.Value\"2\n\x03Map\x12+\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x1a.aerospike.vector.MapEntry\"0\n\x04List\x12(\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x17.aerospike.vector.Value\"r\n\x06Vector\x12.\n\x08\x62oolData\x18\x01 \x01(\x0b\x32\x1a.aerospike.vector.BoolDataH\x00\x12\x30\n\tfloatData\x18\x02 \x01(\x0b\x32\x1b.aerospike.vector.FloatDataH\x00\x42\x06\n\x04\x64\x61ta\"\xb4\x02\n\x05Value\x12\x15\n\x0bstringValue\x18\x01 \x01(\tH\x00\x12\x14\n\nbytesValue\x18\x02 \x01(\x0cH\x00\x12\x12\n\x08intValue\x18\x03 \x01(\x05H\x00\x12\x13\n\tlongValue\x18\x04 \x01(\x03H\x00\x12\x14\n\nfloatValue\x18\x05 \x01(\x02H\x00\x12\x15\n\x0b\x64oubleValue\x18\x06 \x01(\x01H\x00\x12)\n\x08mapValue\x18\x07 \x01(\x0b\x32\x15.aerospike.vector.MapH\x00\x12+\n\tlistValue\x18\x08 \x01(\x0b\x32\x16.aerospike.vector.ListH\x00\x12/\n\x0bvectorValue\x18\t \x01(\x0b\x32\x18.aerospike.vector.VectorH\x00\x12\x16\n\x0c\x62ooleanValue\x18\n \x01(\x08H\x00\x42\x07\n\x05value\"=\n\x05\x46ield\x12\x0c\n\x04name\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.aerospike.vector.Value\"A\n\x17\x41\x65rospikeRecordMetadata\x12\x12\n\ngeneration\x18\x01 \x01(\r\x12\x12\n\nexpiration\x18\x02 \x01(\r\"\x85\x01\n\x06Record\x12\'\n\x06\x66ields\x18\x01 \x03(\x0b\x32\x17.aerospike.vector.Field\x12\x46\n\x11\x61\x65rospikeMetadata\x18\x02 \x01(\x0b\x32).aerospike.vector.AerospikeRecordMetadataH\x00\x42\n\n\x08metadata\"z\n\x08Neighbor\x12\"\n\x03key\x18\x01 \x01(\x0b\x32\x15.aerospike.vector.Key\x12-\n\x06record\x18\x02 \x01(\x0b\x32\x18.aerospike.vector.RecordH\x00\x88\x01\x01\x12\x10\n\x08\x64istance\x18\x03 \x01(\x02\x42\t\n\x07_record\"*\n\x07IndexId\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xa8\x01\n\nHnswParams\x12\x0e\n\x01m\x18\x01 \x01(\rH\x00\x88\x01\x01\x12\x1b\n\x0e\x65\x66\x43onstruction\x18\x02 \x01(\rH\x01\x88\x01\x01\x12\x0f\n\x02\x65\x66\x18\x03 \x01(\rH\x02\x88\x01\x01\x12<\n\x0e\x62\x61tchingParams\x18\x04 \x01(\x0b\x32$.aerospike.vector.HnswBatchingParamsB\x04\n\x02_mB\x11\n\x0f_efConstructionB\x05\n\x03_ef\"*\n\x10HnswSearchParams\x12\x0f\n\x02\x65\x66\x18\x01 \x01(\rH\x00\x88\x01\x01\x42\x05\n\x03_ef\"\x84\x01\n\x12HnswBatchingParams\x12\x17\n\nmaxRecords\x18\x01 \x01(\rH\x00\x88\x01\x01\x12\x15\n\x08interval\x18\x02 \x01(\rH\x01\x88\x01\x01\x12\x15\n\x08\x64isabled\x18\x03 \x01(\x08H\x02\x88\x01\x01\x42\r\n\x0b_maxRecordsB\x0b\n\t_intervalB\x0b\n\t_disabled\"N\n\x0cIndexStorage\x12\x16\n\tnamespace\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x10\n\x03set\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x0c\n\n_namespaceB\x06\n\x04_set\"\xe0\x03\n\x0fIndexDefinition\x12%\n\x02id\x18\x01 \x01(\x0b\x32\x19.aerospike.vector.IndexId\x12)\n\x04type\x18\x02 \x01(\x0e\x32\x1b.aerospike.vector.IndexType\x12\x12\n\ndimensions\x18\x03 \x01(\r\x12\x44\n\x14vectorDistanceMetric\x18\x04 \x01(\x0e\x32&.aerospike.vector.VectorDistanceMetric\x12\r\n\x05\x66ield\x18\x05 \x01(\t\x12\x16\n\tsetFilter\x18\x06 \x01(\tH\x01\x88\x01\x01\x12\x32\n\nhnswParams\x18\x07 \x01(\x0b\x32\x1c.aerospike.vector.HnswParamsH\x00\x12=\n\x06labels\x18\x08 \x03(\x0b\x32-.aerospike.vector.IndexDefinition.LabelsEntry\x12\x34\n\x07storage\x18\t \x01(\x0b\x32\x1e.aerospike.vector.IndexStorageH\x02\x88\x01\x01\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x08\n\x06paramsB\x0c\n\n_setFilterB\n\n\x08_storage\"I\n\x13IndexDefinitionList\x12\x32\n\x07indices\x18\x01 \x03(\x0b\x32!.aerospike.vector.IndexDefinition\"\x18\n\x07\x42oolean\x12\r\n\x05value\x18\x01 \x01(\x08*f\n\x14VectorDistanceMetric\x12\x15\n\x11SQUARED_EUCLIDEAN\x10\x00\x12\n\n\x06\x43OSINE\x10\x01\x12\x0f\n\x0b\x44OT_PRODUCT\x10\x02\x12\r\n\tMANHATTAN\x10\x03\x12\x0b\n\x07HAMMING\x10\x04*\x15\n\tIndexType\x12\x08\n\x04HNSW\x10\x00\x42=\n\x1b\x63om.aerospike.vector.clientP\x01Z\x1c\x61\x65rospike.com/vector/protos/b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'types_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\033com.aerospike.vector.clientP\001Z\034aerospike.com/vector/protos/'
   _globals['_INDEXDEFINITION_LABELSENTRY']._options = None
   _globals['_INDEXDEFINITION_LABELSENTRY']._serialized_options = b'8\001'
-  _globals['_VECTORDISTANCEMETRIC']._serialized_start=2350
-  _globals['_VECTORDISTANCEMETRIC']._serialized_end=2452
-  _globals['_INDEXTYPE']._serialized_start=2454
-  _globals['_INDEXTYPE']._serialized_end=2475
+  _globals['_VECTORDISTANCEMETRIC']._serialized_start=2455
+  _globals['_VECTORDISTANCEMETRIC']._serialized_end=2557
+  _globals['_INDEXTYPE']._serialized_start=2559
+  _globals['_INDEXTYPE']._serialized_end=2580
   _globals['_KEY']._serialized_start=34
-  _globals['_KEY']._serialized_end=195
-  _globals['_BOOLDATA']._serialized_start=197
-  _globals['_BOOLDATA']._serialized_end=222
-  _globals['_FLOATDATA']._serialized_start=224
-  _globals['_FLOATDATA']._serialized_end=250
-  _globals['_MAPKEY']._serialized_start=253
-  _globals['_MAPKEY']._serialized_end=401
-  _globals['_MAPENTRY']._serialized_start=403
-  _globals['_MAPENTRY']._serialized_end=492
-  _globals['_MAP']._serialized_start=494
-  _globals['_MAP']._serialized_end=544
-  _globals['_LIST']._serialized_start=546
-  _globals['_LIST']._serialized_end=594
-  _globals['_VECTOR']._serialized_start=596
-  _globals['_VECTOR']._serialized_end=710
-  _globals['_VALUE']._serialized_start=713
-  _globals['_VALUE']._serialized_end=997
-  _globals['_BIN']._serialized_start=999
-  _globals['_BIN']._serialized_end=1058
-  _globals['_RECORD']._serialized_start=1060
-  _globals['_RECORD']._serialized_end=1145
-  _globals['_NEIGHBOR']._serialized_start=1147
-  _globals['_NEIGHBOR']._serialized_end=1269
-  _globals['_INDEXID']._serialized_start=1271
-  _globals['_INDEXID']._serialized_end=1313
-  _globals['_HNSWPARAMS']._serialized_start=1316
-  _globals['_HNSWPARAMS']._serialized_end=1484
-  _globals['_HNSWSEARCHPARAMS']._serialized_start=1486
-  _globals['_HNSWSEARCHPARAMS']._serialized_end=1528
-  _globals['_HNSWBATCHINGPARAMS']._serialized_start=1531
-  _globals['_HNSWBATCHINGPARAMS']._serialized_end=1663
-  _globals['_AEROSPIKEINDEXSTORAGE']._serialized_start=1665
-  _globals['_AEROSPIKEINDEXSTORAGE']._serialized_end=1752
-  _globals['_INDEXDEFINITION']._serialized_start=1755
-  _globals['_INDEXDEFINITION']._serialized_end=2247
-  _globals['_INDEXDEFINITION_LABELSENTRY']._serialized_start=2167
-  _globals['_INDEXDEFINITION_LABELSENTRY']._serialized_end=2212
-  _globals['_INDEXDEFINITIONLIST']._serialized_start=2249
-  _globals['_INDEXDEFINITIONLIST']._serialized_end=2322
-  _globals['_BOOLEAN']._serialized_start=2324
-  _globals['_BOOLEAN']._serialized_end=2348
+  _globals['_KEY']._serialized_end=179
+  _globals['_BOOLDATA']._serialized_start=181
+  _globals['_BOOLDATA']._serialized_end=206
+  _globals['_FLOATDATA']._serialized_start=208
+  _globals['_FLOATDATA']._serialized_end=234
+  _globals['_MAPKEY']._serialized_start=237
+  _globals['_MAPKEY']._serialized_end=385
+  _globals['_MAPENTRY']._serialized_start=387
+  _globals['_MAPENTRY']._serialized_end=476
+  _globals['_MAP']._serialized_start=478
+  _globals['_MAP']._serialized_end=528
+  _globals['_LIST']._serialized_start=530
+  _globals['_LIST']._serialized_end=578
+  _globals['_VECTOR']._serialized_start=580
+  _globals['_VECTOR']._serialized_end=694
+  _globals['_VALUE']._serialized_start=697
+  _globals['_VALUE']._serialized_end=1005
+  _globals['_FIELD']._serialized_start=1007
+  _globals['_FIELD']._serialized_end=1068
+  _globals['_AEROSPIKERECORDMETADATA']._serialized_start=1070
+  _globals['_AEROSPIKERECORDMETADATA']._serialized_end=1135
+  _globals['_RECORD']._serialized_start=1138
+  _globals['_RECORD']._serialized_end=1271
+  _globals['_NEIGHBOR']._serialized_start=1273
+  _globals['_NEIGHBOR']._serialized_end=1395
+  _globals['_INDEXID']._serialized_start=1397
+  _globals['_INDEXID']._serialized_end=1439
+  _globals['_HNSWPARAMS']._serialized_start=1442
+  _globals['_HNSWPARAMS']._serialized_end=1610
+  _globals['_HNSWSEARCHPARAMS']._serialized_start=1612
+  _globals['_HNSWSEARCHPARAMS']._serialized_end=1654
+  _globals['_HNSWBATCHINGPARAMS']._serialized_start=1657
+  _globals['_HNSWBATCHINGPARAMS']._serialized_end=1789
+  _globals['_INDEXSTORAGE']._serialized_start=1791
+  _globals['_INDEXSTORAGE']._serialized_end=1869
+  _globals['_INDEXDEFINITION']._serialized_start=1872
+  _globals['_INDEXDEFINITION']._serialized_end=2352
+  _globals['_INDEXDEFINITION_LABELSENTRY']._serialized_start=2271
+  _globals['_INDEXDEFINITION_LABELSENTRY']._serialized_end=2316
+  _globals['_INDEXDEFINITIONLIST']._serialized_start=2354
+  _globals['_INDEXDEFINITIONLIST']._serialized_end=2427
+  _globals['_BOOLEAN']._serialized_start=2429
+  _globals['_BOOLEAN']._serialized_end=2453
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2_grpc.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/shared/proto_generated/vector_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search/types.py` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,119 +16,116 @@
     """
 
     def __init__(self, *, host: str, port: int, is_tls: Optional[bool] = False) -> None:
         self.host = host
         self.port = port
         self.is_tls = is_tls
 
+
 class Key(object):
     """
     Represents a record key.
     Used in RecordWithKey.
 
     Args:
         namespace (str): The namespace for the key.
         set (str): The set for the key.
-        digest (bytearray): The digest of the key.
         key (Any): The key itself.
     """
 
-    def __init__(
-        self, *, namespace: str, set: str, digest: bytearray, key: Any
-    ) -> None:
+    def __init__(self, *, namespace: str, set: str, key: Any) -> None:
         self.namespace = namespace
         self.set = set
-        self.digest = digest
         self.key = key
 
     def __str__(self):
         """
         Returns a string representation of the key.
         """
-        return f"Key: namespace='{self.namespace}', set='{self.set}', digest={self.digest}, key={self.key}"
+        return f"Key: namespace='{self.namespace}', set='{self.set}', key={self.key}"
 
 
 class RecordWithKey(object):
     """
-    Represents a record, including a key and bins.
+    Represents a record, including a key and fields.
     Return value for VectorDbClient.get.
 
     Args:
         key (Key): The key of the record.
-        bins (dict[str, Any]): The bins associated with the record.
+        fields (dict[str, Any]): The fields associated with the record.
     """
 
-    def __init__(self, *, key: Key, bins: dict[str, Any]) -> None:
+    def __init__(self, *, key: Key, fields: dict[str, Any]) -> None:
         self.key = key
-        self.bins = bins
+        self.fields = fields
 
     def __str__(self):
         """
-        Returns a string representation of the record, including a key and bins.
+        Returns a string representation of the record, including a key and fields.
         """
-        bins_info = ""
-        for key, value in self.bins.items():
+        fields_info = ""
+        for key, value in self.fields.items():
             if isinstance(value, list):
                 if len(value) > 4:
                     value_str = (
                         "[\n"
                         + ",\n".join("\t\t\t{}".format(val) for val in value[:3])
                         + ",\n\t\t\t...\n\t\t]"
                     )
                 else:
                     value_str = str(value)
             else:
                 value_str = str(value)
-            bins_info += "\n\t\t{}: {}".format(key, value_str)
-        return "{{\n\t{},\n\tbins: {{\n{}\n\t}}\n}}".format(self.key, bins_info)
+            fields_info += "\n\t\t{}: {}".format(key, value_str)
+        return "{{\n\t{},\n\tfields: {{\n{}\n\t}}\n}}".format(self.key, fields_info)
 
 
 class Neighbor(object):
     """
     Represents a neighboring record in the context of approximate nearest neighbor search.
 
-    This class represents a neighboring record in relation to a query record. It includes information such as the key, bins, and distance from the query record.
+    This class represents a neighboring record in relation to a query record. It includes information such as the key, fields, and distance from the query record.
 
     Args:
         key (Key): The Key instance identifying the neighboring record.
-        bins (dict[str, Any]): A dictionary representing bins associated with the neighboring record.
+        fields (dict[str, Any]): A dictionary representing fields associated with the neighboring record.
         distance (float): The distance between the neighboring record and the query record, calculated based on the chosen VectorDistanceMetric.
 
     Notes:
         - The distance metric used to calculate the distance between records is determined by the chosen VectorDistanceMetric.
         - The neighbor's distance indicates how similar or dissimilar it is to the query record based on the chosen distance metric.
         - A smaller distance typically implies greater similarity between records.
 
     """
 
-    def __init__(self, *, key: Key, bins: dict[str, Any], distance: float) -> None:
+    def __init__(self, *, key: Key, fields: dict[str, Any], distance: float) -> None:
         self.key = key
-        self.bins = bins
+        self.fields = fields
         self.distance = distance
 
     def __str__(self):
         """
         Returns a string representation of the neighboring record.
         """
-        bins_info = ""
-        for key, value in self.bins.items():
+        fields_info = ""
+        for key, value in self.fields.items():
             if isinstance(value, list):
                 if len(value) > 4:
                     value_str = (
                         "[\n"
                         + ",\n".join("\t\t\t{}".format(val) for val in value[:3])
                         + ",\n\t\t\t...\n\t\t]"
                     )
                 else:
                     value_str = str(value)
             else:
                 value_str = str(value)
-            bins_info += "\n\t\t{}: {}".format(key, value_str)
-        return "{{\n\t{},\n\tdistance: {},\n\tbins: {{\n{}\n\t}}\n}}".format(
-            self.key, self.distance, bins_info
+            fields_info += "\n\t\t{}: {}".format(key, value_str)
+        return "{{\n\t{},\n\tdistance: {},\n\tfields: {{\n{}\n\t}}\n}}".format(
+            self.key, self.distance, fields_info
         )
 
 
 class VectorDistanceMetric(enum.Enum):
     """
     Enumeration of vector distance metrics.
     """
@@ -224,7 +221,33 @@
         """
         self.ef = ef
 
     def _to_pb2(self):
         params = types_pb2.HnswSearchParams()
         params.ef = self.ef
         return params
+
+
+class AVSError(Exception):
+    """
+    Custom exception raised for errors related to AVS.
+    """
+
+    pass
+
+
+class AVSServerError(AVSError):
+    """
+    Custom exception raised for errors related to the AVS server.
+
+    Attributes:
+        status (int): The status code associated with the error.
+        details (str): Details about the error.
+        debug_error_string (str): Debug error string providing additional error information.
+
+    Args:
+        rpc_error (Exception): The original gRPC error object from which AVSError is derived.
+            This error object is used to extract status, details, and debug information.
+    """
+
+    def __init__(self, *, rpc_error) -> None:
+        self.rpc_error = rpc_error
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/PKG-INFO` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerospike-vector-search
-Version: 0.5.1
+Version: 0.6.0
 Summary: Aerospike Proximus Client Library for Python
 Author-email: "Aerospike, Inc." <info@aerospike.com>
 License: Apache Software License
 Project-URL: Homepage, https://aerospike.com
 Keywords: aerospike,vector,database,ANN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `aerospike-vector-search-0.5.1/src/aerospike_vector_search.egg-info/SOURCES.txt` & `aerospike-vector-search-0.6.0/src/aerospike_vector_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

