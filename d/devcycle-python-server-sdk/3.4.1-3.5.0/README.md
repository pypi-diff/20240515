# Comparing `tmp/devcycle-python-server-sdk-3.4.1.tar.gz` & `tmp/devcycle-python-server-sdk-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcycle-python-server-sdk-3.4.1.tar", last modified: Fri Dec 15 20:15:05 2023, max compression
+gzip compressed data, was "devcycle-python-server-sdk-3.5.0.tar", last modified: Wed May 15 19:13:42 2024, max compression
```

## Comparing `devcycle-python-server-sdk-3.4.1.tar` & `devcycle-python-server-sdk-3.5.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.948382 devcycle-python-server-sdk-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-15 20:15:05.948382 devcycle-python-server-sdk-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.936382 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.940382 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/api/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/api/bucketing_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/api/config_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/api/event_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16332 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/api/local_bucketing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/devcycle_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9372 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.940382 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/managers/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/managers/event_queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.940382 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/bucketed_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/platform_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.940382 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/openfeature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/openfeature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/openfeature/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.940382 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/protobuf/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.940382 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/util/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/util/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.940382 devcycle-python-server-sdk-3.4.1/devcycle_python_server_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-15 20:15:05.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2023-12-15 20:15:05.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 20:15:05.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-15 20:15:05.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_server_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-15 20:15:05.000000 devcycle-python-server-sdk-3.4.1/devcycle_python_server_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.944382 devcycle-python-server-sdk-3.4.1/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/example/cloud_client_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/example/local_bucketing_client_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/example/openfeature_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-15 20:15:05.948382 devcycle-python-server-sdk-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.944382 devcycle-python-server-sdk-3.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.944382 devcycle-python-server-sdk-3.4.1/test/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/api/test_bucketing_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/api/test_config_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/api/test_event_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15631 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/api/test_local_bucketing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.944382 devcycle-python-server-sdk-3.4.1/test/fixture/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/fixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/fixture/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.944382 devcycle-python-server-sdk-3.4.1/test/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/managers/test_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11053 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/managers/test_event_queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.944382 devcycle-python-server-sdk-3.4.1/test/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/models/test_bucketed_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/models/test_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.944382 devcycle-python-server-sdk-3.4.1/test/openfeature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/openfeature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/openfeature/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/openfeature/test_provider_local_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)    11442 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/test_cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13022 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/test_local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:15:05.944382 devcycle-python-server-sdk-3.4.1/test/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/util/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/util/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-15 20:14:52.000000 devcycle-python-server-sdk-3.4.1/test/util/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.533181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/bucketing_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/config_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/event_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/local_bucketing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/devcycle_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/managers/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/managers/event_queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/bucketed_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/platform_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/open_feature_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/open_feature_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/open_feature_provider/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/protobuf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/util/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.537181 devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-15 19:13:41.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-15 19:13:42.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:13:41.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 19:13:41.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 19:13:41.000000 devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/example/cloud_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/example/local_bucketing_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/example/openfeature_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/api/test_bucketing_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/api/test_config_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/api/test_event_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/api/test_local_bucketing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/fixture/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/fixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/fixture/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/managers/test_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11053 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/managers/test_event_queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/models/test_bucketed_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/models/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/openfeature_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/openfeature_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/openfeature_test/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/openfeature_test/test_provider_local_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/test_cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/test_local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:42.541181 devcycle-python-server-sdk-3.5.0/test/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/util/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/util/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-15 19:13:22.000000 devcycle-python-server-sdk-3.5.0/test/util/test_version.py
```

### Comparing `devcycle-python-server-sdk-3.4.1/LICENSE` & `devcycle-python-server-sdk-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/README.md` & `devcycle-python-server-sdk-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/api/bucketing_client.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/api/config_client.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/config_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/api/event_client.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/event_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/api/local_bucketing.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/api/local_bucketing.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/cloud_client.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/cloud_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     CloudClientUnauthorizedError,
 )
 from devcycle_python_sdk.models.user import DevCycleUser
 from devcycle_python_sdk.models.event import DevCycleEvent
 from devcycle_python_sdk.models.variable import Variable
 from devcycle_python_sdk.models.feature import Feature
 from devcycle_python_sdk.util.version import sdk_version
