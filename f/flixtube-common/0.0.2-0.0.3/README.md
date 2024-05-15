# Comparing `tmp/flixtube_common-0.0.2.tar.gz` & `tmp/flixtube_common-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flixtube_common-0.0.2.tar", last modified: Wed May 15 14:35:12 2024, max compression
+gzip compressed data, was "flixtube_common-0.0.3.tar", last modified: Wed May 15 14:41:29 2024, max compression
```

## Comparing `flixtube_common-0.0.2.tar` & `flixtube_common-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:35:12.555598 flixtube_common-0.0.2/
--rw-r--r--   0 adamscarlat   (501) staff       (20)      171 2024-05-15 14:35:12.555342 flixtube_common-0.0.2/PKG-INFO
--rw-r--r--   0 adamscarlat   (501) staff       (20)       38 2024-05-15 14:35:12.555637 flixtube_common-0.0.2/setup.cfg
--rw-r--r--   0 adamscarlat   (501) staff       (20)      312 2024-05-15 14:35:03.000000 flixtube_common-0.0.2/setup.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:35:12.553522 flixtube_common-0.0.2/src/
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:35:12.553877 flixtube_common-0.0.2/src/flixtube_common/
--rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:05:47.000000 flixtube_common-0.0.2/src/flixtube_common/__init__.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:35:12.554709 flixtube_common-0.0.2/src/flixtube_common/cosmosdb/
--rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:31:58.000000 flixtube_common-0.0.2/src/flixtube_common/cosmosdb/__init__.py
--rw-r--r--   0 adamscarlat   (501) staff       (20)     1064 2024-05-15 13:19:14.000000 flixtube_common-0.0.2/src/flixtube_common/cosmosdb/db_operations.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:35:12.555107 flixtube_common-0.0.2/src/flixtube_common.egg-info/
--rw-r--r--   0 adamscarlat   (501) staff       (20)      171 2024-05-15 14:35:12.000000 flixtube_common-0.0.2/src/flixtube_common.egg-info/PKG-INFO
--rw-r--r--   0 adamscarlat   (501) staff       (20)      341 2024-05-15 14:35:12.000000 flixtube_common-0.0.2/src/flixtube_common.egg-info/SOURCES.txt
--rw-r--r--   0 adamscarlat   (501) staff       (20)        1 2024-05-15 14:35:12.000000 flixtube_common-0.0.2/src/flixtube_common.egg-info/dependency_links.txt
--rw-r--r--   0 adamscarlat   (501) staff       (20)       13 2024-05-15 14:35:12.000000 flixtube_common-0.0.2/src/flixtube_common.egg-info/requires.txt
--rw-r--r--   0 adamscarlat   (501) staff       (20)       16 2024-05-15 14:35:12.000000 flixtube_common-0.0.2/src/flixtube_common.egg-info/top_level.txt
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:41:29.173074 flixtube_common-0.0.3/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      171 2024-05-15 14:41:29.172813 flixtube_common-0.0.3/PKG-INFO
+-rw-r--r--   0 adamscarlat   (501) staff       (20)       38 2024-05-15 14:41:29.173117 flixtube_common-0.0.3/setup.cfg
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      312 2024-05-15 14:41:24.000000 flixtube_common-0.0.3/setup.py
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:41:29.171022 flixtube_common-0.0.3/src/
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:41:29.171347 flixtube_common-0.0.3/src/flixtube_common/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:05:47.000000 flixtube_common-0.0.3/src/flixtube_common/__init__.py
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:41:29.172177 flixtube_common-0.0.3/src/flixtube_common/cosmosdb/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:31:58.000000 flixtube_common-0.0.3/src/flixtube_common/cosmosdb/__init__.py
+-rw-r--r--   0 adamscarlat   (501) staff       (20)     1006 2024-05-15 14:41:05.000000 flixtube_common-0.0.3/src/flixtube_common/cosmosdb/db_operations.py
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:41:29.172578 flixtube_common-0.0.3/src/flixtube_common.egg-info/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      171 2024-05-15 14:41:29.000000 flixtube_common-0.0.3/src/flixtube_common.egg-info/PKG-INFO
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      341 2024-05-15 14:41:29.000000 flixtube_common-0.0.3/src/flixtube_common.egg-info/SOURCES.txt
+-rw-r--r--   0 adamscarlat   (501) staff       (20)        1 2024-05-15 14:41:29.000000 flixtube_common-0.0.3/src/flixtube_common.egg-info/dependency_links.txt
+-rw-r--r--   0 adamscarlat   (501) staff       (20)       13 2024-05-15 14:41:29.000000 flixtube_common-0.0.3/src/flixtube_common.egg-info/requires.txt
+-rw-r--r--   0 adamscarlat   (501) staff       (20)       16 2024-05-15 14:41:29.000000 flixtube_common-0.0.3/src/flixtube_common.egg-info/top_level.txt
```

### Comparing `flixtube_common-0.0.2/src/flixtube_common/cosmosdb/db_operations.py` & `flixtube_common-0.0.3/src/flixtube_common/cosmosdb/db_operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from motor.motor_asyncio import AsyncIOMotorDatabase, AsyncIOMotorCollection, AsyncIOMotorClient
 
 class CosmosDbOperations:
   def __init__(self, 
-          host: str,
-          port: str,
+          uri: str,
           username: str,
           password: str     
         ) -> None:
-    self.host = host
-    self.port = port
+    self.uri = uri
     self.username = username
     self.password = password
 
 
   async def get_database_client(self, db_name: str) -> AsyncIOMotorDatabase: # type: ignore
-    mongo_uri = f"mongodb://{self.username}:{self.password}@{self.host}:{self.port}"
+    mongo_uri = f"mongodb://{self.username}:{self.password}@{self.uri}"
     client = AsyncIOMotorClient(mongo_uri)
     database = client[db_name]
     
     yield database
     
     client.close()
```

