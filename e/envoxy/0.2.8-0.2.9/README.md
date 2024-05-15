# Comparing `tmp/envoxy-0.2.8.tar.gz` & `tmp/envoxy-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/envoxy-0.2.8.tar", last modified: Fri Oct 27 16:48:28 2023, max compression
+gzip compressed data, was "dist/envoxy-0.2.9.tar", last modified: Wed Nov  8 19:40:15 2023, max compression
```

## Comparing `envoxy-0.2.8.tar` & `envoxy-0.2.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/envoxy.egg-info/
--rw-r--r--   0 root         (0) root         (0)        7 2023-10-27 16:48:28.000000 envoxy-0.2.8/envoxy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-27 16:48:28.000000 envoxy-0.2.8/envoxy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      282 2023-10-27 16:48:28.000000 envoxy-0.2.8/envoxy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1427 2023-10-27 16:48:28.000000 envoxy-0.2.8/envoxy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     5091 2023-10-27 16:48:28.000000 envoxy-0.2.8/envoxy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2020-01-30 17:54:32.000000 envoxy-0.2.8/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/views/
--rw-rw-r--   0 root         (0) root         (0)     1896 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/views/containers.py
--rw-rw-r--   0 root         (0) root         (0)     4411 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/views/views.py
--rw-r--r--   0 root         (0) root         (0)       44 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/http/
--rw-r--r--   0 root         (0) root         (0)     1427 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/http/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)      128 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/http/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1423 2022-11-17 10:40:18.000000 envoxy-0.2.8/src/envoxy/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/mqtt/
--rw-rw-r--   0 root         (0) root         (0)    14000 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/mqtt/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/mqtt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/redis/
--rw-rw-r--   0 root         (0) root         (0)     1865 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/redis/client.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/postgresql/
--rw-rw-r--   0 root         (0) root         (0)    10149 2023-10-27 16:33:55.000000 envoxy-0.2.8/src/envoxy/postgresql/client.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/postgresql/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      520 2022-11-17 10:40:18.000000 envoxy-0.2.8/src/envoxy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/zeromq/
--rw-rw-r--   0 root         (0) root         (0)    18641 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/zeromq/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/zeromq/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     3115 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/decorators.py
--rw-rw-r--   0 root         (0) root         (0)    17561 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/asserts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/couchdb/
--rw-rw-r--   0 root         (0) root         (0)     3271 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/couchdb/client.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/couchdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/cache/
--rw-r--r--   0 root         (0) root         (0)      513 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/cache/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1856 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/cache/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/utils/
--rw-rw-r--   0 root         (0) root         (0)      825 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/utils/encoders.py
--rw-r--r--   0 root         (0) root         (0)     2417 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/utils/watchdog.py
--rw-r--r--   0 root         (0) root         (0)      569 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/utils/datetime.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      565 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/utils/cache.py
--rw-r--r--   0 root         (0) root         (0)     7338 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/utils/logs.py
--rw-rw-r--   0 root         (0) root         (0)     1397 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/utils/throttle.py
--rw-rw-r--   0 root         (0) root         (0)     1846 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/utils/singleton.py
--rw-rw-r--   0 root         (0) root         (0)     1202 2021-11-09 12:43:56.000000 envoxy-0.2.8/src/envoxy/utils/config.py
--rw-rw-r--   0 root         (0) root         (0)     1237 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/utils/handlers.py
--rw-rw-r--   0 root         (0) root         (0)     1394 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/utils/profiling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/db/
--rw-r--r--   0 root         (0) root         (0)     2934 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/db/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)       46 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/db/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15506 2021-11-09 12:43:56.000000 envoxy-0.2.8/src/envoxy/tests/test_asserts.py
--rw-r--r--   0 root         (0) root         (0)     1204 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/tests/fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 16:48:28.000000 envoxy-0.2.8/src/envoxy/auth/
--rw-rw-r--   0 root         (0) root         (0)     2619 2023-07-05 18:40:52.000000 envoxy-0.2.8/src/envoxy/auth/backends.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.8/src/envoxy/auth/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      230 2023-07-05 18:40:52.000000 envoxy-0.2.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-27 16:48:28.000000 envoxy-0.2.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     4772 2021-11-09 12:43:56.000000 envoxy-0.2.8/README.md
--rw-rw-r--   0 root         (0) root         (0)       64 2023-07-05 18:40:52.000000 envoxy-0.2.8/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     1202 2023-10-27 16:35:14.000000 envoxy-0.2.8/setup.py
--rw-r--r--   0 root         (0) root         (0)     5091 2023-10-27 16:48:28.000000 envoxy-0.2.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/envoxy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        7 2023-11-08 19:40:15.000000 envoxy-0.2.9/envoxy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-08 19:40:15.000000 envoxy-0.2.9/envoxy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      282 2023-11-08 19:40:15.000000 envoxy-0.2.9/envoxy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-11-08 19:40:15.000000 envoxy-0.2.9/envoxy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     5091 2023-11-08 19:40:15.000000 envoxy-0.2.9/envoxy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2020-01-30 17:54:32.000000 envoxy-0.2.9/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/views/
+-rw-rw-r--   0 root         (0) root         (0)     1896 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/views/containers.py
+-rw-rw-r--   0 root         (0) root         (0)     4411 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/views/views.py
+-rw-r--r--   0 root         (0) root         (0)       44 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/http/
+-rw-r--r--   0 root         (0) root         (0)     1427 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/http/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)      128 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/http/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1423 2022-11-17 10:40:18.000000 envoxy-0.2.9/src/envoxy/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/mqtt/
+-rw-rw-r--   0 root         (0) root         (0)    14000 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/mqtt/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/mqtt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/redis/
+-rw-rw-r--   0 root         (0) root         (0)     1865 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/redis/client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/redis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/postgresql/
+-rw-rw-r--   0 root         (0) root         (0)     9827 2023-11-08 19:35:00.000000 envoxy-0.2.9/src/envoxy/postgresql/client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/postgresql/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      520 2022-11-17 10:40:18.000000 envoxy-0.2.9/src/envoxy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/zeromq/
+-rw-rw-r--   0 root         (0) root         (0)    18641 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/zeromq/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/zeromq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     3115 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/decorators.py
+-rw-rw-r--   0 root         (0) root         (0)    17561 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/asserts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/couchdb/
+-rw-rw-r--   0 root         (0) root         (0)     3271 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/couchdb/client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/couchdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/cache/
+-rw-r--r--   0 root         (0) root         (0)      513 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/cache/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1856 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/cache/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/utils/
+-rw-rw-r--   0 root         (0) root         (0)      825 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/utils/encoders.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/utils/watchdog.py
+-rw-r--r--   0 root         (0) root         (0)      569 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/utils/datetime.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      565 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/utils/cache.py
+-rw-r--r--   0 root         (0) root         (0)     7338 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/utils/logs.py
+-rw-rw-r--   0 root         (0) root         (0)     1397 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/utils/throttle.py
+-rw-rw-r--   0 root         (0) root         (0)     1846 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/utils/singleton.py
+-rw-rw-r--   0 root         (0) root         (0)     1202 2021-11-09 12:43:56.000000 envoxy-0.2.9/src/envoxy/utils/config.py
+-rw-rw-r--   0 root         (0) root         (0)     1237 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/utils/handlers.py
+-rw-rw-r--   0 root         (0) root         (0)     1394 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/utils/profiling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/db/
+-rw-r--r--   0 root         (0) root         (0)     2934 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/db/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       46 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/db/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15506 2021-11-09 12:43:56.000000 envoxy-0.2.9/src/envoxy/tests/test_asserts.py
+-rw-r--r--   0 root         (0) root         (0)     1204 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/tests/fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 19:40:15.000000 envoxy-0.2.9/src/envoxy/auth/
+-rw-rw-r--   0 root         (0) root         (0)     2619 2023-07-05 18:40:52.000000 envoxy-0.2.9/src/envoxy/auth/backends.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-01-30 17:54:32.000000 envoxy-0.2.9/src/envoxy/auth/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      230 2023-07-05 18:40:52.000000 envoxy-0.2.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-11-08 19:40:15.000000 envoxy-0.2.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     4772 2021-11-09 12:43:56.000000 envoxy-0.2.9/README.md
+-rw-rw-r--   0 root         (0) root         (0)       64 2023-07-05 18:40:52.000000 envoxy-0.2.9/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)     1202 2023-11-08 19:36:00.000000 envoxy-0.2.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)     5091 2023-11-08 19:40:15.000000 envoxy-0.2.9/PKG-INFO
```

### Comparing `envoxy-0.2.8/envoxy.egg-info/SOURCES.txt` & `envoxy-0.2.9/envoxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/envoxy.egg-info/PKG-INFO` & `envoxy-0.2.9/envoxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envoxy
-Version: 0.2.8
+Version: 0.2.9
 Summary: Envoxy Platform Framework
 Home-page: https://github.com/habitio/envoxy
 Author: Matheus (vorjdux) Santos
 Author-email: vorj.dux@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `envoxy-0.2.8/LICENSE` & `envoxy-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/views/containers.py` & `envoxy-0.2.9/src/envoxy/views/containers.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/views/views.py` & `envoxy-0.2.9/src/envoxy/views/views.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/http/dispatcher.py` & `envoxy-0.2.9/src/envoxy/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/constants.py` & `envoxy-0.2.9/src/envoxy/constants.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/mqtt/dispatcher.py` & `envoxy-0.2.9/src/envoxy/mqtt/dispatcher.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/redis/client.py` & `envoxy-0.2.9/src/envoxy/redis/client.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/postgresql/client.py` & `envoxy-0.2.9/src/envoxy/postgresql/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,16 +89,15 @@
 
         :param server_key: Identifier for the server configuration.
         :param max_retries: Number of retries to get a healthy connection.
         :param delay: Delay between retries.
         :return: Database connection.
         """
   
-        with self._lock:
-            _instance = self._instances.get(server_key)
+        _instance = self._instances.get(server_key)
             
         if not _instance:
             raise DatabaseException(f"No configuration found for server key: {server_key}")
 
         if 'conn_pool' not in _instance:
             self.connect(_instance)
 
@@ -132,32 +131,26 @@
         Returns a configuration value for the server.
 
         :param server_key: Identifier for the server configuration.
         :param key: Configuration key.
         :return: Configuration value.
         """
         
-        with self._lock:
-            return self._instances[server_key]['conf'].get(key, None)
+        return self._instances[server_key]['conf'].get(key, None)
         
     def connect(self, instance, reconnect_attempts=3, reconnect_delay=1):
         """
         Connects to the database server.
 
         :param instance: Instance configuration.
         :param reconnect_attempts: Number of attempts to reconnect.
         :param reconnect_delay: Delay between reconnection attempts.
         :return: None
         """
-
-        if 'conn_pool' in instance and instance['conn_pool'] is not None:
-            with self._lock:
-                instance['conn_pool'].closeall()
-            
-        instance['conn_pool'] = None
+    
         _conf = instance['conf']
 
         _max_conn = int(_conf.get('max_conn', MAX_CONN))
         _timeout = int(_conf.get('timeout', TIMEOUT_CONN))
                 
         _conn_pool = self._retry_on_failure(
             lambda: SemaphoreThreadedConnectionPool(
@@ -193,23 +186,21 @@
         """
 
         # Check and handle broken connections upon release
         if not self._is_connection_healthy(conn):    
             
             conn.close()
             
-            with self._lock:
-                _instance = self._instances[server_key]
+            _instance = self._instances[server_key]
             
             self.connect(_instance)
 
         else:
             
-            with self._lock:
-                self._instances[server_key]['conn_pool'].putconn(conn)
+            self._instances[server_key]['conn_pool'].putconn(conn)
 
     @contextmanager
     def transaction(self, server_key):
         """
         Context manager for database transactions.
 
         :param server_key: Identifier for the server configuration.
```

