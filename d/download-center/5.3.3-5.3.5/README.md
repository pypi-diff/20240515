# Comparing `tmp/download-center-5.3.3.tar.gz` & `tmp/download-center-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/download-center-5.3.3.tar", last modified: Tue Jun  7 06:17:13 2022, max compression
+gzip compressed data, was "download-center-5.3.5.tar", last modified: Tue May 14 08:13:52 2024, max compression
```

## Comparing `download-center-5.3.3.tar` & `download-center-5.3.5.tar`

### file list

```diff
@@ -1,71 +1,80 @@
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.757533 download-center-5.3.3/
--rwxr-xr-x   0 baozhubzhang   (501) staff       (20)       43 2021-12-24 01:52:53.000000 download-center-5.3.3/MANIFEST.in
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     1742 2022-06-07 06:17:13.757302 download-center-5.3.3/PKG-INFO
--rwxr-xr-x   0 baozhubzhang   (501) staff       (20)      854 2022-06-07 06:16:12.000000 download-center-5.3.3/README.md
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.733133 download-center-5.3.3/demo/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)       76 2019-12-09 04:31:05.000000 download-center-5.3.3/demo/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      121 2019-12-09 04:31:05.000000 download-center-5.3.3/demo/config.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.734554 download-center-5.3.3/demo/extractor/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/demo/extractor/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)    13586 2021-10-14 05:09:11.000000 download-center-5.3.3/demo/extractor/baidu_extractor.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     1394 2019-12-09 04:31:05.000000 download-center-5.3.3/demo/extractor/demo_extractor.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.736951 download-center-5.3.3/demo/spider/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/demo/spider/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      898 2021-11-05 06:23:16.000000 download-center-5.3.3/demo/spider/config.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     4321 2022-06-07 05:33:04.000000 download-center-5.3.3/demo/spider/demo_spider.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)    14353 2021-10-23 07:21:27.000000 download-center-5.3.3/demo/spider/get_header_func.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)    12505 2021-11-05 06:29:21.000000 download-center-5.3.3/demo/spider/mum_create_html.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.737613 download-center-5.3.3/demo/store/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/demo/store/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)    13000 2021-11-05 06:26:29.000000 download-center-5.3.3/demo/store/py_store_mysql_pool.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.738489 download-center-5.3.3/download_center/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/__init__.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.740696 download-center-5.3.3/download_center/new_spider/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/__init__.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.743814 download-center-5.3.3/download_center/new_spider/downloader/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/downloader/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     1298 2022-05-27 06:29:48.000000 download-center-5.3.3/download_center/new_spider/downloader/config.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     7982 2022-05-27 06:29:48.000000 download-center-5.3.3/download_center/new_spider/downloader/downloader.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      254 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/downloader/html_capture.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      260 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/downloader/html_downloader.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     9077 2022-05-23 08:37:22.000000 download-center-5.3.3/download_center/new_spider/downloader/html_local_downloader.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      251 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/downloader/html_render.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.745348 download-center-5.3.3/download_center/new_spider/spider/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/spider/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)    16054 2022-01-20 03:10:19.000000 download-center-5.3.3/download_center/new_spider/spider/basespider.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     4675 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/spider/spider.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.748387 download-center-5.3.3/download_center/new_spider/util/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/util/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)    11141 2022-06-07 05:31:55.000000 download-center-5.3.3/download_center/new_spider/util/util_baidu_relate.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      323 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/util/util_md5.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      540 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/util/util_ping.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      777 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/util/util_url.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      709 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/new_spider/util/util_useragent.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.752827 download-center-5.3.3/download_center/store/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     3147 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/baidu_cookies.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      770 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/config.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     9132 2022-05-23 08:23:51.000000 download-center-5.3.3/download_center/store/py_store_mysql_pool.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/store_cache.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     3285 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/store_es.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     4039 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/store_es_v2.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/store_file.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      739 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/store_mongo.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     2014 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/store/store_oss.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.754673 download-center-5.3.3/download_center/util/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        0 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/util/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     6124 2022-05-23 08:37:22.000000 download-center-5.3.3/download_center/util/py_util_basestore.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     2409 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/util/util_log.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     2480 2019-12-09 04:31:05.000000 download-center-5.3.3/download_center/util/util_log_v2.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.740370 download-center-5.3.3/download_center.egg-info/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     1742 2022-06-07 06:17:13.000000 download-center-5.3.3/download_center.egg-info/PKG-INFO
--rw-r--r--   0 baozhubzhang   (501) staff       (20)     1959 2022-06-07 06:17:13.000000 download-center-5.3.3/download_center.egg-info/SOURCES.txt
--rw-r--r--   0 baozhubzhang   (501) staff       (20)        1 2022-06-07 06:17:13.000000 download-center-5.3.3/download_center.egg-info/dependency_links.txt
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      106 2022-06-07 06:17:13.000000 download-center-5.3.3/download_center.egg-info/requires.txt
--rw-r--r--   0 baozhubzhang   (501) staff       (20)       26 2022-06-07 06:17:13.000000 download-center-5.3.3/download_center.egg-info/top_level.txt
--rw-r--r--   0 baozhubzhang   (501) staff       (20)       38 2022-06-07 06:17:13.757615 download-center-5.3.3/setup.cfg
--rwxr-xr-x   0 baozhubzhang   (501) staff       (20)     4025 2022-06-07 06:16:12.000000 download-center-5.3.3/setup.py
-drwxr-xr-x   0 baozhubzhang   (501) staff       (20)        0 2022-06-07 06:17:13.756805 download-center-5.3.3/test/
--rw-r--r--   0 baozhubzhang   (501) staff       (20)       89 2019-12-09 04:31:05.000000 download-center-5.3.3/test/__init__.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      409 2019-12-09 04:31:05.000000 download-center-5.3.3/test/test1.py
--rw-r--r--   0 baozhubzhang   (501) staff       (20)      461 2019-12-09 04:31:05.000000 download-center-5.3.3/test/test2.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.278252 download-center-5.3.5/
+-rwsrwsrwt   0 berry-zhang   (501) staff       (20)       43 2024-01-09 02:58:45.000000 download-center-5.3.5/MANIFEST.in
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1537 2024-05-14 08:13:52.278042 download-center-5.3.5/PKG-INFO
+-rwxrwxrwt   0 berry-zhang   (501) staff       (20)      888 2024-05-14 08:08:09.000000 download-center-5.3.5/README.md
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.263704 download-center-5.3.5/demo/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)       76 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      121 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/config.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.264387 download-center-5.3.5/demo/extractor/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/extractor/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    13586 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/extractor/baidu_extractor.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1394 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/extractor/demo_extractor.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.266471 download-center-5.3.5/demo/spider/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/spider/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      858 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/spider/config.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     4997 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/spider/demo_spider.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     4661 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/spider/demo_spider_list.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    14353 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/spider/get_header_func.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        1 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/spider/html_py3_3.txt
+-rwxrwxrwt   0 berry-zhang   (501) staff       (20)      145 2024-05-14 05:40:36.000000 download-center-5.3.5/demo/spider/log.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    12334 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/spider/mum_create_html.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.266823 download-center-5.3.5/demo/store/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/store/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    12651 2024-05-14 07:31:33.000000 download-center-5.3.5/demo/store/py_store_mysql_pool.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.267381 download-center-5.3.5/download_center/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1347 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/config.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.268362 download-center-5.3.5/download_center/new_spider/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/__init__.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.269765 download-center-5.3.5/download_center/new_spider/downloader/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/downloader/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1298 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/downloader/config.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     7982 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/downloader/downloader.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      254 2024-05-14 07:32:21.000000 download-center-5.3.5/download_center/new_spider/downloader/html_capture.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      260 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/downloader/html_downloader.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     9176 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/downloader/html_local_downloader.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      251 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/downloader/html_render.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.270383 download-center-5.3.5/download_center/new_spider/spider/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/spider/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    16701 2024-05-14 07:43:11.000000 download-center-5.3.5/download_center/new_spider/spider/basespider.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     4675 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/spider/spider.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.274545 download-center-5.3.5/download_center/new_spider/util/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/util/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    71351 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/util/ua_mobile_list.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    47414 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/util/ua_pc_list.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      471 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/util/ua_spider_list.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    37353 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/util/util_baidu.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    12709 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/util/util_baidu_relate.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      323 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/util/util_md5.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      540 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/util/util_ping.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      777 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/util/util_url.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      709 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/new_spider/util/util_useragent.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)       14 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/requirements.txt
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.276288 download-center-5.3.5/download_center/store/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/store/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     3147 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/store/baidu_cookies.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      770 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/store/config.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     9132 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/store/py_store_mysql_pool.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/store/store_cache.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     3285 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/store/store_es.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     4039 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/store/store_es_v2.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/store/store_file.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      739 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/store/store_mongo.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     2014 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/store/store_oss.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.276913 download-center-5.3.5/download_center/util/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/util/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     6124 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/util/py_util_basestore.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     2409 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/util/util_log.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     2480 2024-05-14 07:31:33.000000 download-center-5.3.5/download_center/util/util_log_v2.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.268240 download-center-5.3.5/download_center.egg-info/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1537 2024-05-14 08:13:52.000000 download-center-5.3.5/download_center.egg-info/PKG-INFO
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     2292 2024-05-14 08:13:52.000000 download-center-5.3.5/download_center.egg-info/SOURCES.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        1 2024-05-14 08:13:52.000000 download-center-5.3.5/download_center.egg-info/dependency_links.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      106 2024-05-14 08:13:52.000000 download-center-5.3.5/download_center.egg-info/requires.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)       26 2024-05-14 08:13:52.000000 download-center-5.3.5/download_center.egg-info/top_level.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)       38 2024-05-14 08:13:52.278303 download-center-5.3.5/setup.cfg
+-rwxrwxrwt   0 berry-zhang   (501) staff       (20)     4025 2024-05-14 08:08:09.000000 download-center-5.3.5/setup.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-14 08:13:52.277697 download-center-5.3.5/test/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)       89 2024-05-14 07:31:33.000000 download-center-5.3.5/test/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      409 2024-05-14 07:31:33.000000 download-center-5.3.5/test/test1.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      461 2024-05-14 07:31:33.000000 download-center-5.3.5/test/test2.py
```

### Comparing `download-center-5.3.3/README.md` & `download-center-5.3.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 - 5.2.15: downloader fail
 - 5.2.16: pymysql版本写法问题
 - 5.2.18: v1.0.0及以上请使用from pymysql.converters import escape_string
 - 5.3.0: 使用私有网络 172.17.0.*
 - 5.3.1: spider里可以打印当前ip
 - 5.3.2: 登录是判断当前ip
 - 5.3.3: 添加百度工具包：pc，mb请求头 + 获取真实url
