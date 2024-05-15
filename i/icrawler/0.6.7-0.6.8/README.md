# Comparing `tmp/icrawler-0.6.7.tar.gz` & `tmp/icrawler-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icrawler-0.6.7.tar", last modified: Fri Jun 30 16:00:44 2023, max compression
+gzip compressed data, was "icrawler-0.6.8.tar", last modified: Wed May 15 04:20:23 2024, max compression
```

## Comparing `icrawler-0.6.7.tar` & `icrawler-0.6.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.173752 icrawler-0.6.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 16:00:39.000000 icrawler-0.6.7/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.173752 icrawler-0.6.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-30 16:00:39.000000 icrawler-0.6.7/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-30 16:00:39.000000 icrawler-0.6.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-30 16:00:39.000000 icrawler-0.6.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-30 16:00:39.000000 icrawler-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 16:00:39.000000 icrawler-0.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-30 16:00:44.177752 icrawler-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-30 16:00:39.000000 icrawler-0.6.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/builtin.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/extend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/proxy.rst
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/release_notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-30 16:00:39.000000 icrawler-0.6.7/examples/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-30 16:00:39.000000 icrawler-0.6.7/examples/filelist_demo.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/icrawler/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/icrawler/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/flickr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/urllist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/icrawler/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/storage/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/storage/google_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/icrawler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/utils/cached_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    19650 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/utils/proxy_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/utils/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/utils/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/utils/thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 16:00:43.000000 icrawler-0.6.7/icrawler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/icrawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-30 16:00:44.000000 icrawler-0.6.7/icrawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-30 16:00:44.000000 icrawler-0.6.7/icrawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:00:44.000000 icrawler-0.6.7/icrawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 16:00:44.000000 icrawler-0.6.7/icrawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 16:00:44.000000 icrawler-0.6.7/icrawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-30 16:00:39.000000 icrawler-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 16:00:39.000000 icrawler-0.6.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:00:44.177752 icrawler-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:00:39.000000 icrawler-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-30 16:00:39.000000 icrawler-0.6.7/tests/test_todo.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-30 16:00:39.000000 icrawler-0.6.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:23.001942 icrawler-0.6.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:22.993942 icrawler-0.6.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 04:20:19.000000 icrawler-0.6.8/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:22.993942 icrawler-0.6.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-15 04:20:19.000000 icrawler-0.6.8/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 04:20:19.000000 icrawler-0.6.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-15 04:20:19.000000 icrawler-0.6.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-15 04:20:19.000000 icrawler-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 04:20:19.000000 icrawler-0.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-15 04:20:23.001942 icrawler-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-15 04:20:19.000000 icrawler-0.6.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:22.993942 icrawler-0.6.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/builtin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/extend.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/proxy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-15 04:20:19.000000 icrawler-0.6.8/docs/release_notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:22.993942 icrawler-0.6.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-15 04:20:19.000000 icrawler-0.6.8/examples/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 04:20:19.000000 icrawler-0.6.8/examples/filelist_demo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:22.997942 icrawler-0.6.8/icrawler/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:22.997942 icrawler-0.6.8/icrawler/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/flickr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/builtin/urllist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:23.001942 icrawler-0.6.8/icrawler/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/storage/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/storage/google_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:23.001942 icrawler-0.6.8/icrawler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/utils/cached_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19650 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/utils/proxy_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/utils/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/utils/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-15 04:20:19.000000 icrawler-0.6.8/icrawler/utils/thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 04:20:22.000000 icrawler-0.6.8/icrawler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:23.001942 icrawler-0.6.8/icrawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-15 04:20:22.000000 icrawler-0.6.8/icrawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-15 04:20:22.000000 icrawler-0.6.8/icrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 04:20:22.000000 icrawler-0.6.8/icrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 04:20:22.000000 icrawler-0.6.8/icrawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 04:20:22.000000 icrawler-0.6.8/icrawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-15 04:20:19.000000 icrawler-0.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 04:20:19.000000 icrawler-0.6.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:20:23.001942 icrawler-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:20:19.000000 icrawler-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:20:23.001942 icrawler-0.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-15 04:20:19.000000 icrawler-0.6.8/tests/test_todo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 04:20:19.000000 icrawler-0.6.8/tox.ini
```

### Comparing `icrawler-0.6.7/.github/workflows/push.yaml` & `icrawler-0.6.8/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/.pre-commit-config.yaml` & `icrawler-0.6.8/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 default_language_version:
   python: python3
 repos:
   - repo: https://github.com/PSF/black
