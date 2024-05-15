# Comparing `tmp/aloha-2022.919.1851.tar.gz` & `tmp/aloha-2024.515.1337.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aloha-2022.919.1851.tar", last modified: Mon Sep 19 18:51:41 2022, max compression
+gzip compressed data, was "aloha-2024.515.1337.tar", last modified: Wed May 15 13:37:27 2024, max compression
```

## Comparing `aloha-2022.919.1851.tar` & `aloha-2024.515.1337.tar`

### file list

```diff
@@ -1,94 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.585734 aloha-2022.919.1851/
--rw-r--r--   0 root         (0) root         (0)     1034 2022-09-19 18:51:41.585734 aloha-2022.919.1851/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       65 2022-09-19 18:51:25.000000 aloha-2022.919.1851/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.581734 aloha-2022.919.1851/aloha/
--rw-r--r--   0 root         (0) root         (0)       34 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2022-09-19 18:51:41.000000 aloha-2022.919.1851/aloha/_version.py
--rw-r--r--   0 root         (0) root         (0)      144 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.581734 aloha-2022.919.1851/aloha/config/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      493 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/config/hocon.py
--rw-r--r--   0 root         (0) root         (0)     2604 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/config/paths.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.581734 aloha-2022.919.1851/aloha/db/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1788 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/db/base.py
--rw-r--r--   0 root         (0) root         (0)     2948 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/db/elasticsearch.py
--rw-r--r--   0 root         (0) root         (0)     4229 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/db/kafka.py
--rw-r--r--   0 root         (0) root         (0)     9677 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/db/mongo.py
--rw-r--r--   0 root         (0) root         (0)     1526 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/db/mysql.py
--rw-r--r--   0 root         (0) root         (0)     1788 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/db/postgres.py
--rw-r--r--   0 root         (0) root         (0)     2069 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/db/redis.py
--rw-r--r--   0 root         (0) root         (0)     1850 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/db/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.581734 aloha-2022.919.1851/aloha/encrypt/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/encrypt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2964 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/encrypt/aes.py
--rw-r--r--   0 root         (0) root         (0)      486 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/encrypt/hash.py
--rw-r--r--   0 root         (0) root         (0)      621 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/encrypt/jwt.py
--rw-r--r--   0 root         (0) root         (0)     7025 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/encrypt/rsa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.581734 aloha-2022.919.1851/aloha/encrypt/vault/
--rw-r--r--   0 root         (0) root         (0)      173 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/encrypt/vault/__init__.py
--rw-r--r--   0 root         (0) root         (0)      780 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/encrypt/vault/base.py
--rw-r--r--   0 root         (0) root         (0)     3574 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/encrypt/vault/cyberark.py
--rw-r--r--   0 root         (0) root         (0)      563 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/encrypt/vault/plain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.581734 aloha-2022.919.1851/aloha/logger/
--rw-r--r--   0 root         (0) root         (0)      171 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1947 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/logger/handler.py
--rw-r--r--   0 root         (0) root         (0)     1671 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/logger/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.581734 aloha-2022.919.1851/aloha/script/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/script/__init__.py
--rw-r--r--   0 root         (0) root         (0)      503 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/script/base.py
--rw-r--r--   0 root         (0) root         (0)     5240 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/script/compile.py
--rw-r--r--   0 root         (0) root         (0)      155 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/script/info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.581734 aloha-2022.919.1851/aloha/service/
--rw-r--r--   0 root         (0) root         (0)      204 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.581734 aloha-2022.919.1851/aloha/service/api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1154 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/api/v0.py
--rw-r--r--   0 root         (0) root         (0)     4880 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/api/v1.py
--rw-r--r--   0 root         (0) root         (0)     3998 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/api/v2.py
--rw-r--r--   0 root         (0) root         (0)     1184 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.585734 aloha-2022.919.1851/aloha/service/http/
--rw-r--r--   0 root         (0) root         (0)      144 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2333 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/http/base_api_client.py
--rw-r--r--   0 root         (0) root         (0)     2404 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/http/base_api_handler.py
--rw-r--r--   0 root         (0) root         (0)      830 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/http/plain_http_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.585734 aloha-2022.919.1851/aloha/service/openapi/
--rw-r--r--   0 root         (0) root         (0)       34 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/openapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4230 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/openapi/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.585734 aloha-2022.919.1851/aloha/service/streamer/
--rw-r--r--   0 root         (0) root         (0)      199 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/streamer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6839 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/streamer/base.py
--rw-r--r--   0 root         (0) root         (0)      547 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/streamer/managed_model.py
--rw-r--r--   0 root         (0) root         (0)     4132 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/streamer/multiprocess.py
--rw-r--r--   0 root         (0) root         (0)     6055 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/streamer/redis.py
--rw-r--r--   0 root         (0) root         (0)     1516 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/streamer/threaded.py
--rw-r--r--   0 root         (0) root         (0)     2131 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/service/web.py
--rw-r--r--   0 root         (0) root         (0)      674 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.585734 aloha-2022.919.1851/aloha/testing/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/testing/service_v1.py
--rw-r--r--   0 root         (0) root         (0)     1001 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/testing/service_v2.py
--rw-r--r--   0 root         (0) root         (0)      183 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/testing/unit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.585734 aloha-2022.919.1851/aloha/times/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/times/__init__.py
--rw-r--r--   0 root         (0) root         (0)      616 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/times/timeout_async.py
--rw-r--r--   0 root         (0) root         (0)     6972 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/times/timeout_asyncio.py
--rw-r--r--   0 root         (0) root         (0)     1616 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/times/timeout_signal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.585734 aloha-2022.919.1851/aloha/util/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)      993 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/util/html.py
--rw-r--r--   0 root         (0) root         (0)      530 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/util/json.py
--rw-r--r--   0 root         (0) root         (0)      502 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/util/random.py
--rw-r--r--   0 root         (0) root         (0)     1439 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/util/sys_cuda.py
--rw-r--r--   0 root         (0) root         (0)     4336 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/util/sys_gpu.py
--rw-r--r--   0 root         (0) root         (0)     4216 2022-09-19 18:51:25.000000 aloha-2022.919.1851/aloha/util/sys_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 18:51:41.581734 aloha-2022.919.1851/aloha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1034 2022-09-19 18:51:41.000000 aloha-2022.919.1851/aloha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1895 2022-09-19 18:51:41.000000 aloha-2022.919.1851/aloha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-19 18:51:41.000000 aloha-2022.919.1851/aloha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2022-09-19 18:51:41.000000 aloha-2022.919.1851/aloha.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-19 18:51:37.000000 aloha-2022.919.1851/aloha.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      218 2022-09-19 18:51:41.000000 aloha-2022.919.1851/aloha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-09-19 18:51:41.000000 aloha-2022.919.1851/aloha.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-19 18:51:41.585734 aloha-2022.919.1851/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1933 2022-09-19 18:51:25.000000 aloha-2022.919.1851/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.861252 aloha-2024.515.1337/
+-rw-r--r--   0 root         (0) root         (0)     4489 2024-05-15 13:37:27.861252 aloha-2024.515.1337/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1599 2024-05-15 13:37:15.000000 aloha-2024.515.1337/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.845252 aloha-2024.515.1337/aloha/
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha/_version.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.845252 aloha-2024.515.1337/aloha/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      533 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/config/hocon.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/config/paths.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/base.py
+-rw-r--r--   0 root         (0) root         (0)     2948 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/elasticsearch.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/kafka.py
+-rw-r--r--   0 root         (0) root         (0)     9677 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/mongo.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/redis.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/db/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/encrypt/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3404 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/aes.py
+-rw-r--r--   0 root         (0) root         (0)      486 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/hash.py
+-rw-r--r--   0 root         (0) root         (0)      617 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/jwt.py
+-rw-r--r--   0 root         (0) root         (0)     7076 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/rsa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/encrypt/vault/
+-rw-r--r--   0 root         (0) root         (0)      173 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/vault/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      831 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/vault/base.py
+-rw-r--r--   0 root         (0) root         (0)     3686 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/vault/cyberark.py
+-rw-r--r--   0 root         (0) root         (0)      563 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/encrypt/vault/plain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/logger/
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/logger/handler.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/script/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/script/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/script/base.py
+-rw-r--r--   0 root         (0) root         (0)     5570 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/script/compile.py
+-rw-r--r--   0 root         (0) root         (0)       95 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/script/info.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/script/start.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/service/
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.849252 aloha-2024.515.1337/aloha/service/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/api/v0.py
+-rw-r--r--   0 root         (0) root         (0)     4880 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/api/v1.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/api/v2.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.853252 aloha-2024.515.1337/aloha/service/http/
+-rw-r--r--   0 root         (0) root         (0)      164 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/http/base_api_client.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/http/base_api_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/http/files.py
+-rw-r--r--   0 root         (0) root         (0)      830 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/http/plain_http_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.853252 aloha-2024.515.1337/aloha/service/openapi/
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/openapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/openapi/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.853252 aloha-2024.515.1337/aloha/service/streamer/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/streamer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/streamer/base.py
+-rw-r--r--   0 root         (0) root         (0)      547 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/streamer/managed_model.py
+-rw-r--r--   0 root         (0) root         (0)     4132 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/streamer/multiprocess.py
+-rw-r--r--   0 root         (0) root         (0)     6200 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/streamer/redis.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/streamer/threaded.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/service/web.py
+-rw-r--r--   0 root         (0) root         (0)      674 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.853252 aloha-2024.515.1337/aloha/testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/testing/service_v1.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/testing/service_v2.py
+-rw-r--r--   0 root         (0) root         (0)      183 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/testing/unit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.853252 aloha-2024.515.1337/aloha/times/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/times/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/times/timeout_async.py
+-rw-r--r--   0 root         (0) root         (0)     6972 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/times/timeout_asyncio.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/times/timeout_signal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.857252 aloha-2024.515.1337/aloha/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/html.py
+-rw-r--r--   0 root         (0) root         (0)      530 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/json.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/random.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/sys_cuda.py
+-rw-r--r--   0 root         (0) root         (0)     4335 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/sys_gpu.py
+-rw-r--r--   0 root         (0) root         (0)     4306 2024-05-15 13:37:15.000000 aloha-2024.515.1337/aloha/util/sys_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:37:27.857252 aloha-2024.515.1337/aloha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4489 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 13:37:23.000000 aloha-2024.515.1337/aloha.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      570 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-15 13:37:27.000000 aloha-2024.515.1337/aloha.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 13:37:27.861252 aloha-2024.515.1337/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-05-15 13:37:15.000000 aloha-2024.515.1337/setup.py
```

### Comparing `aloha-2022.919.1851/aloha/config/paths.py` & `aloha-2024.515.1337/aloha/config/paths.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 __all__ = ('get_resource_dir', 'get_config_dir', 'get_current_module_dir', 'get_project_base_dir', 'path_join')
 
 import os