+- 5.3.5: 添加本地模式代理
 
 
 #### 新下载中心参数，参考 newDownloadReadme.md 文件
 
 使用方法：
 config={"param": {"et":13,'cu',url}}
 request = SpiderRequest(headers=headers, urls=urls,config = config)
```

### Comparing `download-center-5.3.3/demo/extractor/baidu_extractor.py` & `download-center-5.3.5/demo/extractor/baidu_extractor.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/demo/extractor/demo_extractor.py` & `download-center-5.3.5/demo/extractor/demo_extractor.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/demo/spider/demo_spider.py` & `download-center-5.3.5/demo/spider/demo_spider_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,35 +32,39 @@
 
 
 class DemoSpider(BaseSpider):
     def __init__(self, remote=True):
         super(DemoSpider, self).__init__(remote=remote)
         self.log = UtilLogger('DemoSpider', os.path.join(os.path.dirname(os.path.abspath(__file__)), 'log_demo_spider'))
         # self.ext = BaiduExtractor()
-        self.downloader.reset_ip()
+        # self.downloader.reset_ip()
 
     def get_user_password(self):
-        return 'zhangbz', 'Welcome#1'
+        return 'test', 'Welcome#1'
 
-    def tn(self):
-        return random.choice(
-            ['50000021_hao_pg', 'site888_3_pg', '77021190_cpr', 'site5566', '520com_pg', '51010079_cpr'])
+    # def tn(self):
+    #     return random.choice(
+    #         ['baiduhome_pg'])
+        # return random.choice(
+        #     ['50000021_hao_pg', 'site888_3_pg', '77021190_cpr', 'site5566', '520com_pg', '51010079_cpr'])
 
-    # 'url': 'https://www.baidu.com/s?%s' % (urllib.parse.urlencode({'word': '联想', 'ie': 'utf-8', 'tn': self.tn()})),
     def start_requests(self):
         try:
            for i in range(100):
                urls = [{
-                   'url': 'https://m.baidu.com/s?%s' % (urllib.parse.urlencode({'word': '联想','pn':10})),
+                   'url': 'https://www.baidu.com/s?%s' % (urllib.parse.urlencode({'word': '联想','pn':10})),
+                   # 'type': 1,
                    'type': 17,
                    'unique_key':self.get_unique_key()#默认md5 url 字段，不写则表示相同链接只查一次
                }]
-               config={"param": {'cu':'https://m.baidu.com','et':3},"conf_district_id":0}
+               config={"param": {'cu':'https://www.baidu.com','et':0},"conf_district_id":0}
                untilBaidu = UtilBaiduRelate()
-               request = SpiderRequest(headers=untilBaidu.getBaiduMbHeader(), urls=urls,config=config)
+               # headers = untilBaidu.getBaiduMbHeader()
+               headers = untilBaidu.getBaiduPcHeader()
+               request = SpiderRequest(headers=headers, urls=urls,config=config)
                self.sending_queue.put(request)
                time.sleep(0.1)
 
         except Exception:
             self.log.error('获取初始请求出错: {}'.format(traceback.format_exc()))
 
     def get_stores(self):
@@ -78,22 +82,23 @@
 
         Returns:
         根据自己的解析类型做不同的处理，默认返回html
         """
         if task_status == '2':
             config = request.config
             try:
-
                 self.store_queue.put(result["result"])
-
                 # result = json.loads(result["result"])
-                # if '联想' not in result["result"]:
-                #     print("结果抓取失败")
-                # else:
-                #     print("成功!，长度：{},url：{}".format(len(result), url['url']))
+                if result["code"] not in [0,200]:#老版下载中心是0,新版下载中心是 200
+                    print("结果获取错误。code:{}".format(result["code"]))
+                    return
+                if '百度安全验证' in result["result"]:
+                    print("结果抓取失败，百度安全验证")
+                else :
+                    print("成功!，长度：{},url：{}".format(len(result), url['url']))
             except Exception as e:
                 print('失败！url：{}'.format( url['url']))
 
             # rdata = self.ext.ext ractor(result["result"])
             # self.store_queue.put(result)
             # if isinstance(rdata, int):
             #     print("request ua: {}".format(request.headers["User-Agent"]))
@@ -113,14 +118,15 @@
         结果存储按需使用
         :return:
         """
         pass
 
 
 def main():
+    # spider = DemoSpider(remote=False)
     spider = DemoSpider(remote=True)
     spider.run(1, 1, 1, 1, record_log=True)   # 测试
     # spider.run(spider_count=1000, record_log=True)
     # spider.run(record_log=True)               # error
