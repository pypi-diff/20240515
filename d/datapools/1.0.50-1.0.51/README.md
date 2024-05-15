# Comparing `tmp/datapools-1.0.50.tar.gz` & `tmp/datapools-1.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.50.tar", last modified: Wed May 15 15:00:45 2024, max compression
+gzip compressed data, was "datapools-1.0.51.tar", last modified: Wed May 15 15:13:35 2024, max compression
```

## Comparing `datapools-1.0.50.tar` & `datapools-1.0.51.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.214233 datapools-1.0.50/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 15:00:35.000000 datapools-1.0.50/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    17986 2024-05-15 15:00:35.000000 datapools-1.0.50/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-15 15:00:35.000000 datapools-1.0.50/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 15:00:35.000000 datapools-1.0.50/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-15 15:00:45.214233 datapools-1.0.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 15:00:35.000000 datapools-1.0.50/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.202232 datapools-1.0.50/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.202232 datapools-1.0.50/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.202232 datapools-1.0.50/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/plugins/freesound_org/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/freesound_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/freesound_org/freesound_org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-15 15:00:45.000000 datapools-1.0.50/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-15 15:00:45.000000 datapools-1.0.50/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:00:45.000000 datapools-1.0.50/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 15:00:45.000000 datapools-1.0.50/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-15 15:00:45.000000 datapools-1.0.50/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 15:00:45.000000 datapools-1.0.50/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:00:45.214233 datapools-1.0.50/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-15 15:00:35.000000 datapools-1.0.50/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:35.000000 datapools-1.0.50/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 15:00:35.000000 datapools-1.0.50/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-15 15:00:35.000000 datapools-1.0.50/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.639833 datapools-1.0.51/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 15:13:27.000000 datapools-1.0.51/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    18109 2024-05-15 15:13:27.000000 datapools-1.0.51/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-15 15:13:27.000000 datapools-1.0.51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 15:13:27.000000 datapools-1.0.51/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-15 15:13:35.639833 datapools-1.0.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 15:13:27.000000 datapools-1.0.51/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.627833 datapools-1.0.51/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.627833 datapools-1.0.51/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.627833 datapools-1.0.51/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.627833 datapools-1.0.51/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.627833 datapools-1.0.51/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.631832 datapools-1.0.51/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.631832 datapools-1.0.51/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.631832 datapools-1.0.51/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.631832 datapools-1.0.51/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.631832 datapools-1.0.51/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.631832 datapools-1.0.51/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.631832 datapools-1.0.51/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.631832 datapools-1.0.51/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.631832 datapools-1.0.51/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.631832 datapools-1.0.51/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.631832 datapools-1.0.51/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.635833 datapools-1.0.51/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.635833 datapools-1.0.51/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.635833 datapools-1.0.51/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.635833 datapools-1.0.51/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16563 2024-05-15 15:13:27.000000 datapools-1.0.51/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.635833 datapools-1.0.51/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-15 15:13:35.000000 datapools-1.0.51/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-15 15:13:35.000000 datapools-1.0.51/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:13:35.000000 datapools-1.0.51/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 15:13:35.000000 datapools-1.0.51/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-15 15:13:35.000000 datapools-1.0.51/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 15:13:35.000000 datapools-1.0.51/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:13:35.639833 datapools-1.0.51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-15 15:13:27.000000 datapools-1.0.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:35.635833 datapools-1.0.51/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:13:27.000000 datapools-1.0.51/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 15:13:27.000000 datapools-1.0.51/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-15 15:13:27.000000 datapools-1.0.51/tests/test_base.py
```

### Comparing `datapools-1.0.50/HISTORY.md` & `datapools-1.0.51/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Linter. [sergpsu]
+- Linter. [sergpsu]
+
+
+1.0.50 (2024-05-15)
+-------------------
+- Release: version 1.0.50 🚀 [sergpsu]
 - Publish session stats update as redis pubsub. [sergpsu]
 - Merge remote-tracking branch 'origin/master' into sergpsu-fixes.
   [sergpsu]
 - Merge pull request #67 from torrentsai/sergpsu-fixes. [S]
 
   Producer task rejection bugfix