+import warnings
 
 
 def path_join(*args) -> str:
     p = os.path.join(*args)
     p = os.path.expanduser(p)
     p = os.path.expandvars(p)
     p = os.path.abspath(p)
@@ -43,21 +44,27 @@
         if env_profile is None:
             files_config = 'main.conf'
         else:
             files_config = 'main-%s.conf' % env_profile
 
     files = files_config.split(',')
     ret = []
+    msgs = []
     for f in files:
         file = get_config_dir(f)
         if not os.path.exists(file):
-            raise RuntimeError('Config file [%s] does not exists!' % file)
+            msgs.append('Expecting config file [%s] but it does not exists!' % file)
         else:
             print('  ---> Loading config file [%s]' % file)
-        ret.append(os.path.expandvars(f))
+            ret.append(os.path.expandvars(f))
+    if len(ret) == 0:
+        msgs.append('No config files set properly, EMPTY config will be used!')
+
+    if len(msgs) > 0:
+        warnings.warn('\n'.join(msgs))
     return ret
 
 
 def get_current_module_dir(file_caller: str) -> str:
     dirs = file_caller.split(os.sep)
     return os.sep.join(dirs[:-1])
```

### Comparing `aloha-2022.919.1851/aloha/db/base.py` & `aloha-2024.515.1337/aloha/db/base.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/db/elasticsearch.py` & `aloha-2024.515.1337/aloha/db/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/db/kafka.py` & `aloha-2024.515.1337/aloha/db/kafka.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __all__ = ('KafkaOperator',)
 
 import json
 import typing
+
 import confluent_kafka as kafka
 import confluent_kafka.admin as kafka_admin
 
 from ..logger import LOG
 
 LOG.debug('Version of confluent_kafka client = %s' % kafka.__version__)
```

### Comparing `aloha-2022.919.1851/aloha/db/mongo.py` & `aloha-2024.515.1337/aloha/db/mongo.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/db/mysql.py` & `aloha-2024.515.1337/aloha/db/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 LOG.debug('Version of pymysql = %s' % pymysql.__version__)
 
 
 class MySqlOperator:
     def __init__(self, db_config, **kwargs):
         password_vault = PasswordVault.get_vault(db_config.get('vault_type'), db_config.get('vault_config'))
         self._config = {
-            'user': db_config['user'],
-            'password': password_vault.get_password(db_config['password']),
             'host': db_config['host'],
             'port': db_config['port'],
-            'dbname': db_config['dbname']
+            'user': db_config['user'],
+            'password': password_vault.get_password(db_config['password']),
+            'dbname': db_config['dbname'],
         }
 
         try:
             self.db = create_engine(
                 'mysql+pymysql://{user}:{password}@{host}:{port}/{dbname}'.format(**self._config),
                 encoding='utf-8', pool_size=50, pool_recycle=500, pool_pre_ping=True, **kwargs
             )