```

### Comparing `download-center-5.3.3/demo/spider/get_header_func.py` & `download-center-5.3.5/demo/spider/get_header_func.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/demo/spider/mum_create_html.py` & `download-center-5.3.5/demo/spider/mum_create_html.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-# -*- coding:utf-8 -*-
-"""
-@Time : 2021/10/15 13:09
-@Author: LiADai(李晗)
-@File : huawei_bankuai_page_spider.py
-@ 版块下帖子链接/帖子title抓取，并标注发帖时间/是否加V或精华、热门帖
-"""
-import ssl
-
-import requests
-
-from demo.spider import config
-
-ssl._create_default_https_context = ssl._create_unverified_context
-import logging
-import os
-import urllib3
-import warnings
-import sys
-from queue import Queue
-import random
-import time
-from download_center.new_spider.downloader.downloader import SpiderRequest
-from download_center.new_spider.spider.basespider import BaseSpider
-from demo.store.py_store_mysql_pool import StoreMysqlPool
-
-urllib3.disable_warnings()
-warnings.filterwarnings('ignore')
-file_name = os.path.basename(__file__).split('.')[0]
-PROJECT_PATH = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-sys.path.append(PROJECT_PATH)
-logging.basicConfig(filename='{}/logs/{}.log'.format(PROJECT_PATH, file_name), level=logging.INFO,
-                    format='%(asctime)s - %(levelname)s - %(name)s : %(message)s')
-
-class mum_creat_tool(BaseSpider):
-    def __init__(self, remote=True):
-        super(mum_creat_tool, self).__init__(remote)
-        #版块下的数据，只允许访问2K条，登录也没用
-        self.dataList = [
-            {"name":"荣耀Magic系列","path":"https://club.hihonor.com/cn/forum-3965-{}.html?filter=lastpost","page":369},
-            {"name":"荣耀数字系列","path":"https://club.hihonor.com/cn/forum-3484-{}.html?filter=lastpost","page":183},
-            {"name": "荣耀V系列", "path": "https://club.hihonor.com/cn/forum-3159-{}.html?filter=lastpost", "page": 69},
-            {"name": "荣耀X系列", "path": "https://club.hihonor.com/cn/forum-4280-{}.html?filter=lastpost", "page": 45},
-            {"name": "荣耀Play系列", "path": "https://club.hihonor.com/cn/forum-3666-{}.html?filter=lastpost", "page": 14},
-            {"name": "荣耀畅玩系列", "path": "https://club.hihonor.com/cn/forum-4526-{}.html?filter=lastpost", "page": 4},
-            {"name": "问题反馈", "path": "https://club.hihonor.com/cn/forum-4508-{}.html?filter=lastpost", "page": 69},
-            {"name": "荣耀亲选", "path": "https://club.hihonor.com/cn/forum-154-{}.html?filter=lastpost", "page": 2},
-            {"name": "智能家居", "path": "https://club.hihonor.com/cn/forum-1835-{}.html?filter=lastpost", "page": 4},
-            {"name": "智能穿戴", "path": "https://club.hihonor.com/cn/forum-4301-{}.html?filter=lastpost", "page": 10},
-            {"name": "公测内测", "path": "https://club.hihonor.com/cn/forum-4149-{}.html?filter=lastpost", "page": 3},
-            {"name": "Magic UI 4.0", "path": "https://club.hihonor.com/cn/forum-455-{}.html?filter=lastpost","page": 7},
-            {"name": "使用技巧", "path": "https://club.hihonor.com/cn/forum-3667-{}.html?filter=lastpost", "page": 4},
-            {"name": "荣耀云服务", "path": "https://club.hihonor.com/cn/forum-4522-{}.html?filter=lastpost", "page": 1},
-            {"name": "爱美食", "path": "https://club.hihonor.com/cn/forum-713-{}.html?filter=lastpost", "page": 46},
-            {"name": "爱旅行", "path": "https://club.hihonor.com/cn/forum-721-{}.html?filter=lastpost", "page": 41},
-            {"name": "爱运动", "path": "https://club.hihonor.com/cn/forum-910-{}.html?filter=lastpost", "page": 47},
-            {"name": "爱主题", "path": "https://club.hihonor.com/cn/forum-1053-{}.html?filter=lastpost", "page": 113},
-            {"name": "爱游戏", "path": "https://club.hihonor.com/cn/forum-4400-{}.html?filter=lastpost", "page": 31},
-            {"name": "爱摄影", "path": "https://club.hihonor.com/cn/forum-141-{}.html?filter=lastpost", "page": 470},
-            {"name": "慢生活", "path": "https://club.hihonor.com/cn/forum-64-{}.html?filter=lastpost", "page": 12},
-            {"name": "荣耀电竞堂", "path": "https://club.hihonor.com/cn/forum-1046-{}.html?filter=lastpost", "page": 1},
-            {"name": "王者荣耀", "path": "https://club.hihonor.com/cn/forum-4513-{}.html?filter=lastpost", "page": 4},
-            {"name": "使命召唤手游", "path": "https://club.hihonor.com/cn/forum-4514-{}.html?filter=lastpost", "page": 28},
-            {"name": "穿越火线", "path": "https://club.hihonor.com/cn/forum-4515-{}.html?filter=lastpost", "page": 1},
-            {"name": "QQ飞车手游", "path": "https://club.hihonor.com/cn/forum-4516-{}.html?filter=lastpost", "page": 1},
-            {"name": "荣耀同城", "path": "https://club.hihonor.com/cn/forum-267-{}.html?filter=lastpost", "page": 2},
-            {"name": "荣耀高校", "path": "https://club.hihonor.com/cn/forum-4346-{}.html?filter=lastpost", "page": 1},
-            {"name": "荣耀创意精英挑战赛", "path": "https://club.hihonor.com/cn/forum-4528-{}.html?filter=lastpost", "page": 1},
-            {"name": "大V申请", "path": "https://club.hihonor.com/cn/forum-150-{}.html?filter=lastpost", "page": 35},
-            {"name": "申诉建议", "path": "https://club.hihonor.com/cn/forum-152-{}.html?filter=lastpost", "page": 3},
-            {"name": "笔记本", "path": "https://club.hihonor.com/cn/forum-4333-{}.html?filter=lastpost", "page": 16},
-            {"name": "平板", "path": "https://club.hihonor.com/cn/forum-4529-{}.html?filter=lastpost", "page": 22},
-            {"name": "耳机音箱", "path": "https://club.hihonor.com/cn/forum-3719-{}.html?filter=lastpost", "page": 4}
-        ]
-        self.table_name = "huawei_bankuai_page"
-        #User-Agent
-        self.pc_useragent_list = [
-            "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/78.0.3904.97 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.3",
-            "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/78.0.3904.108 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:78.0) Gecko/20100101 Firefox/78.0",
-            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.110 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.110 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/64.0.3282.186 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.111 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.1 (KHTML, like Gecko) Chrome/21.0.1180.83 Safari/537.1",
-            "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/69.0.3497.100 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.2; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.90 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.111 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/57.0.2987.133 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/51.0.2704.79 Safari/537.36 Edge/14.14393",
-            "Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.1 (KHTML, like Gecko) Chrome/21.0.1180.83 Safari/537.1",
-            "Mozilla/5.0 (Windows NT 5.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.90 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/46.0.2486.0 Safari/537.36 Edge/13.10586",
-            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36"
-        ]
-
-        #链接数据库
-        try:
-            self.db_225_connect = StoreMysqlPool(**config.db_225_test)
-        except:
-            self.db_225_connect = StoreMysqlPool(**config.db_225_test)
-        self.store_queue = Queue()
-
-    #请求页面
-    def start_requests(self):
-       sql = 'SELECT id,url FROM mum_url WHERE `status` = 0 limit 10;'
-       data = self.db_225_connect.query(sql)
-       for id,url  in data:
-           self.id = id
-           headers = {
-               "Accept":"text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-               "User-Agent": random.choice(self.pc_useragent_list),
-               "Cookie":"VONA_COMMON_LOG_KEY=8b16f212-f212-764e-470d-b0b5d5a2aed8; VONALOGID=881c783d432ddf2cd36f254f29bafa41; sajssdk_2015_cross_new_user=1; sensorsdata2015jssdkcross=%7B%22distinct_id%22%3A%2217ceeb79ca317-067dc9a3b6ad32-57b193e-2073600-17ceeb79ca4640%22%2C%22first_id%22%3A%22%22%2C%22props%22%3A%7B%22%24latest_traffic_source_type%22%3A%22%E7%9B%B4%E6%8E%A5%E6%B5%81%E9%87%8F%22%2C%22%24latest_search_keyword%22%3A%22%E6%9C%AA%E5%8F%96%E5%88%B0%E5%80%BC_%E7%9B%B4%E6%8E%A5%E6%89%93%E5%BC%80%22%2C%22%24latest_referrer%22%3A%22%22%7D%2C%22%24device_id%22%3A%2217ceeb79ca317-067dc9a3b6ad32-57b193e-2073600-17ceeb79ca4640%22%7D; krt.vis=92970e09-4014-4ef6-8c50-516b5cc659c6; Hm_lvt_c86e2c4bb4ad01427261d9484e89bf8b=1636092584; Hm_lpvt_c86e2c4bb4ad01427261d9484e89bf8b=1636092584; CUSTCD=; CustomerCode=; wechat_binded=; AUTHPHONE=; MISUMIVONAEC=%7b%22ABt%22%3a%22b%22%7d; VONAEC_TOP_WOS_BALOON=opened; depocity=%5b119%2c224%2c257%2c289%2c317%2c340%5d; Qs_lvt_294485=1636092584; Qs_pv_294485=2514124822837465600; _ga=GA1.3.2007463036.1636092584; _gid=GA1.3.216996045.1636092584; krt.context=session%3a84134014-1b92-4af6-b8cc-8e4096bb34fe%3bcontext_mode%3aother; _dc_gtm_UA-143948235-1=1; _ga-ch=GA1.3.2007463036.1636092584; _ga-ch_gid=GA1.3.506639854.1636092585; _dc_gtm_UA-6311415-1=1; _gaexp=GAX1.3.sG8KycnKQaK90ZtJ3XtaGQ.19014.0; _gat=1; mediav=%7b%22eid%22%3a%2267947%22%2c%22ep%22%3a%22%22%2c%22vid%22%3a%22%22%2c%22ctn%22%3a%22%22%2c%22vvid%22%3a%22%22%2c%22_mvnf%22%3a1%2c%22_mvctn%22%3a0%2c%22_mvck%22%3a1%2c%22_refnf%22%3a1%7d",
-               "Host":"www.misumi.com.cn"
-           }
-           # requests.get(url=url,headers=headers,verify=False)
-           spider_request = SpiderRequest(headers=headers, urls=url,config={"redirect": 1})
-           self.sending_queue.put(spider_request)
-
-           self.db_225_connect.do('UPDATE mum_url SET `status` = 1 WHERE id = {};'.format(self.id))
-           time.sleep(1)
-           break
-
-    #详情返回
-    def deal_response_results_status(self, task_status, url, result, request):
-        if task_status == '2':
-            ext_type = url["ext_type"]
-            print("详情返回成功。。。")
-            if ext_type==2:
-                res = self.get_details_info(url, result['result'])
-        else:
-            print("下载中心方法失败")
-
-    # 详情处理
-    def get_details_info(self, url, html):
-        print(self.id)
-        print(html)
-        pass
-
-
-    #下载中心 用户账号、密码
-    def get_user_password(self):
-        return "test", "Welcome#1"
-        # return 'caihaijun', 'caihaijun'
-
-    def is_start(self):
-        return self.sended_queue.qsize() < self.sended_queue_maxsize and self.sending_queue.qsize() < self.sended_queue_maxsize \
-               and self.response_queue.qsize() < self.sended_queue_maxsize
-
-
-
-
-
-if __name__ == "__main__":
-    spider = mum_creat_tool(remote=True)
-    timeout_time = -1  # 永不停止 18秒 停止
-    process_pool = 5  # 线程数 debug用单线程
-    spider.run(1, 1, 1, 1, timeout_time, timeout_time, timeout_time,
-               timeout_time, True)
-
-
-
-
-
-
+# -*- coding:utf-8 -*-
+"""
+@Time : 2021/10/15 13:09
+@Author: LiADai(李晗)
+@File : huawei_bankuai_page_spider.py
+@ 版块下帖子链接/帖子title抓取，并标注发帖时间/是否加V或精华、热门帖
+"""
+import ssl
+
+import requests
+
+from demo.spider import config
+
+ssl._create_default_https_context = ssl._create_unverified_context
+import logging
+import os
+import urllib3
+import warnings
+import sys
+from queue import Queue
+import random
+import time
+from download_center.new_spider.downloader.downloader import SpiderRequest
+from download_center.new_spider.spider.basespider import BaseSpider
+from demo.store.py_store_mysql_pool import StoreMysqlPool
+
+urllib3.disable_warnings()
+warnings.filterwarnings('ignore')
+file_name = os.path.basename(__file__).split('.')[0]
+PROJECT_PATH = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+sys.path.append(PROJECT_PATH)
+logging.basicConfig(filename='{}/logs/{}.log'.format(PROJECT_PATH, file_name), level=logging.INFO,
+                    format='%(asctime)s - %(levelname)s - %(name)s : %(message)s')
+
+class mum_creat_tool(BaseSpider):
+    def __init__(self, remote=True):
+        super(mum_creat_tool, self).__init__(remote)
+        #版块下的数据，只允许访问2K条，登录也没用
+        self.dataList = [
+            {"name":"荣耀Magic系列","path":"https://club.hihonor.com/cn/forum-3965-{}.html?filter=lastpost","page":369},
+            {"name":"荣耀数字系列","path":"https://club.hihonor.com/cn/forum-3484-{}.html?filter=lastpost","page":183},
+            {"name": "荣耀V系列", "path": "https://club.hihonor.com/cn/forum-3159-{}.html?filter=lastpost", "page": 69},
+            {"name": "荣耀X系列", "path": "https://club.hihonor.com/cn/forum-4280-{}.html?filter=lastpost", "page": 45},
+            {"name": "荣耀Play系列", "path": "https://club.hihonor.com/cn/forum-3666-{}.html?filter=lastpost", "page": 14},
+            {"name": "荣耀畅玩系列", "path": "https://club.hihonor.com/cn/forum-4526-{}.html?filter=lastpost", "page": 4},
+            {"name": "问题反馈", "path": "https://club.hihonor.com/cn/forum-4508-{}.html?filter=lastpost", "page": 69},
+            {"name": "荣耀亲选", "path": "https://club.hihonor.com/cn/forum-154-{}.html?filter=lastpost", "page": 2},
+            {"name": "智能家居", "path": "https://club.hihonor.com/cn/forum-1835-{}.html?filter=lastpost", "page": 4},
+            {"name": "智能穿戴", "path": "https://club.hihonor.com/cn/forum-4301-{}.html?filter=lastpost", "page": 10},
+            {"name": "公测内测", "path": "https://club.hihonor.com/cn/forum-4149-{}.html?filter=lastpost", "page": 3},
+            {"name": "Magic UI 4.0", "path": "https://club.hihonor.com/cn/forum-455-{}.html?filter=lastpost","page": 7},
+            {"name": "使用技巧", "path": "https://club.hihonor.com/cn/forum-3667-{}.html?filter=lastpost", "page": 4},
+            {"name": "荣耀云服务", "path": "https://club.hihonor.com/cn/forum-4522-{}.html?filter=lastpost", "page": 1},
+            {"name": "爱美食", "path": "https://club.hihonor.com/cn/forum-713-{}.html?filter=lastpost", "page": 46},
+            {"name": "爱旅行", "path": "https://club.hihonor.com/cn/forum-721-{}.html?filter=lastpost", "page": 41},
+            {"name": "爱运动", "path": "https://club.hihonor.com/cn/forum-910-{}.html?filter=lastpost", "page": 47},
+            {"name": "爱主题", "path": "https://club.hihonor.com/cn/forum-1053-{}.html?filter=lastpost", "page": 113},
+            {"name": "爱游戏", "path": "https://club.hihonor.com/cn/forum-4400-{}.html?filter=lastpost", "page": 31},
+            {"name": "爱摄影", "path": "https://club.hihonor.com/cn/forum-141-{}.html?filter=lastpost", "page": 470},
+            {"name": "慢生活", "path": "https://club.hihonor.com/cn/forum-64-{}.html?filter=lastpost", "page": 12},
+            {"name": "荣耀电竞堂", "path": "https://club.hihonor.com/cn/forum-1046-{}.html?filter=lastpost", "page": 1},
+            {"name": "王者荣耀", "path": "https://club.hihonor.com/cn/forum-4513-{}.html?filter=lastpost", "page": 4},
+            {"name": "使命召唤手游", "path": "https://club.hihonor.com/cn/forum-4514-{}.html?filter=lastpost", "page": 28},
+            {"name": "穿越火线", "path": "https://club.hihonor.com/cn/forum-4515-{}.html?filter=lastpost", "page": 1},
+            {"name": "QQ飞车手游", "path": "https://club.hihonor.com/cn/forum-4516-{}.html?filter=lastpost", "page": 1},
+            {"name": "荣耀同城", "path": "https://club.hihonor.com/cn/forum-267-{}.html?filter=lastpost", "page": 2},
+            {"name": "荣耀高校", "path": "https://club.hihonor.com/cn/forum-4346-{}.html?filter=lastpost", "page": 1},
+            {"name": "荣耀创意精英挑战赛", "path": "https://club.hihonor.com/cn/forum-4528-{}.html?filter=lastpost", "page": 1},
+            {"name": "大V申请", "path": "https://club.hihonor.com/cn/forum-150-{}.html?filter=lastpost", "page": 35},
+            {"name": "申诉建议", "path": "https://club.hihonor.com/cn/forum-152-{}.html?filter=lastpost", "page": 3},
+            {"name": "笔记本", "path": "https://club.hihonor.com/cn/forum-4333-{}.html?filter=lastpost", "page": 16},
+            {"name": "平板", "path": "https://club.hihonor.com/cn/forum-4529-{}.html?filter=lastpost", "page": 22},
+            {"name": "耳机音箱", "path": "https://club.hihonor.com/cn/forum-3719-{}.html?filter=lastpost", "page": 4}
+        ]
+        self.table_name = "huawei_bankuai_page"
+        #User-Agent
+        self.pc_useragent_list = [
+            "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/78.0.3904.97 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.3",
+            "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/78.0.3904.108 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:78.0) Gecko/20100101 Firefox/78.0",
+            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.110 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.110 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/64.0.3282.186 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.111 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.1 (KHTML, like Gecko) Chrome/21.0.1180.83 Safari/537.1",
+            "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/69.0.3497.100 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.2; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.90 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.111 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/57.0.2987.133 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/51.0.2704.79 Safari/537.36 Edge/14.14393",
+            "Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.1 (KHTML, like Gecko) Chrome/21.0.1180.83 Safari/537.1",
+            "Mozilla/5.0 (Windows NT 5.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.90 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36",
+            "Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/46.0.2486.0 Safari/537.36 Edge/13.10586",
+            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36"
+        ]
+
+        #链接数据库
+        try:
+            self.db_225_connect = StoreMysqlPool(**config.db_225_test)
+        except:
+            self.db_225_connect = StoreMysqlPool(**config.db_225_test)
+        self.store_queue = Queue()
+
+    #请求页面
+    def start_requests(self):
+       sql = 'SELECT id,url FROM mum_url WHERE `status` = 0 limit 10;'
+       data = self.db_225_connect.query(sql)
+       for id,url  in data:
+           self.id = id
+           headers = {
+               "Accept":"text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
+               "User-Agent": random.choice(self.pc_useragent_list),
+               "Cookie":"VONA_COMMON_LOG_KEY=8b16f212-f212-764e-470d-b0b5d5a2aed8; VONALOGID=881c783d432ddf2cd36f254f29bafa41; sajssdk_2015_cross_new_user=1; sensorsdata2015jssdkcross=%7B%22distinct_id%22%3A%2217ceeb79ca317-067dc9a3b6ad32-57b193e-2073600-17ceeb79ca4640%22%2C%22first_id%22%3A%22%22%2C%22props%22%3A%7B%22%24latest_traffic_source_type%22%3A%22%E7%9B%B4%E6%8E%A5%E6%B5%81%E9%87%8F%22%2C%22%24latest_search_keyword%22%3A%22%E6%9C%AA%E5%8F%96%E5%88%B0%E5%80%BC_%E7%9B%B4%E6%8E%A5%E6%89%93%E5%BC%80%22%2C%22%24latest_referrer%22%3A%22%22%7D%2C%22%24device_id%22%3A%2217ceeb79ca317-067dc9a3b6ad32-57b193e-2073600-17ceeb79ca4640%22%7D; krt.vis=92970e09-4014-4ef6-8c50-516b5cc659c6; Hm_lvt_c86e2c4bb4ad01427261d9484e89bf8b=1636092584; Hm_lpvt_c86e2c4bb4ad01427261d9484e89bf8b=1636092584; CUSTCD=; CustomerCode=; wechat_binded=; AUTHPHONE=; MISUMIVONAEC=%7b%22ABt%22%3a%22b%22%7d; VONAEC_TOP_WOS_BALOON=opened; depocity=%5b119%2c224%2c257%2c289%2c317%2c340%5d; Qs_lvt_294485=1636092584; Qs_pv_294485=2514124822837465600; _ga=GA1.3.2007463036.1636092584; _gid=GA1.3.216996045.1636092584; krt.context=session%3a84134014-1b92-4af6-b8cc-8e4096bb34fe%3bcontext_mode%3aother; _dc_gtm_UA-143948235-1=1; _ga-ch=GA1.3.2007463036.1636092584; _ga-ch_gid=GA1.3.506639854.1636092585; _dc_gtm_UA-6311415-1=1; _gaexp=GAX1.3.sG8KycnKQaK90ZtJ3XtaGQ.19014.0; _gat=1; mediav=%7b%22eid%22%3a%2267947%22%2c%22ep%22%3a%22%22%2c%22vid%22%3a%22%22%2c%22ctn%22%3a%22%22%2c%22vvid%22%3a%22%22%2c%22_mvnf%22%3a1%2c%22_mvctn%22%3a0%2c%22_mvck%22%3a1%2c%22_refnf%22%3a1%7d",
+               "Host":"www.misumi.com.cn"
+           }
+           # requests.get(url=url,headers=headers,verify=False)
+           spider_request = SpiderRequest(headers=headers, urls=url,config={"redirect": 1})
+           self.sending_queue.put(spider_request)
+
+           self.db_225_connect.do('UPDATE mum_url SET `status` = 1 WHERE id = {};'.format(self.id))
+           time.sleep(1)
+           break
+
+    #详情返回
+    def deal_response_results_status(self, task_status, url, result, request):
+        if task_status == '2':
+            ext_type = url["ext_type"]
+            print("详情返回成功。。。")
+            if ext_type==2:
+                res = self.get_details_info(url, result['result'])
+        else:
+            print("下载中心方法失败")
+
+    # 详情处理
+    def get_details_info(self, url, html):
+        print(self.id)
+        print(html)
+        pass
+
+
+    #下载中心 用户账号、密码
+    def get_user_password(self):
+        return "test", "Welcome#1"
+        # return 'caihaijun', 'caihaijun'
+
+    def is_start(self):
+        return self.sended_queue.qsize() < self.sended_queue_maxsize and self.sending_queue.qsize() < self.sended_queue_maxsize \
+               and self.response_queue.qsize() < self.sended_queue_maxsize
+
+
+
+
+
+if __name__ == "__main__":
+    spider = mum_creat_tool(remote=True)
+    timeout_time = -1  # 永不停止 18秒 停止
+    process_pool = 5  # 线程数 debug用单线程
+    spider.run(1, 1, 1, 1, timeout_time, timeout_time, timeout_time,
+               timeout_time, True)
+
+
+
+
+
+
```

### Comparing `download-center-5.3.3/demo/store/py_store_mysql_pool.py` & `download-center-5.3.5/demo/store/py_store_mysql_pool.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,349 +1,349 @@
-# -*- coding: utf8 -*-
-from collections import OrderedDict
-from copy import deepcopy
-import pymysql
-import time
-from DBUtils.PooledDB import PooledDB
-from DBUtils.PersistentDB import PersistentDB
-import traceback
-from datetime import datetime
-import warnings
-
-warnings.filterwarnings('ignore')
-
-
-class StoreMysqlPool(object):
-    """
-    mysql读写相关操作，pymysql，使用PooledDB连接池
-    Args:
-        host:数据库ip
-        user:数据库用户名
-        password:数据库用户密码
-        db:数据库名
-        port:数据库端口，默认3306
-        mincached:最少的空闲连接数， 默认为1
-        charset:数据库编码，默认utf8
-    """
-
-    def __init__(self, host="", user="", password="", db="", port=3306, mincached=1,
-                 pattern=1, charset="utf8"):
-        self.host = host
-
-        if pattern == 1:
-            self.pool = PooledDB(pymysql, mincached, host=host, user=user, passwd=password, db=db, port=port,
-                                 charset=charset)
-            self.close_able = True
-        elif pattern == 2:
-            self.pool = PersistentDB(pymysql, host=host, user=user, passwd=password, db=db, port=port,
-                                     charset=charset)
-
-            self.close_able = False
-        self._last_use_time = time.time()
-
-    def close(self, db):
-        if db is not None:
-            db.close()
-
-    def connect(self):
-        return self.pool.connection()
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.close_all()
-
-    @staticmethod
-    def _cursor(db):
-        # return db.cursor(pymysql.cursors.DictCursor)
-        return db.cursor()
-
-    def query(self, sql):
-        """
-        根据sql查询
-        Returns：
-            数组的数组，外层数组元素为一行，内存数组元素为一行的一列
-        """
-        db = self.connect()
-        cur = self._cursor(db)
-        rows = []
-        try:
-            cur.execute(sql)
-            db.commit()
-            rows = cur.fetchall()
-        except pymysql.OperationalError:
-            print(traceback.format_exc())
-        except Exception:
-            print(traceback.format_exc())
-        finally:
-            cur.close()
-            self.close(db)
-        return rows
-
-    def count(self, tb):
-        """
-        返回某表的行数
-        Args:
-            tb:字符串，表名称
-        """
-        sql = 'select count(*) from %s' % tb
-        results = self.query(sql)
-        if len(results) == 1 and len(results[0]) == 1:
-            return int(results[0][0])
-
-    def do(self, sql, flag='rowcount'):
-        """
-        执行sql，insert/delete/update操作
-        Args:
-            sql:要执行的sql
-            flag:返回值类型，flag=lastrowid返回lastrowid，flag=rowcount返回rowcount
-        """
-        db = self.connect()
-        cur = self._cursor(db)
-        r = None
-        try:
-            cur.execute(sql)
-            db.commit()
-            r = 1
-            if flag == 'lastrowid':
-                r = cur.lastrowid
-            elif flag == 'rowcount':
-                r = cur.rowcount
-        except pymysql.OperationalError:
-            print("time: %s; Error on %s: %s" % (str(datetime.now()), self.host, sql[0: 200]))
-            print(traceback.format_exc())
-            r = -1
-        except Exception:
-            print("time: %s; Error to MySQL on %s: %s" % (str(datetime.now()), self.host, sql[0: 200]))
-            print(traceback.format_exc())
-            r = -1
-        finally:
-            cur.close()
-            self.close(db)
-        return r
-
-    def save(self, table, data, mapping_fields=dict()):
-        """
-        将字典直接insert到数据库
-        Args:
-            table:字符串，插入目标表的名称
-            data:字典格式，key为字段名称，value为字段值，如{'id':'1','name':'temp'}
-            mapping_fields: 用于保持data字典的key与数据库字段的对应关系，
-                            如果结果字典的某个key不包含在mapping_fields中，则将直接使用key作为字段名
-        """
-
-        if len(data) <= 0:
-            return -1
-        try:
-            fields = ''
-            values = ''
-            for d in data:
-                if d in mapping_fields:
-                    fields += "`%s`," % (str(mapping_fields[d]))
-                else:
-                    fields += "`%s`," % (str(d))
-                values += "'%s'," % (pymysql.escape_string(str(data[d])))
-            if len(fields) <= 0 or len(values) <= 0:
-                return -1
-            sql = "insert ignore into %s(%s) values(%s)" % (table, fields[:-1], values[:-1])
-            return self.do(sql)
-        except Exception:
-            print(traceback.format_exc())
-            return -1
-
-    def saveMany(self, sql, values, flag='lastrowid'):
-        """
-        执行sql，insert/delete/update操作
-        :param table: 'insert into table(id,name) values(%s,%s)'
-        :param names: 字符串
-        :param values:[{1,2},{1,2},...]  是一个列表，列表中的每一个元素必须是元组！！！
-        :param flag:
-        :return:
-        """
-        db = self.connect()
-        cur = self._cursor(db)
-        r = None
-        try:
-            cur.executemany(sql, values)
-            db.commit()
-            r = 1
-            if flag == 'lastrowid':
-                r = cur.lastrowid
-            elif flag == 'rowcount':
-                r = cur.rowcount
-
-        except pymysql.OperationalError:
-            print("Error connecting to MySQL on %s: %s" % (self.host, sql[0:255]))
-            print(traceback.format_exc())
-            r = -1
-        except Exception:
-            print("Error connecting to MySQL on %s: %s" % (self.host, sql[0:255]))
-            print(traceback.format_exc())
-            r = -1
-        finally:
-            cur.close()
-            self.close(db)
-        return r
-
-    def update(self, table, data, field, mapping_fields=dict()):
-        """
-        将字典直接update到数据库
-        Args:
-            table:字符串，更新目标表的名称
-            data:字典格式，key为字段名称，value为字段值，如{'id':'1','name':'temp'}
-            field:唯一索引字段，即根据该字段判断是否为同一条记录，作为where条件
-            mapping_fields: 用于保持data字典的key与数据库字段的对应关系，
-                            如果结果字典的某个key不包含在mapping_fields中，则将直接使用key作为字段名
-        """
-        if len(data) <= 0:
-            return -1
-        else:
-            try:
-                values = ''
-                field_value = None
-                for d in data:
-                    key = d
-                    if d in mapping_fields:
-                        key = mapping_fields[d]
-                    if key == field:
-                        field_value = data[d]
-                    values += "%s='%s'," % (str(key), pymysql.escape_string(str(data[d])))
-                if len(values) <= 0 or field_value is None:
-                    return -1
-                sql = "update " + table + " set " + values[:-1] + " where " + field + "='" + pymysql.escape_string(
-                        str(field_value)) + "'"
-                return self.do(sql, flag='rowcount')
-            except Exception:
-                print(traceback.format_exc())
-                return -1
-
-    def saveorupdate(self, table, data, field, mapping_fields=dict()):
-        """
-        将字典更新到数据库，如果已存在则update，不存在则insert
-        Args:
-            table:字符串，更新目标表的名称
-            data:字典格式，key为字段名称，value为字段值，如{'id':'1','name':'temp'}
-            field:唯一索引字段，即根据词字段判断是否为同一条记录，作为where条件
-            mapping_fields: 用于保持data字典的key与数据库字段的对应关系，
-                            如果结果字典的某个key不包含在mapping_fields中，则将直接使用key作为字段名
-        """
-        if len(data) <= 0:
-            return -1
-        try:
-            field_value = None
-            if field in data:
-                field_value = data[field]
-            else:
-                for key in mapping_fields:
-                    if mapping_fields[key] == field and key in data:
-                        field_value = data[key]
-            if field_value is None:
-                return -1
-            querysql = "select count(1) from " + table + " where " + field + "='" + pymysql.escape_string(
-                    str(field_value)) + "'"
-            ed = self.query(querysql)
-            if ed and ed[0][0] > 0:
-                return self.update(table, data, field, mapping_fields)
-            else:
-                return self.save(table, data, mapping_fields)
-        except Exception:
-            print(traceback.format_exc())
-            return -1
-
-    def tableCreate(self, tb_name, likeTable):
-        """
-        创建数据表格
-        :param tb_name: table's name
-        :return: 1 ok , -1 error
-        """
-        # sql = "SELECT table_name FROM information_schema.TABLES WHERE table_name ='{}';".format(tb_name)
-        sql = "show tables;"
-        datas = self.query(sql)
-        if tb_name in [str(i[0]) for i in datas]:
-            # 存在
-            sql = "select * from {} limit 10;".format(tb_name)
-            if not self.query(sql):
-                print("{} 是空表, 正在truncate.....".format(tb_name))
-                sql = " truncate {};".format(tb_name)
-                datas = self.query(sql)
-            else:
-                print("表格存在：{}".format(tb_name))
-
-        else:
-            # 不存在 创建 清空
-            print("{} 表格不存在，正在创建....".format(tb_name))
-            sql = "create table {} like {};".format(tb_name, likeTable)
-            datas = self.query(sql)
-            sql = " truncate {};".format(tb_name)
-            datas = self.query(sql)
-        return 1
-
-    def dictsToOrderDicts(self, list_dicts):
-        alist = []
-        # list_dicts = [list_dicts] if isinstance(list_dicts, dict) else list_dicts
-        ks = list_dicts[0].keys()  # 有序
-        order_dict = OrderedDict()
-        for adict in list_dicts:
-            for k in ks:
-                order_dict[k] = adict[k]
-            alist.append(deepcopy(order_dict))
-        return alist
-
-    def insert_many(self, table, list_dicts, conflict=''):
-        '''
-        [批量插入]
-        :param store_name:
-        :param table:
-        :param list_dicts:
-        :param conflict: 冲突更新字段 local_date=CURRENT_DATE() or ['local_date','fields']
-        :return:
-        '''
-        try:
-            if len(list_dicts):
-                orderDicts = self.dictsToOrderDicts(list_dicts)
-                ks = orderDicts[0].keys()  # 获取键值
-                if conflict:
-                    if isinstance(conflict, str):
-                        insert_sql = "insert ignore into {} ({}) values ({})  ON DUPLICATE KEY UPDATE {}".format(
-                                table, ", ".join(ks), ("%s," * len(ks)).strip(","), conflict)
-                    else:
-                        if len(conflict):
-                            conflict = ','.join(['{}=VALUES({})'.format(field, field) for field in conflict])
-                            insert_sql = "insert ignore into {} ({}) values ({})  ON DUPLICATE KEY UPDATE {}".format(
-                                    table, ", ".join(ks), ("%s," * len(ks)).strip(","), conflict)
-                        else:
-                            return -1
-
-                else:
-                    insert_sql = "insert ignore into {} ({}) values ({})".format(table, ", ".join(ks),
-                                                                                 ("%s," * len(ks)).strip(","))
-                values = []
-                for adict in list_dicts:
-                    values.append(tuple(adict.values()))
-                res = self.saveMany(insert_sql, values, flag="rowcount")
-                return res
-            else:
-                return -3
-        except:
-            return -2
-
-    def close_all(self):
-        """
-        关闭连接池全部连接
-        请在确保连接不再需要时确认
-        :return:
-        """
-        if self.close_able:
-            self.pool.close()
-
-
-def test():
-    db = {
-        'host': 'localhost',
-        'user': 'root',
-        'password': '',
-        'db': 'test'
-    }
-    mq = StoreMysqlPool(**db)
-    print(mq.count('urls'))
-
-
-if __name__ == "__main__":
-    test()
+# -*- coding: utf8 -*-
+from collections import OrderedDict
+from copy import deepcopy
+import pymysql
+import time
+from DBUtils.PooledDB import PooledDB
+from DBUtils.PersistentDB import PersistentDB
+import traceback
+from datetime import datetime
+import warnings
+
+warnings.filterwarnings('ignore')
+
+
+class StoreMysqlPool(object):
+    """
+    mysql读写相关操作，pymysql，使用PooledDB连接池
+    Args:
+        host:数据库ip
+        user:数据库用户名
+        password:数据库用户密码
+        db:数据库名
+        port:数据库端口，默认3306
+        mincached:最少的空闲连接数， 默认为1
+        charset:数据库编码，默认utf8
+    """
+
+    def __init__(self, host="", user="", password="", db="", port=3306, mincached=1,
+                 pattern=1, charset="utf8"):
+        self.host = host
+
+        if pattern == 1:
+            self.pool = PooledDB(pymysql, mincached, host=host, user=user, passwd=password, db=db, port=port,
+                                 charset=charset)
+            self.close_able = True
+        elif pattern == 2:
+            self.pool = PersistentDB(pymysql, host=host, user=user, passwd=password, db=db, port=port,
+                                     charset=charset)
+
+            self.close_able = False
+        self._last_use_time = time.time()
+
+    def close(self, db):
+        if db is not None:
+            db.close()
+
+    def connect(self):
+        return self.pool.connection()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close_all()
+
+    @staticmethod
+    def _cursor(db):
+        # return db.cursor(pymysql.cursors.DictCursor)
+        return db.cursor()
+
+    def query(self, sql):
+        """
+        根据sql查询
+        Returns：
+            数组的数组，外层数组元素为一行，内存数组元素为一行的一列
+        """
+        db = self.connect()
+        cur = self._cursor(db)
+        rows = []
+        try:
+            cur.execute(sql)
+            db.commit()
+            rows = cur.fetchall()
+        except pymysql.OperationalError:
+            print(traceback.format_exc())
+        except Exception:
+            print(traceback.format_exc())
+        finally:
+            cur.close()
+            self.close(db)
+        return rows
+
+    def count(self, tb):
+        """
+        返回某表的行数
+        Args:
+            tb:字符串，表名称
+        """
+        sql = 'select count(*) from %s' % tb
+        results = self.query(sql)
+        if len(results) == 1 and len(results[0]) == 1:
+            return int(results[0][0])
+
+    def do(self, sql, flag='rowcount'):
+        """
+        执行sql，insert/delete/update操作
+        Args:
+            sql:要执行的sql
+            flag:返回值类型，flag=lastrowid返回lastrowid，flag=rowcount返回rowcount
+        """
+        db = self.connect()
+        cur = self._cursor(db)
+        r = None
+        try:
+            cur.execute(sql)
+            db.commit()
+            r = 1
+            if flag == 'lastrowid':
+                r = cur.lastrowid
+            elif flag == 'rowcount':
+                r = cur.rowcount
+        except pymysql.OperationalError:
+            print("time: %s; Error on %s: %s" % (str(datetime.now()), self.host, sql[0: 200]))
+            print(traceback.format_exc())
+            r = -1
+        except Exception:
+            print("time: %s; Error to MySQL on %s: %s" % (str(datetime.now()), self.host, sql[0: 200]))
+            print(traceback.format_exc())
+            r = -1
+        finally:
+            cur.close()
+            self.close(db)
+        return r
+
+    def save(self, table, data, mapping_fields=dict()):
+        """
+        将字典直接insert到数据库
+        Args:
+            table:字符串，插入目标表的名称
+            data:字典格式，key为字段名称，value为字段值，如{'id':'1','name':'temp'}
+            mapping_fields: 用于保持data字典的key与数据库字段的对应关系，
+                            如果结果字典的某个key不包含在mapping_fields中，则将直接使用key作为字段名
+        """
+
+        if len(data) <= 0:
+            return -1
+        try:
+            fields = ''
+            values = ''
+            for d in data:
+                if d in mapping_fields:
+                    fields += "`%s`," % (str(mapping_fields[d]))
+                else:
+                    fields += "`%s`," % (str(d))
+                values += "'%s'," % (pymysql.escape_string(str(data[d])))
+            if len(fields) <= 0 or len(values) <= 0:
+                return -1
+            sql = "insert ignore into %s(%s) values(%s)" % (table, fields[:-1], values[:-1])
+            return self.do(sql)
+        except Exception:
+            print(traceback.format_exc())
+            return -1
+
+    def saveMany(self, sql, values, flag='lastrowid'):
+        """
+        执行sql，insert/delete/update操作
+        :param table: 'insert into table(id,name) values(%s,%s)'
+        :param names: 字符串
+        :param values:[{1,2},{1,2},...]  是一个列表，列表中的每一个元素必须是元组！！！
+        :param flag:
+        :return:
+        """
+        db = self.connect()
+        cur = self._cursor(db)
+        r = None
+        try:
+            cur.executemany(sql, values)
+            db.commit()
+            r = 1
+            if flag == 'lastrowid':
+                r = cur.lastrowid
+            elif flag == 'rowcount':
+                r = cur.rowcount
+
+        except pymysql.OperationalError:
+            print("Error connecting to MySQL on %s: %s" % (self.host, sql[0:255]))
+            print(traceback.format_exc())
+            r = -1
+        except Exception:
+            print("Error connecting to MySQL on %s: %s" % (self.host, sql[0:255]))
+            print(traceback.format_exc())
+            r = -1
+        finally:
+            cur.close()
+            self.close(db)
+        return r
+
+    def update(self, table, data, field, mapping_fields=dict()):
+        """
+        将字典直接update到数据库
+        Args:
+            table:字符串，更新目标表的名称
+            data:字典格式，key为字段名称，value为字段值，如{'id':'1','name':'temp'}
+            field:唯一索引字段，即根据该字段判断是否为同一条记录，作为where条件
+            mapping_fields: 用于保持data字典的key与数据库字段的对应关系，
+                            如果结果字典的某个key不包含在mapping_fields中，则将直接使用key作为字段名
+        """
+        if len(data) <= 0:
+            return -1
+        else:
+            try:
+                values = ''
+                field_value = None
+                for d in data:
+                    key = d
+                    if d in mapping_fields:
+                        key = mapping_fields[d]
+                    if key == field:
+                        field_value = data[d]
+                    values += "%s='%s'," % (str(key), pymysql.escape_string(str(data[d])))
+                if len(values) <= 0 or field_value is None:
+                    return -1
+                sql = "update " + table + " set " + values[:-1] + " where " + field + "='" + pymysql.escape_string(
+                        str(field_value)) + "'"
+                return self.do(sql, flag='rowcount')
+            except Exception:
+                print(traceback.format_exc())
+                return -1
+
+    def saveorupdate(self, table, data, field, mapping_fields=dict()):
+        """
+        将字典更新到数据库，如果已存在则update，不存在则insert
+        Args:
+            table:字符串，更新目标表的名称
+            data:字典格式，key为字段名称，value为字段值，如{'id':'1','name':'temp'}
+            field:唯一索引字段，即根据词字段判断是否为同一条记录，作为where条件
+            mapping_fields: 用于保持data字典的key与数据库字段的对应关系，
+                            如果结果字典的某个key不包含在mapping_fields中，则将直接使用key作为字段名
+        """
+        if len(data) <= 0:
+            return -1
+        try:
+            field_value = None
+            if field in data:
+                field_value = data[field]
+            else:
+                for key in mapping_fields:
+                    if mapping_fields[key] == field and key in data:
+                        field_value = data[key]
+            if field_value is None:
+                return -1
+            querysql = "select count(1) from " + table + " where " + field + "='" + pymysql.escape_string(
+                    str(field_value)) + "'"
+            ed = self.query(querysql)
+            if ed and ed[0][0] > 0:
+                return self.update(table, data, field, mapping_fields)
+            else:
+                return self.save(table, data, mapping_fields)
+        except Exception:
+            print(traceback.format_exc())
+            return -1
+
+    def tableCreate(self, tb_name, likeTable):
+        """
+        创建数据表格
+        :param tb_name: table's name
+        :return: 1 ok , -1 error
+        """
+        # sql = "SELECT table_name FROM information_schema.TABLES WHERE table_name ='{}';".format(tb_name)
+        sql = "show tables;"
+        datas = self.query(sql)
+        if tb_name in [str(i[0]) for i in datas]:
+            # 存在
+            sql = "select * from {} limit 10;".format(tb_name)
+            if not self.query(sql):
+                print("{} 是空表, 正在truncate.....".format(tb_name))
+                sql = " truncate {};".format(tb_name)
+                datas = self.query(sql)
+            else:
+                print("表格存在：{}".format(tb_name))
+
+        else:
+            # 不存在 创建 清空
+            print("{} 表格不存在，正在创建....".format(tb_name))
+            sql = "create table {} like {};".format(tb_name, likeTable)
+            datas = self.query(sql)
+            sql = " truncate {};".format(tb_name)
+            datas = self.query(sql)
+        return 1
+
+    def dictsToOrderDicts(self, list_dicts):
+        alist = []
+        # list_dicts = [list_dicts] if isinstance(list_dicts, dict) else list_dicts
+        ks = list_dicts[0].keys()  # 有序
+        order_dict = OrderedDict()
+        for adict in list_dicts:
+            for k in ks:
+                order_dict[k] = adict[k]
+            alist.append(deepcopy(order_dict))
+        return alist
+
+    def insert_many(self, table, list_dicts, conflict=''):
+        '''
+        [批量插入]
+        :param store_name:
+        :param table:
+        :param list_dicts:
+        :param conflict: 冲突更新字段 local_date=CURRENT_DATE() or ['local_date','fields']
+        :return:
+        '''
+        try:
+            if len(list_dicts):
+                orderDicts = self.dictsToOrderDicts(list_dicts)
+                ks = orderDicts[0].keys()  # 获取键值
+                if conflict:
+                    if isinstance(conflict, str):
+                        insert_sql = "insert ignore into {} ({}) values ({})  ON DUPLICATE KEY UPDATE {}".format(
+                                table, ", ".join(ks), ("%s," * len(ks)).strip(","), conflict)
+                    else:
+                        if len(conflict):
+                            conflict = ','.join(['{}=VALUES({})'.format(field, field) for field in conflict])
+                            insert_sql = "insert ignore into {} ({}) values ({})  ON DUPLICATE KEY UPDATE {}".format(
+                                    table, ", ".join(ks), ("%s," * len(ks)).strip(","), conflict)
+                        else:
+                            return -1
+
+                else:
+                    insert_sql = "insert ignore into {} ({}) values ({})".format(table, ", ".join(ks),
+                                                                                 ("%s," * len(ks)).strip(","))
+                values = []
+                for adict in list_dicts:
+                    values.append(tuple(adict.values()))
+                res = self.saveMany(insert_sql, values, flag="rowcount")
+                return res
+            else:
+                return -3
+        except:
+            return -2
+
+    def close_all(self):
+        """
+        关闭连接池全部连接
+        请在确保连接不再需要时确认
+        :return:
+        """
+        if self.close_able:
+            self.pool.close()
+
+
+def test():
+    db = {
+        'host': 'localhost',
+        'user': 'root',
+        'password': '',
+        'db': 'test'
+    }
+    mq = StoreMysqlPool(**db)
+    print(mq.count('urls'))
+
+
+if __name__ == "__main__":
+    test()
```

### Comparing `download-center-5.3.3/download_center/new_spider/downloader/config.py` & `download-center-5.3.5/download_center/new_spider/downloader/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/new_spider/downloader/downloader.py` & `download-center-5.3.5/download_center/new_spider/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/new_spider/downloader/html_local_downloader.py` & `download-center-5.3.5/download_center/new_spider/downloader/html_local_downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,39 +110,39 @@
                 data = param.get("post_data", None)
                 method = param.get("method", None)
                 filter = param.get('filter', 0)
 
                 for url in urls:
                     result = {"url": url["url"], "status": "3", "result": "", "header": "",
                               "redirect_url": "", "code": 0, "type": url_type}
