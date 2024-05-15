# Comparing `tmp/libem-0.0.6.tar.gz` & `tmp/libem-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libem-0.0.6.tar", last modified: Fri May 10 00:29:05 2024, max compression
+gzip compressed data, was "libem-0.0.7.tar", last modified: Wed May 15 18:52:16 2024, max compression
```

## Comparing `libem-0.0.6.tar` & `libem-0.0.7.tar`

### file list

```diff
@@ -1,80 +1,83 @@
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.144738 libem-0.0.6/
--rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.6/LICENSE
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-10 00:29:05.144613 libem-0.0.6/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)     1343 2024-05-09 21:01:57.000000 libem-0.0.6/README.md
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.133544 libem-0.0.6/cli/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-05 16:25:37.000000 libem-0.0.6/cli/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1367 2024-05-09 01:15:34.000000 libem-0.0.6/cli/libem
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.134961 libem-0.0.6/libem/
--rw-r--r--   0 silv       (501) staff       (20)      347 2024-05-09 21:43:35.000000 libem-0.0.6/libem/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.136252 libem-0.0.6/libem/browse/
--rw-r--r--   0 silv       (501) staff       (20)       92 2024-05-05 00:16:54.000000 libem-0.0.6/libem/browse/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1623 2024-05-09 00:19:21.000000 libem-0.0.6/libem/browse/function.py
--rw-r--r--   0 silv       (501) staff       (20)       85 2024-05-05 01:29:22.000000 libem-0.0.6/libem/browse/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)      318 2024-05-09 21:57:54.000000 libem-0.0.6/libem/browse/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.136934 libem-0.0.6/libem/calibrate/
--rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-09 20:29:02.000000 libem-0.0.6/libem/calibrate/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     4420 2024-05-09 22:17:00.000000 libem-0.0.6/libem/calibrate/function.py
--rw-r--r--   0 silv       (501) staff       (20)      436 2024-05-09 22:15:40.000000 libem-0.0.6/libem/calibrate/interface.py
--rw-r--r--   0 silv       (501) staff       (20)      751 2024-05-09 16:23:53.000000 libem-0.0.6/libem/constant.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.138641 libem-0.0.6/libem/core/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.6/libem/core/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     3823 2024-05-08 06:37:24.000000 libem-0.0.6/libem/core/eval.py
--rw-r--r--   0 silv       (501) staff       (20)     3784 2024-05-09 16:55:50.000000 libem-0.0.6/libem/core/log.py
--rw-r--r--   0 silv       (501) staff       (20)     3216 2024-05-09 03:20:14.000000 libem-0.0.6/libem/core/model.py
--rw-r--r--   0 silv       (501) staff       (20)     4989 2024-05-09 23:45:31.000000 libem-0.0.6/libem/core/struct.py
--rw-r--r--   0 silv       (501) staff       (20)      907 2024-05-09 16:10:45.000000 libem-0.0.6/libem/core/telemetry.py
--rw-r--r--   0 silv       (501) staff       (20)     1098 2024-05-08 21:50:28.000000 libem-0.0.6/libem/core/trace.py
--rw-r--r--   0 silv       (501) staff       (20)     1020 2024-05-09 21:08:05.000000 libem-0.0.6/libem/core/util.py
--rw-r--r--   0 silv       (501) staff       (20)       35 2024-05-07 06:37:47.000000 libem-0.0.6/libem/function.py
--rw-r--r--   0 silv       (501) staff       (20)      936 2024-05-09 21:46:11.000000 libem-0.0.6/libem/interface.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.139469 libem-0.0.6/libem/match/
--rw-r--r--   0 silv       (501) staff       (20)       90 2024-05-05 00:16:44.000000 libem-0.0.6/libem/match/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1473 2024-05-09 18:24:22.000000 libem-0.0.6/libem/match/function.py
--rw-r--r--   0 silv       (501) staff       (20)      197 2024-05-07 17:01:12.000000 libem-0.0.6/libem/match/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)      613 2024-05-09 22:52:49.000000 libem-0.0.6/libem/match/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      216 2024-05-07 06:42:34.000000 libem-0.0.6/libem/parameter.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.140217 libem-0.0.6/libem/prepare/
--rw-r--r--   0 silv       (501) staff       (20)       94 2024-05-05 04:43:06.000000 libem-0.0.6/libem/prepare/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.141361 libem-0.0.6/libem/prepare/datasets/
--rw-r--r--   0 silv       (501) staff       (20)      134 2024-05-09 00:08:47.000000 libem-0.0.6/libem/prepare/datasets/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     2954 2024-05-09 00:05:08.000000 libem-0.0.6/libem/prepare/datasets/abt_buy.py
--rw-r--r--   0 silv       (501) staff       (20)     2698 2024-05-09 00:06:05.000000 libem-0.0.6/libem/prepare/datasets/amazon_google.py
--rw-r--r--   0 silv       (501) staff       (20)     2763 2024-05-09 00:08:08.000000 libem-0.0.6/libem/prepare/datasets/dblp_acm.py
--rw-r--r--   0 silv       (501) staff       (20)     2760 2024-05-09 00:08:21.000000 libem-0.0.6/libem/prepare/datasets/dblp_scholar.py
--rw-r--r--   0 silv       (501) staff       (20)     2792 2024-05-09 00:08:37.000000 libem-0.0.6/libem/prepare/datasets/walmart_amazon.py
--rw-r--r--   0 silv       (501) staff       (20)       72 2024-05-08 23:56:27.000000 libem-0.0.6/libem/prepare/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.6/libem/prepare/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 00:06:37.000000 libem-0.0.6/libem/prepare/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-07 15:43:38.000000 libem-0.0.6/libem/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.142178 libem-0.0.6/libem/tune/
--rw-r--r--   0 silv       (501) staff       (20)      129 2024-05-08 00:48:47.000000 libem-0.0.6/libem/tune/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:18:54.000000 libem-0.0.6/libem/tune/function.py
--rw-r--r--   0 silv       (501) staff       (20)      224 2024-05-09 21:34:22.000000 libem-0.0.6/libem/tune/interface.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.142885 libem-0.0.6/libem/tune/learn/
--rw-r--r--   0 silv       (501) staff       (20)      110 2024-05-07 23:38:41.000000 libem-0.0.6/libem/tune/learn/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     2946 2024-05-09 23:25:30.000000 libem-0.0.6/libem/tune/learn/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-08 23:52:04.000000 libem-0.0.6/libem/tune/learn/interface.py
--rw-r--r--   0 silv       (501) staff       (20)      131 2024-05-09 06:30:44.000000 libem-0.0.6/libem/tune/learn/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)      730 2024-05-09 23:34:00.000000 libem-0.0.6/libem/tune/learn/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.143293 libem-0.0.6/libem/tune/load/
--rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.6/libem/tune/load/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:05.000000 libem-0.0.6/libem/tune/load/function.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.143699 libem-0.0.6/libem/tune/save/
--rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.6/libem/tune/save/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:04.000000 libem-0.0.6/libem/tune/save/function.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.144108 libem-0.0.6/libem/tune/search/
--rw-r--r--   0 silv       (501) staff       (20)       97 2024-05-07 06:21:06.000000 libem-0.0.6/libem/tune/search/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-07 06:36:20.000000 libem-0.0.6/libem/tune/search/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-07 06:26:56.000000 libem-0.0.6/libem/tune/storage.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.135511 libem-0.0.6/libem.egg-info/
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-10 00:29:05.000000 libem-0.0.6/libem.egg-info/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)     1514 2024-05-10 00:29:05.000000 libem-0.0.6/libem.egg-info/SOURCES.txt
--rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-10 00:29:05.000000 libem-0.0.6/libem.egg-info/dependency_links.txt
--rw-r--r--   0 silv       (501) staff       (20)      133 2024-05-10 00:29:05.000000 libem-0.0.6/libem.egg-info/requires.txt
--rw-r--r--   0 silv       (501) staff       (20)       16 2024-05-10 00:29:05.000000 libem-0.0.6/libem.egg-info/top_level.txt
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-10 00:29:05.144366 libem-0.0.6/serve/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-04 23:17:56.000000 libem-0.0.6/serve/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      578 2024-05-04 23:21:19.000000 libem-0.0.6/serve/run.py
--rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-10 00:29:05.144770 libem-0.0.6/setup.cfg
--rw-r--r--   0 silv       (501) staff       (20)      449 2024-05-10 00:29:00.000000 libem-0.0.6/setup.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.060260 libem-0.0.7/
+-rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.7/LICENSE
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-15 18:52:16.060141 libem-0.0.7/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)     1343 2024-05-09 21:01:57.000000 libem-0.0.7/README.md
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.047972 libem-0.0.7/cli/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-05 16:25:37.000000 libem-0.0.7/cli/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1366 2024-05-14 01:22:05.000000 libem-0.0.7/cli/libem
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.049429 libem-0.0.7/libem/
+-rw-r--r--   0 silv       (501) staff       (20)      382 2024-05-14 16:05:14.000000 libem-0.0.7/libem/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.050907 libem-0.0.7/libem/browse/
+-rw-r--r--   0 silv       (501) staff       (20)       92 2024-05-05 00:16:54.000000 libem-0.0.7/libem/browse/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     3406 2024-05-14 16:05:14.000000 libem-0.0.7/libem/browse/function.py
+-rw-r--r--   0 silv       (501) staff       (20)       99 2024-05-15 18:04:36.000000 libem-0.0.7/libem/browse/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      318 2024-05-09 21:57:54.000000 libem-0.0.7/libem/browse/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.051568 libem-0.0.7/libem/calibrate/
+-rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-09 20:29:02.000000 libem-0.0.7/libem/calibrate/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     4420 2024-05-09 22:17:00.000000 libem-0.0.7/libem/calibrate/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      436 2024-05-09 22:15:40.000000 libem-0.0.7/libem/calibrate/interface.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.051859 libem-0.0.7/libem/calibrate/optimize/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-12 21:34:51.000000 libem-0.0.7/libem/calibrate/optimize/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      851 2024-05-14 16:08:26.000000 libem-0.0.7/libem/constant.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.053773 libem-0.0.7/libem/core/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.7/libem/core/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     3823 2024-05-08 06:37:24.000000 libem-0.0.7/libem/core/eval.py
+-rw-r--r--   0 silv       (501) staff       (20)      159 2024-05-14 16:05:14.000000 libem-0.0.7/libem/core/exception.py
+-rw-r--r--   0 silv       (501) staff       (20)     3779 2024-05-14 16:05:14.000000 libem-0.0.7/libem/core/log.py
+-rw-r--r--   0 silv       (501) staff       (20)     4455 2024-05-14 16:16:25.000000 libem-0.0.7/libem/core/model.py
+-rw-r--r--   0 silv       (501) staff       (20)     5185 2024-05-15 18:04:10.000000 libem-0.0.7/libem/core/struct.py
+-rw-r--r--   0 silv       (501) staff       (20)      911 2024-05-15 18:14:15.000000 libem-0.0.7/libem/core/telemetry.py
+-rw-r--r--   0 silv       (501) staff       (20)     1098 2024-05-08 21:50:28.000000 libem-0.0.7/libem/core/trace.py
+-rw-r--r--   0 silv       (501) staff       (20)     1020 2024-05-09 21:08:05.000000 libem-0.0.7/libem/core/util.py
+-rw-r--r--   0 silv       (501) staff       (20)       35 2024-05-07 06:37:47.000000 libem-0.0.7/libem/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      973 2024-05-14 16:15:38.000000 libem-0.0.7/libem/interface.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.054655 libem-0.0.7/libem/match/
+-rw-r--r--   0 silv       (501) staff       (20)       90 2024-05-05 00:16:44.000000 libem-0.0.7/libem/match/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1666 2024-05-15 18:17:15.000000 libem-0.0.7/libem/match/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      211 2024-05-15 18:00:54.000000 libem-0.0.7/libem/match/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      668 2024-05-15 17:54:20.000000 libem-0.0.7/libem/match/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-14 16:07:48.000000 libem-0.0.7/libem/parameter.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.055322 libem-0.0.7/libem/prepare/
+-rw-r--r--   0 silv       (501) staff       (20)       94 2024-05-05 04:43:06.000000 libem-0.0.7/libem/prepare/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.056686 libem-0.0.7/libem/prepare/datasets/
+-rw-r--r--   0 silv       (501) staff       (20)      134 2024-05-09 00:08:47.000000 libem-0.0.7/libem/prepare/datasets/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     2954 2024-05-09 00:05:08.000000 libem-0.0.7/libem/prepare/datasets/abt_buy.py
+-rw-r--r--   0 silv       (501) staff       (20)     2698 2024-05-09 00:06:05.000000 libem-0.0.7/libem/prepare/datasets/amazon_google.py
+-rw-r--r--   0 silv       (501) staff       (20)     2764 2024-05-14 16:05:14.000000 libem-0.0.7/libem/prepare/datasets/dblp_acm.py
+-rw-r--r--   0 silv       (501) staff       (20)     2760 2024-05-09 00:08:21.000000 libem-0.0.7/libem/prepare/datasets/dblp_scholar.py
+-rw-r--r--   0 silv       (501) staff       (20)     2792 2024-05-09 00:08:37.000000 libem-0.0.7/libem/prepare/datasets/walmart_amazon.py
+-rw-r--r--   0 silv       (501) staff       (20)       72 2024-05-08 23:56:27.000000 libem-0.0.7/libem/prepare/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.7/libem/prepare/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 00:06:37.000000 libem-0.0.7/libem/prepare/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-07 15:43:38.000000 libem-0.0.7/libem/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.057504 libem-0.0.7/libem/tune/
+-rw-r--r--   0 silv       (501) staff       (20)      129 2024-05-08 00:48:47.000000 libem-0.0.7/libem/tune/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       31 2024-05-14 16:19:43.000000 libem-0.0.7/libem/tune/catalog.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:18:54.000000 libem-0.0.7/libem/tune/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      224 2024-05-09 21:34:22.000000 libem-0.0.7/libem/tune/interface.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.058463 libem-0.0.7/libem/tune/learn/
+-rw-r--r--   0 silv       (501) staff       (20)      110 2024-05-07 23:38:41.000000 libem-0.0.7/libem/tune/learn/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     3022 2024-05-14 16:12:58.000000 libem-0.0.7/libem/tune/learn/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-08 23:52:04.000000 libem-0.0.7/libem/tune/learn/interface.py
+-rw-r--r--   0 silv       (501) staff       (20)      131 2024-05-15 17:57:55.000000 libem-0.0.7/libem/tune/learn/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      730 2024-05-09 23:34:00.000000 libem-0.0.7/libem/tune/learn/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.058857 libem-0.0.7/libem/tune/load/
+-rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.7/libem/tune/load/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:05.000000 libem-0.0.7/libem/tune/load/function.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.059236 libem-0.0.7/libem/tune/save/
+-rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.7/libem/tune/save/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:04.000000 libem-0.0.7/libem/tune/save/function.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.059652 libem-0.0.7/libem/tune/search/
+-rw-r--r--   0 silv       (501) staff       (20)       97 2024-05-07 06:21:06.000000 libem-0.0.7/libem/tune/search/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-07 06:36:20.000000 libem-0.0.7/libem/tune/search/function.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.050106 libem-0.0.7/libem.egg-info/
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-15 18:52:16.000000 libem-0.0.7/libem.egg-info/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)     1575 2024-05-15 18:52:16.000000 libem-0.0.7/libem.egg-info/SOURCES.txt
+-rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-15 18:52:16.000000 libem-0.0.7/libem.egg-info/dependency_links.txt
+-rw-r--r--   0 silv       (501) staff       (20)      137 2024-05-15 18:52:16.000000 libem-0.0.7/libem.egg-info/requires.txt
+-rw-r--r--   0 silv       (501) staff       (20)       16 2024-05-15 18:52:16.000000 libem-0.0.7/libem.egg-info/top_level.txt
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.059903 libem-0.0.7/serve/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-04 23:17:56.000000 libem-0.0.7/serve/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      578 2024-05-04 23:21:19.000000 libem-0.0.7/serve/run.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-15 18:52:16.060291 libem-0.0.7/setup.cfg
+-rw-r--r--   0 silv       (501) staff       (20)      449 2024-05-15 18:52:02.000000 libem-0.0.7/setup.py
```

### Comparing `libem-0.0.6/LICENSE` & `libem-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `libem-0.0.6/README.md` & `libem-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `libem-0.0.6/cli/libem` & `libem-0.0.7/cli/libem`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
     entity1 = args.e1
     entity2 = args.e2
     configs = args.calibrate
     if configs:
         libem.calibrate(dict(configs))
 
-
     result = libem.match(entity1, entity2)
     print("Match result:", result)
 
 
 def parse_key_value_pair(arg_value):
     """ Parse a key-value pair, separated by '=' """
     if '=' not in arg_value:
```

