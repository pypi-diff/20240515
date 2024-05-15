# Comparing `tmp/dailycheckin-24.3.7.tar.gz` & `tmp/dailycheckin-24.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/dailycheckin/dailycheckin/dist/.tmp-tbt5tazd/dailycheckin-24.3.7.tar", last modified: Thu Mar  7 07:16:20 2024, max compression
+gzip compressed data, was "/home/runner/work/dailycheckin/dailycheckin/dist/.tmp-z6cpxj_o/dailycheckin-24.5.15.tar", last modified: Wed May 15 01:57:23 2024, max compression
```

## Comparing `dailycheckin-24.3.7.tar` & `dailycheckin-24.5.15.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      299 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       23 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/acfun/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/acfun/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7399 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/acfun/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/aliyun/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/aliyun/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2974 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/aliyun/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/aolaxing/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/aolaxing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3368 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/aolaxing/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/baidu/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/baidu/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2109 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/baidu/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/bilibili/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/bilibili/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16575 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/bilibili/main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2084 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/enshan/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/enshan/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1841 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/enshan/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/imaotai/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/imaotai/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12669 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/imaotai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/iqiyi/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/iqiyi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17634 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/iqiyi/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/kgqq/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/kgqq/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8847 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/kgqq/main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5039 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/mimotion/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/mimotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/mimotion/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/smzdm/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/smzdm/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6895 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/smzdm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/tieba/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/tieba/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4427 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/tieba/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11414 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/utils/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/v2ex/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/v2ex/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3794 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/v2ex/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin/youdao/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/youdao/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2539 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/dailycheckin/youdao/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 07:16:19.000000 dailycheckin-24.3.7/dailycheckin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/dailycheckin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 07:16:20.000000 dailycheckin-24.3.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2195 2024-03-07 07:16:14.000000 dailycheckin-24.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      299 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/acfun/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/acfun/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7399 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/acfun/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/aliyun/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/aliyun/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2974 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/aliyun/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/aolaxing/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/aolaxing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3368 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/aolaxing/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/baidu/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/baidu/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2109 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/baidu/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/bilibili/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/bilibili/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16575 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/bilibili/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2084 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/enshan/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/enshan/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1841 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/enshan/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/imaotai/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/imaotai/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12669 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/imaotai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/iqiyi/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/iqiyi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18766 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/iqiyi/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/kgqq/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/kgqq/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8847 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/kgqq/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5039 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/mimotion/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/mimotion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/mimotion/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/smzdm/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/smzdm/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6895 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/smzdm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/tieba/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/tieba/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4427 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/tieba/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11608 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/utils/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/v2ex/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/v2ex/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3794 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/v2ex/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin/youdao/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/youdao/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2539 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/dailycheckin/youdao/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/dailycheckin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 01:57:23.000000 dailycheckin-24.5.15/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2195 2024-05-15 01:57:20.000000 dailycheckin-24.5.15/setup.py
```

### Comparing `dailycheckin-24.3.7/LICENSE` & `dailycheckin-24.5.15/LICENSE`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/PKG-INFO` & `dailycheckin-24.5.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dailycheckin
-Version: 24.3.7
+Version: 24.5.15
 Summary: dailycheckin
 Home-page: https://sitoi.cn
 Author: Sitoi
 Author-email: 133397418@qq.com
 License: MIT
 Project-URL: Documentation, https://sitoi.github.io/dailycheckin/
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dailycheckin-24.3.7/README.md` & `dailycheckin-24.5.15/README.md`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/acfun/main.py` & `dailycheckin-24.5.15/dailycheckin/acfun/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/aliyun/main.py` & `dailycheckin-24.5.15/dailycheckin/aliyun/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/aolaxing/main.py` & `dailycheckin-24.5.15/dailycheckin/aolaxing/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/baidu/main.py` & `dailycheckin-24.5.15/dailycheckin/baidu/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/bilibili/main.py` & `dailycheckin-24.5.15/dailycheckin/bilibili/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/configs.py` & `dailycheckin-24.5.15/dailycheckin/configs.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/enshan/main.py` & `dailycheckin-24.5.15/dailycheckin/enshan/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/imaotai/main.py` & `dailycheckin-24.5.15/dailycheckin/imaotai/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,15 @@
                     lng=lng,
                     reserve_rule=reserve_rule,
                 )
                 if max_shop_id == "0":
                     continue
                 reservation_params = self.act_params(max_shop_id, item)
                 reservation_msg = self.reservation(reservation_params)
