# Comparing `tmp/datapools-1.0.49.tar.gz` & `tmp/datapools-1.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.49.tar", last modified: Sat May 11 13:59:45 2024, max compression
+gzip compressed data, was "datapools-1.0.50.tar", last modified: Wed May 15 15:00:45 2024, max compression
```

## Comparing `datapools-1.0.49.tar` & `datapools-1.0.50.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.458255 datapools-1.0.49/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-11 13:59:36.000000 datapools-1.0.49/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-05-11 13:59:36.000000 datapools-1.0.49/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-11 13:59:36.000000 datapools-1.0.49/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-11 13:59:36.000000 datapools-1.0.49/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-11 13:59:45.458255 datapools-1.0.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-11 13:59:36.000000 datapools-1.0.49/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.438255 datapools-1.0.49/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.442255 datapools-1.0.49/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.442255 datapools-1.0.49/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.446255 datapools-1.0.49/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.446255 datapools-1.0.49/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.446255 datapools-1.0.49/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.446255 datapools-1.0.49/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.446255 datapools-1.0.49/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/freesound_org/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/freesound_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/freesound_org/freesound_org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-11 13:59:45.000000 datapools-1.0.49/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-11 13:59:45.000000 datapools-1.0.49/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 13:59:45.000000 datapools-1.0.49/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-11 13:59:45.000000 datapools-1.0.49/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-11 13:59:45.000000 datapools-1.0.49/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-11 13:59:45.000000 datapools-1.0.49/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 13:59:45.458255 datapools-1.0.49/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-11 13:59:36.000000 datapools-1.0.49/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:36.000000 datapools-1.0.49/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-11 13:59:36.000000 datapools-1.0.49/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-11 13:59:36.000000 datapools-1.0.49/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.214233 datapools-1.0.50/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 15:00:35.000000 datapools-1.0.50/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    17986 2024-05-15 15:00:35.000000 datapools-1.0.50/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-15 15:00:35.000000 datapools-1.0.50/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 15:00:35.000000 datapools-1.0.50/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-15 15:00:45.214233 datapools-1.0.50/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-15 15:00:35.000000 datapools-1.0.50/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.202232 datapools-1.0.50/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.202232 datapools-1.0.50/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.202232 datapools-1.0.50/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.206232 datapools-1.0.50/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-05-15 15:00:35.000000 datapools-1.0.50/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-15 15:00:45.000000 datapools-1.0.50/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-15 15:00:45.000000 datapools-1.0.50/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:00:45.000000 datapools-1.0.50/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 15:00:45.000000 datapools-1.0.50/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-15 15:00:45.000000 datapools-1.0.50/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 15:00:45.000000 datapools-1.0.50/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:00:45.214233 datapools-1.0.50/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-15 15:00:35.000000 datapools-1.0.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:45.210233 datapools-1.0.50/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:00:35.000000 datapools-1.0.50/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 15:00:35.000000 datapools-1.0.50/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-15 15:00:35.000000 datapools-1.0.50/tests/test_base.py
```

### Comparing `datapools-1.0.49/HISTORY.md` & `datapools-1.0.50/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Publish session stats update as redis pubsub. [sergpsu]
+- Merge remote-tracking branch 'origin/master' into sergpsu-fixes.
+  [sergpsu]
+- Merge pull request #67 from torrentsai/sergpsu-fixes. [S]
+
+  Producer task rejection bugfix
+
+
+1.0.49 (2024-05-11)
+-------------------
+- Release: version 1.0.49 🚀 [sergpsu]
 - Merge remote-tracking branch 'origin/master' into sergpsu-fixes.
   [sergpsu]
 - Merge pull request #66 from torrentsai/sergpsu-fixes. [S]
 
   Session validation
 - Producer task rejection bugfix. [sergpsu]
```

### Comparing `datapools-1.0.49/LICENSE` & `datapools-1.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/PKG-INFO` & `datapools-1.0.50/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.49
+Version: 1.0.50
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.49/README.md` & `datapools-1.0.50/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/api.py` & `datapools-1.0.50/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/cli.py` & `datapools-1.0.50/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/common/backend_api.py` & `datapools-1.0.50/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/common/queues/__init__.py` & `datapools-1.0.50/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/common/queues/rabbitmq.py` & `datapools-1.0.50/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/common/queues/types.py` & `datapools-1.0.50/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/common/session_manager.py` & `datapools-1.0.50/datapools/common/session_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,125 +17,148 @@
 class SessionStatus(Enum):
     NORMAL = 0
     STOPPED = 1
 
 
 class Session:
     id: str