### Comparing `libem-0.0.6/libem/browse/function.py` & `libem-0.0.7/libem/match/function.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,59 @@
-import os
-import json
-
-from langchain_google_community import GoogleSearchAPIWrapper
-from langchain_core.tools import Tool
+import time
 
 import libem
-from libem.browse import prompt
+from libem.match import prompt, parameter
 from libem.core.struct import Prompt
+from libem.core import model
 
 schema = {
     "type": "function",
     "function": {
-        "name": "browse",
-        "description": Prompt.join(
-            prompt.description(), prompt.rule()
-        ),
+        "name": "match",
+        "description": "Perform entity matching given two entity description.",
         "parameters": {
             "type": "object",
             "properties": {
-                "entity": {
+                "left": {
                     "type": "string",
-                    "description": "Entity description",
+                    "description": "Description of the first entity",
+                },
+                "right": {
+                    "type": "string",
+                    "description": "Description of the second entity",
                 },
             },
-            "required": ["entity"],
+            "required": ["left", "right"],
         },
     }
 }
 
 
-def func(entity):
-    return google(entity)
-
+def func(left, right):
+    start = time.time()
+    match_prompt = Prompt.join(
+        prompt.query(
+            left=left,
+            right=right
+        ),
+        prompt.rule(),
+        prompt.experience(),
+        prompt.output(),
+    )
+    model_output = model.call(
+        prompt=match_prompt,
+        tools=parameter.tools(),
+        model=parameter.model(),
+        temperature=parameter.temperature(),
+        seed=libem.LIBEM_SEED,
+    )
+    pred = parse_output(model_output)
+    libem.trace.add({"match": {"left": left, "right": right, "model_output": model_output,
+                               "pred": pred, "prompt": match_prompt,
+                               "latency": time.time() - start}})
+    return pred
 
-""" Google search function """
 
-# Set up environment variables for Google API if they are not already set
-os.environ.setdefault(
-    "GOOGLE_CSE_ID",
-    libem.LIBEM_CONFIG.get("GOOGLE_CSE_ID", "")
-)
-os.environ.setdefault(
-    "GOOGLE_API_KEY",
-    libem.LIBEM_CONFIG.get("GOOGLE_API_KEY", "")
-)
-
-
-def google(entity):
-    # Ensure required environment variables are set
-    if not os.environ.get("GOOGLE_CSE_ID") or not os.environ.get("GOOGLE_API_KEY"):
-        raise EnvironmentError(f"GOOGLE_CSE_ID or GOOGLE_API_KEY is not set. "
-                               f"Check your environment or {libem.LIBEM_CONFIG_FILE}.")
-
-    tool = Tool(
-        name="google_search",
-        description="Search Google and return the first result.",
-        func=GoogleSearchAPIWrapper(k=1).run,
-    )
-    desc = tool.run(entity)
-    return json.dumps(
-        {
-            "Entity description:": desc,
-        })
+def parse_output(output: str) -> str:
+    libem.debug("Match raw output:", output)
+    output = output.split("\n")[-1].lower()
+    return "yes" if "yes" in output else "no"
```

### Comparing `libem-0.0.6/libem/calibrate/function.py` & `libem-0.0.7/libem/calibrate/function.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.6/libem/constant.py` & `libem-0.0.7/libem/constant.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 try:
     with open(LIBEM_CONFIG_FILE, "r") as f:
         LIBEM_CONFIG = yaml.load(f, Loader=yaml.SafeLoader)
 except FileNotFoundError:
     print(f"Config file not found at {LIBEM_CONFIG_FILE}")
     sys.exit(1)
 
-LIBEM_DO_LOG = False
 LIBEM_LOG_DIR = os.path.join(
     os.path.dirname(__file__),
     "..", "logs")
+LIBEM_DO_LOG = bool(int(os.environ.get("LIBEM_DO_LOG", False)))
 # DEBUG: 10, INFO: 20, WARNING: 30, ERROR: 40
 LIBEM_LOG_LEVEL = \
-    os.environ.get("LIBEM_LOG_LEVEL", logging.INFO)
+    int(os.environ.get("LIBEM_LOG_LEVEL", logging.INFO))
 LIBEM_3RD_PARTY_LOG_LEVEL = \
     os.environ.get("LIBEM_3RD_PARTY_LOG_LEVEL", logging.WARNING)
+
+LIBEM_SEED = int(os.environ.get("LIBEM_SEED", 42))
```

### Comparing `libem-0.0.6/libem/core/eval.py` & `libem-0.0.7/libem/core/eval.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.6/libem/core/log.py` & `libem-0.0.7/libem/core/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,48 +6,47 @@
 import libem
 
 logging.basicConfig(level=libem.LIBEM_3RD_PARTY_LOG_LEVEL)
 # logger and log files are lazily initialized
 # when log method is called for the first time
 _logger = None
 
-
 def info(*args, **kwargs):
     if libem.LIBEM_LOG_LEVEL <= logging.INFO:
         print(*args, **kwargs)
 
     if libem.LIBEM_DO_LOG:
-        msg = "".join(map(str, *args))
+        msg = "".join(map(str, args))
         log(msg, typ="info")
 
 
 def debug(*args, **kwargs):
     if libem.LIBEM_LOG_LEVEL <= logging.DEBUG:
         print(*args, **kwargs)
 
     if libem.LIBEM_DO_LOG:
-        msg = " ".join(map(str, *args))
+        msg = " ".join(map(str, args))
         log(msg, typ="debug")
 
 
 def warn(*args, **kwargs):
     if libem.LIBEM_LOG_LEVEL <= logging.WARNING:
         print(*args, **kwargs)
 
-    msg = " ".join(map(str, *args))
+    msg = " ".join(map(str, args))
     if libem.LIBEM_DO_LOG:
         log(msg, typ="warning")
     raise Warning(msg)
 
 
 def error(*args, **kwargs):
     if libem.LIBEM_LOG_LEVEL <= logging.ERROR:
         print(*args, **kwargs)
 
-    msg = " ".join(map(str, *args))
+    msg = " ".join(map(str, args))
     if libem.LIBEM_DO_LOG:
         log(msg, typ="error")
     raise Exception(msg)
 
 
 def log(message, typ="info"):
     global _logger
```

### Comparing `libem-0.0.6/libem/core/struct.py` & `libem-0.0.7/libem/core/struct.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import typing
+import copy
 
 
 class Tunable(abc.ABC):
     @abc.abstractmethod
     def update(self, value):
         pass
 
@@ -57,14 +58,17 @@
                 'value': self.value,
                 'options': self.options,
                 'optimal': self.optimal
             }
         else:
             return self.value
 