```

### Comparing `datapools-1.0.50/LICENSE` & `datapools-1.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/PKG-INFO` & `datapools-1.0.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.50
+Version: 1.0.51
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.50/README.md` & `datapools-1.0.51/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/api.py` & `datapools-1.0.51/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/cli.py` & `datapools-1.0.51/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/common/backend_api.py` & `datapools-1.0.51/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/common/queues/__init__.py` & `datapools-1.0.51/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/common/queues/rabbitmq.py` & `datapools-1.0.51/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/common/queues/types.py` & `datapools-1.0.51/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/common/session_manager.py` & `datapools-1.0.51/datapools/common/session_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,16 +144,15 @@
 
     def has(self, session_id) -> bool:
         res = self.r.exists(SessionManager.get_meta_key(session_id))
         # logger.info( f'sessionmanager.has {res=} {type(res)=}')
         return res
 
     def get(self, session_id) -> Optional[Session]:
-        if self.has(session_id):
-            return Session(session_id, self.r)
+        return Session(session_id, self.r) if self.has(session_id) else None
 
     def remove(self, session_id):
         self.r.delete(SessionManager.get_meta_key(session_id))
         self.r.delete(SessionManager.get_urls_key(session_id))
         self.r.delete(SessionManager.get_content_key(session_id))
 
     def gen_session_id(self) -> str:
```

### Comparing `datapools-1.0.50/datapools/common/stoppable.py` & `datapools-1.0.51/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/common/storage/base_storage.py` & `datapools-1.0.51/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/common/storage/file_storage.py` & `datapools-1.0.51/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.51/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.51/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/common/types.py` & `datapools-1.0.51/datapools/common/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/producer/base_producer.py` & `datapools-1.0.51/datapools/producer/base_producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,16 +131,16 @@
             logger.error(f"Catched: {traceback.format_exc()}")
             logger.error(f"!!!!!!! Exception in Datapools::router_loop() {e}")
 
     async def process_content(self, session: Session, raw_data, task):
         # path = os.path.join(self.cfg.STORAGE_PATH, str(datapool_id))
         if not self.is_shared_storage():
             path = self.cfg.STORAGE_PATH
-            if not os.path.exists(path):
-                os.mkdir(path)
+            if not os.path.exists(path):  # type: ignore
+                os.mkdir(path)  # type: ignore
             storage = FileStorage(path)
             # put data into persistent storage
             await storage.put(task["storage_id"], raw_data)
 
         if session.exists():  # session may have been deleted while processing content
             session.inc_evaluated_content()
```

### Comparing `datapools-1.0.50/datapools/scheduler/scheduler.py` & `datapools-1.0.51/datapools/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.51/datapools/worker/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.51/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/plugins/default/default.py` & `datapools-1.0.51/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.51/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/plugins/freesound_org/freesound_org.py` & `datapools-1.0.51/datapools/worker/plugins/freesound_org/freesound_org.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.51/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.51/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.51/datapools/worker/plugins/s3/s3.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.51/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.51/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.51/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.51/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/datapools/worker/worker.py` & `datapools-1.0.51/datapools/worker/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
             QueueMessage(session_id, QueueMessageType.Report, {"task": deepcopy(task), "status": status.value})
         )
 
     async def _add_back_task(self, session_id, task: CrawlerBackTask):
         await self.reports_queue.push(QueueMessage(session_id, QueueMessageType.Task, task.to_dict()))
 
     def _get_plugin_object(self, cls, session_id) -> BasePlugin:
-        ctx = WorkerContext(session=self.session_manager.get(session_id), storage=self.storage)
+        ctx = WorkerContext(session=self.session_manager.get(session_id), storage=self.storage)  # type: ignore
 
         args = [ctx]
         kwargs = {}
         logger.info(f"_get_plugin_object {cls=}")
 
         # convert class name into config plugins key
         # example: GoogleDrivePlugin => google_drive
```

### Comparing `datapools-1.0.50/datapools.egg-info/PKG-INFO` & `datapools-1.0.51/datapools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.50
+Version: 1.0.51
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.50/datapools.egg-info/SOURCES.txt` & `datapools-1.0.51/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/setup.py` & `datapools-1.0.51/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.50/tests/test_base.py` & `datapools-1.0.51/tests/test_base.py`

 * *Files identical despite different names*

