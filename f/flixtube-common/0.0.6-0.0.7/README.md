# Comparing `tmp/flixtube_common-0.0.6.tar.gz` & `tmp/flixtube_common-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flixtube_common-0.0.6.tar", last modified: Wed May 15 15:30:50 2024, max compression
+gzip compressed data, was "flixtube_common-0.0.7.tar", last modified: Wed May 15 15:36:26 2024, max compression
```

## Comparing `flixtube_common-0.0.6.tar` & `flixtube_common-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:30:50.476457 flixtube_common-0.0.6/
--rw-r--r--   0 adamscarlat   (501) staff       (20)      202 2024-05-15 15:30:50.476151 flixtube_common-0.0.6/PKG-INFO
--rw-r--r--   0 adamscarlat   (501) staff       (20)       38 2024-05-15 15:30:50.476509 flixtube_common-0.0.6/setup.cfg
--rw-r--r--   0 adamscarlat   (501) staff       (20)      335 2024-05-15 15:30:43.000000 flixtube_common-0.0.6/setup.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:30:50.473693 flixtube_common-0.0.6/src/
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:30:50.474032 flixtube_common-0.0.6/src/flixtube_common/
--rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:05:47.000000 flixtube_common-0.0.6/src/flixtube_common/__init__.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:30:50.475088 flixtube_common-0.0.6/src/flixtube_common/cosmosdb/
--rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:31:58.000000 flixtube_common-0.0.6/src/flixtube_common/cosmosdb/__init__.py
--rw-r--r--   0 adamscarlat   (501) staff       (20)     1006 2024-05-15 14:41:05.000000 flixtube_common-0.0.6/src/flixtube_common/cosmosdb/db_operations.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:30:50.475536 flixtube_common-0.0.6/src/flixtube_common/rabbitmq/
--rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:27:51.000000 flixtube_common-0.0.6/src/flixtube_common/rabbitmq/__init__.py
--rw-r--r--   0 adamscarlat   (501) staff       (20)     2524 2024-05-15 15:30:25.000000 flixtube_common-0.0.6/src/flixtube_common/rabbitmq/pika_client.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:30:50.475898 flixtube_common-0.0.6/src/flixtube_common.egg-info/
--rw-r--r--   0 adamscarlat   (501) staff       (20)      202 2024-05-15 15:30:50.000000 flixtube_common-0.0.6/src/flixtube_common.egg-info/PKG-INFO
--rw-r--r--   0 adamscarlat   (501) staff       (20)      426 2024-05-15 15:30:50.000000 flixtube_common-0.0.6/src/flixtube_common.egg-info/SOURCES.txt
--rw-r--r--   0 adamscarlat   (501) staff       (20)        1 2024-05-15 15:30:50.000000 flixtube_common-0.0.6/src/flixtube_common.egg-info/dependency_links.txt
--rw-r--r--   0 adamscarlat   (501) staff       (20)       29 2024-05-15 15:30:50.000000 flixtube_common-0.0.6/src/flixtube_common.egg-info/requires.txt
--rw-r--r--   0 adamscarlat   (501) staff       (20)       16 2024-05-15 15:30:50.000000 flixtube_common-0.0.6/src/flixtube_common.egg-info/top_level.txt
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:36:26.644916 flixtube_common-0.0.7/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      202 2024-05-15 15:36:26.644710 flixtube_common-0.0.7/PKG-INFO
+-rw-r--r--   0 adamscarlat   (501) staff       (20)       38 2024-05-15 15:36:26.644951 flixtube_common-0.0.7/setup.cfg
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      335 2024-05-15 15:36:16.000000 flixtube_common-0.0.7/setup.py
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:36:26.642379 flixtube_common-0.0.7/src/
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:36:26.642727 flixtube_common-0.0.7/src/flixtube_common/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:05:47.000000 flixtube_common-0.0.7/src/flixtube_common/__init__.py
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:36:26.643629 flixtube_common-0.0.7/src/flixtube_common/cosmosdb/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:31:58.000000 flixtube_common-0.0.7/src/flixtube_common/cosmosdb/__init__.py
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      967 2024-05-15 15:35:53.000000 flixtube_common-0.0.7/src/flixtube_common/cosmosdb/db_operations.py
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:36:26.644124 flixtube_common-0.0.7/src/flixtube_common/rabbitmq/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:27:51.000000 flixtube_common-0.0.7/src/flixtube_common/rabbitmq/__init__.py
+-rw-r--r--   0 adamscarlat   (501) staff       (20)     2524 2024-05-15 15:30:25.000000 flixtube_common-0.0.7/src/flixtube_common/rabbitmq/pika_client.py
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:36:26.644487 flixtube_common-0.0.7/src/flixtube_common.egg-info/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      202 2024-05-15 15:36:26.000000 flixtube_common-0.0.7/src/flixtube_common.egg-info/PKG-INFO
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      426 2024-05-15 15:36:26.000000 flixtube_common-0.0.7/src/flixtube_common.egg-info/SOURCES.txt
+-rw-r--r--   0 adamscarlat   (501) staff       (20)        1 2024-05-15 15:36:26.000000 flixtube_common-0.0.7/src/flixtube_common.egg-info/dependency_links.txt
+-rw-r--r--   0 adamscarlat   (501) staff       (20)       29 2024-05-15 15:36:26.000000 flixtube_common-0.0.7/src/flixtube_common.egg-info/requires.txt
+-rw-r--r--   0 adamscarlat   (501) staff       (20)       16 2024-05-15 15:36:26.000000 flixtube_common-0.0.7/src/flixtube_common.egg-info/top_level.txt
```

### Comparing `flixtube_common-0.0.6/src/flixtube_common/cosmosdb/db_operations.py` & `flixtube_common-0.0.7/src/flixtube_common/cosmosdb/db_operations.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,15 +7,15 @@
           password: str     
         ) -> None:
     self.uri = uri
     self.username = username
     self.password = password
 
 
-  async def get_database_client(self, db_name: str) -> AsyncIOMotorDatabase: # type: ignore
+  async def get_database_client(self, db_name: str):
     mongo_uri = f"mongodb://{self.username}:{self.password}@{self.uri}"
     client = AsyncIOMotorClient(mongo_uri)
     database = client[db_name]
     
     yield database
     
     client.close()
```

### Comparing `flixtube_common-0.0.6/src/flixtube_common/rabbitmq/pika_client.py` & `flixtube_common-0.0.7/src/flixtube_common/rabbitmq/pika_client.py`

 * *Files identical despite different names*