+    def copy(self):
+        return copy.deepcopy(self)
+
 
 class Prompt(Parameter):
     class Rule:
         def __init__(self, rules: list[str] = None,
                      intro: str = "Rules to follow:",
                      sep="\n", bullet="-"):
             self.rules = rules or []
@@ -99,14 +103,17 @@
                 self.rules.extend(rule.rules)
             return self
 
         def export(self, *args, **kwargs):
             _, _ = args, kwargs
             return self.__call__()
 
+        def copy(self):
+            return copy.deepcopy(self)
+
     class Experience:
         def __init__(self, mistakes: list[str] = None,
                      intro: str = "Mistakes to avoid:",
                      sep="\n", bullet="-"):
             self.mistakes = mistakes or []
             self.intro = intro
             self.sep = sep
@@ -139,14 +146,17 @@
                 self.mistakes.extend(mistake.miscakes)
             return self
 
         def export(self, *args, **kwargs):
             _, _ = args, kwargs
             return self.__call__()
 
+        def copy(self):
+            return copy.deepcopy(self)
+
     @classmethod
     def join(cls, *prompts, sep="\n"):
         to_join = []
         for prompt in prompts:
             if isinstance(prompt, str):
                 to_join.append(prompt)
             elif isinstance(prompt, (cls.Rule, cls.Experience)):
