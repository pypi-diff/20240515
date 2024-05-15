# Comparing `tmp/geodefi-2.0.0.tar.gz` & `tmp/geodefi-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodefi-2.0.0.tar", last modified: Tue Mar  5 11:21:44 2024, max compression
+gzip compressed data, was "geodefi-2.0.1.tar", last modified: Fri Mar  8 21:28:29 2024, max compression
```

## Comparing `geodefi-2.0.0.tar` & `geodefi-2.0.1.tar`

### file list

```diff
@@ -1,64 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:21:44.184340 geodefi-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-05 11:21:35.000000 geodefi-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-05 11:21:35.000000 geodefi-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-03-05 11:21:44.184340 geodefi-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-03-05 11:21:35.000000 geodefi-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:21:44.176340 geodefi-2.0.0/geodefi/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:21:44.176340 geodefi-2.0.0/geodefi/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/classes/beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/classes/id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/classes/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/classes/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/classes/portal.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/classes/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/classes/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:21:44.180340 geodefi-2.0.0/geodefi/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/exceptions/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/geodefi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:21:44.180340 geodefi-2.0.0/geodefi/globals/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/globals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/globals/beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/globals/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/globals/id.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/globals/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/globals/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/globals/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:21:44.180340 geodefi-2.0.0/geodefi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/abi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:21:44.184340 geodefi-2.0.0/geodefi/utils/bls/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/bls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/bls/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/bls/keystore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/bls/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/bls/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/bls/staking_deposit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/bls/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/id.py
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/merkle.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/solidity.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-05 11:21:35.000000 geodefi-2.0.0/geodefi/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:21:44.184340 geodefi-2.0.0/geodefi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-03-05 11:21:44.000000 geodefi-2.0.0/geodefi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-05 11:21:44.000000 geodefi-2.0.0/geodefi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 11:21:44.000000 geodefi-2.0.0/geodefi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 11:21:44.000000 geodefi-2.0.0/geodefi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 11:21:44.000000 geodefi-2.0.0/geodefi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-05 11:21:44.000000 geodefi-2.0.0/geodefi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-05 11:21:44.184340 geodefi-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-05 11:21:35.000000 geodefi-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:21:44.184340 geodefi-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-05 11:21:35.000000 geodefi-2.0.0/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-03-05 11:21:35.000000 geodefi-2.0.0/tests/test_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    22101 2024-03-05 11:21:35.000000 geodefi-2.0.0/tests/test_merkle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-05 11:21:35.000000 geodefi-2.0.0/tests/test_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-03-05 11:21:35.000000 geodefi-2.0.0/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-03-05 11:21:35.000000 geodefi-2.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-05 11:21:35.000000 geodefi-2.0.0/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-03-05 11:21:35.000000 geodefi-2.0.0/tests/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-05 11:21:35.000000 geodefi-2.0.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.253625 geodefi-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-08 21:28:20.000000 geodefi-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-08 21:28:20.000000 geodefi-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-03-08 21:28:29.253625 geodefi-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-03-08 21:28:20.000000 geodefi-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.237625 geodefi-2.0.1/geodefi/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.237625 geodefi-2.0.1/geodefi/abis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.237625 geodefi-2.0.1/geodefi/abis/holesky/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.241625 geodefi-2.0.1/geodefi/abis/holesky/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)   102007 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/abis/holesky/middleware/ERC20Middleware.json
+-rw-r--r--   0 runner    (1001) docker     (127)   176454 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/abis/holesky/middleware/ERC20PermitMiddleware.json
+-rw-r--r--   0 runner    (1001) docker     (127)   104213 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/abis/holesky/middleware/ERC20RebaseMiddleware.json
+-rw-r--r--   0 runner    (1001) docker     (127)   179192 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/abis/holesky/middleware/ERC20RebasePermitMiddleware.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.241625 geodefi-2.0.1/geodefi/abis/holesky/package/
+-rw-r--r--   0 runner    (1001) docker     (127)    89480 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/abis/holesky/package/Portal.json
+-rw-r--r--   0 runner    (1001) docker     (127)   358960 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/abis/holesky/package/WithdrawalContract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.241625 geodefi-2.0.1/geodefi/abis/holesky/token/
+-rw-r--r--   0 runner    (1001) docker     (127)   228056 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/abis/holesky/token/gETH.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.245625 geodefi-2.0.1/geodefi/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/classes/beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/classes/id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/classes/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/classes/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/classes/portal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/classes/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/classes/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.245625 geodefi-2.0.1/geodefi/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/exceptions/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/geodefi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.245625 geodefi-2.0.1/geodefi/globals/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/globals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/globals/beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/globals/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/globals/id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/globals/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/globals/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/globals/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.249625 geodefi-2.0.1/geodefi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/abi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.249625 geodefi-2.0.1/geodefi/utils/bls/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/bls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/bls/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/bls/keystore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/bls/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/bls/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/bls/staking_deposit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/bls/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/merkle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/solidity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-08 21:28:20.000000 geodefi-2.0.1/geodefi/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.253625 geodefi-2.0.1/geodefi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-03-08 21:28:29.000000 geodefi-2.0.1/geodefi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-08 21:28:29.000000 geodefi-2.0.1/geodefi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 21:28:29.000000 geodefi-2.0.1/geodefi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 21:28:29.000000 geodefi-2.0.1/geodefi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 21:28:29.000000 geodefi-2.0.1/geodefi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-08 21:28:29.000000 geodefi-2.0.1/geodefi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-08 21:28:29.253625 geodefi-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-08 21:28:20.000000 geodefi-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:28:29.249625 geodefi-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-08 21:28:20.000000 geodefi-2.0.1/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-03-08 21:28:20.000000 geodefi-2.0.1/tests/test_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22101 2024-03-08 21:28:20.000000 geodefi-2.0.1/tests/test_merkle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-08 21:28:20.000000 geodefi-2.0.1/tests/test_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-03-08 21:28:20.000000 geodefi-2.0.1/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-03-08 21:28:20.000000 geodefi-2.0.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-08 21:28:20.000000 geodefi-2.0.1/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-03-08 21:28:20.000000 geodefi-2.0.1/tests/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-08 21:28:20.000000 geodefi-2.0.1/tests/test_version.py
```

### Comparing `geodefi-2.0.0/LICENSE` & `geodefi-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/PKG-INFO` & `geodefi-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodefi
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python SDK for Geodefi Ecosystem
 Home-page: https://www.geode.fi/
 Author: IceBear
 Author-email: admin@geode.fi
 License: MIT
 Keywords: ethereum,geode,web3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,21 +16,21 @@
 License-File: LICENSE
 Requires-Dist: web3==6.10.0
 Requires-Dist: py_ecc==6.0.0
 Requires-Dist: ssz==0.3.1
 
 # geodefi
 