+    r: redis.Redis
+    meta_key: str
+    urls_key: str
+    content_key: str
+    stats_channel: str
 
-    def __init__(self, session_id, redis_inst):
+    def __init__(self, session_id, redis_inst: redis.Redis):
         self.id = session_id
-        self.redis = redis_inst
+        self.r = redis_inst
         self.meta_key = SessionManager.get_meta_key(self.id)
         self.urls_key = SessionManager.get_urls_key(self.id)
         self.content_key = SessionManager.get_content_key(self.id)
+        self.stats_channel = Session.get_stats_channel(self.id)
+
+    @staticmethod
+    def get_stats_channel(session_id_or_mask):
+        return f"stats_channel_{session_id_or_mask}"
+
+    @staticmethod
+    def get_stats_channel_mask():
+        return Session.get_stats_channel("*")
+
+    @staticmethod
+    def get_session_id_by_channel(channel_name):
+        return channel_name[14:]
 
     def get_meta(self):
-        raw = self.redis.hgetall(self.meta_key)
+        raw = self.r.hgetall(self.meta_key)
         res = {
             "hint_id": raw[b"hint_id"].decode(),
             "url": raw[b"url"].decode(),
             "total_tasks": int(raw[b"total_tasks"]),
             "complete_tasks": int(raw[b"complete_tasks"]),
             "failed_tasks": int(raw[b"failed_tasks"]),
             "rejected_tasks": int(raw[b"rejected_tasks"]),
             "crawled_content": int(raw[b"crawled_content"]),
             "evaluated_content": int(raw[b"evaluated_content"]),
             "status": int(raw[b"status"] if b"status" in raw else SessionStatus.NORMAL.value),
         }
         return res
 
     def set_status(self, status: SessionStatus):
-        self.redis.hset(self.meta_key, "status", status.value)
+        self.r.hset(self.meta_key, "status", status.value)
 
     def is_stopped(self):
-        status = self.redis.hget(self.meta_key, "status")
+        status = self.r.hget(self.meta_key, "status")
         return status is not None and int(status) == SessionStatus.STOPPED.value
 
     def add_url(self, url):
         # urls are stored in sets
-        res = self.redis.sadd(self.urls_key, url)
+        res = self.r.sadd(self.urls_key, url)
         if res:
-            self.redis.hincrby(self.meta_key, "total_tasks", 1)
+            self.r.hincrby(self.meta_key, "total_tasks", 1)
         return res == 1
 
     def has_url(self, url):
-        res = self.redis.sismember(self.urls_key, url)
+        res = self.r.sismember(self.urls_key, url)
         # logger.info( f'has_url {res=} {type(res)=}')
         return res
 
     def add_content(self, url):
-        return self.redis.sadd(self.content_key, url)
+        return self.r.sadd(self.content_key, url)
 
     def has_content(self, url):
-        return self.redis.sismember(self.content_key, url)
+        return self.r.sismember(self.content_key, url)
 
     def inc_complete_urls(self):
-        self.redis.hincrby(self.meta_key, "complete_tasks", 1)
+        self.r.hincrby(self.meta_key, "complete_tasks", 1)
+        self.r.publish(self.stats_channel, 1)
 
     def inc_failed_urls(self):
-        self.redis.hincrby(self.meta_key, "failed_tasks", 1)
+        self.r.hincrby(self.meta_key, "failed_tasks", 1)
+        self.r.publish(self.stats_channel, 1)
 
     def inc_rejected_urls(self):
-        self.redis.hincrby(self.meta_key, "rejected_tasks", 1)
+        self.r.hincrby(self.meta_key, "rejected_tasks", 1)
+        self.r.publish(self.stats_channel, 1)
 
     def inc_crawled_content(self):
-        self.redis.hincrby(self.meta_key, "crawled_content", 1)
+        self.r.hincrby(self.meta_key, "crawled_content", 1)
+        self.r.publish(self.stats_channel, 1)
 
     def inc_evaluated_content(self):
-        self.redis.hincrby(self.meta_key, "evaluated_content", 1)
+        self.r.hincrby(self.meta_key, "evaluated_content", 1)
+        self.r.publish(self.stats_channel, 1)
 
     def exists(self):