```

### Comparing `libem-0.0.6/libem/core/telemetry.py` & `libem-0.0.7/libem/core/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def start(self):
         """Starts tracing."""
         self.reset()
         return self
 
     def reset(self):
         self.history.append(self.telemetry)
-        self.trace = []
+        self.telemetry = []
         return self
 
     def stop(self):
         return self
 
     def add(self, report):
         self.telemetry.append(report)
```

### Comparing `libem-0.0.6/libem/core/trace.py` & `libem-0.0.7/libem/core/trace.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.6/libem/core/util.py` & `libem-0.0.7/libem/core/util.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.6/libem/interface.py` & `libem-0.0.7/libem/interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import random
 
+import libem
 import libem.core.model as model
 from libem.core.struct import Prompt
 from libem import prompt, parameter
 
 """Chat access"""
 
 
 def chat(message):
     return model.call(
         prompt=Prompt.join(prompt.role(), message, sep="\n"),
         tools=["libem.match"],
         model=parameter.model(),
         temperature=parameter.temperature(),
+        seed=libem.LIBEM_SEED,
     )
 
 
 """Programmatic access"""
 from libem.match import func as match_func
 from libem.calibrate import func as calibrate_func
 from libem.tune import func as tune_func
 
 
 def match(left, right,
           always=None,
-          guess=False,
-          seed=42) -> str:
+          guess=False) -> str:
     if always is not None:
         return always
 
     if guess:
-        random.seed(seed)
+        random.seed(libem.LIBEM_SEED)
         return random.choice(["yes", "no"])
 
     return match_func(left, right)
 
 
 def calibrate(*args, **kwargs):
     return calibrate_func(*args, **kwargs)
```

### Comparing `libem-0.0.6/libem/prepare/datasets/abt_buy.py` & `libem-0.0.7/libem/prepare/datasets/abt_buy.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.6/libem/prepare/datasets/amazon_google.py` & `libem-0.0.7/libem/prepare/datasets/amazon_google.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.6/libem/prepare/datasets/dblp_acm.py` & `libem-0.0.7/libem/prepare/datasets/dblp_acm.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
               "from the DBLP and ACM digital libraries."
 
 # sample data:
 # {"id_left":"dblp_1835","title_left":"wavelet-based histograms for selectivity estimation","authors_left":"jeffrey scott vitter , yossi matias , min wang","venue_left":"sigmod conference","year_left":1998,"cluster_id_left":2110,
 # "id_right":"acm_184","title_right":"wavelet-based histograms for selectivity estimation","authors_right":"yossi matias , jeffrey scott vitter , min wang","venue_right":"international conference on management of data","year_right":1998,"cluster_id_right":2110,
 # "label":1,"pair_id":"dblp_1835#acm_184"}
 def read(file, schema=True):