-from devcycle_python_sdk.openfeature.provider import DevCycleProvider
+from devcycle_python_sdk.open_feature_provider.provider import DevCycleProvider
 
-from openfeature.provider.provider import AbstractProvider
+from openfeature.provider import AbstractProvider
 
 logger = logging.getLogger(__name__)
 
 
 class DevCycleCloudClient(AbstractDevCycleClient):
     """
     The DevCycle Python SDK that utilizes the DevCycle Bucketing API for feature and variable evaluation
```

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/devcycle_client.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/devcycle_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing
 from abc import abstractmethod
 
 from devcycle_python_sdk.models.user import DevCycleUser
 from devcycle_python_sdk.models.variable import Variable
 
-from openfeature.provider.provider import AbstractProvider
+from openfeature.provider import AbstractProvider
 
 
 class AbstractDevCycleClient:
     """
     A common interface for all DevCycle Clients
     """
```

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/exceptions.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/local_client.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/local_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from devcycle_python_sdk.managers.event_queue_manager import EventQueueManager
 from devcycle_python_sdk.models.bucketed_config import BucketedConfig
 from devcycle_python_sdk.models.event import DevCycleEvent, EventType
 from devcycle_python_sdk.models.feature import Feature
 from devcycle_python_sdk.models.platform_data import default_platform_data
 from devcycle_python_sdk.models.user import DevCycleUser
 from devcycle_python_sdk.models.variable import Variable
-from devcycle_python_sdk.openfeature.provider import DevCycleProvider
-from openfeature.provider.provider import AbstractProvider
+from devcycle_python_sdk.open_feature_provider.provider import DevCycleProvider
+from openfeature.provider import AbstractProvider
 
 logger = logging.getLogger(__name__)
 
 
 class DevCycleLocalClient(AbstractDevCycleClient):
     """
     The DevCycle Python SDK that utilizes the local bucketing library for feature and variable evaluation
```

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/managers/config_manager.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/managers/config_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/managers/event_queue_manager.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/managers/event_queue_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/bucketed_config.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/bucketed_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,22 +51,24 @@
         )
 
 
 @dataclass
 class ProjectSettings:
     edge_db: Optional[EdgeDBSettings]
     opt_in: Optional[OptInSettings]
+    disable_passthrough_rollouts: Optional[bool]
 
     @classmethod
     def from_json(cls, data: dict) -> "ProjectSettings":
         return cls(
             edge_db=EdgeDBSettings.from_json(data["edgeDB"])
             if "edgeDB" in data
             else None,
             opt_in=OptInSettings.from_json(data["optIn"]) if "optIn" in data else None,
+            disable_passthrough_rollouts=data.get("disablePassthroughRollouts", False),
         )
 
 
 @dataclass
 class Project:
     id: str
     key: str
```

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/event.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/event.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/feature.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/feature.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/platform_data.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/platform_data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/user.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,17 @@
             custom_data[key] = value
         else:
             raise InvalidContextError(
                 "Custom property values must be strings, numbers, booleans or None"
             )
 
     @staticmethod
-    def create_user_from_context(context: EvaluationContext) -> "DevCycleUser":
+    def create_user_from_context(
+        context: Optional[EvaluationContext],
+    ) -> "DevCycleUser":
         """
         Builds a DevCycleUser instance from the evaluation context. Will raise a TargetingKeyMissingError if
         the context does not contain a valid targeting key or user_id attribute
 
         :param context: The evaluation context to build the user from
         :return: A DevCycleUser instance
         """