-
+                    proxies = request.config.get("proxies", None)
                     # start = time.time()
                     self.download_html_by_requests(url["url"], result, data, headers, req=requests, filter=filter,
-                                                   method=method)
+                                                   method=method, proxies=proxies)
                     # print(
                     #     "url: {}; length: {}; time: {}".format(url["url"], len(result["result"]), time.time() - start))
 
                     results[url['md5']] = result
                 return results
             except Exception:
                 print(traceback.format_exc())
         return 0
 
-    def download_html_by_requests(self, url, result, data, headers, req=None, filter=0, method=None):
+    def download_html_by_requests(self, url, result, data, headers, req=None, filter=0, method=None, proxies=None):
         """
         :param task:
         :param result:
         :param data:
         :param headers:
         :param req:        requests
         :param filter:  0 默认不过滤 1 过滤
         :return:
         """
         try:
-            response = self.transfer_requests(req, url, data, headers, None, method)
+            response = self.transfer_requests(req, url, data, headers, proxies, method)
             try:
                 if response.encoding == 'ISO-8859-1':
                     encodings = requests.utils.get_encodings_from_content(response.text)
                     if encodings:
                         encoding = encodings[0]
                     else:
                         encoding = response.apparent_encoding
```

### Comparing `download-center-5.3.3/download_center/new_spider/spider/basespider.py` & `download-center-5.3.5/download_center/new_spider/spider/basespider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # -*- coding: utf8 -*-
+import json
 