-    with open(file) as f:
+    with open(file) as f: 
         for line in f:
             data = json.loads(line.strip())
             parsed_data = {'left': {}, 'right': {}, 'label': data.get('label', None)}
 
             # clean the data
             trim = ["cluster_id_left", "cluster_id_right", "id_left", "id_right"]
             if schema:
```

### Comparing `libem-0.0.6/libem/prepare/datasets/dblp_scholar.py` & `libem-0.0.7/libem/prepare/datasets/dblp_scholar.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.6/libem/prepare/datasets/walmart_amazon.py` & `libem-0.0.7/libem/prepare/datasets/walmart_amazon.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.6/libem/tune/learn/function.py` & `libem-0.0.7/libem/tune/learn/function.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 schema = {}
 
 
 def func(*args, **kwargs):
     return learn(*args, **kwargs)
 
 
-def predict(dataset) -> (list, list, list, list):
+def predict(dataset) -> tuple[list, list, list, list]:
     preds, truths = [], []
     mistakes, successes = [], []
 
     for i, record in enumerate(dataset):
         left, right, truth = record["left"], record["right"], record["label"]
 
         pred = libem.match(left, right)
@@ -38,16 +38,16 @@
         if pred == truth:
             successes.append(outcome)
         else:
             mistakes.append(outcome)
     return preds, truths, mistakes, successes
 
 
