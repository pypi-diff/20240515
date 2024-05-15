# Comparing `tmp/ghga_service_commons-3.1.2.tar.gz` & `tmp/ghga_service_commons-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_service_commons-3.1.2.tar", last modified: Mon Apr 15 14:09:36 2024, max compression
+gzip compressed data, was "ghga_service_commons-3.1.3.tar", last modified: Wed Apr 17 12:16:26 2024, max compression
```

## Comparing `ghga_service_commons-3.1.2.tar` & `ghga_service_commons-3.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.115130 ghga_service_commons-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-15 14:09:36.115130 ghga_service_commons-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:09:36.115130 ghga_service_commons-3.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.103130 ghga_service_commons-3.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.107130 ghga_service_commons-3.1.2/src/ghga_service_commons/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.107130 ghga_service_commons-3.1.2/src/ghga_service_commons/api/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/api/di.py
--rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/api/mock_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/api/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.107130 ghga_service_commons-3.1.2/src/ghga_service_commons/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/auth/ghga.py
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/auth/jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/auth/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.111130 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/base_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.111130 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.111130 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.111130 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/handlers/fastapi_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.111130 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/crypt4gh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/jwt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/multinode_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/simple_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/temp_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/utc_dates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.111130 ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-15 14:09:36.000000 ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-15 14:09:36.000000 ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:09:36.000000 ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 14:09:36.000000 ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 14:09:36.000000 ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:16:26.918820 ghga_service_commons-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-17 12:16:26.918820 ghga_service_commons-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 12:16:26.918820 ghga_service_commons-3.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:16:26.906820 ghga_service_commons-3.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:16:26.906820 ghga_service_commons-3.1.3/src/ghga_service_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:16:26.910820 ghga_service_commons-3.1.3/src/ghga_service_commons/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/api/di.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/api/mock_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/api/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:16:26.910820 ghga_service_commons-3.1.3/src/ghga_service_commons/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/auth/ghga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/auth/jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/auth/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:16:26.910820 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/base_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:16:26.914820 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/client/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/client/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/client/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:16:26.914820 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/server/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:16:26.914820 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/server/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/server/handlers/fastapi_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:16:26.914820 ghga_service_commons-3.1.3/src/ghga_service_commons/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/utils/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/utils/crypt4gh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/utils/jwt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/utils/multinode_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/utils/simple_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/utils/temp_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-17 12:16:18.000000 ghga_service_commons-3.1.3/src/ghga_service_commons/utils/utc_dates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:16:26.914820 ghga_service_commons-3.1.3/src/ghga_service_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-17 12:16:26.000000 ghga_service_commons-3.1.3/src/ghga_service_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-17 12:16:26.000000 ghga_service_commons-3.1.3/src/ghga_service_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:16:26.000000 ghga_service_commons-3.1.3/src/ghga_service_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-17 12:16:26.000000 ghga_service_commons-3.1.3/src/ghga_service_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 12:16:26.000000 ghga_service_commons-3.1.3/src/ghga_service_commons.egg-info/top_level.txt
```

### Comparing `ghga_service_commons-3.1.2/LICENSE` & `ghga_service_commons-3.1.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+   Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
    for the German Human Genome-Phenome Archive (GHGA)
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/PKG-INFO` & `ghga_service_commons-3.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: ghga_service_commons
-Version: 3.1.2
+Version: 3.1.3
 Summary: A library that contains common functionality used in services of GHGA
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/ghga-service-commons
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,18 +32,18 @@
 Provides-Extra: dev
 Requires-Dist: requests<3,>=2.31; extra == "dev"
 Provides-Extra: objectstorage
 Requires-Dist: hexkit<4,>=2; extra == "objectstorage"
 Provides-Extra: all
 Requires-Dist: ghga-service-commons[api,auth,crypt,dev,objectstorage]; extra == "all"
 