-                time.sleep(10)
+                time.sleep(20)
                 award_msg = self.getUserEnergyAward()
                 msg.append(reservation_msg)
                 msg.append(award_msg)
         except BaseException as e:
             msg.append(
                 {
                     "name": "申购结果",
```

### Comparing `dailycheckin-24.3.7/dailycheckin/iqiyi/main.py` & `dailycheckin-24.5.15/dailycheckin/iqiyi/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,21 @@
             else ""
         )
         __dfp = (
             re.findall(r"__dfp=(.*?);", cookie)[0]
             if re.findall(r"__dfp=(.*?);", cookie)
             else ""
         )
-        return p00001, p00002, p00003, __dfp
+        __dfp = __dfp.split("@")[0]
+        qyid = (
+            re.findall(r"QC005=(.*?);", cookie)[0]
+            if re.findall(r"QC005=(.*?);", cookie)
+            else ""
+        )
+        return p00001, p00002, p00003, __dfp, qyid
 
     @staticmethod
     def user_information(p00001):
         """
         账号信息查询
         """
         time.sleep(3)
@@ -72,37 +78,55 @@
                 ]
         else:
             msg = [
                 {"name": "账号信息", "value": res.get("msg")},
             ]
         return msg
 
-    def sign(self, p00001, p00003):
+    def k(self, secret_key, data, split="|"):
+        result_string = split.join(f"{key}={data[key]}" for key in sorted(data))
+        return md5((result_string + split + secret_key).encode("utf-8")).hexdigest()
+
+    def sign(self, p00001, p00003, dfp, qyid):
         """
         VIP 签到
         """
-        qyid = uuid4().hex[:16]
         time_stamp = int(time.time() * 1000)
