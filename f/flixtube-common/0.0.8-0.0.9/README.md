# Comparing `tmp/flixtube_common-0.0.8.tar.gz` & `tmp/flixtube_common-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flixtube_common-0.0.8.tar", last modified: Wed May 15 15:42:19 2024, max compression
+gzip compressed data, was "flixtube_common-0.0.9.tar", last modified: Wed May 15 16:10:45 2024, max compression
```

## Comparing `flixtube_common-0.0.8.tar` & `flixtube_common-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:42:19.949064 flixtube_common-0.0.8/
--rw-r--r--   0 adamscarlat   (501) staff       (20)      202 2024-05-15 15:42:19.948677 flixtube_common-0.0.8/PKG-INFO
--rw-r--r--   0 adamscarlat   (501) staff       (20)       38 2024-05-15 15:42:19.949118 flixtube_common-0.0.8/setup.cfg
--rw-r--r--   0 adamscarlat   (501) staff       (20)      335 2024-05-15 15:42:11.000000 flixtube_common-0.0.8/setup.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:42:19.946115 flixtube_common-0.0.8/src/
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:42:19.946479 flixtube_common-0.0.8/src/flixtube_common/
--rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:05:47.000000 flixtube_common-0.0.8/src/flixtube_common/__init__.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:42:19.947371 flixtube_common-0.0.8/src/flixtube_common/cosmosdb/
--rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:31:58.000000 flixtube_common-0.0.8/src/flixtube_common/cosmosdb/__init__.py
--rw-r--r--   0 adamscarlat   (501) staff       (20)     1008 2024-05-15 15:41:59.000000 flixtube_common-0.0.8/src/flixtube_common/cosmosdb/db_operations.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:42:19.947926 flixtube_common-0.0.8/src/flixtube_common/rabbitmq/
--rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:27:51.000000 flixtube_common-0.0.8/src/flixtube_common/rabbitmq/__init__.py
--rw-r--r--   0 adamscarlat   (501) staff       (20)     2524 2024-05-15 15:30:25.000000 flixtube_common-0.0.8/src/flixtube_common/rabbitmq/pika_client.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:42:19.948317 flixtube_common-0.0.8/src/flixtube_common.egg-info/
--rw-r--r--   0 adamscarlat   (501) staff       (20)      202 2024-05-15 15:42:19.000000 flixtube_common-0.0.8/src/flixtube_common.egg-info/PKG-INFO
--rw-r--r--   0 adamscarlat   (501) staff       (20)      426 2024-05-15 15:42:19.000000 flixtube_common-0.0.8/src/flixtube_common.egg-info/SOURCES.txt
--rw-r--r--   0 adamscarlat   (501) staff       (20)        1 2024-05-15 15:42:19.000000 flixtube_common-0.0.8/src/flixtube_common.egg-info/dependency_links.txt
--rw-r--r--   0 adamscarlat   (501) staff       (20)       29 2024-05-15 15:42:19.000000 flixtube_common-0.0.8/src/flixtube_common.egg-info/requires.txt
--rw-r--r--   0 adamscarlat   (501) staff       (20)       16 2024-05-15 15:42:19.000000 flixtube_common-0.0.8/src/flixtube_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:45.254694 flixtube_common-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-15 16:10:45.254694 flixtube_common-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:10:45.254694 flixtube_common-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-15 16:10:35.000000 flixtube_common-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:45.250694 flixtube_common-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:45.250694 flixtube_common-0.0.9/src/flixtube_common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:35.000000 flixtube_common-0.0.9/src/flixtube_common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:45.254694 flixtube_common-0.0.9/src/flixtube_common/cosmosdb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:35.000000 flixtube_common-0.0.9/src/flixtube_common/cosmosdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-15 16:10:35.000000 flixtube_common-0.0.9/src/flixtube_common/cosmosdb/db_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:45.254694 flixtube_common-0.0.9/src/flixtube_common/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:35.000000 flixtube_common-0.0.9/src/flixtube_common/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-15 16:10:35.000000 flixtube_common-0.0.9/src/flixtube_common/rabbitmq/pika_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:45.254694 flixtube_common-0.0.9/src/flixtube_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-15 16:10:45.000000 flixtube_common-0.0.9/src/flixtube_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 16:10:45.000000 flixtube_common-0.0.9/src/flixtube_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:10:45.000000 flixtube_common-0.0.9/src/flixtube_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 16:10:45.000000 flixtube_common-0.0.9/src/flixtube_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 16:10:45.000000 flixtube_common-0.0.9/src/flixtube_common.egg-info/top_level.txt
```

### Comparing `flixtube_common-0.0.8/src/flixtube_common/cosmosdb/db_operations.py` & `flixtube_common-0.0.9/src/flixtube_common/cosmosdb/db_operations.py`

 * *Files identical despite different names*

### Comparing `flixtube_common-0.0.8/src/flixtube_common/rabbitmq/pika_client.py` & `flixtube_common-0.0.9/src/flixtube_common/rabbitmq/pika_client.py`

 * *Files identical despite different names*