-**geodefi**  is a Python library for interacting with `geode.fi <https://www.geode.fi>`_ smart contract infrastructure.
+**geodefi**  is a Python library for interacting with [geode.fi](https://www.geode.fi) smart contract infrastructure.
 
-`geode.fi <https://www.geode.fi>`_ is an open source **Decentralized Infrastructure Provider** aiming to create a secure closed-environment for the wider Decentralized Finance landscape.
+[geode.fi](https://www.geode.fi) an open source **Decentralized Infrastructure Provider** aiming to create a secure closed-environment for the wider Decentralized Finance landscape.
 Currently providing a set of smart contracts which allows anyone to create their own Staking Pool on Ethereum.
 Soon, much more.
 
-Built on top of `web3.py <https://web3py.readthedocs.io/en/stable/>`_, Geodefi offers a comprehensive set of functions and utilities that simplify the process of interacting with the protocol's smart contract infrastructure.
+Built on top of [web3.py](https://web3py.readthedocs.io/en/stable) Geodefi offers a comprehensive set of functions and utilities that simplify the process of interacting with the protocol's smart contract infrastructure.
 
 Whether you're looking to query contract data or execute transactions, **geodefi** Python SDK has you covered! With a user-friendly and highly efficient interface, this SDK also provides cool features such as built-in cache, easy wallet management etc.
 
 ## Features
 
 - Supports Ethereum Holesky testnet (as of v2.0.0) where The Protocol is deployed.
 - Provides a simple and intuitive API for managing validators, operators, pools, tokens, and other smart contracts/packages.
```

### Comparing `geodefi-2.0.0/README.md` & `geodefi-2.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # geodefi
 
-**geodefi**  is a Python library for interacting with `geode.fi <https://www.geode.fi>`_ smart contract infrastructure.
+**geodefi**  is a Python library for interacting with [geode.fi](https://www.geode.fi) smart contract infrastructure.
 
-`geode.fi <https://www.geode.fi>`_ is an open source **Decentralized Infrastructure Provider** aiming to create a secure closed-environment for the wider Decentralized Finance landscape.
+[geode.fi](https://www.geode.fi) an open source **Decentralized Infrastructure Provider** aiming to create a secure closed-environment for the wider Decentralized Finance landscape.
 Currently providing a set of smart contracts which allows anyone to create their own Staking Pool on Ethereum.
 Soon, much more.
 
-Built on top of `web3.py <https://web3py.readthedocs.io/en/stable/>`_, Geodefi offers a comprehensive set of functions and utilities that simplify the process of interacting with the protocol's smart contract infrastructure.
+Built on top of [web3.py](https://web3py.readthedocs.io/en/stable) Geodefi offers a comprehensive set of functions and utilities that simplify the process of interacting with the protocol's smart contract infrastructure.
 
 Whether you're looking to query contract data or execute transactions, **geodefi** Python SDK has you covered! With a user-friendly and highly efficient interface, this SDK also provides cool features such as built-in cache, easy wallet management etc.
 
 ## Features
 
 - Supports Ethereum Holesky testnet (as of v2.0.0) where The Protocol is deployed.
 - Provides a simple and intuitive API for managing validators, operators, pools, tokens, and other smart contracts/packages.
```

### Comparing `geodefi-2.0.0/geodefi/classes/beacon.py` & `geodefi-2.0.1/geodefi/classes/beacon.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/classes/id.py` & `geodefi-2.0.1/geodefi/classes/id.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/classes/operator.py` & `geodefi-2.0.1/geodefi/classes/operator.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/classes/pool.py` & `geodefi-2.0.1/geodefi/classes/pool.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/classes/portal.py` & `geodefi-2.0.1/geodefi/classes/portal.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/classes/token.py` & `geodefi-2.0.1/geodefi/classes/token.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/classes/validator.py` & `geodefi-2.0.1/geodefi/classes/validator.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/exceptions/main.py` & `geodefi-2.0.1/geodefi/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/geodefi.py` & `geodefi-2.0.1/geodefi/geodefi.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/globals/beacon.py` & `geodefi-2.0.1/geodefi/globals/beacon.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/globals/constants.py` & `geodefi-2.0.1/geodefi/globals/constants.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/globals/validator.py` & `geodefi-2.0.1/geodefi/globals/validator.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/utils/abi.py` & `geodefi-2.0.1/geodefi/utils/abi.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/utils/bls/crypto.py` & `geodefi-2.0.1/geodefi/utils/bls/crypto.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/utils/bls/keystore.py` & `geodefi-2.0.1/geodefi/utils/bls/keystore.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/utils/bls/main.py` & `geodefi-2.0.1/geodefi/utils/bls/main.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/utils/bls/serialize.py` & `geodefi-2.0.1/geodefi/utils/bls/serialize.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/utils/bls/staking_deposit.py` & `geodefi-2.0.1/geodefi/utils/bls/staking_deposit.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/utils/bls/validate.py` & `geodefi-2.0.1/geodefi/utils/bls/validate.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/utils/id.py` & `geodefi-2.0.1/geodefi/utils/id.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/utils/merkle.py` & `geodefi-2.0.1/geodefi/utils/merkle.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi/utils/wrappers.py` & `geodefi-2.0.1/geodefi/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/geodefi.egg-info/PKG-INFO` & `geodefi-2.0.1/geodefi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodefi
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python SDK for Geodefi Ecosystem
 Home-page: https://www.geode.fi/
 Author: IceBear
 Author-email: admin@geode.fi
 License: MIT
 Keywords: ethereum,geode,web3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,21 +16,21 @@
 License-File: LICENSE
 Requires-Dist: web3==6.10.0
 Requires-Dist: py_ecc==6.0.0
 Requires-Dist: ssz==0.3.1
 
 # geodefi
 
-**geodefi**  is a Python library for interacting with `geode.fi <https://www.geode.fi>`_ smart contract infrastructure.
+**geodefi**  is a Python library for interacting with [geode.fi](https://www.geode.fi) smart contract infrastructure.
 
-`geode.fi <https://www.geode.fi>`_ is an open source **Decentralized Infrastructure Provider** aiming to create a secure closed-environment for the wider Decentralized Finance landscape.
+[geode.fi](https://www.geode.fi) an open source **Decentralized Infrastructure Provider** aiming to create a secure closed-environment for the wider Decentralized Finance landscape.
 Currently providing a set of smart contracts which allows anyone to create their own Staking Pool on Ethereum.
 Soon, much more.
 
-Built on top of `web3.py <https://web3py.readthedocs.io/en/stable/>`_, Geodefi offers a comprehensive set of functions and utilities that simplify the process of interacting with the protocol's smart contract infrastructure.
+Built on top of [web3.py](https://web3py.readthedocs.io/en/stable) Geodefi offers a comprehensive set of functions and utilities that simplify the process of interacting with the protocol's smart contract infrastructure.
 
 Whether you're looking to query contract data or execute transactions, **geodefi** Python SDK has you covered! With a user-friendly and highly efficient interface, this SDK also provides cool features such as built-in cache, easy wallet management etc.
 
 ## Features
 
 - Supports Ethereum Holesky testnet (as of v2.0.0) where The Protocol is deployed.
 - Provides a simple and intuitive API for managing validators, operators, pools, tokens, and other smart contracts/packages.
```

### Comparing `geodefi-2.0.0/setup.cfg` & `geodefi-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/tests/test_crypto.py` & `geodefi-2.0.1/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/tests/test_id.py` & `geodefi-2.0.1/tests/test_id.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/tests/test_merkle.py` & `geodefi-2.0.1/tests/test_merkle.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/tests/test_operator.py` & `geodefi-2.0.1/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/tests/test_pool.py` & `geodefi-2.0.1/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/tests/test_utils.py` & `geodefi-2.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/tests/test_validate.py` & `geodefi-2.0.1/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/tests/test_validator.py` & `geodefi-2.0.1/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `geodefi-2.0.0/tests/test_version.py` & `geodefi-2.0.1/tests/test_version.py`

 * *Files identical despite different names*