-    rev: 23.3.0
+    rev: 24.4.2
     hooks:
       - id: black
         args: [--safe, --quiet]
   - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
         name: isort
   # - repo: https://github.com/PyCQA/flake8
   #   rev: 6.0.0
   #   hooks:
   #     - id: flake8
   #       additional_dependencies:
   #         - flake8-bugbear
   #         - flake8-comprehensions
   #         - flake8-simplify
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.7.0
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.12.1
+    rev: 2.1.1
     hooks:
       - id: pyproject-fmt
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.4.1
+    rev: v1.10.0
     hooks:
       - id: mypy
         additional_dependencies:
           - types-requests
           - types-six
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.5
+    rev: v2.2.6
     hooks:
       - id: codespell
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.9-for-vscode
+    rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-ast
       - id: check-byte-order-marker
       - id: check-builtin-literals
       - id: check-case-conflict
       - id: check-docstring-first
```

### Comparing `icrawler-0.6.7/LICENSE` & `icrawler-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/PKG-INFO` & `icrawler-0.6.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icrawler
-Version: 0.6.7
+Version: 0.6.8
 Summary: A multi-thread crawler framework with many builtin image crawlers provided.
 Author-email: Kai Chen <chenkaidev@gmail.com>, Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Kai Chen <chenkaidev@gmail.com>, Zhiyuan Chen <this@zyc.ai>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Kai Chen
         
@@ -38,13 +38,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: bs4
+Requires-Dist: lxml
+Requires-Dist: pillow
+Requires-Dist: pyyaml
+Requires-Dist: requests
+Requires-Dist: six
```

### Comparing `icrawler-0.6.7/README.rst` & `icrawler-0.6.8/README.rst`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/docs/Makefile` & `icrawler-0.6.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/docs/api.rst` & `icrawler-0.6.8/docs/api.rst`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/docs/builtin.rst` & `icrawler-0.6.8/docs/builtin.rst`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/docs/conf.py` & `icrawler-0.6.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/docs/extend.rst` & `icrawler-0.6.8/docs/extend.rst`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/docs/make.bat` & `icrawler-0.6.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/docs/proxy.rst` & `icrawler-0.6.8/docs/proxy.rst`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/docs/release_notes.rst` & `icrawler-0.6.8/docs/release_notes.rst`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/examples/crawl.py` & `icrawler-0.6.8/examples/crawl.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/builtin/baidu.py` & `icrawler-0.6.8/icrawler/builtin/baidu.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/builtin/bing.py` & `icrawler-0.6.8/icrawler/builtin/bing.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/builtin/filter.py` & `icrawler-0.6.8/icrawler/builtin/filter.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/builtin/flickr.py` & `icrawler-0.6.8/icrawler/builtin/flickr.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/builtin/google.py` & `icrawler-0.6.8/icrawler/builtin/google.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,24 +146,29 @@
         soup = BeautifulSoup(response.content.decode("utf-8", "ignore"), "lxml")
         # image_divs = soup.find_all('script')
         image_divs = soup.find_all(name="script")
         for div in image_divs:
             # txt = div.text
             txt = str(div)
             # if not txt.startswith('AF_initDataCallback'):
-            if "AF_initDataCallback" not in txt:
-                continue
-            if "ds:0" in txt or "ds:1" not in txt:
-                continue
+            # if "AF_initDataCallback" not in txt:
+            #     continue
+            # if "ds:0" in txt or "ds:1" not in txt:
+            #     continue
             # txt = re.sub(r"^AF_initDataCallback\({.*key: 'ds:(\d)'.+data:function\(\){return (.+)}}\);?$",
             #             "\\2", txt, 0, re.DOTALL)
             # meta = json.loads(txt)
             # data = meta[31][0][12][2]
             # uris = [img[1][3][0] for img in data if img[0] == 1]
 