-def learn(dataset: list or typing.Iterable,
-          metric: str = "libem.core.eval.f1") -> (float, Prompt.Rule, Prompt.Experience):
+def learn(dataset: list | typing.Iterable,
+          metric: str = "libem.core.eval.f1") -> tuple[float, Prompt.Rule, Prompt.Experience]:
     preds, truths, mistakes, successes = predict(dataset)
     metric_func = libem_util.get_func(metric)
     score = metric_func(preds, truths)
 
     libem.info("Tool: learn - metric:", metric, "score:", score)
 
     # if lots of mistakes, learn from rules
@@ -64,14 +64,15 @@
     message = model.call(
         prompt=Prompt.join(
             prompt.recap_success(successes=successes),
             prompt.gen_rules(),
         ),
         model=parameter.model(),
         temperature=parameter.temperature(),
+        seed=libem.LIBEM_SEED,
         tools=[],
     )
     libem.info("Learned: ", message)
     rules = message.split("\n")
     return Prompt.Rule(rules)
 
 
@@ -80,21 +81,22 @@
     message = model.call(
         prompt=Prompt.join(
             prompt.recap_mistake(mistakes=mistakes),
             prompt.gen_rules(),
         ),
         model=parameter.model(),
         temperature=parameter.temperature(),
+        seed=libem.LIBEM_SEED,
         tools=[],
     )
     libem.info("Learned: ", message)
     mistakes = message.split("\n")
     return Prompt.Experience(mistakes)
 
 