-from download_center.new_spider.downloader.downloader import Downloader
-from download_center.new_spider.downloader.downloader import SpiderRequest
-from download_center.new_spider.downloader.html_local_downloader import HtmlLocalDownloader
-from download_center.new_spider.util.util_useragent import UtilUseragent
+import requests
+from downloader_client.download_center.new_spider.downloader.downloader import Downloader
+from downloader_client.download_center.new_spider.downloader.downloader import SpiderRequest
+from downloader_client.download_center.new_spider.downloader.html_local_downloader import HtmlLocalDownloader
+from downloader_client.download_center.new_spider.util.util_useragent import UtilUseragent
+from downloader_client.download_center import config
 # from Queue import LifoQueue
 from queue import Queue
 from queue import Empty
 from threading import Thread
 import time
 import traceback
 import objgraph
@@ -157,14 +160,21 @@
         获取url爬取结果。将sended_queue队列中的SpiderRequest对象通过downloader到下载中心去获取抓取到的html
         """
         start_time = time.time()
         while True:
             try:
                 if self.response_queue.qsize() < self.response_queue_max:
                     request = self.sended_queue.get(timeout=1)
+                    if not self.remote:
+                        user, password = self.get_user_password()
+                        data = {"user": user, "password": password}
+                        # 获取代理 ip
+                        r = requests.post(config.AGENCYIP_URL.format(config.DOWNLOADER_CENTER_IP[config.ENVIR]),
+                                          data=data, timeout=config.REQUEST_TIMEOUT)
+                        request.config["proxies"] = json.loads(r.text)["proxy"]
                     results = self.downloader.get(request)
                     #status = results[request.urls[0]['unique_md5']]
                     self.response_queue.put((request, results))
                     start_time = time.time()
                     self.get_wait()     # wait confirm
                 else:
                     time.sleep(10)
```

### Comparing `download-center-5.3.3/download_center/new_spider/spider/spider.py` & `download-center-5.3.5/download_center/new_spider/spider/spider.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/new_spider/util/util_baidu_relate.py` & `download-center-5.3.5/download_center/new_spider/util/util_baidu_relate.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,25 +80,27 @@
         ]
         return random.choice(pc_useragent_list)
 
     def getBaiduPcHeader(self):
         headers = {
             "User-Agent": self.get_pc_useragent(),
             'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
-            # 'Accept-Language':'zh-CN,zh;q=0.9,en-CN;q=0.8,en;q=0.7,ar-XB;q=0.6,ar;q=0.5',
+            'Accept-Language':'zh-CN,zh;q=0.9,en-CN;q=0.8,en;q=0.7,ar-XB;q=0.6,ar;q=0.5',
+            # 'Accept-Encoding': 'gzip, deflate, br',
             'Cookie': self.get_baidu_pc_cookie()
         }
 
         return headers
 
     def getBaiduMbHeader(self):
         headers = {
             "User-Agent": self.get_mobile_useragent(),
             'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
-            # 'Accept-Language':'zh-CN,zh;q=0.9,en-CN;q=0.8,en;q=0.7,ar-XB;q=0.6,ar;q=0.5',
+            'Accept-Language':'zh-CN,zh;q=0.9,en-CN;q=0.8,en;q=0.7,ar-XB;q=0.6,ar;q=0.5',
+            'Accept-Encoding':'gzip, deflate, br',
             'Cookie': self.get_baidu_mb_cookie()
         }
 
         return headers
 
     # 获取百度移动端cookie
     def get_baidu_mb_cookie(self):
@@ -149,13 +151,34 @@
             else:
                 return self.get_real_url(baidu_url, try_count + 1)
                 # return ''
         except Exception as err:
             return self.get_real_url(baidu_url, try_count + 1)
             # return ''
 
+    def generate_weixin_user_agent(self):
+        iOS_version_random = random.randint(12, 15)
+        android_version_random = random.randint(8, 12)
+
+        uas = [
+            f'Mozilla/5.0 (Linux; Android {android_version_random}; RMX3115 Build/SP1A.210812.016; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3225 MMWEBSDK/20220402 Mobile Safari/537.36 MMWEBID/7093 MicroMessenger/8.0.22.2140(0x2800{android_version_random}E6) WeChat/arm64 Weixin NetType/4G Language/zh_CN ABI/arm64',
+            f'Mozilla/5.0 (iPhone; CPU iPhone OS {iOS_version_random}_4_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/{iOS_version_random}E148 MicroMessenger/8.0.22(0x1800{iOS_version_random}28) NetType/WIFI Language/zh_CN',
+            f'Mozilla/5.0 (Linux; Android {android_version_random}; M2007J1SC Build/QKQ1.200419.002; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3225 MMWEBSDK/20220402 Mobile Safari/537.36 MMWEBID/2728 MicroMessenger/8.0.22.2140(0x2800{android_version_random}F2) WeChat/arm64 Weixin NetType/WIFI Language/zh_CN ABI/arm64'
+        ]
+        return random.choice(uas)
+
+    #获取详情页百家号cookie
+    def get_baijiahao_cookie(self):
+        url = 'http://124.220.177.240:5022/baijiahao/random'
+        ddd = requests.get(url).json()
+        line = ''
+        for k, v in ddd.items():
+            line += f'{k}={v}; '
+        # print(line)
+        return line
+
 def test():
     untilBaidu = UtilBaiduRelate()
     print(untilBaidu.getBaiduPcHeader())
 
 if __name__ == '__main__':
     test()
```

### Comparing `download-center-5.3.3/download_center/new_spider/util/util_ping.py` & `download-center-5.3.5/download_center/new_spider/util/util_ping.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/new_spider/util/util_url.py` & `download-center-5.3.5/download_center/new_spider/util/util_url.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/new_spider/util/util_useragent.py` & `download-center-5.3.5/download_center/new_spider/util/util_useragent.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/store/baidu_cookies.py` & `download-center-5.3.5/download_center/store/baidu_cookies.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/store/config.py` & `download-center-5.3.5/download_center/store/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/store/py_store_mysql_pool.py` & `download-center-5.3.5/download_center/store/py_store_mysql_pool.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/store/store_es.py` & `download-center-5.3.5/download_center/store/store_es.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/store/store_es_v2.py` & `download-center-5.3.5/download_center/store/store_es_v2.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/store/store_mongo.py` & `download-center-5.3.5/download_center/store/store_mongo.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/store/store_oss.py` & `download-center-5.3.5/download_center/store/store_oss.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/util/py_util_basestore.py` & `download-center-5.3.5/download_center/util/py_util_basestore.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/util/util_log.py` & `download-center-5.3.5/download_center/util/util_log.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center/util/util_log_v2.py` & `download-center-5.3.5/download_center/util/util_log_v2.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.3/download_center.egg-info/SOURCES.txt` & `download-center-5.3.5/download_center.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,24 @@
 demo/config.py
 demo/extractor/__init__.py
 demo/extractor/baidu_extractor.py
 demo/extractor/demo_extractor.py
 demo/spider/__init__.py
 demo/spider/config.py
 demo/spider/demo_spider.py
+demo/spider/demo_spider_list.py
 demo/spider/get_header_func.py
+demo/spider/html_py3_3.txt
+demo/spider/log.txt
 demo/spider/mum_create_html.py
 demo/store/__init__.py
 demo/store/py_store_mysql_pool.py
 download_center/__init__.py
+download_center/config.py
+download_center/requirements.txt
 download_center.egg-info/PKG-INFO
 download_center.egg-info/SOURCES.txt
 download_center.egg-info/dependency_links.txt
 download_center.egg-info/requires.txt
 download_center.egg-info/top_level.txt
 download_center/new_spider/__init__.py
 download_center/new_spider/downloader/__init__.py
@@ -27,14 +32,18 @@
 download_center/new_spider/downloader/html_downloader.py
 download_center/new_spider/downloader/html_local_downloader.py
 download_center/new_spider/downloader/html_render.py
 download_center/new_spider/spider/__init__.py
 download_center/new_spider/spider/basespider.py
 download_center/new_spider/spider/spider.py
 download_center/new_spider/util/__init__.py
+download_center/new_spider/util/ua_mobile_list.txt
+download_center/new_spider/util/ua_pc_list.txt
+download_center/new_spider/util/ua_spider_list.txt
+download_center/new_spider/util/util_baidu.py
 download_center/new_spider/util/util_baidu_relate.py
 download_center/new_spider/util/util_md5.py
 download_center/new_spider/util/util_ping.py
 download_center/new_spider/util/util_url.py
 download_center/new_spider/util/util_useragent.py
 download_center/store/__init__.py
 download_center/store/baidu_cookies.py
```

### Comparing `download-center-5.3.3/setup.py` & `download-center-5.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'download-center'
 DESCRIPTION = 'spider framework for winndoo.'
 URL = 'http://git.winndoo.cn:82/python/download_center/downloader_client.git'
 EMAIL = 'baozhu.zhang@winndoo.com'
 AUTHOR = 'Welcome#1'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '5.3.3'
+VERSION = '5.3.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'pymongo',
     'oss2',
     'redis',
     'DBUtils',
```

