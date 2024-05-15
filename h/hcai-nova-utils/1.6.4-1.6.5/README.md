# Comparing `tmp/hcai-nova-utils-1.6.4.tar.gz` & `tmp/hcai-nova-utils-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-utils-1.6.4.tar", last modified: Tue Mar 26 20:32:59 2024, max compression
+gzip compressed data, was "hcai-nova-utils-1.6.5.tar", last modified: Wed Mar 27 14:56:52 2024, max compression
```

## Comparing `hcai-nova-utils-1.6.4.tar` & `hcai-nova-utils-1.6.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.154928 hcai-nova-utils-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-26 20:32:59.154928 hcai-nova-utils-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.142928 hcai-nova-utils-1.6.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.146928 hcai-nova-utils-1.6.4/docs/docsource/
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/docs/docsource/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.150928 hcai-nova-utils-1.6.4/hcai_nova_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-26 20:32:59.000000 hcai-nova-utils-1.6.4/hcai_nova_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-03-26 20:32:59.000000 hcai-nova-utils-1.6.4/hcai_nova_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 20:32:59.000000 hcai-nova-utils-1.6.4/hcai_nova_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-26 20:32:59.000000 hcai-nova-utils-1.6.4/hcai_nova_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-26 20:32:59.000000 hcai-nova-utils-1.6.4/hcai_nova_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-26 20:32:59.000000 hcai-nova-utils-1.6.4/hcai_nova_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.146928 hcai-nova-utils-1.6.4/nova_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.146928 hcai-nova-utils-1.6.4/nova_utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18117 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.146928 hcai-nova-utils-1.6.4/nova_utils/data/file_reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/file_reader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.146928 hcai-nova-utils-1.6.4/nova_utils/data/file_reader/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/file_reader/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/file_reader/video/decord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/file_reader/video/decord_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/file_reader/video/imageio.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/file_reader/video/moviepy.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/file_reader/video/pyav.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.150928 hcai-nova-utils-1.6.4/nova_utils/data/handler/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38866 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/handler/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/handler/ihandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    40390 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/handler/nova_db_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/handler/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/handler/url_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.150928 hcai-nova-utils-1.6.4/nova_utils/data/provider/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23375 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    15768 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/provider/dataset_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/data/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.150928 hcai-nova-utils-1.6.4/nova_utils/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/interfaces/server_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.150928 hcai-nova-utils-1.6.4/nova_utils/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/scripts/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/scripts/process.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:59.150928 hcai-nova-utils-1.6.4/nova_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/utils/anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10799 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/utils/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/utils/path_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/utils/request_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/utils/ssi_data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    24367 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/utils/ssi_xml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/utils/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/nova_utils/utils/type_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-26 20:32:44.000000 hcai-nova-utils-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 20:32:59.154928 hcai-nova-utils-1.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.070778 hcai-nova-utils-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-27 14:56:52.070778 hcai-nova-utils-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.062779 hcai-nova-utils-1.6.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.062779 hcai-nova-utils-1.6.5/docs/docsource/
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/docs/docsource/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.070778 hcai-nova-utils-1.6.5/hcai_nova_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-27 14:56:52.000000 hcai-nova-utils-1.6.5/hcai_nova_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-03-27 14:56:52.000000 hcai-nova-utils-1.6.5/hcai_nova_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 14:56:52.000000 hcai-nova-utils-1.6.5/hcai_nova_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-27 14:56:52.000000 hcai-nova-utils-1.6.5/hcai_nova_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-27 14:56:52.000000 hcai-nova-utils-1.6.5/hcai_nova_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 14:56:52.000000 hcai-nova-utils-1.6.5/hcai_nova_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.062779 hcai-nova-utils-1.6.5/nova_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.066779 hcai-nova-utils-1.6.5/nova_utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18117 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.066779 hcai-nova-utils-1.6.5/nova_utils/data/file_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/file_reader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.066779 hcai-nova-utils-1.6.5/nova_utils/data/file_reader/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/file_reader/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/file_reader/video/decord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/file_reader/video/decord_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/file_reader/video/imageio.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/file_reader/video/moviepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/file_reader/video/pyav.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.066779 hcai-nova-utils-1.6.5/nova_utils/data/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38866 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/handler/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/handler/ihandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40383 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/handler/nova_db_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/handler/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/handler/url_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.066779 hcai-nova-utils-1.6.5/nova_utils/data/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23375 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15768 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/provider/dataset_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/data/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.066779 hcai-nova-utils-1.6.5/nova_utils/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/interfaces/server_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.070778 hcai-nova-utils-1.6.5/nova_utils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/scripts/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/scripts/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:52.070778 hcai-nova-utils-1.6.5/nova_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/utils/anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10799 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/utils/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/utils/path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/utils/request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/utils/ssi_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24367 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/utils/ssi_xml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/utils/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/nova_utils/utils/type_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-27 14:56:39.000000 hcai-nova-utils-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 14:56:52.070778 hcai-nova-utils-1.6.5/setup.cfg
```

### Comparing `hcai-nova-utils-1.6.4/PKG-INFO` & `hcai-nova-utils-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-utils
-Version: 1.6.4
+Version: 1.6.5
 Summary: This repository contains utility functions and interfaces that can be used to interact with the NOVA annotation tool.
 Author-email: Dominik Schiller <dominik.schiller@uni-a.de>
 Project-URL: Documentation, https://hcmlab.github.io/nova-utils/docbuild/
 Project-URL: Repository, https://github.com/hcmlab/nova-utils
 Keywords: NOVA,utility,annotation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `hcai-nova-utils-1.6.4/docs/docsource/conf.py` & `hcai-nova-utils-1.6.5/docs/docsource/conf.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/hcai_nova_utils.egg-info/PKG-INFO` & `hcai-nova-utils-1.6.5/hcai_nova_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-utils
-Version: 1.6.4
+Version: 1.6.5
 Summary: This repository contains utility functions and interfaces that can be used to interact with the NOVA annotation tool.
 Author-email: Dominik Schiller <dominik.schiller@uni-a.de>
 Project-URL: Documentation, https://hcmlab.github.io/nova-utils/docbuild/
 Project-URL: Repository, https://github.com/hcmlab/nova-utils
 Keywords: NOVA,utility,annotation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `hcai-nova-utils-1.6.4/hcai_nova_utils.egg-info/SOURCES.txt` & `hcai-nova-utils-1.6.5/hcai_nova_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/annotation.py` & `hcai-nova-utils-1.6.5/nova_utils/data/annotation.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/data.py` & `hcai-nova-utils-1.6.5/nova_utils/data/data.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/file_reader/video/decord.py` & `hcai-nova-utils-1.6.5/nova_utils/data/file_reader/video/decord.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/file_reader/video/decord_batch.py` & `hcai-nova-utils-1.6.5/nova_utils/data/file_reader/video/decord_batch.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/handler/file_handler.py` & `hcai-nova-utils-1.6.5/nova_utils/data/handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/handler/ihandler.py` & `hcai-nova-utils-1.6.5/nova_utils/data/handler/ihandler.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/handler/nova_db_handler.py` & `hcai-nova-utils-1.6.5/nova_utils/data/handler/nova_db_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,17 +549,17 @@
 
             (anno_data_doc,) = anno_doc["data"]
 
             # build annotation object
             (scheme_doc,) = anno_doc["scheme"]
 
         scheme_type = scheme_doc["type"]