```

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/models/variable.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/models/variable.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/openfeature/provider.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/open_feature_provider/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from typing import Any, Optional, Union, List
 
 from devcycle_python_sdk import AbstractDevCycleClient
 from devcycle_python_sdk.models.user import DevCycleUser
 
-from openfeature.provider.provider import AbstractProvider
+from openfeature.provider import AbstractProvider
 from openfeature.evaluation_context import EvaluationContext
 from openfeature.flag_evaluation import FlagResolutionDetails, Reason
 from openfeature.exception import ErrorCode, InvalidContextError, TypeMismatchError
 from openfeature.hook import Hook
 from openfeature.provider.metadata import Metadata
 
 logger = logging.getLogger(__name__)
```

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/options.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/options.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/protobuf/utils.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/protobuf/utils.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py` & `devcycle-python-server-sdk-3.5.0/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/devcycle_python_server_sdk.egg-info/SOURCES.txt` & `devcycle-python-server-sdk-3.5.0/devcycle_python_server_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 devcycle_python_sdk/models/bucketed_config.py
 devcycle_python_sdk/models/error_response.py
 devcycle_python_sdk/models/event.py
 devcycle_python_sdk/models/feature.py
 devcycle_python_sdk/models/platform_data.py
 devcycle_python_sdk/models/user.py
 devcycle_python_sdk/models/variable.py
-devcycle_python_sdk/openfeature/__init__.py
-devcycle_python_sdk/openfeature/provider.py
+devcycle_python_sdk/open_feature_provider/__init__.py
+devcycle_python_sdk/open_feature_provider/provider.py
 devcycle_python_sdk/protobuf/__init__.py
 devcycle_python_sdk/protobuf/utils.py
 devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
 devcycle_python_sdk/util/__init__.py
 devcycle_python_sdk/util/strings.py
 devcycle_python_sdk/util/version.py
 devcycle_python_server_sdk.egg-info/PKG-INFO
@@ -55,14 +55,14 @@
 test/fixture/data.py
 test/managers/__init__.py
 test/managers/test_config_manager.py
 test/managers/test_event_queue_manager.py
 test/models/__init__.py
 test/models/test_bucketed_config.py
 test/models/test_user.py
-test/openfeature/__init__.py
-test/openfeature/test_provider.py
-test/openfeature/test_provider_local_sdk.py
+test/openfeature_test/__init__.py
+test/openfeature_test/test_provider.py
+test/openfeature_test/test_provider_local_sdk.py
 test/util/__init__.py
 test/util/test_strings.py
 test/util/test_utils.py
 test/util/test_version.py
```

### Comparing `devcycle-python-server-sdk-3.4.1/example/cloud_client_example.py` & `devcycle-python-server-sdk-3.5.0/example/cloud_client_example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/example/local_bucketing_client_example.py` & `devcycle-python-server-sdk-3.5.0/example/local_bucketing_client_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import time
 
 from devcycle_python_sdk import DevCycleLocalClient, DevCycleLocalOptions
 from devcycle_python_sdk.models.user import DevCycleUser
 from devcycle_python_sdk.models.event import DevCycleEvent, EventType
 