```

### Comparing `aloha-2022.919.1851/aloha/db/postgres.py` & `aloha-2024.515.1337/aloha/db/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 LOG.debug('postgres: psycopg2 version = %s' % psycopg2.__version__)
 
 
 class PostgresOperator:
     def __init__(self, db_config, **kwargs):
         password_vault = PasswordVault.get_vault(db_config.get('vault_type'), db_config.get('vault_config'))
         self._config = {
-            'user': db_config['user'],
-            'password': password_vault.get_password(db_config.get('password')),
             'host': db_config['host'],
             'port': db_config['port'],
-            'dbname': db_config['dbname']
+            'user': db_config['user'],
+            'password': password_vault.get_password(db_config.get('password')),
+            'dbname': db_config['dbname'],
         }
         connect_args = {}
         if 'schema' in db_config:
             connect_args['options'] = '-csearch_path={}'.format(db_config['schema'])
 
         try:
             self.engine = create_engine(
```

### Comparing `aloha-2022.919.1851/aloha/db/redis.py` & `aloha-2024.515.1337/aloha/db/redis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 __all__ = ('RedisOperator',)
 
 import redis
+from packaging import version
 
 from .base import PasswordVault
 from ..logger import LOG
 
 
 class RedisOperator:
     def __init__(self, config):
         self._check_redis_version()
 
-        password = config.get('password', None)
         password_vault = PasswordVault.get_vault(config.get('vault_type'), config.get('vault_config'))
         _config = {
             'host': config['host'],
             'port': config.get('port', '6379'),
-            'password': password_vault.get_password(password),
+            'password': password_vault.get_password(config.get('password', None)),
             'decode_responses': config.get('decode_responses', True),
             'retry_on_timeout': True,
             'max_connections': config.get('max_connections', 1000),
             'socket_timeout': 3,
             'socket_connect_timeout': 1,
         }
         if 'db' in config:
             _config['db'] = config['db']
         self._config = _config
 
         self._pool = None
 
     @staticmethod
     def _check_redis_version() -> bool:
+        ver_min = version.parse('4.1.0')
         valid = False
         try:
-            ver = redis.__version__.split('.')
-            ver = tuple(int(i) for i in ver)
-            if ver > (4, 1, 0):
+            ver_cur = version.parse(redis.__version__)
+            if ver_cur >= ver_min:
                 valid = True
                 LOG.debug('Using redis version = %s' % redis.__version__)
         except Exception as e:
             LOG.error('Failed to obtain redis version!')
             LOG.error(str(e))
 
         if not valid:
```

### Comparing `aloha-2022.919.1851/aloha/db/sqlite.py` & `aloha-2024.515.1337/aloha/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/encrypt/aes.py` & `aloha-2024.515.1337/aloha/encrypt/aes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,84 @@
 import base64
 import binascii
-from typing import Union
+from typing import Union, Callable, Optional
 
 from Crypto.Cipher import AES
 from Crypto.Random import get_random_bytes
 from Crypto.Util.Padding import pad, unpad
 
-_AES_CIPHER_METHODS = {  # FULL_CIPHER_NAME: (dict_params,)
-    "AES/ECB/PKCS5Padding": {'mode': AES.MODE_ECB},
-    # "AES/ECB/NoPadding": {'mode': AES.MODE_ECB},
-    # "AES/CBC/PKCS5Padding": {'mode': AES.MODE_CBC, 'iv': b'0000000000000000'},
-    # "AES/CBC/NoPadding": {'mode': AES.MODE_CBC, 'iv': b'0000000000000000'},
+_AES_CIPHER_METHODS = {  # FULL_CIPHER_NAME: (dict_params, pad_style)
+    "AES/ECB/PKCS5Padding": ({'mode': AES.MODE_ECB}, 'pkcs7'),
+    "AES/ECB/NoPadding": ({'mode': AES.MODE_ECB}, 'pkcs7'),
+    "AES/CBC/PKCS7Padding": ({'mode': AES.MODE_CBC, 'iv': b'0000000000000000'}, 'pkcs7'),
+    "AES/CBC/NoPadding": ({'mode': AES.MODE_CBC, 'iv': b'0000000000000000'}, 'x923'),
 }
 
 
 def _generate_key(key_size: int, method='const') -> bytes:
     if method == 'const':
         return b'0' * key_size  # b'b6046801716aec00'
     elif method == 'random':
         return get_random_bytes(key_size)
     raise ValueError('Invalid AES key generate method: [%s]' % method)
 
 
 class AesEncryptor:
+    supported_cipher_methods = _AES_CIPHER_METHODS
+
     def __init__(self, key: Union[str, bytes] = None, key_size: int = 16, cipher_name: str = 'AES/ECB/PKCS5Padding'):
         _key = key
         if key is None:
             _key = _generate_key(key_size)
         elif isinstance(key, str):
             _key = key.encode()
 
         if len(_key) not in (16, 24, 32,):
             raise ValueError("Invalid key size/length [%s] for AesEncryptor!" % len(_key))
 
         self.key_aes, self.block_size = _key, AES.block_size
         # https://pycryptodome.readthedocs.io/en/latest/src/util/util.html
         self.cipher_name = cipher_name
 
-    def encrypt(self, text: str, output_format='hex') -> Union[str, bytes]:
-        padded = pad(text.encode(), block_size=self.block_size)
+    def encrypt(self, text: str, output_format='hex', func_pad: Optional[Callable] = None) -> Union[str, bytes]:
+        dict_params, pad_style = _AES_CIPHER_METHODS.get(self.cipher_name)
+        if not callable(func_pad):
+            func_pad = lambda x: pad(data, block_size=self.block_size, style=pad_style)
 
-        dict_params = _AES_CIPHER_METHODS.get(self.cipher_name)
+        data = text.encode()
+        padded = func_pad(data)
         cipher = AES.new(key=self.key_aes, **dict_params)
         bytes_crypt = cipher.encrypt(padded)
 
         if output_format == 'hex':
             crypt = binascii.b2a_hex(bytes_crypt).decode()
         elif output_format == 'base64':
             crypt = base64.b64encode(bytes_crypt).decode()
         elif output_format in ('bytes', 'bin'):
             crypt = bytes_crypt
         else:
             raise ValueError('Unknown output_type [%s]' % output_format)
         return crypt
 
-    def decrypt(self, text: Union[str, bytes], input_format: str = 'hex') -> Union[str, bytes]:
+    def decrypt(self, text: Union[str, bytes], input_format: str = 'hex', func_unpad: Optional[Callable] = None) -> Union[str, bytes]:
         text += (len(text) % 4) * '='
         if input_format == 'hex':
             crypt = binascii.a2b_hex(text)
         elif input_format == 'base64':
             crypt = base64.b64decode(text)
         elif input_format in ('bytes', 'bin'):
             crypt = text
         else:
             raise ValueError('Unknown output_type [%s]' % input_format)
-        dict_params = _AES_CIPHER_METHODS.get(self.cipher_name)
+        dict_params, pad_style = _AES_CIPHER_METHODS.get(self.cipher_name)
         cipher = AES.new(key=self.key_aes, **dict_params)
         data = cipher.decrypt(crypt)
-        data = unpad(data, block_size=self.block_size)
+        if not callable(func_unpad):
+            func_unpad = lambda x: unpad(x, block_size=self.block_size, style=pad_style)
+        data = func_unpad(data)
         return data.decode('UTF-8')
 
 
 def main():
     a = AesEncryptor()
     src = 'hello~'
     enc = a.encrypt(src, output_format='base64')
```

### Comparing `aloha-2022.919.1851/aloha/encrypt/jwt.py` & `aloha-2024.515.1337/aloha/encrypt/jwt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import jwt
 
 from ..logger import LOG
 
-LOG.debug('Version of pyjwt = %s' % jwt.__version__.__str__())
+LOG.debug('Using pyjwt == %s' % jwt.__version__.__str__())
 
 
 def encode(
         secret_key: str,
         payload: dict,
         headers: dict = None,
         **kwargs
```

### Comparing `aloha-2022.919.1851/aloha/encrypt/rsa.py` & `aloha-2024.515.1337/aloha/encrypt/rsa.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "RSA/ECB/OAEPWithSHA-256AndMGF1Padding": (PKCS1_OAEP, {'hashAlgo': SHA256, 'mgfunc': lambda x, y: pss.MGF1(x, y, SHA1)}),
 }
 
 
 class RsaEncryptor:
     _dict_cache_cipher = {}
     _dict_cache_decipher = {}
+    supported_cipher_methods = _RSA_CIPHER_METHODS
 
     # ref: https://cryptobook.nakov.com/asymmetric-key-ciphers/rsa-encrypt-decrypt-examples
     def __init__(self, key_private: str = None, key_public: str = None, cipher_name: str = 'RSA/ECB/PKCS1Padding'):
         self.key_private, self.key_public = self.load_keys_from_string(key_private=key_private, key_public=key_public)
         assert self._get_cipher_module(cipher_name) is not None, 'Invalid cipher_name!'
         self.cipher_name = cipher_name
```

### Comparing `aloha-2022.919.1851/aloha/encrypt/vault/base.py` & `aloha-2024.515.1337/aloha/encrypt/vault/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-from abc import ABC, abstractmethod
+import abc
+
 from urllib.parse import quote_plus as urlquote
 
 
-class BaseVault(ABC):
-    @abstractmethod
+class BaseVault(abc.ABC):
+    @abc.abstractmethod
     def decrypt_password(self, *args, **kwargs):
         return kwargs.get('password')
 
-    def get_password(self, *args, **kwargs):
-        url_quote = kwargs.pop('url_quote', True)
+    def get_password(self, password, *args, **kwargs):
+        kwargs.update(password if isinstance(password, dict) else {'password': password})
+        url_quote = kwargs.get('url_encode', True)
 
         pwd = self.decrypt_password(*args, **kwargs)
         if pwd is None:
             return None
 
         if url_quote:
             return urlquote(pwd)
         else:
             return pwd
 
 
 class DummyVault(BaseVault):
-    def __init__(self, *args, **kwargs):
-        pass
-
-    def decrypt_password(self, password):
-        return password
+    def decrypt_password(self, *args, **kwargs):
+        return kwargs.get('password')
 
 
 def main():
     vault = DummyVault()
     ret = vault.get_password(None, url_quote=True)
     # print(ret)
     return ret
```

### Comparing `aloha-2022.919.1851/aloha/encrypt/vault/cyberark.py` & `aloha-2024.515.1337/aloha/encrypt/vault/cyberark.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 
 from .base import BaseVault
 from ...encrypt.aes import AesEncryptor
 from ...logger import LOG
 
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
-requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGHT:!DH:!aNULL'
+if hasattr(requests.packages.urllib3.util.ssl_, 'DEFAULT_CIPHERS'):
+    requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGHT:!DH:!aNULL'
 
 
 class CyberArkVault(BaseVault, AesEncryptor):
     _cached: dict = {}
 
     def __init__(self, url: str, app_id: str, key: str = None, safe: str = 'AIM_ELIS_LAS', folder: str = 'root'):
         super().__init__(key)
@@ -33,19 +34,17 @@
             return None
 
         cryptor = AES.new(self.key_aes, AES.MODE_ECB)
         s = cryptor.decrypt(a2b_hex(text.encode()))
         s = s[0: -s[-1]]
         return s.decode()
 
-    def get_cyberark_password(self, object=None, **kwargs):
-        if isinstance(object, dict):
-            kwargs.update(object)
-        elif isinstance(object, str):
-            kwargs.update({'object': object})
+    def get_cyberark_password(self, object: str = None, **kwargs):
+        assert isinstance(object, str)
+        kwargs.update({'object': object})
 
         app_id = kwargs.get('app_id', self.app_id)
         data = {
             "appId": app_id,
             "safe": kwargs.get('safe', self.safe),
             "folder": kwargs.get('folder', self.folder),
             "object": kwargs.get('object', object),
@@ -72,16 +71,19 @@
         return None
 
     def get_password(self, object=None, **kwargs):
         key_for_cache = '{app_id};{safe};{folder};{key};{object}'.format(
             app_id=self.app_id, safe=self.safe, folder=self.folder, key=self.key, object=object
         )
         if key_for_cache not in self._cached:
-            pwd = self.get_cyberark_password(object=object, **kwargs)
-            if kwargs.pop('url_quote', True):  # quote/escape password by default
+            kwargs.update(object if isinstance(object, dict) else {'object': object})
+            url_quote = kwargs.get('url_encode', True)
+
+            pwd = self.get_cyberark_password(**kwargs)
+            if url_quote:  # quote/escape password by default
                 pwd = urlquote(pwd)
             self._cached[key_for_cache] = pwd
         else:
             LOG.debug('Using cached CyberArk key: %s' % key_for_cache)
 
         return self._cached[key_for_cache]
```

### Comparing `aloha-2022.919.1851/aloha/encrypt/vault/plain.py` & `aloha-2024.515.1337/aloha/encrypt/vault/plain.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/logger/handler.py` & `aloha-2024.515.1337/aloha/logger/handler.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/logger/logger.py` & `aloha-2024.515.1337/aloha/logger/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .handler import MultiProcessSafeDailyRotatingFileHandler
 
 
 def setup_logger(logger: logging.Logger, level: int = logging.DEBUG, logger_name: str = None, module: str = None, formatter_str: str = None):
     if not logger.handlers:
         formatter = logging.Formatter(formatter_str or '%(levelname)s> %(asctime)s> %(module)s:%(lineno)s> %(message)s')
 
-        folder = 'logs'
+        folder = os.environ.get('DIR_LOG', 'logs')
         os.makedirs(folder, exist_ok=True)
 
         if module is None:
             from ..settings import SETTINGS
             module = SETTINGS.config.get('APP_MODULE') or os.environ.get('APP_MODULE', 'default')
 
         if logger_name is not None and len(logger_name) > 0:
```

### Comparing `aloha-2022.919.1851/aloha/script/compile.py` & `aloha-2024.515.1337/aloha/script/compile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 #!/usr/bin/env python3
 # This script build a given python package into a package of dynamic library (.so) files.
 
 __all__ = ('build', 'package')
 
-from collections import defaultdict
-
 import argparse
 import glob
 import os
 import shutil
 import time
-from Cython.Build import cythonize
+from collections import defaultdict
 from distutils.core import setup
 
+try:
+    from Cython.Build import cythonize
+except ImportError:
+    raise RuntimeError('Please pip install Cython first!')
+
 
 def _expand(patterns: list = None):
     files = []
     for pattern in patterns:
         for file in glob.glob(pattern):
             files.append(os.path.abspath(file))
     files = sorted(set(files))
     return files
 
 
 def _delete(file_path: str, ignore_errors=True):
+    print('Removing file/folder: %s' % file_path)
     try:
         if os.path.isfile(file_path) or os.path.islink(file_path):
             os.unlink(file_path)
         elif os.path.isdir(file_path):
             shutil.rmtree(file_path)
     except Exception as e:
         if not ignore_errors:
@@ -79,52 +83,52 @@
     n_parallel = os.cpu_count() or 8
 
     # python code -> c code
     cythonized = cythonize(target_cythonize, nthreads=n_parallel, language_level=3)
 
     # c code -> dynamic library file
     path_build_tmp = os.path.join(path_build, '.tmp')
-    setup(ext_modules=cythonized, script_args=["build_ext", "-b", path_build, "-t", path_build_tmp, "-j", n_parallel])
+    script_args = ["build_ext", "-b", path_build, "-t", path_build_tmp, "-j", n_parallel]
+    print('Build args: %s' % ' '.join(str(s) for s in script_args))
+    setup(ext_modules=cythonized, script_args=script_args)
 
     # clean up
     for c_module in cythonized:
         for c_file in c_module.sources:
-            os.remove(c_file)
+            _delete(c_file)
     for py_file in target_cythonize:
-        os.remove(py_file)
-
+        _delete(py_file)
     _delete(path_build_tmp)
 
-    print("\n\nSuccessfully finished building package to: ", path_build)
-
 
 def package(base: str = None, dist: str = 'build', exclude: list = None, keep: list = None, copy_others=True, *args, **kwargs):
     t = time.time()
 
     path_base = os.path.abspath(base or './')
     path_dist = os.path.abspath(dist)
+    os.makedirs(path_dist, exist_ok=True)
+    if len(glob.glob(path_dist + '/*')) > 0:
+        raise ValueError('Dist folder [%s] MUST be an empty directory or an non-existing folder!' % path_dist)
 
     folder_name = os.getcwd().split(os.sep)[-1]
     folder_temp = os.path.join('/tmp/build/', folder_name)
     print('Building project to path:', folder_temp)
     _delete(folder_temp, ignore_errors=True)  # clear the folder first
 
     build(
         base=path_base,  # use current directory by default
         dist=folder_temp,  # target directory for build files
         exclude=exclude,  # exclude this file by default, this is a collection of files/folders to exclude
         keep=keep,  # source files keep as is and not converting to dynamic library
         copy_others=copy_others
     )
-    t = time.time() - t
-    print('Time consumed to build code: %.2f seconds.' % t)
-
-    [_delete(f) for f in glob.glob(path_dist + '/*')]
-    os.makedirs(path_dist, exist_ok=True)
     [shutil.move(f, os.path.join(path_dist, f.split(os.sep)[-1])) for f in glob.glob(folder_temp + '/*')]
+    t = time.time() - t
+    print('\n\nTime consumed to build code: %.2f seconds.' % t)
+    print("Successfully finished building package to: ", path_dist)
 
 
 def main():
     p = argparse.ArgumentParser()
     p.add_argument('--base', type=str, help='root folder which includes source code to build')
     p.add_argument('--dist', type=str, default='build', help='target folder for the binary code')
     p.add_argument('--exclude', type=str, nargs='*', default=(), help='a collection of files/folders to exclude')
```

### Comparing `aloha-2022.919.1851/aloha/service/api/v0.py` & `aloha-2024.515.1337/aloha/service/api/v0.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 
 class APIHandler(AbstractApiHandler, ABC):
     MAP_ERROR_INFO = {
         'BAD_REQUEST': {'code': '5101', 'message': ['Bad request: fail to parse body as JSON object!']}
     }
 
     async def post(self, *args, **kwargs):
-        body_arguments = self.request_body
-        kwargs.update(body_arguments)
+        req_body = self.request_body
+
+        if req_body is not None:  # body_arguments
+            kwargs.update(req_body)
 
         resp = dict(code=5200, message=['success'])
         try:
             result = self.response(*args, **kwargs)  # this call may throw TypeError when argument missing
             resp['data'] = result
         except Exception as e:
             if self.LOG.level == logging.DEBUG:
```

### Comparing `aloha-2022.919.1851/aloha/service/api/v1.py` & `aloha-2024.515.1337/aloha/service/api/v1.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/service/api/v2.py` & `aloha-2024.515.1337/aloha/service/api/v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         if isinstance(resp, (dict, list)):
             resp = json.dumps(resp, ensure_ascii=False, default=str, separators=(',', ':'))
         return self.finish(resp)
 
 
 class APICaller(AbstractApiClient):
     APP_ID_KEYS = AbstractApiClient.config.get('APP_ID_KEYS', {})
-    APP_SECRET_KEY = AbstractApiClient.config['APP_SECRET_KEY']
+    APP_SECRET_KEY = AbstractApiClient.config.get('APP_SECRET_KEY')
 
     def wrap_request_data(self, data: dict) -> dict:
         assert isinstance(data, dict), "Data object must be a dict!"
         return data
 
     def get_headers(self, app_id: str = None, app_key: str = None) -> dict:
         if app_id is None:
```

### Comparing `aloha-2022.919.1851/aloha/service/app.py` & `aloha-2024.515.1337/aloha/service/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,44 +4,46 @@
 
 from ..logger import LOG
 
 try:
     import uvloop
     from tornado.platform.asyncio import AsyncIOMainLoop
 
+    LOG.info('Using uvloop == %s for service event loop...' % uvloop.__version__)
     asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
     AsyncIOMainLoop().install()
-    # asyncio.get_event_loop().run_forever()
-    # ^ the line above should be replaced by the start function below.
-    LOG.info('Using uvloop for service event loop...')
 except ImportError:
-    LOG.warn('[uvloop] NOT installed, fallback to asyncio loop! Please `pip install uvloop`!')
+    LOG.info('[uvloop] NOT installed, fallback to asyncio loop! Consider `pip install uvloop`!')
 
 from .web import WebApplication
 from ..settings import SETTINGS
 
 from tornado.options import options
 
-options['log_file_prefix'] = 'access.log'
-
-io_loop = asyncio.get_event_loop()
-
 
 class Application:
     def __init__(self, *args, **kwargs):
+        options['log_file_prefix'] = 'access.log'
         settings = dict(SETTINGS.config)
         self.web_app = WebApplication(settings)
-        self.io_loop = io_loop
 
     def start(self):
         try:
             self.web_app.start()
-            self.io_loop.run_forever()
+            event_loop = asyncio.get_event_loop()
+            if event_loop.is_running():
+                # notice: the event loop MUST NOT be initialized before web_app starts (as it may fork process)
+                # ref: https://github.com/tornadoweb/tornado/issues/2426#issuecomment-400895086
+                raise RuntimeError('Event loop already running before WebApp starts!')
+            else:
+                event_loop.run_forever()
         except KeyboardInterrupt:
             pass
         except Exception as e:
             raise e
         finally:
             pass
 
     def stop(self):
-        self.io_loop.stop()
+        event_loop = asyncio.get_event_loop()
+        if event_loop.is_running():
+            event_loop.stop()
```

### Comparing `aloha-2022.919.1851/aloha/service/http/base_api_client.py` & `aloha-2024.515.1337/aloha/service/http/base_api_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import uuid
 from abc import ABC, abstractmethod
+from urllib.parse import urljoin
 
 import requests
 from requests.adapters import HTTPAdapter, Retry
 
 from ...logger import LOG
 from ...settings import SETTINGS
 
 
 class AbstractApiClient(ABC):
     LOG = LOG
     RETRY_METHOD_WHITELIST: frozenset = frozenset(['GET', 'POST'])
     RETRY_STATUS_FORCELIST: frozenset = frozenset({413, 429, 503, 502, 504})
     config = SETTINGS.config
 
+    def __init__(self, url_endpoint: str = None, *args, **kwargs):
+        self.url_endpoint = url_endpoint or ''
+        LOG.debug('API Caller URL endpoint set to: %s' % self.url_endpoint)
+
     @classmethod
     def get_request_session(cls, total_retries: int = 3, *args, **kwargs) -> requests.Session:
         session = requests.Session()
         # https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#urllib3.util.Retry.DEFAULT_ALLOWED_METHODS
         retries = Retry(
             total=total_retries, backoff_factor=0.1, method_whitelist=cls.RETRY_METHOD_WHITELIST, status_forcelist=cls.RETRY_STATUS_FORCELIST
         )
@@ -48,20 +53,17 @@
         """
         body = data or dict()
         body.update(kwargs)
         payload = self.wrap_request_data(data=body)
         LOG.debug('Calling api: %s' % api_url)
         session = self.get_request_session()
         resp = session.post(
-            api_url, json=payload, timeout=timeout, headers=self.get_headers()
+            urljoin(self.url_endpoint, api_url), json=payload, timeout=timeout, headers=self.get_headers()
         )
 
         try:
             ret = resp.json()
         except Exception as e:
             LOG.error(str(e))
             raise RuntimeError(resp.text)
 
-        try:
-            return ret['data']
-        except KeyError:
-            raise RuntimeError(resp.text)
+        return ret
```

### Comparing `aloha-2022.919.1851/aloha/service/http/base_api_handler.py` & `aloha-2024.515.1337/aloha/service/http/base_api_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,20 +47,45 @@
 
     @property
     def request_body(self) -> dict:
         content_type: str = self.request_header_content_type
         body_arguments: dict = Optional[None]
 
         if content_type.startswith('multipart/form-data'):  # only parse files when 'Content-Type' starts with 'multipart/form-data'
-            body_arguments = self.request.body_arguments
+            body_arguments = self.request_param  # self.request.body_arguments
         else:
             try:
                 body = self.request.body.decode('utf-8')
                 body_arguments = json.loads(body)
             except (UnicodeDecodeError, json.decoder.JSONDecodeError):  # invalid request body, cannot be parsed as JSON
                 self.finish(self.MAP_ERROR_INFO['BAD_REQUEST'])
         return body_arguments
 
     @property
     def request_param(self) -> dict:
-        url_arguments: dict = {k: v[0].decode('utf-8') for k, v in self.request.arguments.items()}
-        return url_arguments
+        ret: dict = {}
+        for k, v in self.request.arguments.items():
+            val = v[0].decode('utf-8')
+            try:
+                value = json.loads(val)
+            except json.JSONDecodeError:
+                value = val
+            ret[k] = value
+
+        return ret
+
+
+class DefaultHandler404(AbstractApiHandler):
+    def response(self, *args, **kwargs) -> Optional[dict]:
+        return self.prepare()
+
+    def prepare(self):  # for all methods
+        msg = {
+            "code": 404,
+            "status": "error",
+            "message": [
+                'Requested URL cannot be found: %s' % self.request.uri
+            ]
+        }
+        msg = json.dumps(msg, ensure_ascii=False, default=str, separators=(',', ':'))
+        self.set_status(404, reason='Not Found')
+        self.finish(msg)
```

### Comparing `aloha-2022.919.1851/aloha/service/http/plain_http_handler.py` & `aloha-2024.515.1337/aloha/service/http/plain_http_handler.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/service/openapi/client.py` & `aloha-2024.515.1337/aloha/service/openapi/client.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/service/streamer/base.py` & `aloha-2024.515.1337/aloha/service/streamer/base.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/service/streamer/managed_model.py` & `aloha-2024.515.1337/aloha/service/streamer/managed_model.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/service/streamer/multiprocess.py` & `aloha-2024.515.1337/aloha/service/streamer/multiprocess.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/service/streamer/redis.py` & `aloha-2024.515.1337/aloha/service/streamer/redis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import multiprocessing
 import os
 import pickle
 import queue
 import threading
 import time
 
-from redis import Redis
-
 from .base import BaseStreamer, BaseWorker, TIMEOUT, TIME_SLEEP, logger
+from ...logger import LOG
+
+try:
+    from redis import Redis
+except ImportError:
+    LOG.warn('redis not installed, service.streamer.RedisStreamer will no be available!')
 
 
 class RedisWorker(BaseWorker):
     def __init__(self, func_predict, batch_size: int, max_latency=0.1,
                  redis_broker="localhost:6379", prefix='',
                  model_init_args=None, model_init_kwargs=None, *args, **kwargs):
         # assert issubclass(model_class, ManagedModel)
```

### Comparing `aloha-2022.919.1851/aloha/service/streamer/threaded.py` & `aloha-2024.515.1337/aloha/service/streamer/threaded.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/service/web.py` & `aloha-2024.515.1337/aloha/service/web.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         return [
             (HostMatches('(.*)'), handlers)
         ]
 
     def start(self):
         service_settings = self.settings.get('service', {})
 
-        port = service_settings.get('port', 80)
+        port = service_settings.get('port', int(os.environ.get('PORT_SVC', 80)))
         # if overwrite port in param
         port = os.environ.get('port', port)
 
-        num_process = int(service_settings.get('num_process', 1))
-        LOG.info('Starting service with [%s] process at port [%s]...', num_process, port)
+        num_process = int(service_settings.get('num_process', 0))
+        LOG.info('Starting service with [%s] process at port [%s]...', num_process or 'undefined', port)
         self.http_server.bind(port)
         self.http_server.start(num_processes=num_process)
```

### Comparing `aloha-2022.919.1851/aloha/settings.py` & `aloha-2024.515.1337/aloha/settings.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/testing/service_v1.py` & `aloha-2024.515.1337/aloha/testing/service_v1.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from abc import ABC
 
 import requests
 
-from .unit import UnitTestCase
 from aloha.service.api.v1 import APICaller
+from .unit import UnitTestCase
 
 
 class ServiceTestCase(UnitTestCase, ABC, APICaller):
     api_url_base = None
 
     @classmethod
     def setUpClass(cls) -> None:
```

### Comparing `aloha-2022.919.1851/aloha/testing/service_v2.py` & `aloha-2024.515.1337/aloha/testing/service_v2.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC
 
-from .unit import UnitTestCase
 from aloha.service.api.v2 import APICaller
+from .unit import UnitTestCase
 
 
 class ServiceTestCase(UnitTestCase, ABC, APICaller):
     api_url_base = None
 
     @classmethod
     def setUpClass(cls) -> None:
```

### Comparing `aloha-2022.919.1851/aloha/times/timeout_asyncio.py` & `aloha-2024.515.1337/aloha/times/timeout_asyncio.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/times/timeout_signal.py` & `aloha-2024.515.1337/aloha/times/timeout_signal.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/util/html.py` & `aloha-2024.515.1337/aloha/util/html.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/util/json.py` & `aloha-2024.515.1337/aloha/util/json.py`

 * *Files identical despite different names*

### Comparing `aloha-2022.919.1851/aloha/util/sys_cuda.py` & `aloha-2024.515.1337/aloha/util/sys_cuda.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,48 +3,65 @@
 from collections import namedtuple
 
 from ..logger import LOG
 
 Status = namedtuple('Status', 'version,gpu_availability')
 
 
-def get_gpu_status_for_tf() -> dict:
+def get_gpu_status_for_tf(*args, **kwargs) -> dict:
     status = Status(version=None, gpu_availability=False)
     try:
         import tensorflow as tf
         LOG.info('tensorflow version = %s' % tf.__version__)
         status = Status(
             version=tf.__version__,
             gpu_availability=tf.test.is_gpu_available()
         )
     except Exception as e:
         LOG.error('Error detecting CUDA availability for tensorflow')
         LOG.error(str(e))
     return status._asdict()
 
 
-def get_gpu_status_for_torch() -> dict:
+def get_gpu_status_for_torch(*args, **kwargs) -> dict:
     status = Status(version=None, gpu_availability=False)
     try:
         import torch
         LOG.info('torch version = %s' % torch.__version__)
         status = Status(
             version=torch.__version__,
             gpu_availability=torch.cuda.is_available()
         )
     except Exception as e:
         LOG.error('Error detecting CUDA availability for torch')
         LOG.error(str(e))
     return status._asdict()
 
 
-def get_cuda_info() -> dict:
+def get_gpu_status_for_paddle(*args, **kwargs) -> dict:
+    status = Status(version=None, gpu_availability=False)
+    try:
+        import paddle
+        LOG.info('Paddlepaddle version = %s' % paddle.__version__)
+        paddle.utils.run_check()
+        status = Status(
+            version=paddle.__version__,
+            gpu_availability=True
+        )
+    except Exception as e:
+        LOG.error('Error detecting CUDA availability for paddle')
+        LOG.error(str(e))
+    return status._asdict()
+
+
+def get_cuda_info(*args, **kwargs) -> dict:
     return {
         "cuda_availability_for_torch": get_gpu_status_for_torch(),
         "cuda_availability_for_tf": get_gpu_status_for_tf(),
+        "cuda_availability_for_paddle": get_gpu_status_for_paddle(),
     }
 
 
 def main(*args, **kwargs):
     data = get_cuda_info()
     import json
     print(json.dumps(data, ensure_ascii=False, indent=2))
```

### Comparing `aloha-2022.919.1851/aloha/util/sys_gpu.py` & `aloha-2024.515.1337/aloha/util/sys_gpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 try:
     import pynvml as nvml
     from pynvml.smi import nvidia_smi
 
     LOG.debug('Using pynvml == %s' % nvml.__version__)
 except ImportError:
-    LOG.error('Package `pynvml` NOT installed! Cannot get GPU info.')
+    LOG.warn('Package `pynvml` NOT installed! Cannot get GPU info.')
     nvml = nvidia_smi = None
 
 Device = namedtuple('Device', field_names='index,name,arch')
 DeviceStatus = namedtuple('DeviceStatus', field_names='mem_total,mem_free,mem_used,gpu_rate,mem_rate')
 
 
 class NvInfo:
```

### Comparing `aloha-2022.919.1851/aloha/util/sys_info.py` & `aloha-2024.515.1337/aloha/util/sys_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     factor = 1024
     for unit in ["", "K", "M", "G", "T", "P"]:
         if bytes < factor:
             return f"{bytes:.2f}{unit}{suffix}"
         bytes /= factor
 
 
-def get_os_info() -> dict:
+def get_os_info(*args, **kwargs) -> dict:
     ret = {}
 
     boot_time = datetime.fromtimestamp(psutil.boot_time())
     ret['boot_time'] = boot_time.strftime('%Y-%m-%d %H:%M:%S.%f')
 
     uname = platform.uname()
     ret.update(uname._asdict())
     return ret
 
 
-def get_cpu_info() -> dict:
+def get_cpu_info(*args, **kwargs) -> dict:
     cpu_freq = psutil.cpu_freq()  # CPU frequencies
     ret = {
         "num_cores_physical": psutil.cpu_count(logical=False),
         "num_cores_total": psutil.cpu_count(logical=True),
         "freq_max_mhz": f"{cpu_freq.max:.2f}",
         "freq_min_mhz": f"{cpu_freq.min:.2f}",
         "freq_cur_mhz": f"{cpu_freq.current:.2f}",
@@ -46,15 +46,15 @@
     }
     for i, percentage in enumerate(psutil.cpu_percent(percpu=True, interval=1)):
         ret['cpu_percent_core_%02d' % i] = f"{percentage}%"
 
     return ret
 
 
-def get_mem_info() -> dict:
+def get_mem_info(*args, **kwargs) -> dict:
     svmem = psutil.virtual_memory()
     swap = psutil.swap_memory()
 
     return {
         "vm_total": f"{get_size(svmem.total)}",
         "vm_available": f"{get_size(svmem.available)}",
         "vm_used": f"{get_size(svmem.used)}",
@@ -63,15 +63,15 @@
         "swap_total": f"{get_size(swap.total)}",
         "swap_free": f"{get_size(swap.free)}",
         "swap_used": f"{get_size(swap.used)}",
         "swap_percent": f"{swap.percent}%",
     }
 
 
-def get_disk_info() -> dict:
+def get_disk_info(*args, **kwargs) -> dict:
     # get IO statistics since boot
     disk_io = psutil.disk_io_counters()
     partitions = psutil.disk_partitions()
 
     ret = {
         "io_total_read": f"{get_size(disk_io.read_bytes)}",
         "io_total_write": f"{get_size(disk_io.write_bytes)}",
@@ -97,15 +97,15 @@
             pass  # this can be caught due to the disk that isn't ready
 
         ret["partitions"].append(part)
 
     return ret
 
 
-def get_net_info() -> dict:
+def get_net_info(*args, **kwargs) -> dict:
     # get IO statistics since boot
     net_io = psutil.net_io_counters()
 
     # get all network interfaces (virtual and physical)
     if_addresses = psutil.net_if_addrs()
 
     ret = {
@@ -126,15 +126,15 @@
             interface['%s_broadcast' % family] = address.broadcast
 
         ret['interfaces'].append(interface)
 
     return ret
 
 
-def get_sys_info() -> dict:
+def get_sys_info(*args, **kwargs) -> dict:
     return {
         "os_info": get_os_info(),
         "cpu_info": get_cpu_info(),
         "mem_info": get_mem_info(),
         "disk_info": get_disk_info(),
         "net_info": get_net_info(),
     }
```

### Comparing `aloha-2022.919.1851/aloha.egg-info/SOURCES.txt` & `aloha-2024.515.1337/aloha.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -35,24 +35,26 @@
 aloha/logger/__init__.py
 aloha/logger/handler.py
 aloha/logger/logger.py
 aloha/script/__init__.py
 aloha/script/base.py
 aloha/script/compile.py
 aloha/script/info.py
+aloha/script/start.py
 aloha/service/__init__.py
 aloha/service/app.py
 aloha/service/web.py
 aloha/service/api/__init__.py
 aloha/service/api/v0.py
 aloha/service/api/v1.py
 aloha/service/api/v2.py
 aloha/service/http/__init__.py
 aloha/service/http/base_api_client.py
 aloha/service/http/base_api_handler.py
+aloha/service/http/files.py
 aloha/service/http/plain_http_handler.py
 aloha/service/openapi/__init__.py
 aloha/service/openapi/client.py
 aloha/service/streamer/__init__.py
 aloha/service/streamer/base.py
 aloha/service/streamer/managed_model.py
 aloha/service/streamer/multiprocess.py
```

### Comparing `aloha-2022.919.1851/setup.py` & `aloha-2024.515.1337/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,51 +7,57 @@
 
 _now = datetime.now()
 _version = '%s.%02d%02d.%02d%02d' % (_now.year, _now.month, _now.day, _now.hour, _now.minute)
 
 with open('./aloha/_version.py', 'wt') as fp:
     fp.write('__version__ = "%s"\n' % _version)
 
+dict_extra_requires = {
+    'build': ['Cython'],
+    'service': ['requests', 'tornado', 'psutil', 'pyjwt'],
+    'db': ['sqlalchemy<2', 'psycopg2-binary', 'pymysql', 'elasticsearch', 'pymongo', 'redis>4.2.0'],
+    'stream': ['confluent_kafka'],
+    'data': ['pandas'],
+    'report': ['openpyxl>=3', 'XlsxWriter'],
+    'test': ['pytest-cov'],
+    'docs': ['mkdocs', 'mkdocstrings[python]', 'markdown-include', 'mkdocs-material'],
+}
+
 setup(
     name='aloha',
     version=_version,
     author='QPod',
     author_email='45032326+QPod0@users.noreply.github.com',
     license='Apache Software License',
     url='https://github.com/QPod/aloha',
     project_urls={
         'Source': 'https://github.com/QPod/aloha',
         'CI Pipeline': 'https://github.com/QPod/aloha/actions',
-        'Documentation': 'https://github.com/QPod/aloha/wiki',
+        'Documentation': 'https://aloha-python.readthedocs.io/',
     },
 
-    packages=find_packages(where=".", exclude=("app_demo*",)),
+    packages=find_packages(where=".", exclude=("app_common*",)),
     include_package_data=True,
     package_data={},
     platforms='Linux, Mac OS X, Windows',
     zip_safe=False,
-    install_requires=[],
+    install_requires=['attrdict3', 'pyhocon', 'pycryptodome', 'packaging'],
     extras_require={
-        'base': ['pyhocon', 'pycryptodome'],
-        'build': ['Cython'],
-        'service': ['requests', 'tornado', 'psutil'],
-        'db': ['sqlalchemy', 'psycopg2-binary', 'pymysql', 'elasticsearch', 'pymongo', 'redis>4.2.0'],
-        'stream': ['confluent_kafka'],
-        'data': ['pandas'],
-        'report': ['openpyxl>=3']
+        **dict_extra_requires,
+        'all': sorted(y for x in dict_extra_requires.values() for y in x),
     },
     python_requires='>=3.6',
     entry_points={
         'console_scripts': [
             'aloha = aloha.script.base:main'
         ]
     },
 
     data_files=[],
-    description='Aloha.',
+    description='Aloha - a versatile Python utility package for building services',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'Intended Audience :: Science/Research',
```