+            uris = re.findall(r"http[^\[]*?.(?:jpg|png|bmp)", txt)
+            uris = [bytes(uri, "utf-8").decode("unicode-escape") for uri in uris]
+            if uris:
+                return [{"file_url": uri} for uri in uris]
+
             uris = re.findall(r"http[^\[]*?\.(?:jpg|png|bmp)", txt)
             return [{"file_url": uri} for uri in uris]
 
 
 class GoogleImageCrawler(Crawler):
     def __init__(
         self, feeder_cls=GoogleFeeder, parser_cls=GoogleParser, downloader_cls=ImageDownloader, *args, **kwargs
```

### Comparing `icrawler-0.6.7/icrawler/builtin/greedy.py` & `icrawler-0.6.8/icrawler/builtin/greedy.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/builtin/urllist.py` & `icrawler-0.6.8/icrawler/builtin/urllist.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/crawler.py` & `icrawler-0.6.8/icrawler/crawler.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/downloader.py` & `icrawler-0.6.8/icrawler/downloader.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/feeder.py` & `icrawler-0.6.8/icrawler/feeder.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/parser.py` & `icrawler-0.6.8/icrawler/parser.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/storage/base.py` & `icrawler-0.6.8/icrawler/storage/base.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/storage/filesystem.py` & `icrawler-0.6.8/icrawler/storage/filesystem.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/storage/google_storage.py` & `icrawler-0.6.8/icrawler/storage/google_storage.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/utils/cached_queue.py` & `icrawler-0.6.8/icrawler/utils/cached_queue.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/utils/proxy_pool.py` & `icrawler-0.6.8/icrawler/utils/proxy_pool.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/utils/session.py` & `icrawler-0.6.8/icrawler/utils/session.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/utils/signal.py` & `icrawler-0.6.8/icrawler/utils/signal.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler/utils/thread_pool.py` & `icrawler-0.6.8/icrawler/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/icrawler.egg-info/PKG-INFO` & `icrawler-0.6.8/icrawler.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icrawler
-Version: 0.6.7
+Version: 0.6.8
 Summary: A multi-thread crawler framework with many builtin image crawlers provided.
 Author-email: Kai Chen <chenkaidev@gmail.com>, Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Kai Chen <chenkaidev@gmail.com>, Zhiyuan Chen <this@zyc.ai>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Kai Chen
         
@@ -38,13 +38,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: bs4
+Requires-Dist: lxml
+Requires-Dist: pillow
+Requires-Dist: pyyaml
+Requires-Dist: requests
+Requires-Dist: six
```

### Comparing `icrawler-0.6.7/icrawler.egg-info/SOURCES.txt` & `icrawler-0.6.8/icrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.7/pyproject.toml` & `icrawler-0.6.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 [project]
 name = "icrawler"
 description = "A multi-thread crawler framework with many builtin image crawlers provided."
 readme = "README.md"
 keywords = [
   "Crawler",
 ]
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 maintainers = [
-    {name = "Kai Chen", email = "chenkaidev@gmail.com"},
-    {name = "Zhiyuan Chen", email = "this@zyc.ai"},
+  { name = "Kai Chen", email = "chenkaidev@gmail.com" },
+  { name = "Zhiyuan Chen", email = "this@zyc.ai" },
 ]
 authors = [
-    {name = "Kai Chen", email = "chenkaidev@gmail.com"},
-    {name = "Zhiyuan Chen", email = "this@zyc.ai"},
+  { name = "Kai Chen", email = "chenkaidev@gmail.com" },
+  { name = "Zhiyuan Chen", email = "this@zyc.ai" },
 ]
 requires-python = ">=3.7"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Intended Audience :: Education",
   "Intended Audience :: Science/Research",
@@ -31,76 +31,89 @@
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Utilities",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
+  "beautifulsoup4",
+  "bs4",
+  "lxml",
+  "pillow",
   "pyyaml",
+  "requests",
+  "six",
 ]
-[project.urls]
-documentation = "https://icrawler.readthedocs.io/"
-homepage = "https://icrawler.readthedocs.io/"
-repository = "https://github.com/hellock/icrawler"
+urls.documentation = "https://icrawler.readthedocs.io/"
+urls.homepage = "https://icrawler.readthedocs.io/"
+urls.repository = "https://github.com/hellock/icrawler"
 
 [tool.setuptools]
-packages = ["icrawler"]
+packages = [
+  "icrawler",
+]
 
 [tool.setuptools_scm]
 write_to = "icrawler/version.py"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 line_length = 120
 profile = "black"
 
 [tool.flake8]
 max-line-length = 120
 
+[tool.pylint.format]
+max-line-length = 120
+
+[tool.pylint.messages_control]
+disable = """
+  E0012,
+  E0401,
+  R0201,
+  R0801,
+"""
+
+[tool.pylint.reports]
+output-format = "colorized"
+
+[tool.pylint.main]
+fail-under = 9.8
+
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --cov"
 
 [tool.coverage.run]
 branch = true
-omit = ["tests/*", "setup.py"]
+omit = [
+  "tests/*",
+  "setup.py",
+]
 
 [tool.coverage.paths]
-source = ["icrawler"]
+source = [
+  "icrawler",
+]
 
 [tool.coverage.xml]
 output = "coverage.xml"
 
 [tool.coverage.json]
 output = "coverage.json"
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.mypy]
 ignore_missing_imports = true
-
-[tool.pylint.format]
-max-line-length = 120
-
-[tool.pylint.messages_control]
-disable = """
-  E0012,
-  E0401,
-  R0201,
-  R0801,
-"""
-
-[tool.pylint.reports]
-output-format = "colorized"
-
-[tool.pylint.main]
-fail-under = 9.8
```

### Comparing `icrawler-0.6.7/tests/test_todo.py` & `icrawler-0.6.8/tests/test_todo.py`

 * *Files identical despite different names*