-        res = self.redis.exists(self.meta_key)
+        res = self.r.exists(self.meta_key)
         return res
 
 
 class SessionManager:
     def __init__(self, host, port=6379, db=0, protocol=3):
-        self.redis = redis.Redis(host=host, port=port, db=db, protocol=protocol)
+        self.r = redis.Redis(host=host, port=port, db=db, protocol=protocol)
 
     def is_ready(self) -> bool:
         try:
-            self.redis.ping()
+            self.r.ping()
             return True
         except redis.exceptions.ConnectionError:
             return False
 
     def create(self, hint_id=0, url="") -> Session:
         session_id = self.gen_session_id()
-        self.redis.hset(
+        self.r.hset(
             SessionManager.get_meta_key(session_id),
             mapping={
                 "hint_id": hint_id,
                 "url": url,
                 "total_tasks": 0,
                 "complete_tasks": 0,
                 "failed_tasks": 0,
                 "rejected_tasks": 0,
                 "crawled_content": 0,
                 "evaluated_content": 0,
                 "status": SessionStatus.NORMAL.value,
             },
         )
         # logger.info( f'hset result {r=} {type(r)=}')
-        return Session(session_id, self.redis)
+        return Session(session_id, self.r)
 
     def has(self, session_id) -> bool:
-        res = self.redis.exists(SessionManager.get_meta_key(session_id))
+        res = self.r.exists(SessionManager.get_meta_key(session_id))
         # logger.info( f'sessionmanager.has {res=} {type(res)=}')
         return res
 
     def get(self, session_id) -> Optional[Session]:
         if self.has(session_id):
-            return Session(session_id, self.redis)
+            return Session(session_id, self.r)
 
     def remove(self, session_id):
-        self.redis.delete(SessionManager.get_meta_key(session_id))
-        self.redis.delete(SessionManager.get_urls_key(session_id))
-        self.redis.delete(SessionManager.get_content_key(session_id))
+        self.r.delete(SessionManager.get_meta_key(session_id))
+        self.r.delete(SessionManager.get_urls_key(session_id))
+        self.r.delete(SessionManager.get_content_key(session_id))
 
     def gen_session_id(self) -> str:
         # TODO: add existance check
         return md5(str(time.time()).encode()).hexdigest()
 
     @staticmethod
     def get_meta_key(session_id):
@@ -146,12 +169,12 @@
         return f"{SESSION_URLS_KEY_PREFIX}{session_id}"
 
     @staticmethod
     def get_content_key(session_id):
         return f"{SESSION_CONTENT_KEY_PREFIX}{session_id}"
 
     def get_ids(self, limit) -> List[str]:
-        keys = self.redis.keys(f"{SESSION_METADATA_KEY_PREFIX}*")
+        keys = self.r.keys(f"{SESSION_METADATA_KEY_PREFIX}*")
         if len(keys) > limit:
             keys = keys[0:limit]
         n = len(SESSION_METADATA_KEY_PREFIX)
         return [k[n:] for k in keys]
```

### Comparing `datapools-1.0.49/datapools/common/stoppable.py` & `datapools-1.0.50/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/common/storage/base_storage.py` & `datapools-1.0.50/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/common/storage/file_storage.py` & `datapools-1.0.50/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.50/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.50/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/common/types.py` & `datapools-1.0.50/datapools/common/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/producer/base_producer.py` & `datapools-1.0.50/datapools/producer/base_producer.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/scheduler/scheduler.py` & `datapools-1.0.50/datapools/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.50/datapools/worker/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.50/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/plugins/default/default.py` & `datapools-1.0.50/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.50/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/plugins/freesound_org/freesound_org.py` & `datapools-1.0.50/datapools/worker/plugins/freesound_org/freesound_org.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.50/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.50/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.50/datapools/worker/plugins/s3/s3.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.50/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.50/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.50/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.50/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools/worker/worker.py` & `datapools-1.0.50/datapools/worker/worker.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/datapools.egg-info/PKG-INFO` & `datapools-1.0.50/datapools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.49
+Version: 1.0.50
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.49/datapools.egg-info/SOURCES.txt` & `datapools-1.0.50/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/setup.py` & `datapools-1.0.50/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.49/tests/test_base.py` & `datapools-1.0.50/tests/test_base.py`

 * *Files identical despite different names*

