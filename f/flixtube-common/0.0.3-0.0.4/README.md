# Comparing `tmp/flixtube_common-0.0.3.tar.gz` & `tmp/flixtube_common-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flixtube_common-0.0.3.tar", last modified: Wed May 15 14:41:29 2024, max compression
+gzip compressed data, was "flixtube_common-0.0.4.tar", last modified: Wed May 15 15:25:28 2024, max compression
```

## Comparing `flixtube_common-0.0.3.tar` & `flixtube_common-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:41:29.173074 flixtube_common-0.0.3/
--rw-r--r--   0 adamscarlat   (501) staff       (20)      171 2024-05-15 14:41:29.172813 flixtube_common-0.0.3/PKG-INFO
--rw-r--r--   0 adamscarlat   (501) staff       (20)       38 2024-05-15 14:41:29.173117 flixtube_common-0.0.3/setup.cfg
--rw-r--r--   0 adamscarlat   (501) staff       (20)      312 2024-05-15 14:41:24.000000 flixtube_common-0.0.3/setup.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:41:29.171022 flixtube_common-0.0.3/src/
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:41:29.171347 flixtube_common-0.0.3/src/flixtube_common/
--rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:05:47.000000 flixtube_common-0.0.3/src/flixtube_common/__init__.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:41:29.172177 flixtube_common-0.0.3/src/flixtube_common/cosmosdb/
--rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:31:58.000000 flixtube_common-0.0.3/src/flixtube_common/cosmosdb/__init__.py
--rw-r--r--   0 adamscarlat   (501) staff       (20)     1006 2024-05-15 14:41:05.000000 flixtube_common-0.0.3/src/flixtube_common/cosmosdb/db_operations.py
-drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:41:29.172578 flixtube_common-0.0.3/src/flixtube_common.egg-info/
--rw-r--r--   0 adamscarlat   (501) staff       (20)      171 2024-05-15 14:41:29.000000 flixtube_common-0.0.3/src/flixtube_common.egg-info/PKG-INFO
--rw-r--r--   0 adamscarlat   (501) staff       (20)      341 2024-05-15 14:41:29.000000 flixtube_common-0.0.3/src/flixtube_common.egg-info/SOURCES.txt
--rw-r--r--   0 adamscarlat   (501) staff       (20)        1 2024-05-15 14:41:29.000000 flixtube_common-0.0.3/src/flixtube_common.egg-info/dependency_links.txt
--rw-r--r--   0 adamscarlat   (501) staff       (20)       13 2024-05-15 14:41:29.000000 flixtube_common-0.0.3/src/flixtube_common.egg-info/requires.txt
--rw-r--r--   0 adamscarlat   (501) staff       (20)       16 2024-05-15 14:41:29.000000 flixtube_common-0.0.3/src/flixtube_common.egg-info/top_level.txt
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:25:28.436926 flixtube_common-0.0.4/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      202 2024-05-15 15:25:28.436683 flixtube_common-0.0.4/PKG-INFO
+-rw-r--r--   0 adamscarlat   (501) staff       (20)       38 2024-05-15 15:25:28.436970 flixtube_common-0.0.4/setup.cfg
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      335 2024-05-15 15:25:09.000000 flixtube_common-0.0.4/setup.py
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:25:28.434991 flixtube_common-0.0.4/src/
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:25:28.435271 flixtube_common-0.0.4/src/flixtube_common/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:05:47.000000 flixtube_common-0.0.4/src/flixtube_common/__init__.py
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:25:28.436029 flixtube_common-0.0.4/src/flixtube_common/cosmosdb/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)        0 2024-05-15 14:31:58.000000 flixtube_common-0.0.4/src/flixtube_common/cosmosdb/__init__.py
+-rw-r--r--   0 adamscarlat   (501) staff       (20)     1006 2024-05-15 14:41:05.000000 flixtube_common-0.0.4/src/flixtube_common/cosmosdb/db_operations.py
+drwxr-xr-x   0 adamscarlat   (501) staff       (20)        0 2024-05-15 15:25:28.436421 flixtube_common-0.0.4/src/flixtube_common.egg-info/
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      202 2024-05-15 15:25:28.000000 flixtube_common-0.0.4/src/flixtube_common.egg-info/PKG-INFO
+-rw-r--r--   0 adamscarlat   (501) staff       (20)      341 2024-05-15 15:25:28.000000 flixtube_common-0.0.4/src/flixtube_common.egg-info/SOURCES.txt
+-rw-r--r--   0 adamscarlat   (501) staff       (20)        1 2024-05-15 15:25:28.000000 flixtube_common-0.0.4/src/flixtube_common.egg-info/dependency_links.txt
+-rw-r--r--   0 adamscarlat   (501) staff       (20)       29 2024-05-15 15:25:28.000000 flixtube_common-0.0.4/src/flixtube_common.egg-info/requires.txt
+-rw-r--r--   0 adamscarlat   (501) staff       (20)       16 2024-05-15 15:25:28.000000 flixtube_common-0.0.4/src/flixtube_common.egg-info/top_level.txt
```

### Comparing `flixtube_common-0.0.3/src/flixtube_common/cosmosdb/db_operations.py` & `flixtube_common-0.0.4/src/flixtube_common/cosmosdb/db_operations.py`

 * *Files identical despite different names*