-        scheme_description = scheme_doc.get("description")
-        scheme_examples = scheme_doc.get("examples")
-        scheme_attributes = scheme_doc.get("attributes")
+        scheme_description = scheme_doc.get("description", '')
+        scheme_examples = scheme_doc.get("examples", [])
+        scheme_attributes = scheme_doc.get("attributes", [])
         for sa in scheme_attributes:
             sa['values'] = [str(v['value']) for v in sa['values']]
 
         anno_data = None
         anno_duration = 0
 
         # discrete scheme
@@ -1001,18 +1001,18 @@
         amh = AnnotationHandler(db_host=IP, db_port=PORT, db_user=USER, db_password=PASSWORD)
 
         # load
         fs = "Loading {} took {}ms"
         t_start = perf_counter()
         discrete_anno = amh.load(
             dataset="therapai_deliberate_practice",
-            scheme="Verbale Ausdrucksfähigkeit",
+            scheme="transcript",
             annotator="schildom",
             session="224_1",
-            role="therapeut",
+            role="session",
             header_only=False
         )
         t_stop = perf_counter()
         print(fs.format("Discrete annotation", int((t_stop - t_start) * 1000)))
         breakpoint()
         t_start = perf_counter()
         continuous_anno = amh.load(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/handler/request_handler.py` & `hcai-nova-utils-1.6.5/nova_utils/data/handler/request_handler.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/handler/url_handler.py` & `hcai-nova-utils-1.6.5/nova_utils/data/handler/url_handler.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/provider/data_manager.py` & `hcai-nova-utils-1.6.5/nova_utils/data/provider/data_manager.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/provider/dataset_iterator.py` & `hcai-nova-utils-1.6.5/nova_utils/data/provider/dataset_iterator.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/static.py` & `hcai-nova-utils-1.6.5/nova_utils/data/static.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/data/stream.py` & `hcai-nova-utils-1.6.5/nova_utils/data/stream.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/interfaces/server_module.py` & `hcai-nova-utils-1.6.5/nova_utils/interfaces/server_module.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/scripts/parsers.py` & `hcai-nova-utils-1.6.5/nova_utils/scripts/parsers.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/scripts/process.py` & `hcai-nova-utils-1.6.5/nova_utils/scripts/process.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/utils/anno_utils.py` & `hcai-nova-utils-1.6.5/nova_utils/utils/anno_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/utils/cache_utils.py` & `hcai-nova-utils-1.6.5/nova_utils/utils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/utils/json_utils.py` & `hcai-nova-utils-1.6.5/nova_utils/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/utils/request_utils.py` & `hcai-nova-utils-1.6.5/nova_utils/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/utils/ssi_data_types.py` & `hcai-nova-utils-1.6.5/nova_utils/utils/ssi_data_types.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/utils/ssi_xml_utils.py` & `hcai-nova-utils-1.6.5/nova_utils/utils/ssi_xml_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/utils/stream_utils.py` & `hcai-nova-utils-1.6.5/nova_utils/utils/stream_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/utils/string_utils.py` & `hcai-nova-utils-1.6.5/nova_utils/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/nova_utils/utils/type_definitions.py` & `hcai-nova-utils-1.6.5/nova_utils/utils/type_definitions.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-1.6.4/pyproject.toml` & `hcai-nova-utils-1.6.5/pyproject.toml`

 * *Files identical despite different names*