-        data = f"agentType=1|agentversion=1|appKey=basic_pcw|authCookie={p00001}|qyid={qyid}|task_code=natural_month_sign|timestamp={time_stamp}|typeCode=point|userId={p00003}|UKobMjDMsDoScuWOfp6F"
-        sign = md5(data.encode(encoding="utf-8")).hexdigest()
-        url = f"https://community.iqiyi.com/openApi/task/execute?agentType=1&agentversion=1&appKey=basic_pcw&authCookie={p00001}&qyid={qyid}&sign={sign}&task_code=natural_month_sign&timestamp={time_stamp}&typeCode=point&userId={p00003}"
-        body = {
+        sign_date = {
+            "agenttype": 20,
+            "agentversion": "15.4.6",
+            "appKey": "lequ_rn",
+            "appver": "15.4.6",
+            "authCookie": p00001,
+            "qyid": qyid,
+            "srcplatform": 20,
+            "task_code": "natural_month_sign",
+            "timestamp": time_stamp,
+            "userId": p00003,
+        }
+        sign = self.k("cRcFakm9KSPSjFEufg3W", sign_date)
+        sign_date["sign"] = sign
+        data = {
             "natural_month_sign": {
+                "verticalCode": "iQIYI",
                 "taskCode": "iQIYI_mofhr",
-                "agentType": 1,
-                "agentversion": 1,
                 "authCookie": p00001,
                 "qyid": qyid,
-                "verticalCode": "iQIYI",
+                "agentType": 20,
+                "agentVersion": "15.4.6",
+                "dfp": dfp,
+                "signFrom": 1,
             }
         }
+        url = "https://community.iqiyi.com/openApi/task/execute"
         res = requests.post(
             url=url,
-            data=json.dumps(body),
-            headers={"Cookie": f"P00001={p00001}", "Content-Type": "application/json"},
+            params=sign_date,
+            data=json.dumps(data),
+            headers={"Content-Type": "application/json"},
         ).json()
         if res["code"] == "A00000":
             _msg = res["data"]["msg"]
             if _msg:
                 msg = [{"name": "签到天数", "value": _msg}]
             else:
                 try:
@@ -183,14 +207,31 @@
     def lottery(self, p00001, award_list=[]):
         url = "https://act.vip.iqiyi.com/shake-api/lottery"
         params = {
             "P00001": p00001,
             "lotteryType": "0",
             "actCode": "0k9GkUcjqqj4tne8",
         }
+        params = {
+            "P00001": p00001,
+            "deviceID": str(uuid4()),
+            "version": "15.3.0",
+            "platform": str(uuid4())[:16],
+            "lotteryType": "0",
+            "actCode": "0k9GkUcjqqj4tne8",
+            "extendParams": json.dumps(
+                {
+                    "appIds": "iqiyi_pt_vip_iphone_video_autorenew_12m_348yuan_v2",
+                    "supportSk2Identity": True,
+                    "testMode": "0",
+                    "iosSystemVersion": "17.4",
+                    "bundleId": "com.qiyi.iphone",
+                }
+            ),
+        }
         res = requests.get(url, params=params).json()
         msgs = []
         if res.get("code") == "A00000":
             award_info = res.get("data", {}).get("title")
             award_list.append(award_info)
             time.sleep(3)
             return self.lottery(p00001=p00001, award_list=award_list)
@@ -386,25 +427,27 @@
                 gift_list.append(gift_name)
         if gift_list:
             return [{"name": "白金抽奖", "value": "、".join(gift_list)}]
         else:
             return [{"name": "白金抽奖", "value": "未中奖"}]
 
     def main(self):
-        p00001, p00002, p00003, dfp = self.parse_cookie(self.check_item.get("cookie"))
+        p00001, p00002, p00003, dfp, qyid = self.parse_cookie(
+            self.check_item.get("cookie")
+        )
         try:
             user_info = json.loads(unquote(p00002, encoding="utf-8"))
             user_name = user_info.get("user_name")
             user_name = user_name.replace(user_name[3:7], "****")
             nickname = user_info.get("nickname")
         except Exception as e:
             print(f"获取账号信息失败，错误信息: {e}")
             nickname = "未获取到，请检查 Cookie 中 P00002 字段"
             user_name = "未获取到，请检查 Cookie 中 P00002 字段"
-        sign_msg = self.sign(p00001=p00001, p00003=p00003)
+        sign_msg = self.sign(p00001=p00001, p00003=p00003, dfp=dfp, qyid=qyid)
         _user_msg = self.user_information(p00001=p00001)
         lotto_lottery_msg = self.lotto_lottery(p00001=p00001)
         if _user_msg[4].get("value") != "非 VIP 用户":
             watch_msg = self.start_watch(p00001=p00001, p00003=p00003, dfp=dfp)
             level_right_msg = self.level_right(p00001=p00001)
         else:
             watch_msg = {"name": "视频时长", "value": "非 VIP 用户"}
```

### Comparing `dailycheckin-24.3.7/dailycheckin/kgqq/main.py` & `dailycheckin-24.5.15/dailycheckin/kgqq/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/main.py` & `dailycheckin-24.5.15/dailycheckin/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/mimotion/main.py` & `dailycheckin-24.5.15/dailycheckin/mimotion/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/smzdm/main.py` & `dailycheckin-24.5.15/dailycheckin/smzdm/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/tieba/main.py` & `dailycheckin-24.5.15/dailycheckin/tieba/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/utils/message.py` & `dailycheckin-24.5.15/dailycheckin/utils/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,19 +119,28 @@
         url=f"https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key={qywx_key}",
         data=json.dumps({"msgtype": "text", "text": {"content": content}}),
     )
     return
 
 
 def message2qywxapp(
-    qywx_corpid, qywx_agentid, qywx_corpsecret, qywx_touser, qywx_media_id, content
+    qywx_corpid,
+    qywx_agentid,
+    qywx_corpsecret,
+    qywx_touser,
+    qywx_media_id,
+    qywx_origin,
+    content,
 ):
     print("企业微信应用消息推送开始")