-![tests](https://github.com/ghga-de/ghga-service-commons/actions/workflows/unit_and_int_tests.yaml/badge.svg)
+![tests](https://github.com/ghga-de/ghga-service-commons/actions/workflows/tests.yaml/badge.svg)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/ghga_service_commons.svg)](https://pypi.python.org/pypi/ghga_service_commons/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ghga_service_commons.svg)](https://pypi.python.org/pypi/ghga_service_commons/)
-[![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga_service_commons/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga_service_commons?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga-service-commons/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga-service-commons?branch=main)
 
 # ghga-service-commons
 This Python library serves as a collection of common utilities used by
 the microservices developed at German Human Genome-Phenome Archive (GHGA).
 
 It collects boilerplate code for common functionalities such as API server setup,
 authentication and authorization.
```

### Comparing `ghga_service_commons-3.1.2/README.md` & `ghga_service_commons-3.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-![tests](https://github.com/ghga-de/ghga-service-commons/actions/workflows/unit_and_int_tests.yaml/badge.svg)
+![tests](https://github.com/ghga-de/ghga-service-commons/actions/workflows/tests.yaml/badge.svg)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/ghga_service_commons.svg)](https://pypi.python.org/pypi/ghga_service_commons/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ghga_service_commons.svg)](https://pypi.python.org/pypi/ghga_service_commons/)
-[![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga_service_commons/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga_service_commons?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga-service-commons/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga-service-commons?branch=main)
 
 # ghga-service-commons
 This Python library serves as a collection of common utilities used by
 the microservices developed at German Human Genome-Phenome Archive (GHGA).
 
 It collects boilerplate code for common functionalities such as API server setup,
 authentication and authorization.
```

### Comparing `ghga_service_commons-3.1.2/pyproject.toml` & `ghga_service_commons-3.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "ghga_service_commons"
-version = "3.1.2"
+version = "3.1.3"
 description = "A library that contains common functionality used in services of GHGA"
 dependencies = [
     "pydantic >=2, <3",
 ]
 
 [project.license]
 text = "Apache 2.0"
@@ -160,7 +161,10 @@
 warn_unused_ignores = true
 check_untyped_defs = true
 no_site_packages = false
 
 [tool.pytest.ini_options]
 minversion = "8.0"
 asyncio_mode = "strict"
+
+[tool.tox]
+legacy_tox_ini = "    [tox]\n    env_list = py3{9,12}\n\n    [gh-actions]\n    python =\n        3.9: py39\n        3.10: py310\n        3.11: py311\n        3.12: py312\n\n    [testenv]\n    pass_env =\n        TC_HOST\n        DOCKER_HOST\n    deps =\n        --no-deps -r ./lock/requirements-dev.txt\n    commands = pytest {posargs}\n"
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/__init__.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/__main__.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/api/__init__.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/api/api.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/api/di.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/api/di.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/api/mock_router.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/api/mock_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/api/testing.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/api/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/auth/__init__.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/auth/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/auth/context.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/auth/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/auth/ghga.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/auth/ghga.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/auth/jwt_auth.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/auth/jwt_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/auth/policies.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/auth/policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/__init__.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/base_exception.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/base_exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/__init__.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/custom_types.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/client/custom_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/exceptions.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/mapping.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/client/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/translator.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/client/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/models.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/__init__.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/exceptions.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/server/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/handlers/__init__.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/server/handlers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/handlers/fastapi_.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/server/handlers/fastapi_.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/validation.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/httpyexpect/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/__init__.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/context.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/utils/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/crypt.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/utils/crypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/crypt4gh.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/utils/crypt4gh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/files.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/utils/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/jwt_helpers.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/utils/jwt_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/multinode_storage.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/utils/multinode_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/simple_token.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/utils/simple_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/temp_files.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/utils/temp_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/utc_dates.py` & `ghga_service_commons-3.1.3/src/ghga_service_commons/utils/utc_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/PKG-INFO` & `ghga_service_commons-3.1.3/src/ghga_service_commons.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: ghga_service_commons
-Version: 3.1.2
+Version: 3.1.3
 Summary: A library that contains common functionality used in services of GHGA
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/ghga-service-commons
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,18 +32,18 @@
 Provides-Extra: dev
 Requires-Dist: requests<3,>=2.31; extra == "dev"
 Provides-Extra: objectstorage
 Requires-Dist: hexkit<4,>=2; extra == "objectstorage"
 Provides-Extra: all
 Requires-Dist: ghga-service-commons[api,auth,crypt,dev,objectstorage]; extra == "all"
 
-![tests](https://github.com/ghga-de/ghga-service-commons/actions/workflows/unit_and_int_tests.yaml/badge.svg)
+![tests](https://github.com/ghga-de/ghga-service-commons/actions/workflows/tests.yaml/badge.svg)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/ghga_service_commons.svg)](https://pypi.python.org/pypi/ghga_service_commons/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ghga_service_commons.svg)](https://pypi.python.org/pypi/ghga_service_commons/)
-[![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga_service_commons/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga_service_commons?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga-service-commons/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga-service-commons?branch=main)
 
 # ghga-service-commons
 This Python library serves as a collection of common utilities used by
 the microservices developed at German Human Genome-Phenome Archive (GHGA).
 
 It collects boilerplate code for common functionalities such as API server setup,
 authentication and authorization.
```

### Comparing `ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/SOURCES.txt` & `ghga_service_commons-3.1.3/src/ghga_service_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