-def check(dataset, metric: str = "libem.core.eval.f1") -> (float, list):
+def check(dataset, metric: str = "libem.core.eval.f1") -> tuple[float, list]:
     preds, truths, mistakes, successes = predict(dataset)
     metric_func = libem_util.get_func(metric)
     score = metric_func(preds, truths)
 
     libem.info("Tool: check - metric:", metric, "score:", score)
     return score, mistakes
```

### Comparing `libem-0.0.6/libem/tune/learn/prompt.py` & `libem-0.0.7/libem/tune/learn/prompt.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.6/libem.egg-info/SOURCES.txt` & `libem-0.0.7/libem.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 libem/browse/__init__.py
 libem/browse/function.py
 libem/browse/parameter.py
 libem/browse/prompt.py
 libem/calibrate/__init__.py
 libem/calibrate/function.py
 libem/calibrate/interface.py
+libem/calibrate/optimize/__init__.py
 libem/core/__init__.py
 libem/core/eval.py
+libem/core/exception.py
 libem/core/log.py
 libem/core/model.py
 libem/core/struct.py
 libem/core/telemetry.py
 libem/core/trace.py
 libem/core/util.py
 libem/match/__init__.py
@@ -40,17 +42,17 @@
 libem/prepare/datasets/__init__.py
 libem/prepare/datasets/abt_buy.py
 libem/prepare/datasets/amazon_google.py
 libem/prepare/datasets/dblp_acm.py
 libem/prepare/datasets/dblp_scholar.py
 libem/prepare/datasets/walmart_amazon.py
 libem/tune/__init__.py
+libem/tune/catalog.py
 libem/tune/function.py
 libem/tune/interface.py
-libem/tune/storage.py
 libem/tune/learn/__init__.py
 libem/tune/learn/function.py
 libem/tune/learn/interface.py
 libem/tune/learn/parameter.py
 libem/tune/learn/prompt.py
 libem/tune/load/__init__.py
 libem/tune/load/function.py
```

### Comparing `libem-0.0.6/serve/run.py` & `libem-0.0.7/serve/run.py`

 * *Files identical despite different names*