### Comparing `envoxy-0.2.8/src/envoxy/__init__.py` & `envoxy-0.2.9/src/envoxy/__init__.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/zeromq/dispatcher.py` & `envoxy-0.2.9/src/envoxy/zeromq/dispatcher.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/decorators.py` & `envoxy-0.2.9/src/envoxy/decorators.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/asserts.py` & `envoxy-0.2.9/src/envoxy/asserts.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/couchdb/client.py` & `envoxy-0.2.9/src/envoxy/couchdb/client.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/cache/__init__.py` & `envoxy-0.2.9/src/envoxy/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/cache/redis.py` & `envoxy-0.2.9/src/envoxy/cache/redis.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/utils/encoders.py` & `envoxy-0.2.9/src/envoxy/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/utils/watchdog.py` & `envoxy-0.2.9/src/envoxy/utils/watchdog.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/utils/datetime.py` & `envoxy-0.2.9/src/envoxy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/utils/cache.py` & `envoxy-0.2.9/src/envoxy/utils/cache.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/utils/logs.py` & `envoxy-0.2.9/src/envoxy/utils/logs.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/utils/throttle.py` & `envoxy-0.2.9/src/envoxy/utils/throttle.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/utils/singleton.py` & `envoxy-0.2.9/src/envoxy/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/utils/config.py` & `envoxy-0.2.9/src/envoxy/utils/config.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/utils/handlers.py` & `envoxy-0.2.9/src/envoxy/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/utils/profiling.py` & `envoxy-0.2.9/src/envoxy/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/db/dispatcher.py` & `envoxy-0.2.9/src/envoxy/db/dispatcher.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/tests/test_asserts.py` & `envoxy-0.2.9/src/envoxy/tests/test_asserts.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/tests/fixtures.py` & `envoxy-0.2.9/src/envoxy/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/src/envoxy/auth/backends.py` & `envoxy-0.2.9/src/envoxy/auth/backends.py`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/README.md` & `envoxy-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `envoxy-0.2.8/setup.py` & `envoxy-0.2.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     return os.path.join(data_dir, path)
 
 with open(find_file('README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='envoxy',
-    version='0.2.8',
+    version='0.2.9',
     description='Envoxy Platform Framework',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Matheus (vorjdux) Santos',
     author_email='vorj.dux@gmail.com',
     url='https://github.com/habitio/envoxy',
     packages=find_packages(where='src/', exclude=("tests", "templates")),
```

### Comparing `envoxy-0.2.8/PKG-INFO` & `envoxy-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envoxy
-Version: 0.2.8
+Version: 0.2.9
 Summary: Envoxy Platform Framework
 Home-page: https://github.com/habitio/envoxy
 Author: Matheus (vorjdux) Santos
 Author-email: vorj.dux@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