-VARIABLE_KEY = "test-boolean-variable"
+VARIABLE_KEY = "python-example-tests"
 
 logger = logging.getLogger(__name__)
 
 
 def main():
     """
     Sample usage of the Python Server SDK using Local Bucketing.
```

### Comparing `devcycle-python-server-sdk-3.4.1/example/openfeature_example.py` & `devcycle-python-server-sdk-3.5.0/example/openfeature_example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/pyproject.toml` & `devcycle-python-server-sdk-3.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/setup.py` & `devcycle-python-server-sdk-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/test/api/test_bucketing_client.py` & `devcycle-python-server-sdk-3.5.0/test/api/test_bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/test/api/test_config_client.py` & `devcycle-python-server-sdk-3.5.0/test/api/test_config_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/test/api/test_event_client.py` & `devcycle-python-server-sdk-3.5.0/test/api/test_event_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/test/api/test_local_bucketing.py` & `devcycle-python-server-sdk-3.5.0/test/api/test_local_bucketing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import json
 import logging
 import unittest
 
 from devcycle_python_sdk.api.local_bucketing import LocalBucketing, WASMAbortError
 from devcycle_python_sdk.models.bucketed_config import (
     Environment,
-    EdgeDBSettings,
     FeatureVariation,
-    OptInColors,
-    OptInSettings,
     Project,
     ProjectSettings,
 )
 from devcycle_python_sdk.models.feature import Feature
 from devcycle_python_sdk.models.variable import Variable
 from devcycle_python_sdk.models.platform_data import default_platform_data
 from devcycle_python_sdk.models.user import DevCycleUser
@@ -207,30 +204,23 @@
                 evalReason=None,
             ),
         }
 
         self.assertIsNotNone(result)
         self.assertEqual(result.user, user)
         self.assertEqual(
-            result.project,
             Project(
                 id="61f97628ff4afcb6d057dbf0",
                 key="emma-project",
                 a0_organization="org_tPyJN5dvNNirKar7",
                 settings=ProjectSettings(
-                    edge_db=EdgeDBSettings(enabled=False),
-                    opt_in=OptInSettings(
-                        enabled=True,
-                        title="EarlyAccess",
-                        description="Getearlyaccesstobetafeaturesbelow!",
-                        image_url="",
-                        colors=OptInColors(primary="#531cd9", secondary="#16dec0"),
-                    ),
+                    edge_db=None, opt_in=None, disable_passthrough_rollouts=False
                 ),
             ),
+            result.project,
         )
         self.assertEqual(
             result.environment,
             Environment(id="61f97628ff4afcb6d057dbf2", key="development"),
         )
         self.assertEqual(
             result.features,
```

### Comparing `devcycle-python-server-sdk-3.4.1/test/fixture/data.py` & `devcycle-python-server-sdk-3.5.0/test/fixture/data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/test/managers/test_config_manager.py` & `devcycle-python-server-sdk-3.5.0/test/managers/test_config_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/test/managers/test_event_queue_manager.py` & `devcycle-python-server-sdk-3.5.0/test/managers/test_event_queue_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/test/models/test_bucketed_config.py` & `devcycle-python-server-sdk-3.5.0/test/models/test_bucketed_config.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/test/models/test_user.py` & `devcycle-python-server-sdk-3.5.0/test/models/test_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import unittest
 
 from devcycle_python_sdk.models.user import DevCycleUser
 
-from openfeature.provider.provider import EvaluationContext
+from openfeature.provider import EvaluationContext
 from openfeature.exception import TargetingKeyMissingError, InvalidContextError
 
 
 logger = logging.getLogger(__name__)
 
 
 class DevCycleUserTest(unittest.TestCase):
```

### Comparing `devcycle-python-server-sdk-3.4.1/test/openfeature/test_provider.py` & `devcycle-python-server-sdk-3.5.0/test/openfeature_test/test_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 import unittest
 from unittest.mock import MagicMock
 
-from openfeature.provider.provider import EvaluationContext
+from openfeature.provider import EvaluationContext
 from openfeature.flag_evaluation import Reason
 from openfeature.exception import (
     ErrorCode,
     TargetingKeyMissingError,
     InvalidContextError,
     TypeMismatchError,
 )
 
 from devcycle_python_sdk.models.variable import Variable, TypeEnum
 
-from devcycle_python_sdk.openfeature.provider import (
+from devcycle_python_sdk.open_feature_provider.provider import (
     DevCycleProvider,
 )
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `devcycle-python-server-sdk-3.4.1/test/openfeature/test_provider_local_sdk.py` & `devcycle-python-server-sdk-3.5.0/test/openfeature_test/test_provider_local_sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import unittest
 
 import responses
 
 from devcycle_python_sdk import DevCycleLocalClient, DevCycleLocalOptions
 from test.fixture.data import small_config_json
 
-from openfeature.provider.provider import EvaluationContext
+from openfeature.provider import EvaluationContext
 from openfeature.flag_evaluation import Reason
 
 logger = logging.getLogger(__name__)
 
 
 class DevCycleProviderWithLocalSDKTest(unittest.TestCase):
     """
```

### Comparing `devcycle-python-server-sdk-3.4.1/test/test_cloud_client.py` & `devcycle-python-server-sdk-3.5.0/test/test_cloud_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/test/test_local_client.py` & `devcycle-python-server-sdk-3.5.0/test/test_local_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/test/util/test_strings.py` & `devcycle-python-server-sdk-3.5.0/test/util/test_strings.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.4.1/test/util/test_utils.py` & `devcycle-python-server-sdk-3.5.0/test/util/test_utils.py`

 * *Files identical despite different names*