+    base_url = "https://qyapi.weixin.qq.com"
+    if qywx_origin:
+        base_url = qywx_origin
     res = requests.get(
-        f"https://qyapi.weixin.qq.com/cgi-bin/gettoken?corpid={qywx_corpid}&corpsecret={qywx_corpsecret}"
+        f"{base_url}/cgi-bin/gettoken?corpid={qywx_corpid}&corpsecret={qywx_corpsecret}"
     )
     token = res.json().get("access_token", False)
     if qywx_media_id:
         data = {
             "touser": qywx_touser,
             "msgtype": "mpnews",
             "agentid": int(qywx_agentid),
@@ -157,15 +166,15 @@
                 "title": "Dailycheckin 签到通知",
                 "description": content,
                 "url": "https://github.com/Sitoi/dailycheckin",
                 "btntxt": "开源项目",
             },
         }
     requests.post(
-        url=f"https://qyapi.weixin.qq.com/cgi-bin/message/send?access_token={token}",
+        url=f"{base_url}/cgi-bin/message/send?access_token={token}",
         data=json.dumps(data),
     )
     return
 
 
 def message2pushplus(pushplus_token, content, pushplus_topic=None):
     print("Pushplus 推送开始")
@@ -215,14 +224,15 @@
     coolpushemail = notice_info.get("coolpushemail")
     qywx_key = notice_info.get("qywx_key")
     qywx_corpid = notice_info.get("qywx_corpid")
     qywx_agentid = notice_info.get("qywx_agentid")
     qywx_corpsecret = notice_info.get("qywx_corpsecret")
     qywx_touser = notice_info.get("qywx_touser")
     qywx_media_id = notice_info.get("qywx_media_id")
+    qywx_origin = notice_info.get("qywx_origin")
     pushplus_token = notice_info.get("pushplus_token")
     pushplus_topic = notice_info.get("pushplus_topic")
     merge_push = notice_info.get("merge_push")
     content_str = "\n————————————\n\n".join(content_list)
     message_list = [content_str]
     try:
         notice = important_notice()
@@ -267,14 +277,15 @@
             try:
                 message2qywxapp(
                     qywx_corpid=qywx_corpid,
                     qywx_agentid=qywx_agentid,
                     qywx_corpsecret=qywx_corpsecret,
                     qywx_touser=qywx_touser,
                     qywx_media_id=qywx_media_id,
+                    qywx_origin=qywx_origin,
                     content=message,
                 )
             except Exception as e:
                 print("企业微信应用消息推送失败", e)
         if bark_url:
             try:
                 message2bark(bark_url=bark_url, content=message)
```

### Comparing `dailycheckin-24.3.7/dailycheckin/v2ex/main.py` & `dailycheckin-24.5.15/dailycheckin/v2ex/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin/youdao/main.py` & `dailycheckin-24.5.15/dailycheckin/youdao/main.py`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/dailycheckin.egg-info/PKG-INFO` & `dailycheckin-24.5.15/dailycheckin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dailycheckin
-Version: 24.3.7
+Version: 24.5.15
 Summary: dailycheckin
 Home-page: https://sitoi.cn
 Author: Sitoi
 Author-email: 133397418@qq.com
 License: MIT
 Project-URL: Documentation, https://sitoi.github.io/dailycheckin/
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dailycheckin-24.3.7/dailycheckin.egg-info/SOURCES.txt` & `dailycheckin-24.5.15/dailycheckin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dailycheckin-24.3.7/setup.py` & `dailycheckin-24.5.15/setup.py`

 * *Files identical despite different names*

