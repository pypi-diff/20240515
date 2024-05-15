# Comparing `tmp/evv4esm-0.5.0.tar.gz` & `tmp/evv4esm-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evv4esm-0.5.0.tar", last modified: Mon Dec  4 21:34:42 2023, max compression
+gzip compressed data, was "evv4esm-0.5.1.tar", last modified: Wed May 15 13:49:51 2024, max compression
```

## Comparing `evv4esm-0.5.0.tar` & `evv4esm-0.5.1.tar`

### file list

```diff
@@ -1,64 +1,75 @@
-drwxr-xr-x   0 ac.mkelleher (20888) cels     (20001)        0 2023-12-04 21:34:42.507102 evv4esm-0.5.0/
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     1492 2021-06-30 02:42:06.000000 evv4esm-0.5.0/LICENSE
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)      133 2021-06-30 02:42:06.000000 evv4esm-0.5.0/MANIFEST.in
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     1938 2023-12-04 21:34:42.505845 evv4esm-0.5.0/PKG-INFO
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)      848 2023-02-01 20:01:49.000000 evv4esm-0.5.0/README.md
-drwxr-xr-x   0 ac.mkelleher (20888) cels     (20001)        0 2023-12-04 21:34:42.171444 evv4esm-0.5.0/evv4esm/
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     2744 2023-12-04 21:25:57.000000 evv4esm-0.5.0/evv4esm/__init__.py
--rwxr-xr-x   0 ac.mkelleher (20888) cels     (20001)     7485 2023-02-01 20:01:49.000000 evv4esm-0.5.0/evv4esm/__main__.py
-drwxr-xr-x   0 ac.mkelleher (20888) cels     (20001)        0 2023-12-04 21:34:42.183392 evv4esm-0.5.0/evv4esm/ensembles/
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)        0 2022-02-10 21:43:16.000000 evv4esm-0.5.0/evv4esm/ensembles/__init__.py
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     6057 2023-12-04 21:25:57.000000 evv4esm-0.5.0/evv4esm/ensembles/e3sm.py
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     8565 2023-12-04 21:25:57.000000 evv4esm-0.5.0/evv4esm/ensembles/tools.py
-drwxr-xr-x   0 ac.mkelleher (20888) cels     (20001)        0 2023-12-04 21:34:42.247875 evv4esm-0.5.0/evv4esm/extensions/
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)        0 2022-02-10 21:43:16.000000 evv4esm-0.5.0/evv4esm/extensions/__init__.py
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     4045 2021-06-30 02:42:06.000000 evv4esm-0.5.0/evv4esm/extensions/ks.bib
--rwxr-xr-x   0 ac.mkelleher (20888) cels     (20001)    16856 2023-12-04 21:25:57.000000 evv4esm-0.5.0/evv4esm/extensions/ks.py
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     3801 2021-11-17 23:37:37.000000 evv4esm-0.5.0/evv4esm/extensions/ks_vars.json
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)    16819 2023-12-04 21:25:57.000000 evv4esm-0.5.0/evv4esm/extensions/kso.py
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)      176 2023-03-08 16:47:09.000000 evv4esm-0.5.0/evv4esm/extensions/ocean_vars.json
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)      294 2021-06-30 02:42:06.000000 evv4esm-0.5.0/evv4esm/extensions/pg.bib
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)    17506 2023-12-04 21:25:57.000000 evv4esm-0.5.0/evv4esm/extensions/pg.py
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)      436 2021-06-30 02:42:06.000000 evv4esm-0.5.0/evv4esm/extensions/tsc.bib
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)    36679 2023-02-01 20:01:49.000000 evv4esm-0.5.0/evv4esm/extensions/tsc.py
-drwxr-xr-x   0 ac.mkelleher (20888) cels     (20001)        0 2023-12-04 21:34:42.288828 evv4esm-0.5.0/evv4esm/resources/
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)       25 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/.gitignore
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)       15 2022-02-10 21:43:16.000000 evv4esm-0.5.0/evv4esm/resources/__init__.py
-drwxr-xr-x   0 ac.mkelleher (20888) cels     (20001)        0 2023-12-04 21:34:42.305094 evv4esm-0.5.0/evv4esm/resources/css/
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)      918 2021-11-12 21:11:15.000000 evv4esm-0.5.0/evv4esm/resources/css/acknowledgments.css
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)      792 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/css/captionjs.min.css
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)    29503 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/css/jquery-ui.min.css
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     2831 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/css/lightbox.min.css
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     3454 2021-11-12 21:11:15.000000 evv4esm-0.5.0/evv4esm/resources/css/livv.css
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     6137 2022-01-24 15:28:42.000000 evv4esm-0.5.0/evv4esm/resources/css/normalize.css
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)    15406 2022-01-24 15:28:42.000000 evv4esm-0.5.0/evv4esm/resources/favicon.ico
-drwxr-xr-x   0 ac.mkelleher (20888) cels     (20001)        0 2023-12-04 21:34:42.443418 evv4esm-0.5.0/evv4esm/resources/imgs/
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)    17302 2021-11-12 21:11:28.000000 evv4esm-0.5.0/evv4esm/resources/imgs/DOE-BER-logo.png
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)  5268054 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/imgs/DOE-logo.png
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)    73756 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/imgs/ORNL-logo.png
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)  7312764 2021-11-12 21:11:33.000000 evv4esm-0.5.0/evv4esm/resources/imgs/background.jpg
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)      280 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/imgs/close.png
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     7517 2021-11-12 21:11:37.000000 evv4esm-0.5.0/evv4esm/resources/imgs/icon.svg
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     8476 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/imgs/loading.gif
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     1350 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/imgs/next.png
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     1360 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/imgs/prev.png
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     2841 2022-01-24 15:28:42.000000 evv4esm-0.5.0/evv4esm/resources/index.html
-drwxr-xr-x   0 ac.mkelleher (20888) cels     (20001)        0 2023-12-04 21:34:42.490986 evv4esm-0.5.0/evv4esm/resources/js/
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     4715 2023-12-04 21:25:57.000000 evv4esm-0.5.0/evv4esm/resources/js/common.js
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)   240427 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/js/jquery-ui.min.js
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     2308 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/js/jquery.caption.min.js
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)    85589 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/js/jquery.min.js
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     9372 2021-11-11 21:14:39.000000 evv4esm-0.5.0/evv4esm/resources/js/lightbox.min.js
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     9771 2022-01-24 15:28:42.000000 evv4esm-0.5.0/evv4esm/resources/js/lightbox.min.map
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     2893 2022-01-24 15:28:42.000000 evv4esm-0.5.0/evv4esm/resources/validation.html
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     3426 2022-02-10 21:43:16.000000 evv4esm-0.5.0/evv4esm/utils.py
-drwxr-xr-x   0 ac.mkelleher (20888) cels     (20001)        0 2023-12-04 21:34:42.504625 evv4esm-0.5.0/evv4esm.egg-info/
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     1938 2023-12-04 21:34:41.000000 evv4esm-0.5.0/evv4esm.egg-info/PKG-INFO
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     1592 2023-12-04 21:34:41.000000 evv4esm-0.5.0/evv4esm.egg-info/SOURCES.txt
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)        1 2023-12-04 21:34:41.000000 evv4esm-0.5.0/evv4esm.egg-info/dependency_links.txt
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)       46 2023-12-04 21:34:41.000000 evv4esm-0.5.0/evv4esm.egg-info/entry_points.txt
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)        1 2022-03-07 15:13:32.000000 evv4esm-0.5.0/evv4esm.egg-info/not-zip-safe
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)       84 2023-12-04 21:34:41.000000 evv4esm-0.5.0/evv4esm.egg-info/requires.txt
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)        8 2023-12-04 21:34:41.000000 evv4esm-0.5.0/evv4esm.egg-info/top_level.txt
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)       38 2023-12-04 21:34:42.507253 evv4esm-0.5.0/setup.cfg
--rw-r--r--   0 ac.mkelleher (20888) cels     (20001)     3478 2023-12-04 21:25:57.000000 evv4esm-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:51.767401 evv4esm-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 13:49:46.000000 evv4esm-0.5.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:51.735401 evv4esm-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:51.739401 evv4esm-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-15 13:49:46.000000 evv4esm-0.5.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-15 13:49:46.000000 evv4esm-0.5.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-15 13:49:46.000000 evv4esm-0.5.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-15 13:49:46.000000 evv4esm-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-15 13:49:46.000000 evv4esm-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-15 13:49:46.000000 evv4esm-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 13:49:46.000000 evv4esm-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-15 13:49:51.763401 evv4esm-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-15 13:49:46.000000 evv4esm-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:51.739401 evv4esm-0.5.1/evv4esm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7176 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:51.739401 evv4esm-0.5.1/evv4esm/ensembles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/ensembles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/ensembles/e3sm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/ensembles/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:51.743401 evv4esm-0.5.1/evv4esm/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/extensions/ks.bib
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16856 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/extensions/ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/extensions/ks_vars.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16820 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/extensions/kso.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/extensions/ocean_vars.json
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/extensions/pg.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/extensions/pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/extensions/tsc.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    39198 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/extensions/tsc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:51.743401 evv4esm-0.5.1/evv4esm/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:51.743401 evv4esm-0.5.1/evv4esm/resources/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/css/acknowledgments.css
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/css/captionjs.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29504 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/css/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/css/lightbox.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/css/livv.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/css/normalize.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:51.763401 evv4esm-0.5.1/evv4esm/resources/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)    17302 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/imgs/DOE-BER-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)  5268054 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/imgs/DOE-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73756 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/imgs/ORNL-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)  7312764 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/imgs/background.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/imgs/close.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/imgs/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/imgs/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/imgs/next.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/imgs/prev.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:51.763401 evv4esm-0.5.1/evv4esm/resources/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/js/common.js
+-rw-r--r--   0 runner    (1001) docker     (127)   240428 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/js/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/js/jquery.caption.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    85589 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/js/lightbox.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/js/lightbox.min.map
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/resources/validation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-15 13:49:46.000000 evv4esm-0.5.1/evv4esm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:51.763401 evv4esm-0.5.1/evv4esm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-15 13:49:51.000000 evv4esm-0.5.1/evv4esm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-15 13:49:51.000000 evv4esm-0.5.1/evv4esm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:49:51.000000 evv4esm-0.5.1/evv4esm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 13:49:51.000000 evv4esm-0.5.1/evv4esm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-15 13:49:51.000000 evv4esm-0.5.1/evv4esm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 13:49:51.000000 evv4esm-0.5.1/evv4esm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-15 13:49:46.000000 evv4esm-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:49:51.767401 evv4esm-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:49:51.763401 evv4esm-0.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-15 13:49:46.000000 evv4esm-0.5.1/test/MVK_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-15 13:49:46.000000 evv4esm-0.5.1/test/TSC_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-15 13:49:46.000000 evv4esm-0.5.1/test/test_evv.py
```

### Comparing `evv4esm-0.5.0/LICENSE` & `evv4esm-0.5.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,7 @@
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
```

### Comparing `evv4esm-0.5.0/PKG-INFO` & `evv4esm-0.5.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 Metadata-Version: 2.1
 Name: evv4esm
-Version: 0.5.0
+Version: 0.5.1
 Summary: Extended verification and validation for earth system models
-Home-page: https://github.com/LIVVkit/evv4esm
-Author: Joseph H. Kennedy
-Author-email: kennedyjh@ornl.gov
-Maintainer: Michael Kelleher
-Maintainer-email: kelleherme@ornl.gov
-License: BSD
+Author-email: Michael Kelleher <kelleherme@ornl.gov>, "Joseph H. Kennedy" <kennedyjh@ornl.gov>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/LIVVkit/evv4esm
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools
 Requires-Dist: six
 Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: pandas
+Requires-Dist: pandas>=2.1.0
 Requires-Dist: livvkit>=3.0.1
 Requires-Dist: netCDF4
 Requires-Dist: matplotlib
-Requires-Dist: pybtex
-Requires-Dist: statsmodels==0.14.0
+Requires-Dist: pybtex>=0.24.0
+Requires-Dist: statsmodels>=0.14.0
+Provides-Extra: dev
+Requires-Dist: modelmimic; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
   Extended Verification and Validation for Earth System Models
 ===============================================================================
 
 EVV is a python-based toolkit for extended verification and validation of Earth
 system models (ESMs). Currently, it provides a number tests to determine if
 modifications to an ESM is *climate changing.*
@@ -48,10 +58,10 @@
 Want to send us a private message?
 
 
 **Michael Kelleher**
 * github: @mkstratos
 * email: <a href="mailto:kelleherme@ornl.gov">kelleherme [at] ornl.gov</a>
 
-**Joseph H. Kennedy** 
+**Joseph H. Kennedy**
 * github: @jhkennedy
 * email: <a href="mailto:kennedyjh@ornl.gov">kennedyjh [at] ornl.gov</a>
```

#### html2text {}

```diff
@@ -1,23 +1,31 @@
-Metadata-Version: 2.1 Name: evv4esm Version: 0.5.0 Summary: Extended
-verification and validation for earth system models Home-page: https://
-github.com/LIVVkit/evv4esm Author: Joseph H. Kennedy Author-email:
-kennedyjh@ornl.gov Maintainer: Michael Kelleher Maintainer-email:
-kelleherme@ornl.gov License: BSD Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
-Topic :: Scientific/Engineering Classifier: Topic :: Software Development ::
-Testing Classifier: License :: OSI Approved :: BSD License Classifier:
+Metadata-Version: 2.1 Name: evv4esm Version: 0.5.1 Summary: Extended
+verification and validation for earth system models Author-email: Michael
+Kelleher
+ornl.gov>, "Joseph H. Kennedy"
+ornl.gov> License: BSD-3-Clause Project-URL: Homepage, https://github.com/
+LIVVkit/evv4esm Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Software Development :: Testing
+Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
+:: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: six Requires-Dist: numpy Requires-Dist: scipy Requires-Dist:
-pandas Requires-Dist: livvkit>=3.0.1 Requires-Dist: netCDF4 Requires-Dist:
-matplotlib Requires-Dist: pybtex Requires-Dist: statsmodels==0.14.0 Extended
-Verification and Validation for Earth System Models
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Requires-Python: >=3.6 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: setuptools Requires-Dist: six Requires-
+Dist: numpy Requires-Dist: scipy Requires-Dist: pandas>=2.1.0 Requires-Dist:
+livvkit>=3.0.1 Requires-Dist: netCDF4 Requires-Dist: matplotlib Requires-Dist:
+pybtex>=0.24.0 Requires-Dist: statsmodels>=0.14.0 Provides-Extra: dev Requires-
+Dist: modelmimic; extra == "dev" Requires-Dist: ruff; extra == "dev" Requires-
+Dist: black; extra == "dev" Requires-Dist: isort; extra == "dev" Requires-Dist:
+pytest; extra == "dev" Extended Verification and Validation for Earth System
+Models
 ===============================================================================
 EVV is a python-based toolkit for extended verification and validation of Earth
 system models (ESMs). Currently, it provides a number tests to determine if
 modifications to an ESM is *climate changing.* Contact =========== If you would
 like to suggest features, request tests, discuss contributions, report bugs,
 ask questions, or contact us for any reason, use the [Issue Tracker](https://
 github.com/LIVVkit/evv4esm/issues). Want to send us a private message?
```

### Comparing `evv4esm-0.5.0/README.md` & `evv4esm-0.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 Want to send us a private message?
 
 
 **Michael Kelleher**
 * github: @mkstratos
 * email: <a href="mailto:kelleherme@ornl.gov">kelleherme [at] ornl.gov</a>
 
-**Joseph H. Kennedy** 
+**Joseph H. Kennedy**
 * github: @jhkennedy
 * email: <a href="mailto:kennedyjh@ornl.gov">kennedyjh [at] ornl.gov</a>
```

### Comparing `evv4esm-0.5.0/evv4esm/__init__.py` & `evv4esm-0.5.1/evv4esm/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,39 +24,54 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
-__version_info__ = (0, 5, 0)
-__version__ = '.'.join(str(vi) for vi in __version_info__)
+__version_info__ = (0, 5, 1)
+__version__ = ".".join(str(vi) for vi in __version_info__)
 
-PASS_COLOR = '#389933'
-L_PASS_COLOR = '#93DA90'
+PASS_COLOR = "#389933"
+L_PASS_COLOR = "#93DA90"
 
-FAIL_COLOR = '#BF3F46'
-L_FAIL_COLOR = '#E68388'
+FAIL_COLOR = "#BF3F46"
+L_FAIL_COLOR = "#E68388"
 
-human_color_names = {'pass': ('green', 'light green'),
-                     PASS_COLOR: 'green',
-                     L_PASS_COLOR: 'light green',
-                     'fail': ('red', 'light red'),
-                     FAIL_COLOR: 'red',
-                     L_FAIL_COLOR: 'light red'}
-
-pf_color_picker = {'Pass': PASS_COLOR, 'pass': PASS_COLOR,
-                   'Accept': PASS_COLOR, 'accept': PASS_COLOR,
-                   'Fail': FAIL_COLOR, 'fail': FAIL_COLOR,
-                   'Reject': FAIL_COLOR, 'reject': FAIL_COLOR}
-
-light_pf_color_picker = {'Pass': L_PASS_COLOR, 'pass': L_PASS_COLOR,
-                         'Accept': L_PASS_COLOR, 'accept': L_PASS_COLOR,
-                         PASS_COLOR: L_PASS_COLOR,
-                         'Fail': L_FAIL_COLOR, 'fail': L_FAIL_COLOR,
-                         'Reject': L_FAIL_COLOR, 'reject': L_FAIL_COLOR,
-                         FAIL_COLOR: L_FAIL_COLOR}
+human_color_names = {
+    "pass": ("green", "light green"),
+    PASS_COLOR: "green",
+    L_PASS_COLOR: "light green",
+    "fail": ("red", "light red"),
+    FAIL_COLOR: "red",
+    L_FAIL_COLOR: "light red",
+}
+
+pf_color_picker = {
+    "Pass": PASS_COLOR,
+    "pass": PASS_COLOR,
+    "Accept": PASS_COLOR,
+    "accept": PASS_COLOR,
+    "Fail": FAIL_COLOR,
+    "fail": FAIL_COLOR,
+    "Reject": FAIL_COLOR,
+    "reject": FAIL_COLOR,
+}
+
+light_pf_color_picker = {
+    "Pass": L_PASS_COLOR,
+    "pass": L_PASS_COLOR,
+    "Accept": L_PASS_COLOR,
+    "accept": L_PASS_COLOR,
+    PASS_COLOR: L_PASS_COLOR,
+    "Fail": L_FAIL_COLOR,
+    "fail": L_FAIL_COLOR,
+    "Reject": L_FAIL_COLOR,
+    "reject": L_FAIL_COLOR,
+    FAIL_COLOR: L_FAIL_COLOR,
+}
 
 
 class EVVException(Exception):
     """Base class for EVV exceptions"""
+
     pass
```

### Comparing `evv4esm-0.5.0/evv4esm/__main__.py` & `evv4esm-0.5.1/evv4esm/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,164 +1,193 @@
 #!/usr/bin/env python
 # coding=utf-8
 # Copyright (c) 2018 UT-BATTELLE, LLC
 # All rights reserved.
-# 
+#
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
-# 
+#
 # 1. Redistributions of source code must retain the above copyright notice, this
 # list of conditions and the following disclaimer.
-# 
+#
 # 2. Redistributions in binary form must reproduce the above copyright notice,
 # this list of conditions and the following disclaimer in the documentation
 # and/or other materials provided with the distribution.
-# 
+#
 # 3. Neither the name of the copyright holder nor the names of its contributors
 # may be used to endorse or promote products derived from this software without
 # specific prior written permission.
-# 
+#
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
 # ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import argparse
 import os
 import sys
 import time
-import argparse
 
-import evv4esm
 import livvkit
 from livvkit.util import options
 
+import evv4esm
+
 
 def parse_args(args=None):
-    parser = argparse.ArgumentParser(description=__doc__,
-                                     formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-
-    parser.add_argument('-e', '--extensions',
-                        action='store',
-                        nargs='+',
-                        default=None,
-                        help='Specify the location of the JSON configuration files for the extended V&V tests to run.')
-  
-    parser.add_argument('-o', '--out-dir',
-                        default=os.path.join(os.getcwd(), "vv_" + time.strftime("%Y-%m-%d")),
-                        help='Location to output the EVV webpages.')
-
-    parser.add_argument('-s', '--serve',
-                        nargs='?', type=int, const=8000,
-                        help=' '.join(['Start a simple HTTP server for the output website specified',
-                                       'by OUT_DIR on port SERVE.'
-                                       ])
-                        )
-
-    parser.add_argument('-p', '--pool-size',
-                        nargs='?',
-                        type=int,
-                        default=(options.mp.cpu_count() - 1 or 1),
-                        help='The number of multiprocessing processes to run '
-                             'analyses in. If zero, processes will run serially '
-                             'outside of the multiprocessing module.')
-
-    parser.add_argument('--version',
-                        action='version',
-                        version='EVV {}'.format(evv4esm.__version__),
-                        help="Show EVV's version number and exit"
-                        )
+    parser = argparse.ArgumentParser(
+        description=__doc__, formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
+
+    parser.add_argument(
+        "-e",
+        "--extensions",
+        action="store",
+        nargs="+",
+        default=None,
+        help="Specify the location of the JSON configuration files for the extended V&V tests to run.",
+    )
+
+    parser.add_argument(
+        "-o",
+        "--out-dir",
+        default=os.path.join(os.getcwd(), "vv_" + time.strftime("%Y-%m-%d")),
+        help="Location to output the EVV webpages.",
+    )
+
+    parser.add_argument(
+        "-s",
+        "--serve",
+        nargs="?",
+        type=int,
+        const=8000,
+        help=" ".join(
+            [
+                "Start a simple HTTP server for the output website specified",
+                "by OUT_DIR on port SERVE.",
+            ]
+        ),
+    )
+
+    parser.add_argument(
+        "-p",
+        "--pool-size",
+        nargs="?",
+        type=int,
+        default=(options.mp.cpu_count() - 1 or 1),
+        help="The number of multiprocessing processes to run "
+        "analyses in. If zero, processes will run serially "
+        "outside of the multiprocessing module.",
+    )
+
+    parser.add_argument(
+        "--version",
+        action="version",
+        version="EVV {}".format(evv4esm.__version__),
+        help="Show EVV's version number and exit",
+    )
 
     args = parser.parse_args(args)
 
     if args.extensions:
-        options.parse_args(['-V']+args.extensions + ['-o', args.out_dir])
-    
+        options.parse_args(["-V"] + args.extensions + ["-o", args.out_dir])
+
     from evv4esm import resources
+
     args.livv_resource_dir = livvkit.resource_dir
     livvkit.resource_dir = os.sep.join(resources.__path__)
     return args
 
 
 def main(cl_args=None):
-    """ Direct execution. """
+    """Direct execution."""
 
     if cl_args is None and len(sys.argv) > 1:
         cl_args = sys.argv[1:]
     args = parse_args(cl_args)
 
-    print("--------------------------------------------------------------------")
-    print("                   ______  __      __ __      __                    ")
-    print("                  |  ____| \ \    / / \ \    / /                    ")
-    print("                  | |__     \ \  / /   \ \  / /                     ")
-    print("                  |  __|     \ \/ /     \ \/ /                      ")
-    print("                  | |____     \  /       \  /                       ")
-    print("                  |______|     \/         \/                        ")
-    print("                                                                    ")
-    print("    Extended Verification and Validation for Earth System Models    ")
-    print("--------------------------------------------------------------------")
+    print(r"--------------------------------------------------------------------")
+    print(r"                   ______  __      __ __      __                    ")
+    print(r"                  |  ____| \ \    / / \ \    / /                    ")
+    print(r"                  | |__     \ \  / /   \ \  / /                     ")
+    print(r"                  |  __|     \ \/ /     \ \/ /                      ")
+    print(r"                  | |____     \  /       \  /                       ")
+    print(r"                  |______|     \/         \/                        ")
+    print(r"                                                                    ")
+    print(r"    Extended Verification and Validation for Earth System Models    ")
+    print(r"--------------------------------------------------------------------")
     print("")
     print("  Current run: " + livvkit.timestamp)
     print("  User: " + livvkit.user)
     print("  OS Type: " + livvkit.os_type)
     print("  Machine: " + livvkit.machine)
     print("  " + livvkit.comment)
 
+    from livvkit import elements, scheduler
     from livvkit.components import validation
-    from livvkit import scheduler
     from livvkit.util import functions
-    from livvkit import elements
 
     livvkit.pool_size = args.pool_size
     if args.extensions:
         functions.setup_output()
         summary_elements = []
         validation_config = {}
         print(" -----------------------------------------------------------------")
         print("   Beginning extensions test suite ")
         print(" -----------------------------------------------------------------")
         print("")
         for conf in livvkit.validation_model_configs:
-            validation_config = functions.merge_dicts(validation_config,
-                                                      functions.read_json(conf))
-            summary_elements.extend(scheduler.run_quiet("validation", validation, validation_config,
-                                                        group=False))
+            validation_config = functions.merge_dicts(
+                validation_config, functions.read_json(conf)
+            )
+            summary_elements.extend(
+                scheduler.run_quiet(
+                    "validation", validation, validation_config, group=False
+                )
+            )
         print(" -----------------------------------------------------------------")
         print("   Extensions test suite complete ")
         print(" -----------------------------------------------------------------")
         print("")
 
         result = elements.Page("Summary", "", elements=summary_elements)
         with open(os.path.join(livvkit.output_dir, "index.json"), "w") as index_data:
             index_data.write(result._repr_json())
         print("-------------------------------------------------------------------")
         print(" Done!  Results can be seen in a web browser at:")
-        print("   " + os.path.join(livvkit.output_dir, 'index.html'))
+        print("   " + os.path.join(livvkit.output_dir, "index.html"))
         print("-------------------------------------------------------------------")
 
     if args.serve:
         import http.server as server
         import socketserver as socket
 
-        httpd = socket.TCPServer(('', args.serve), server.SimpleHTTPRequestHandler)
+        httpd = socket.TCPServer(("", args.serve), server.SimpleHTTPRequestHandler)
 
         sa = httpd.socket.getsockname()
-        print('\nServing HTTP on {host} port {port} (http://{host}:{port}/)'.format(host=sa[0], port=sa[1]))
-        print('\nView the generated website by navigating to:')
-        print('\n    http://{host}:{port}/{path}/index.html'.format(host=sa[0], port=sa[1],
-                                                                    path=os.path.relpath(args.out_dir)
-                                                                    ))
-        print('\nExit by pressing `ctrl+c` to send a keyboard interrupt.\n')
+        print(
+            "\nServing HTTP on {host} port {port} (http://{host}:{port}/)".format(
+                host=sa[0], port=sa[1]
+            )
+        )
+        print("\nView the generated website by navigating to:")
+        print(
+            "\n    http://{host}:{port}/{path}/index.html".format(
+                host=sa[0], port=sa[1], path=os.path.relpath(args.out_dir)
+            )
+        )
+        print("\nExit by pressing `ctrl+c` to send a keyboard interrupt.\n")
         try:
             httpd.serve_forever()
         except KeyboardInterrupt:
-            print('\nKeyboard interrupt received, exiting.\n')
+            print("\nKeyboard interrupt received, exiting.\n")
             sys.exit(0)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `evv4esm-0.5.0/evv4esm/ensembles/e3sm.py` & `evv4esm-0.5.1/evv4esm/ensembles/e3sm.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,25 +26,23 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """E3SM specific ensemble functions."""
 
-import six
-
+import glob
 import os
 import re
-import glob
-
 from collections import OrderedDict
 from functools import partial
 
 import numpy as np
 import pandas as pd
+import six
 from netCDF4 import Dataset
 
 
 def component_file_instance(component, case_file):
     search_regex = r"{c}_[0-9]+".format(c=component)
     result = re.search(search_regex, case_file).group(0)
     return int(result.replace("{}_".format(component), ""))
@@ -60,23 +58,27 @@
     else:
         search_regex = r"{}\.[0-9]+-[0-9]+.nc".format(hist_name)
 
     result = re.search(search_regex, case_file).group(0)
     return result.replace("{}.".format(hist_name), "").replace(".nc", "")
 
 
-def component_monthly_files(dir_, component, ninst, hist_name="h0", nmonth_max=12, date_style="short"):
+def component_monthly_files(
+    dir_, component, ninst, hist_name="h0", nmonth_max=12, date_style="short"
+):
     if date_style == "full":
         date_search = "????-??-??-??"
     elif date_style == "med":
         date_search = "????-??-??"
     else:
         date_search = "????-??"
 
-    base = "{d}/*{c}_????.{n}.{ds}.nc".format(d=dir_, c=component, n=hist_name, ds=date_search)
+    base = "{d}/*{c}_????.{n}.{ds}.nc".format(
+        d=dir_, c=component, n=hist_name, ds=date_search
+    )
     search = os.path.normpath(base)
     result = sorted(glob.glob(search))
 
     instance_files = OrderedDict()
     _file_date_str = partial(file_date_str, style=date_style, hist_name=hist_name)
     for ii in range(1, ninst + 1):
         instance_files[ii] = sorted(
@@ -111,30 +113,44 @@
 
                 data = None
                 try:
                     data = Dataset(file_)
                     if variable_set is None:
                         variable_set = set(data.variables.keys())
                 except OSError as E:
-                    six.raise_from(BaseException('Could not open netCDF dataset: {}'.format(file_)), E)
+                    six.raise_from(
+                        BaseException(
+                            "Could not open netCDF dataset: {}".format(file_)
+                        ),
+                        E,
+                    )
 
                 for var in data.variables.keys():
                     if var not in variable_set:
                         continue
-                    if len(data.variables[var].shape) < 2 or var in ['time_bnds', 'date_written', 'time_written']:
+                    if len(data.variables[var].shape) < 2 or var in [
+                        "time_bnds",
+                        "date_written",
+                        "time_written",
+                    ]:
                         continue
-                    elif 'ncol' not in data.variables[var].dimensions:
+                    elif "ncol" not in data.variables[var].dimensions:
                         continue
                     else:
                         m = np.mean(data.variables[var][0, ...])
 
                     desc = "{long_name}{units}".format(**get_variable_meta(data, var))
-                    monthly_avgs.append((case, var, '{:04}'.format(inst), date_str, m, desc))
-
-    monthly_avgs = pd.DataFrame(monthly_avgs, columns=('case', 'variable', 'instance', 'date', 'monthly_mean', 'desc'))
+                    monthly_avgs.append(
+                        (case, var, "{:04}".format(inst), date_str, m, desc)
+                    )
+
+    monthly_avgs = pd.DataFrame(
+        monthly_avgs,
+        columns=("case", "variable", "instance", "date", "monthly_mean", "desc"),
+    )
     return monthly_avgs
 
 
 def load_mpas_climatology_ensemble(files, field_name, mask_value=None):
     # Get the first file to set up ensemble array output
     with Dataset(files[0], "r") as dset:
         _field = dset.variables[field_name][:].squeeze()
```

### Comparing `evv4esm-0.5.0/evv4esm/ensembles/tools.py` & `evv4esm-0.5.1/evv4esm/ensembles/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """General tools for working with ensembles."""
 import os
+
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
-from matplotlib.gridspec import GridSpec
 
-from evv4esm import pf_color_picker, light_pf_color_picker
+from evv4esm import light_pf_color_picker, pf_color_picker
 
 
 def monthly_to_annual_avg(var_data, cal="ignore"):
     if len(var_data) != 12:
         raise ValueError(
             "Error! There are 12 months in a year; "
             "you passed in {} monthly averages.".format(len(var_data))
@@ -166,18 +166,24 @@
                 label=test_name,
             )
             ax4.set_xlim(tuple(norm_rng))
             ax4.legend()
 
         else:
             ax3.hist(
-                norm_ref, bins=n_q, color=pf_color_picker.get(pf, "#1F77B4"), edgecolor="k"
+                norm_ref,
+                bins=n_q,
+                color=pf_color_picker.get(pf, "#1F77B4"),
+                edgecolor="k",
             )
             ax4.hist(
-                norm_test, bins=n_q, color=pf_color_picker.get(pf, "#1F77B4"), edgecolor="k"
+                norm_test,
+                bins=n_q,
+                color=pf_color_picker.get(pf, "#1F77B4"),
+                edgecolor="k",
             )
 
             # Check if these distributions are wildly different. If they are, use different
             # colours for the bottom axis? Otherwise set the scales to be the same [0, 1]
             if abs(norm_ref.mean() - norm_test.mean()) >= 0.5:
                 ax3.tick_params(axis="x", colors="C0")
                 ax3.spines["bottom"].set_color("C0")
```

### Comparing `evv4esm-0.5.0/evv4esm/extensions/ks.bib` & `evv4esm-0.5.1/evv4esm/extensions/ks.bib`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,7 @@
 pages = {1094342019837341},
 year = {0},
 doi = {10.1177/1094342019837341},
 URL = {https://doi.org/10.1177/1094342019837341},
 eprint = {https://doi.org/10.1177/1094342019837341},
 abstract = {We present a methodology for solution reproducibility for the Energy Exascale Earth System Model during its ongoing software infrastructure development to prepare for exascale computers. The nonlinear chaotic nature of climate system simulations precludes traditional model verification approaches since machine precision differences—resulting from code refactoring, changes in software environment, and so on—grow exponentially to a different weather state. Here, we leverage the nature of climate as a statistical description of the atmosphere in order to establish model reproducibility. We evaluate the degree to which two-sample equality of distribution tests can confidently detect the change in climate from minor tuning parameter changes on model output variables in order to establish the level of difference that indicates a new climate. To apply this (baselined test), we target a section of the model’s development cycle wherein no intentional science changes have been applied to its source code. We compare an ensemble of short simulations that were conducted using a verified model configuration against a new ensemble with the same configuration but with the latest software infrastructure (Common Infrastructure for Modeling the Earth, CIME5.0), compiler versions, and software libraries. We also compare these against ensemble simulations conducted using the original version of the software infrastructure (CIME4.0) of the earlier model configuration, but with the latest compilers and software libraries, to test the impact of new compilers and libraries in isolation from additional software infrastructure. The two-sample equality of distribution tests indicates that these ensembles indeed represent the same climate.}
 }
-
```

### Comparing `evv4esm-0.5.0/evv4esm/extensions/ks.py` & `evv4esm-0.5.1/evv4esm/extensions/ks.py`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/extensions/ks_vars.json` & `evv4esm-0.5.1/evv4esm/extensions/ks_vars.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -231,8 +231,8 @@
 00000e60: 6f34 5f61 335f 5352 4622 2c0a 2020 2020  o4_a3_SRF",.    
 00000e70: 2020 2020 2020 2020 2020 2273 6f61 5f61            "soa_a
 00000e80: 315f 3222 2c0a 2020 2020 2020 2020 2020  1_2",.          
 00000e90: 2020 2020 2273 6f61 5f61 315f 5352 4622      "soa_a1_SRF"
 00000ea0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00000eb0: 2273 6f61 5f61 325f 3222 2c0a 2020 2020  "soa_a2_2",.    
 00000ec0: 2020 2020 2020 2020 2020 2273 6f61 5f61            "soa_a
-00000ed0: 325f 5352 4622 5d0a 7d                   2_SRF"].}
+00000ed0: 325f 5352 4622 5d0a 7d0a                 2_SRF"].}.
```

### Comparing `evv4esm-0.5.0/evv4esm/extensions/kso.py` & `evv4esm-0.5.1/evv4esm/extensions/kso.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,24 +48,25 @@
 from collections import OrderedDict
 from pathlib import Path
 from pprint import pprint
 
 import livvkit
 import numpy as np
 import pandas as pd
-from evv4esm import EVVException, human_color_names
-from evv4esm.ensembles import e3sm
-from evv4esm.ensembles.tools import prob_plot
-from evv4esm.utils import bib2html
 from livvkit import elements as el
 from livvkit.util import functions as fn
 from livvkit.util.LIVVDict import LIVVDict
 from scipy import stats
 from statsmodels.stats import multitest as smm
 
+from evv4esm import EVVException, human_color_names
+from evv4esm.ensembles import e3sm
+from evv4esm.ensembles.tools import prob_plot
+from evv4esm.utils import bib2html
+
 
 def variable_set(name):
     var_sets = fn.read_json(os.path.join(os.path.dirname(__file__), "ocean_vars.json"))
     try:
         the_set = var_sets[name.lower()]
         return set(the_set)
     except KeyError as _err:
```

### Comparing `evv4esm-0.5.0/evv4esm/extensions/pg.py` & `evv4esm-0.5.1/evv4esm/extensions/pg.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,53 +32,50 @@
 This tests the null hypothesis that the reference (n) and modified (m) model
 ensembles represent the same atmospheric state after each physics parameterization
 is applied within a single time-step using the two-sample (n and m) T-test for equal
 averages at a 95% confidence level. Ensembles are generated by repeating the
 simulation for many initial conditions, with each initial condition subject to
 multiple perturbations.
 """
-import six
-
-import os
-import math
 import argparse
-# import logging
+import math
+import os
+from collections import OrderedDict
 from pathlib import Path
-
 from pprint import pprint
-from collections import OrderedDict
 
+import livvkit
+import matplotlib.patches as mpatches
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-
-import matplotlib.pyplot as plt
-import matplotlib.patches as mpatches
-
-from scipy import stats
-from netCDF4 import Dataset
-
-import livvkit
+import six
 from livvkit import elements as el
 from livvkit.util import functions as fn
-from livvkit.util.LIVVDict import LIVVDict
+from netCDF4 import Dataset
+from scipy import stats
 
 from evv4esm.utils import bib2html
 
 # logger = logging.getLogger(__name__)
 
 
 def parse_args(args=None):
-    parser = argparse.ArgumentParser(description=__doc__,
-                                     formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser = argparse.ArgumentParser(
+        description=__doc__, formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
 
-    parser.add_argument('-c', '--config',
-                        type=fn.read_json,
-                        default='test/pge_pc0101123.json',
-                        help='A JSON config file containing a `pg` dictionary defining ' +
-                             'the options.')
+    parser.add_argument(
+        "-c",
+        "--config",
+        type=fn.read_json,
+        default="test/pge_pc0101123.json",
+        help="A JSON config file containing a `pg` dictionary defining "
+        + "the options.",
+    )
 
     args = parser.parse_args(args)
     name = args.config.keys()[0]
     config = args.config[name]
 
     return name, config
 
@@ -89,15 +86,17 @@
     perturbation index (pi)  subscripts
 
     instances use 1-based indexes and vary according to this function:
         ii = ci * len(PERTURBATIONS) + pi + 1
     where both pi and ci use 0-based indexes.
     """
     perturbation_index = (instance_number - 1) % total_perturbations
-    initial_condition = (instance_number - 1 - perturbation_index) // total_perturbations
+    initial_condition = (
+        instance_number - 1 - perturbation_index
+    ) // total_perturbations
     return initial_condition, perturbation_index
 
 
 def _sub2instance(initial_condition, perturbation_index, total_perturbations):
     """
     Converts initial condition index (ci) and perturbation index (pi) subscripts
     to an instance number (ii)
@@ -106,48 +105,55 @@
         ii = ci * len(PERTURBATIONS) + pi + 1
     where both pi and ci use 0-based indexes.
     """
     instance = initial_condition * total_perturbations + perturbation_index + 1
     return instance
 
 
-def rmse_writer(file_name, rmse, perturbation_names, perturbation_variables, init_file_template, model_name):
+def rmse_writer(
+    file_name,
+    rmse,
+    perturbation_names,
+    perturbation_variables,
+    init_file_template,
+    model_name,
+):
     """
     Opens and writes a netcdf file for PGE curves
     This function is here purely to avoid duplicate
     codes so that it is easy to maintain code longterm
     """
 
-    with Dataset(file_name, 'w') as nc:
+    with Dataset(file_name, "w") as nc:
         ninit, nprt_m1, nvars = rmse.shape
 
-        nc.createDimension('ninit', ninit)
-        nc.createDimension('nprt', nprt_m1 + 1)
-        nc.createDimension('nprt_m1', nprt_m1)
-        nc.createDimension('nvars', nvars)
-
-        nc_init_cond = nc.createVariable('init_cond_files', str, 'ninit')
-        nc_perturbation = nc.createVariable('perturbation_names', str, 'nprt')
-        nc_variables = nc.createVariable('perturbation_variables', str, 'nvars')
-        nc_rmse = nc.createVariable('rmse', 'f8', ('ninit', 'nprt_m1', 'nvars'))
+        nc.createDimension("ninit", ninit)
+        nc.createDimension("nprt", nprt_m1 + 1)
+        nc.createDimension("nprt_m1", nprt_m1)
+        nc.createDimension("nvars", nvars)
+
+        nc_init_cond = nc.createVariable("init_cond_files", str, "ninit")
+        nc_perturbation = nc.createVariable("perturbation_names", str, "nprt")
+        nc_variables = nc.createVariable("perturbation_variables", str, "nvars")
+        nc_rmse = nc.createVariable("rmse", "f8", ("ninit", "nprt_m1", "nvars"))
 
         # NOTE: Assignment to netcdf4 variable length string array can be done
         #       via numpy arrays, or in a for loop using integer indices.
         # NOTE: Numpy arrays can't be created from a generator for some dumb reason,
         #       so protect with list
         nc_perturbation[:] = np.array(list(perturbation_names))
         nc_variables[:] = np.array(list(perturbation_variables))
         nc_rmse[:] = rmse[:]
 
         for icond in range(0, ninit):
             # NOTE: Zero vs One based indexing
-            nc_init_cond[icond] = init_file_template.format(model_name, 'i', icond+1)
+            nc_init_cond[icond] = init_file_template.format(model_name, "i", icond + 1)
 
 
-def variables_rmse(ifile_test, ifile_cntl, var_list, var_pefix=''):
+def variables_rmse(ifile_test, ifile_cntl, var_list, var_pefix=""):
     """
     Compute RMSE difference between perturbation and control for a set of
     variables
 
     Args:
          ifile_test: Path to a NetCDF dataset for a perturbed simulation
          ifile_cntl: Path to a NetCDF dataset for the control simulation
@@ -157,196 +163,240 @@
     returns:
         rmse (pandas.DataFrame): A dataframe containing the RMSE and maximum
             difference details between the perturbed and control simulation
 
     """
 
     with Dataset(ifile_test) as ftest, Dataset(ifile_cntl) as fcntl:
-        lat = ftest.variables['lat']
-        lon = ftest.variables['lon']
+        lat = ftest.variables["lat"]
+        lon = ftest.variables["lon"]
 
-        rmse = pd.DataFrame(columns=('RMSE', 'max diff', 'i', 'j', 'control', 'test', 'lat', 'lon'), index=var_list)
+        rmse = pd.DataFrame(
+            columns=("RMSE", "max diff", "i", "j", "control", "test", "lat", "lon"),
+            index=var_list,
+        )
 
         # reshape for RMSE
         dims = len(ftest.variables[var_pefix + var_list[0]].dimensions)
         if dims == 3:  # see if it is SE grid
             nx, ny = ftest.variables[var_pefix + var_list[0]][0, ...].shape
             nz = 1
         else:
             nx, ny, nz = ftest.variables[var_pefix + var_list[0]][0, ...].shape
 
         for ivar, vvar in enumerate(var_list):
             var = var_pefix + vvar
             if var in ftest.variables:
-                vtest = ftest.variables[var.strip()][0, ...]  # first dimension is time (=0)
-                vcntl = fcntl.variables[var.strip()][0, ...]  # first dimension is time (=0)
+                vtest = ftest.variables[var.strip()][
+                    0, ...
+                ]  # first dimension is time (=0)
+                vcntl = fcntl.variables[var.strip()][
+                    0, ...
+                ]  # first dimension is time (=0)
 
-                vrmse = math.sqrt(((vtest - vcntl)**2).mean()) / np.mean(vcntl)
+                vrmse = math.sqrt(((vtest - vcntl) ** 2).mean()) / np.mean(vcntl)
 
                 diff = abs(vtest[...] - vcntl[...])
                 ind_max = np.unravel_index(diff.argmax(), diff.shape)
 
-                rmse.loc[vvar] = (vrmse, diff[ind_max], ind_max[0], ind_max[1],
-                                  vcntl[ind_max], vtest[ind_max],
-                                  lat[ind_max[1]], lon[ind_max[1]])
+                rmse.loc[vvar] = (
+                    vrmse,
+                    diff[ind_max],
+                    ind_max[0],
+                    ind_max[1],
+                    vcntl[ind_max],
+                    vtest[ind_max],
+                    lat[ind_max[1]],
+                    lon[ind_max[1]],
+                )
     return rmse
 
 
 def _print_details(details):
     for set_ in details:
-        print('-' * 80)
+        print("-" * 80)
         print(set_)
-        print('-' * 80)
+        print("-" * 80)
         pprint(details[set_])
 
 
 def main(args):
-    
+
     nvar = len(args.variables)
     nprt = len(args.perturbations)
 
     # for test cases (new environment etc.)
     # logger.debug("PGN_INFO: Test case comparison...")
 
     rmse_prototype = {}
     for icond in range(args.ninit):
         prt_rmse = {}
         for iprt, prt_name in enumerate(args.perturbations):
-            if prt_name == 'woprt':
+            if prt_name == "woprt":
                 continue
             iinst_ctrl = _sub2instance(icond, 0, nprt)
-            ifile_ctrl = os.path.join(args.ref_dir,
-                                      args.instance_file_template.format('', args.component, iinst_ctrl, '_woprt'))
+            ifile_ctrl = os.path.join(
+                args.ref_dir,
+                args.instance_file_template.format(
+                    "", args.component, iinst_ctrl, "_woprt"
+                ),
+            )
             # logger.debug("PGN_INFO:CNTL_TST:" + ifile_cntl)
 
             iinst_test = _sub2instance(icond, iprt, nprt)
-            ifile_test = os.path.join(args.test_dir,
-                                      args.instance_file_template.format(
-                                              args.test_case + '.', args.component, iinst_test, '_' + prt_name))
+            ifile_test = os.path.join(
+                args.test_dir,
+                args.instance_file_template.format(
+                    args.test_case + ".", args.component, iinst_test, "_" + prt_name
+                ),
+            )
             # logger.debug("PGN_INFO:TEST_TST:" + ifile_test)
 
-            prt_rmse[prt_name] = variables_rmse(ifile_test, ifile_ctrl, args.variables, 't_')
+            prt_rmse[prt_name] = variables_rmse(
+                ifile_test, ifile_ctrl, args.variables, "t_"
+            )
 
         rmse_prototype[icond] = pd.concat(prt_rmse)
 
     rmse = pd.concat(rmse_prototype)
-    comp_rmse = np.reshape(rmse.RMSE.values, (args.ninit, nprt-1, nvar))
+    comp_rmse = np.reshape(rmse.RMSE.values, (args.ninit, nprt - 1, nvar))
 
-    rmse_writer(os.path.join(args.test_dir, 'comp_cld.nc'),
-                comp_rmse, args.perturbations.keys(), args.variables, args.init_file_template, args.init_model)
+    rmse_writer(
+        os.path.join(args.test_dir, "comp_cld.nc"),
+        comp_rmse,
+        args.perturbations.keys(),
+        args.variables,
+        args.init_file_template,
+        args.init_model,
+    )
 
     details = OrderedDict()
     with Dataset(os.path.join(args.ref_dir, args.pge_cld)) as ref_cld:
-        ref_dims = ref_cld.variables['rmse'].shape
+        ref_dims = ref_cld.variables["rmse"].shape
         cmp_dims = (args.ninit, nprt - 1, nvar)
         try:
-            assert(ref_dims == cmp_dims)
+            assert ref_dims == cmp_dims
         except AssertionError as e:
             be = BaseException(
-                    'PGE curve dimensions (ninit, nptr, nvar) should be the same:\n'
-                    '    CLD:{}  COMP:{}'.format(ref_dims, cmp_dims))
+                "PGE curve dimensions (ninit, nptr, nvar) should be the same:\n"
+                "    CLD:{}  COMP:{}".format(ref_dims, cmp_dims)
+            )
             six.raise_from(be, e)
 
-        ref_rmse = ref_cld.variables['rmse'][...]
-        details['ref. data'] = ref_rmse
+        ref_rmse = ref_cld.variables["rmse"][...]
+        details["ref. data"] = ref_rmse
 
     pge_ends_cld = ref_rmse[:, :, -1]
     pge_ends_comp = comp_rmse[:, :, -1]
 
     # run the t-test
     pge_ends_cld = pge_ends_cld.flatten().astype(np.float32)
     pge_ends_comp = pge_ends_comp.flatten().astype(np.float32)
     t_stat, p_val = stats.ttest_ind(pge_ends_cld, pge_ends_comp)
 
     if np.isnan((t_stat, p_val)).any() or np.isinf((t_stat, p_val)).any():
-        details['T test (t, p)'] = (None, None)
+        details["T test (t, p)"] = (None, None)
     else:
-        details['T test (t, p)'] = '({:.3f}, {:.3f})'.format(t_stat, p_val)
+        details["T test (t, p)"] = "({:.3f}, {:.3f})".format(t_stat, p_val)
 
     # logger.warn(" T value:" + str(t_stat))
     # logger.warn(" P value:" + str(p_val))
     crit = 0.05
     if t_stat is None:
-        details['h0'] = '-'
+        details["h0"] = "-"
     elif p_val < crit:
-        details['h0'] = 'reject'
+        details["h0"] = "reject"
     else:
-        details['h0'] = 'accept'
+        details["h0"] = "accept"
 
     # logger.debug("PGN_INFO: POST PROCESSING PHASE ENDS")
 
-    details['test data'] = rmse
+    details["test data"] = rmse
 
     ref_max_y = ref_rmse.max(axis=(0, 1)).astype(np.double)
     ref_min_y = ref_rmse.min(axis=(0, 1)).astype(np.double)
 
     cmp_max_y = comp_rmse.max(axis=(0, 1)).astype(np.double)
     cmp_min_y = comp_rmse.min(axis=(0, 1)).astype(np.double)
 
-    img_file = os.path.relpath(os.path.join(args.img_dir, 'plot_comp.png'), os.getcwd())
-    fig, (ax1, ax2) = plt.subplots(ncols=2, figsize=(10, 8), sharey='all', gridspec_kw={'width_ratios': [3, 1]})
-    plt.rc('font', family='serif')
-
-    ax1.semilogy(ref_max_y, color='C0')
-    ax1.semilogy(ref_min_y, color='C0')
-    ax1.fill_between(range(ref_dims[-1]), ref_min_y, ref_max_y, color='C0', alpha=0.5)
-
-    ax1.semilogy(cmp_max_y, color='C1')
-    ax1.semilogy(cmp_min_y, color='C1')
-    ax1.fill_between(range(cmp_dims[-1]), cmp_min_y, cmp_max_y, color='C1', alpha=0.5)
+    img_file = os.path.relpath(os.path.join(args.img_dir, "plot_comp.png"), os.getcwd())
+    fig, (ax1, ax2) = plt.subplots(
+        ncols=2, figsize=(10, 8), sharey="all", gridspec_kw={"width_ratios": [3, 1]}
+    )
+    plt.rc("font", family="serif")
+
+    ax1.semilogy(ref_max_y, color="C0")
+    ax1.semilogy(ref_min_y, color="C0")
+    ax1.fill_between(range(ref_dims[-1]), ref_min_y, ref_max_y, color="C0", alpha=0.5)
+
+    ax1.semilogy(cmp_max_y, color="C1")
+    ax1.semilogy(cmp_min_y, color="C1")
+    ax1.fill_between(range(cmp_dims[-1]), cmp_min_y, cmp_max_y, color="C1", alpha=0.5)
 
     ax1.set_xticks(range(len(args.variables)))
-    ax1.set_xticklabels(args.variables, rotation=45, ha='right')
-    ax1.set_ylabel('Temperature RMSE (K)')
+    ax1.set_xticklabels(args.variables, rotation=45, ha="right")
+    ax1.set_ylabel("Temperature RMSE (K)")
 
-    patch_list = [mpatches.Patch(color='C0', alpha=0.5, label='Ref.'),
-                  mpatches.Patch(color='C1', alpha=0.5, label='Test')]
-    ax1.legend(handles=patch_list, loc='upper left')
+    patch_list = [
+        mpatches.Patch(color="C0", alpha=0.5, label="Ref."),
+        mpatches.Patch(color="C1", alpha=0.5, label="Test"),
+    ]
+    ax1.legend(handles=patch_list, loc="upper left")
 
-    scale_std = 1/np.sqrt(len(pge_ends_comp))
+    scale_std = 1 / np.sqrt(len(pge_ends_comp))
     tval_crit = stats.t.ppf(1 - crit, df=len(pge_ends_comp) - 1)
-    ax2.errorbar(1, pge_ends_cld.mean(), xerr=np.stack([[0.1, 0.1]]).T,
-                 fmt='none', ecolor='C0')
+    ax2.errorbar(
+        1, pge_ends_cld.mean(), xerr=np.stack([[0.1, 0.1]]).T, fmt="none", ecolor="C0"
+    )
     # Note: Because these are so close to zero, but are best plotted on a
     #        semilogy plot, the mean ± 2*σ/√N range or the mean ± Tc*σ/√N, where
     #        Tc is the critical t test value, can cross zero.
-    ax2.errorbar(1, pge_ends_comp.mean(), yerr=pge_ends_comp.std() * tval_crit * scale_std,
-                 fmt='oC1', elinewidth=20, ecolor='C1', alpha=0.5)
+    ax2.errorbar(
+        1,
+        pge_ends_comp.mean(),
+        yerr=pge_ends_comp.std() * tval_crit * scale_std,
+        fmt="oC1",
+        elinewidth=20,
+        ecolor="C1",
+        alpha=0.5,
+    )
     # ax2.errorbar(0.5, pge_ends_comp.mean(), yerr=pge_ends_comp.std() * 2 * scale_std,
     #              fmt='k.', elinewidth=20, ecolor='C1', alpha=0.5)
 
     ax2.set_xlim([0.8, 1.2])
     ax2.set_xticks([1])
-    ax2.set_xticklabels([args.variables[-1]], rotation=45, ha='right')
+    ax2.set_xticklabels([args.variables[-1]], rotation=45, ha="right")
 
     plt.tight_layout()
-    plt.savefig(img_file, bbox_inches='tight')
+    plt.savefig(img_file, bbox_inches="tight")
     plt.close(fig)
 
-    img_desc = 'Left: The evolution of the maximum temperature (K) RMSE over a ' \
-               'single time step for the {test} simulation (orange) and the {ref} ' \
-               'simulation (blue), plotted with a log scale on the y-axis. ' \
-               'The x-axis details the physical parameterizations ' \
-               'and/or Fortran code modules executed within this time step. ' \
-               'Right: the blue line indicates the {ref} ensemble mean at the ' \
-               'end of the time step and the orange circle is the {test} ensemble mean. ' \
-               'The orange box highlights the threshold values corresponding to the ' \
-               'critical P {crit}% in the two-sided t-test. For the test to pass, ' \
-               'the orange box must overlap the blue line. Note: Due to the logscale, ' \
-               'the orange box may not appear thicker than the line or may appear ' \
-               'exceptionally large as  these  values  are very close to zero and ' \
-               'the mean ± Tc*σ/√N range may cross zero, where Tc is the  critical ' \
-               't-test value, σ is the ensemble standard deviation, N is the size ' \
-               'of the ensemble, and σ/√N represents the t-test scaling ' \
-               'parameter.'.format(test=args.test_name, ref=args.ref_name, crit=crit * 100)
+    img_desc = (
+        "Left: The evolution of the maximum temperature (K) RMSE over a "
+        "single time step for the {test} simulation (orange) and the {ref} "
+        "simulation (blue), plotted with a log scale on the y-axis. "
+        "The x-axis details the physical parameterizations "
+        "and/or Fortran code modules executed within this time step. "
+        "Right: the blue line indicates the {ref} ensemble mean at the "
+        "end of the time step and the orange circle is the {test} ensemble mean. "
+        "The orange box highlights the threshold values corresponding to the "
+        "critical P {crit}% in the two-sided t-test. For the test to pass, "
+        "the orange box must overlap the blue line. Note: Due to the logscale, "
+        "the orange box may not appear thicker than the line or may appear "
+        "exceptionally large as  these  values  are very close to zero and "
+        "the mean ± Tc*σ/√N range may cross zero, where Tc is the  critical "
+        "t-test value, σ is the ensemble standard deviation, N is the size "
+        "of the ensemble, and σ/√N represents the t-test scaling "
+        "parameter.".format(test=args.test_name, ref=args.ref_name, crit=crit * 100)
+    )
     # img_link = os.path.join(os.path.basename(args.img_dir), os.path.basename(img_file))
     img_link = Path(*Path(args.img_dir).parts[-2:], Path(img_file).name)
-    img_gallery = el.Gallery('', [
-        el.Image(args.test_case, img_desc, img_link, height=600, relative_to="")
-    ])
+    img_gallery = el.Gallery(
+        "", [el.Image(args.test_case, img_desc, img_link, height=600, relative_to="")]
+    )
     return details, img_gallery
 
 
 def run(name, config, print_details=False):
     """
     Runs the extension.
 
@@ -357,73 +407,86 @@
                        (default: False)
 
     Returns:
        A LIVVkit page element containing the LIVVkit elements to display on a webpage
     """
 
     # FIXME: move into a config to NameSpace function
-    test_args = OrderedDict([(k.replace('-', '_'), v) for k, v in config.items()])
+    test_args = OrderedDict([(k.replace("-", "_"), v) for k, v in config.items()])
     test_args = argparse.Namespace(**test_args)
 
-    test_args.img_dir = os.path.join(livvkit.output_dir, 'validation', 'imgs', name)
+    test_args.img_dir = os.path.join(livvkit.output_dir, "validation", "imgs", name)
     fn.mkdir_p(test_args.img_dir)
 
     details, img_gal = main(test_args)
 
     res_table = el.Table(
         title="Results",
         data=OrderedDict(
             {
-                'Null hypothesis': [details['h0']],
-                'T test (t, p)': [details['T test (t, p)']],
-                'Test status': ['pass' if details['h0'] == 'accept' else 'fail'],
-                'Ensembles': ['statistically identical' if details['h0'] == 'accept' else 'statistically different'],
+                "Null hypothesis": [details["h0"]],
+                "T test (t, p)": [details["T test (t, p)"]],
+                "Test status": ["pass" if details["h0"] == "accept" else "fail"],
+                "Ensembles": [
+                    "statistically identical"
+                    if details["h0"] == "accept"
+                    else "statistically different"
+                ],
             }
-        )
+        ),
     )
     if print_details:
         _print_details(details)
 
-    bib_html = bib2html(os.path.join(os.path.dirname(__file__), 'pg.bib'))
+    bib_html = bib2html(os.path.join(os.path.dirname(__file__), "pg.bib"))
     tabs = el.Tabs({"Figures": [img_gal], "References": [el.RawHTML(bib_html)]})
-    page = el.Page(name, __doc__.replace('\n\n', '<br/><br/>'), elements=[res_table, tabs])
+    page = el.Page(
+        name, __doc__.replace("\n\n", "<br/><br/>"), elements=[res_table, tabs]
+    )
 
     return page
 
 
 def print_summary(summary):
-    print('    Perturbation growth test: {}'.format(summary['']['Case']))
-    print('      Null hypothesis: {}'.format(summary['']['Null hypothesis']))
-    print('      T Test (t, p): {}'.format(summary['']['T test (t, p)']))
-    print('      Ensembles: {}\n'.format(summary['']['Ensembles']))
+    print("    Perturbation growth test: {}".format(summary[""]["Case"]))
+    print("      Null hypothesis: {}".format(summary[""]["Null hypothesis"]))
+    print("      T Test (t, p): {}".format(summary[""]["T test (t, p)"]))
+    print("      Ensembles: {}\n".format(summary[""]["Ensembles"]))
 
 
 def summarize_result(results_page):
-    summary = {'Case': results_page.title}
-    
+    summary = {"Case": results_page.title}
+
     for elem in results_page.elements:
         if isinstance(elem, el.Table) and elem.title == "Results":
-            summary['Test status'] = 'pass' if elem.data['Null hypothesis'][0] == 'accept' else 'fail'
-            summary['Null hypothesis'] = elem.data['Null hypothesis'][0]
-            summary['T test (t, p)'] = elem.data['T test (t, p)'][0]
-            summary['Ensembles'] = 'statistically identical' if elem.data['Null hypothesis'][0] == 'accept' else 'statistically different'
+            summary["Test status"] = (
+                "pass" if elem.data["Null hypothesis"][0] == "accept" else "fail"
+            )
+            summary["Null hypothesis"] = elem.data["Null hypothesis"][0]
+            summary["T test (t, p)"] = elem.data["T test (t, p)"][0]
+            summary["Ensembles"] = (
+                "statistically identical"
+                if elem.data["Null hypothesis"][0] == "accept"
+                else "statistically different"
+            )
             break
         else:
             continue
-    return {'': summary}
+    return {"": summary}
 
 
 def populate_metadata():
     """
     Generates the metadata needed for the output summary page
     """
-    metadata = {'Type': 'ValSummary',
-                'Title': 'Validation',
-                'TableTitle': 'Perturbation growth test',
-                'Headers': ['Test status', 'Null hypothesis', 'T test (t, p)', 'Ensembles']
-                }
+    metadata = {
+        "Type": "ValSummary",
+        "Title": "Validation",
+        "TableTitle": "Perturbation growth test",
+        "Headers": ["Test status", "Null hypothesis", "T test (t, p)", "Ensembles"],
+    }
     return metadata
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     test_name, test_config = parse_args()
     run(test_name, test_config, print_details=True)
```

### Comparing `evv4esm-0.5.0/evv4esm/resources/css/acknowledgments.css` & `evv4esm-0.5.1/evv4esm/resources/css/acknowledgments.css`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #acknowledgments {
     clear: both;
     width: 80%;
     min-width: 800px;
     padding: 1em 0px 0.5em 0px;
-    border: 0px solid white; 
+    border: 0px solid white;
     margin-left: auto;
     margin-right: auto;
     margin-bottom: 120px;
     text-align: justify;
     border-style: solid;
     color: #111111;
     background-color: white;
@@ -21,30 +21,30 @@
 #acklogo {
     width: 98%;
     padding-top: 15px;
     text-align: justify;
 }
 
 #acklogo {
-    margin-left: auto; 
+    margin-left: auto;
     margin-right: auto;
     text-align: justify;
 }
 
 #acklogo:after {
     content: "";
     width: 100%;
     display: block;
 }
 
 #acklogo a {
     vertical-align: top;
     display: inline-block;
 }
-    
+
 #logoORNL {
     padding-top: 30px;
     height: 75px;
 }
 
 #logoDOESC {
     padding-top: 30px;
```

### Comparing `evv4esm-0.5.0/evv4esm/resources/css/captionjs.min.css` & `evv4esm-0.5.1/evv4esm/resources/css/captionjs.min.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-.captionjs{line-height:0}.captionjs figcaption{line-height:1;-ms-box-sizing:border-box;-o-box-sizing:border-box;box-sizing:border-box;width:100%}.captionjs.captionjs-animated,.captionjs.captionjs-hidden,.captionjs.captionjs-stacked{position:relative;overflow:hidden}.captionjs.captionjs-animated figcaption,.captionjs.captionjs-hidden figcaption,.captionjs.captionjs-stacked figcaption{position:absolute}.captionjs.captionjs-stacked figcaption{bottom:0}.captionjs.captionjs-animated figcaption{-webkit-transition:.25s bottom;transition:.25s bottom}.captionjs.captionjs-animated:hover figcaption{bottom:0!important}.captionjs.captionjs-hidden figcaption{-webkit-transition:.25s margin-bottom;transition:.25s margin-bottom}.captionjs.captionjs-hidden:hover figcaption{margin-bottom:0!important}
+.captionjs{line-height:0}.captionjs figcaption{line-height:1;-ms-box-sizing:border-box;-o-box-sizing:border-box;box-sizing:border-box;width:100%}.captionjs.captionjs-animated,.captionjs.captionjs-hidden,.captionjs.captionjs-stacked{position:relative;overflow:hidden}.captionjs.captionjs-animated figcaption,.captionjs.captionjs-hidden figcaption,.captionjs.captionjs-stacked figcaption{position:absolute}.captionjs.captionjs-stacked figcaption{bottom:0}.captionjs.captionjs-animated figcaption{-webkit-transition:.25s bottom;transition:.25s bottom}.captionjs.captionjs-animated:hover figcaption{bottom:0!important}.captionjs.captionjs-hidden figcaption{-webkit-transition:.25s margin-bottom;transition:.25s margin-bottom}.captionjs.captionjs-hidden:hover figcaption{margin-bottom:0!important}
```

### Comparing `evv4esm-0.5.0/evv4esm/resources/css/jquery-ui.min.css` & `evv4esm-0.5.1/evv4esm/resources/css/jquery-ui.min.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 /*! jQuery UI - v1.11.4 - 2016-04-07
 * http://jqueryui.com
 * Includes: core.css, draggable.css, resizable.css, selectable.css, sortable.css, accordion.css, autocomplete.css, button.css, datepicker.css, dialog.css, menu.css, progressbar.css, selectmenu.css, slider.css, spinner.css, tabs.css, tooltip.css, theme.css
 * To view and modify this theme, visit http://jqueryui.com/themeroller/?ffDefault=Arial%2CHelvetica%2Csans-serif&fsDefault=1em&fwDefault=normal&cornerRadius=3px&bgColorHeader=%23ffffff&bgTextureHeader=flat&borderColorHeader=%23ffffff&fcHeader=%23333333&iconColorHeader=%23444444&bgColorContent=%23ffffff&bgTextureContent=flat&borderColorContent=%2366c2ff&fcContent=%23333333&iconColorContent=%23444444&bgColorDefault=%23ffffff&bgTextureDefault=flat&borderColorDefault=%23c5c5c5&fcDefault=%23454545&iconColorDefault=%23777777&bgColorHover=%23ededed&bgTextureHover=flat&borderColorHover=%23cccccc&fcHover=%232b2b2b&iconColorHover=%23555555&bgColorActive=%2366c2ff&bgTextureActive=flat&borderColorActive=%2366c2ff&fcActive=%23ffffff&iconColorActive=%23ffffff&bgColorHighlight=%23fffa90&bgTextureHighlight=flat&borderColorHighlight=%23dad55e&fcHighlight=%23777620&iconColorHighlight=%23777620&bgColorError=%23fddfdf&bgTextureError=flat&borderColorError=%23f1a899&fcError=%235f3f3f&iconColorError=%23cc0000&bgColorOverlay=%23aaaaaa&bgTextureOverlay=flat&bgImgOpacityOverlay=0&opacityOverlay=30&bgColorShadow=%23666666&bgTextureShadow=flat&bgImgOpacityShadow=0&opacityShadow=30&thicknessShadow=5px&offsetTopShadow=0px&offsetLeftShadow=0px&cornerRadiusShadow=8px&bgImgOpacityHeader=&bgImgOpacityContent=&bgImgOpacityDefault=&bgImgOpacityHover=&bgImgOpacityActive=&bgImgOpacityHighlight=&bgImgOpacityError=
 * Copyright jQuery Foundation and other contributors; Licensed MIT */
 
-.ui-helper-hidden{display:none}.ui-helper-hidden-accessible{border:0;clip:rect(0 0 0 0);height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;width:1px}.ui-helper-reset{margin:0;padding:0;border:0;outline:0;line-height:1.3;text-decoration:none;font-size:100%;list-style:none}.ui-helper-clearfix:before,.ui-helper-clearfix:after{content:"";display:table;border-collapse:collapse}.ui-helper-clearfix:after{clear:both}.ui-helper-clearfix{min-height:0}.ui-helper-zfix{width:100%;height:100%;top:0;left:0;position:absolute;opacity:0;filter:Alpha(Opacity=0)}.ui-front{z-index:100}.ui-state-disabled{cursor:default!important}.ui-icon{display:block;text-indent:-99999px;overflow:hidden;background-repeat:no-repeat}.ui-widget-overlay{position:fixed;top:0;left:0;width:100%;height:100%}.ui-draggable-handle{-ms-touch-action:none;touch-action:none}.ui-resizable{position:relative}.ui-resizable-handle{position:absolute;font-size:0.1px;display:block;-ms-touch-action:none;touch-action:none}.ui-resizable-disabled .ui-resizable-handle,.ui-resizable-autohide .ui-resizable-handle{display:none}.ui-resizable-n{cursor:n-resize;height:7px;width:100%;top:-5px;left:0}.ui-resizable-s{cursor:s-resize;height:7px;width:100%;bottom:-5px;left:0}.ui-resizable-e{cursor:e-resize;width:7px;right:-5px;top:0;height:100%}.ui-resizable-w{cursor:w-resize;width:7px;left:-5px;top:0;height:100%}.ui-resizable-se{cursor:se-resize;width:12px;height:12px;right:1px;bottom:1px}.ui-resizable-sw{cursor:sw-resize;width:9px;height:9px;left:-5px;bottom:-5px}.ui-resizable-nw{cursor:nw-resize;width:9px;height:9px;left:-5px;top:-5px}.ui-resizable-ne{cursor:ne-resize;width:9px;height:9px;right:-5px;top:-5px}.ui-selectable{-ms-touch-action:none;touch-action:none}.ui-selectable-helper{position:absolute;z-index:100;border:1px dotted black}.ui-sortable-handle{-ms-touch-action:none;touch-action:none}.ui-accordion .ui-accordion-header{display:block;cursor:pointer;position:relative;margin:2px 0 0 0;padding:.5em .5em .5em .7em;min-height:0;font-size:100%}.ui-accordion .ui-accordion-icons{padding-left:2.2em}.ui-accordion .ui-accordion-icons .ui-accordion-icons{padding-left:2.2em}.ui-accordion .ui-accordion-header .ui-accordion-header-icon{position:absolute;left:.5em;top:50%;margin-top:-8px}.ui-accordion .ui-accordion-content{padding:1em 2.2em;border-top:0;overflow:auto}.ui-autocomplete{position:absolute;top:0;left:0;cursor:default}.ui-button{display:inline-block;position:relative;padding:0;line-height:normal;margin-right:.1em;cursor:pointer;vertical-align:middle;text-align:center;overflow:visible}.ui-button,.ui-button:link,.ui-button:visited,.ui-button:hover,.ui-button:active{text-decoration:none}.ui-button-icon-only{width:2.2em}button.ui-button-icon-only{width:2.4em}.ui-button-icons-only{width:3.4em}button.ui-button-icons-only{width:3.7em}.ui-button .ui-button-text{display:block;line-height:normal}.ui-button-text-only .ui-button-text{padding:.4em 1em}.ui-button-icon-only .ui-button-text,.ui-button-icons-only .ui-button-text{padding:.4em;text-indent:-9999999px}.ui-button-text-icon-primary .ui-button-text,.ui-button-text-icons .ui-button-text{padding:.4em 1em .4em 2.1em}.ui-button-text-icon-secondary .ui-button-text,.ui-button-text-icons .ui-button-text{padding:.4em 2.1em .4em 1em}.ui-button-text-icons .ui-button-text{padding-left:2.1em;padding-right:2.1em}input.ui-button{padding:.4em 1em}.ui-button-icon-only .ui-icon,.ui-button-text-icon-primary .ui-icon,.ui-button-text-icon-secondary .ui-icon,.ui-button-text-icons .ui-icon,.ui-button-icons-only .ui-icon{position:absolute;top:50%;margin-top:-8px}.ui-button-icon-only .ui-icon{left:50%;margin-left:-8px}.ui-button-text-icon-primary .ui-button-icon-primary,.ui-button-text-icons .ui-button-icon-primary,.ui-button-icons-only .ui-button-icon-primary{left:.5em}.ui-button-text-icon-secondary .ui-button-icon-secondary,.ui-button-text-icons .ui-button-icon-secondary,.ui-button-icons-only .ui-button-icon-secondary{right:.5em}.ui-buttonset{margin-right:7px}.ui-buttonset .ui-button{margin-left:0;margin-right:-.3em}input.ui-button::-moz-focus-inner,button.ui-button::-moz-focus-inner{border:0;padding:0}.ui-datepicker{width:17em;padding:.2em .2em 0;display:none}.ui-datepicker .ui-datepicker-header{position:relative;padding:.2em 0}.ui-datepicker .ui-datepicker-prev,.ui-datepicker .ui-datepicker-next{position:absolute;top:2px;width:1.8em;height:1.8em}.ui-datepicker .ui-datepicker-prev-hover,.ui-datepicker .ui-datepicker-next-hover{top:1px}.ui-datepicker .ui-datepicker-prev{left:2px}.ui-datepicker .ui-datepicker-next{right:2px}.ui-datepicker .ui-datepicker-prev-hover{left:1px}.ui-datepicker .ui-datepicker-next-hover{right:1px}.ui-datepicker .ui-datepicker-prev span,.ui-datepicker .ui-datepicker-next span{display:block;position:absolute;left:50%;margin-left:-8px;top:50%;margin-top:-8px}.ui-datepicker .ui-datepicker-title{margin:0 2.3em;line-height:1.8em;text-align:center}.ui-datepicker .ui-datepicker-title select{font-size:1em;margin:1px 0}.ui-datepicker select.ui-datepicker-month,.ui-datepicker select.ui-datepicker-year{width:45%}.ui-datepicker table{width:100%;font-size:.9em;border-collapse:collapse;margin:0 0 .4em}.ui-datepicker th{padding:.7em .3em;text-align:center;font-weight:bold;border:0}.ui-datepicker td{border:0;padding:1px}.ui-datepicker td span,.ui-datepicker td a{display:block;padding:.2em;text-align:right;text-decoration:none}.ui-datepicker .ui-datepicker-buttonpane{background-image:none;margin:.7em 0 0 0;padding:0 .2em;border-left:0;border-right:0;border-bottom:0}.ui-datepicker .ui-datepicker-buttonpane button{float:right;margin:.5em .2em .4em;cursor:pointer;padding:.2em .6em .3em .6em;width:auto;overflow:visible}.ui-datepicker .ui-datepicker-buttonpane button.ui-datepicker-current{float:left}.ui-datepicker.ui-datepicker-multi{width:auto}.ui-datepicker-multi .ui-datepicker-group{float:left}.ui-datepicker-multi .ui-datepicker-group table{width:95%;margin:0 auto .4em}.ui-datepicker-multi-2 .ui-datepicker-group{width:50%}.ui-datepicker-multi-3 .ui-datepicker-group{width:33.3%}.ui-datepicker-multi-4 .ui-datepicker-group{width:25%}.ui-datepicker-multi .ui-datepicker-group-last .ui-datepicker-header,.ui-datepicker-multi .ui-datepicker-group-middle .ui-datepicker-header{border-left-width:0}.ui-datepicker-multi .ui-datepicker-buttonpane{clear:left}.ui-datepicker-row-break{clear:both;width:100%;font-size:0}.ui-datepicker-rtl{direction:rtl}.ui-datepicker-rtl .ui-datepicker-prev{right:2px;left:auto}.ui-datepicker-rtl .ui-datepicker-next{left:2px;right:auto}.ui-datepicker-rtl .ui-datepicker-prev:hover{right:1px;left:auto}.ui-datepicker-rtl .ui-datepicker-next:hover{left:1px;right:auto}.ui-datepicker-rtl .ui-datepicker-buttonpane{clear:right}.ui-datepicker-rtl .ui-datepicker-buttonpane button{float:left}.ui-datepicker-rtl .ui-datepicker-buttonpane button.ui-datepicker-current,.ui-datepicker-rtl .ui-datepicker-group{float:right}.ui-datepicker-rtl .ui-datepicker-group-last .ui-datepicker-header,.ui-datepicker-rtl .ui-datepicker-group-middle .ui-datepicker-header{border-right-width:0;border-left-width:1px}.ui-dialog{overflow:hidden;position:absolute;top:0;left:0;padding:.2em;outline:0}.ui-dialog .ui-dialog-titlebar{padding:.4em 1em;position:relative}.ui-dialog .ui-dialog-title{float:left;margin:.1em 0;white-space:nowrap;width:90%;overflow:hidden;text-overflow:ellipsis}.ui-dialog .ui-dialog-titlebar-close{position:absolute;right:.3em;top:50%;width:20px;margin:-10px 0 0 0;padding:1px;height:20px}.ui-dialog .ui-dialog-content{position:relative;border:0;padding:.5em 1em;background:none;overflow:auto}.ui-dialog .ui-dialog-buttonpane{text-align:left;border-width:1px 0 0 0;background-image:none;margin-top:.5em;padding:.3em 1em .5em .4em}.ui-dialog .ui-dialog-buttonpane .ui-dialog-buttonset{float:right}.ui-dialog .ui-dialog-buttonpane button{margin:.5em .4em .5em 0;cursor:pointer}.ui-dialog .ui-resizable-se{width:12px;height:12px;right:-5px;bottom:-5px;background-position:16px 16px}.ui-draggable .ui-dialog-titlebar{cursor:move}.ui-menu{list-style:none;padding:0;margin:0;display:block;outline:none}.ui-menu .ui-menu{position:absolute}.ui-menu .ui-menu-item{position:relative;margin:0;padding:3px 1em 3px .4em;cursor:pointer;min-height:0;list-style-image:url("data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7")}.ui-menu .ui-menu-divider{margin:5px 0;height:0;font-size:0;line-height:0;border-width:1px 0 0 0}.ui-menu .ui-state-focus,.ui-menu .ui-state-active{margin:-1px}.ui-menu-icons{position:relative}.ui-menu-icons .ui-menu-item{padding-left:2em}.ui-menu .ui-icon{position:absolute;top:0;bottom:0;left:.2em;margin:auto 0}.ui-menu .ui-menu-icon{left:auto;right:0}.ui-progressbar{height:2em;text-align:left;overflow:hidden}.ui-progressbar .ui-progressbar-value{margin:-1px;height:100%}.ui-progressbar .ui-progressbar-overlay{background:url("data:image/gif;base64,R0lGODlhKAAoAIABAAAAAP///yH/C05FVFNDQVBFMi4wAwEAAAAh+QQJAQABACwAAAAAKAAoAAACkYwNqXrdC52DS06a7MFZI+4FHBCKoDeWKXqymPqGqxvJrXZbMx7Ttc+w9XgU2FB3lOyQRWET2IFGiU9m1frDVpxZZc6bfHwv4c1YXP6k1Vdy292Fb6UkuvFtXpvWSzA+HycXJHUXiGYIiMg2R6W459gnWGfHNdjIqDWVqemH2ekpObkpOlppWUqZiqr6edqqWQAAIfkECQEAAQAsAAAAACgAKAAAApSMgZnGfaqcg1E2uuzDmmHUBR8Qil95hiPKqWn3aqtLsS18y7G1SzNeowWBENtQd+T1JktP05nzPTdJZlR6vUxNWWjV+vUWhWNkWFwxl9VpZRedYcflIOLafaa28XdsH/ynlcc1uPVDZxQIR0K25+cICCmoqCe5mGhZOfeYSUh5yJcJyrkZWWpaR8doJ2o4NYq62lAAACH5BAkBAAEALAAAAAAoACgAAAKVDI4Yy22ZnINRNqosw0Bv7i1gyHUkFj7oSaWlu3ovC8GxNso5fluz3qLVhBVeT/Lz7ZTHyxL5dDalQWPVOsQWtRnuwXaFTj9jVVh8pma9JjZ4zYSj5ZOyma7uuolffh+IR5aW97cHuBUXKGKXlKjn+DiHWMcYJah4N0lYCMlJOXipGRr5qdgoSTrqWSq6WFl2ypoaUAAAIfkECQEAAQAsAAAAACgAKAAAApaEb6HLgd/iO7FNWtcFWe+ufODGjRfoiJ2akShbueb0wtI50zm02pbvwfWEMWBQ1zKGlLIhskiEPm9R6vRXxV4ZzWT2yHOGpWMyorblKlNp8HmHEb/lCXjcW7bmtXP8Xt229OVWR1fod2eWqNfHuMjXCPkIGNileOiImVmCOEmoSfn3yXlJWmoHGhqp6ilYuWYpmTqKUgAAIfkECQEAAQAsAAAAACgAKAAAApiEH6kb58biQ3FNWtMFWW3eNVcojuFGfqnZqSebuS06w5V80/X02pKe8zFwP6EFWOT1lDFk8rGERh1TTNOocQ61Hm4Xm2VexUHpzjymViHrFbiELsefVrn6XKfnt2Q9G/+Xdie499XHd2g4h7ioOGhXGJboGAnXSBnoBwKYyfioubZJ2Hn0RuRZaflZOil56Zp6iioKSXpUAAAh+QQJAQABACwAAAAAKAAoAAACkoQRqRvnxuI7kU1a1UU5bd5tnSeOZXhmn5lWK3qNTWvRdQxP8qvaC+/yaYQzXO7BMvaUEmJRd3TsiMAgswmNYrSgZdYrTX6tSHGZO73ezuAw2uxuQ+BbeZfMxsexY35+/Qe4J1inV0g4x3WHuMhIl2jXOKT2Q+VU5fgoSUI52VfZyfkJGkha6jmY+aaYdirq+lQAACH5BAkBAAEALAAAAAAoACgAAAKWBIKpYe0L3YNKToqswUlvznigd4wiR4KhZrKt9Upqip61i9E3vMvxRdHlbEFiEXfk9YARYxOZZD6VQ2pUunBmtRXo1Lf8hMVVcNl8JafV38aM2/Fu5V16Bn63r6xt97j09+MXSFi4BniGFae3hzbH9+hYBzkpuUh5aZmHuanZOZgIuvbGiNeomCnaxxap2upaCZsq+1kAACH5BAkBAAEALAAAAAAoACgAAAKXjI8By5zf4kOxTVrXNVlv1X0d8IGZGKLnNpYtm8Lr9cqVeuOSvfOW79D9aDHizNhDJidFZhNydEahOaDH6nomtJjp1tutKoNWkvA6JqfRVLHU/QUfau9l2x7G54d1fl995xcIGAdXqMfBNadoYrhH+Mg2KBlpVpbluCiXmMnZ2Sh4GBqJ+ckIOqqJ6LmKSllZmsoq6wpQAAAh+QQJAQABACwAAAAAKAAoAAAClYx/oLvoxuJDkU1a1YUZbJ59nSd2ZXhWqbRa2/gF8Gu2DY3iqs7yrq+xBYEkYvFSM8aSSObE+ZgRl1BHFZNr7pRCavZ5BW2142hY3AN/zWtsmf12p9XxxFl2lpLn1rseztfXZjdIWIf2s5dItwjYKBgo9yg5pHgzJXTEeGlZuenpyPmpGQoKOWkYmSpaSnqKileI2FAAACH5BAkBAAEALAAAAAAoACgAAAKVjB+gu+jG4kORTVrVhRlsnn2dJ3ZleFaptFrb+CXmO9OozeL5VfP99HvAWhpiUdcwkpBH3825AwYdU8xTqlLGhtCosArKMpvfa1mMRae9VvWZfeB2XfPkeLmm18lUcBj+p5dnN8jXZ3YIGEhYuOUn45aoCDkp16hl5IjYJvjWKcnoGQpqyPlpOhr3aElaqrq56Bq7VAAAOw==");height:100%;filter:alpha(opacity=25);opacity:0.25}.ui-progressbar-indeterminate .ui-progressbar-value{background-image:none}.ui-selectmenu-menu{padding:0;margin:0;position:absolute;top:0;left:0;display:none}.ui-selectmenu-menu .ui-menu{overflow:auto;overflow-x:hidden;padding-bottom:1px}.ui-selectmenu-menu .ui-menu .ui-selectmenu-optgroup{font-size:1em;font-weight:bold;line-height:1.5;padding:2px 0.4em;margin:0.5em 0 0 0;height:auto;border:0}.ui-selectmenu-open{display:block}.ui-selectmenu-button{display:inline-block;overflow:hidden;position:relative;text-decoration:none;cursor:pointer}.ui-selectmenu-button span.ui-icon{right:0.5em;left:auto;margin-top:-8px;position:absolute;top:50%}.ui-selectmenu-button span.ui-selectmenu-text{text-align:left;padding:0.4em 2.1em 0.4em 1em;display:block;line-height:1.4;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.ui-slider{position:relative;text-align:left}.ui-slider .ui-slider-handle{position:absolute;z-index:2;width:1.2em;height:1.2em;cursor:default;-ms-touch-action:none;touch-action:none}.ui-slider .ui-slider-range{position:absolute;z-index:1;font-size:.7em;display:block;border:0;background-position:0 0}.ui-slider.ui-state-disabled .ui-slider-handle,.ui-slider.ui-state-disabled .ui-slider-range{filter:inherit}.ui-slider-horizontal{height:.8em}.ui-slider-horizontal .ui-slider-handle{top:-.3em;margin-left:-.6em}.ui-slider-horizontal .ui-slider-range{top:0;height:100%}.ui-slider-horizontal .ui-slider-range-min{left:0}.ui-slider-horizontal .ui-slider-range-max{right:0}.ui-slider-vertical{width:.8em;height:100px}.ui-slider-vertical .ui-slider-handle{left:-.3em;margin-left:0;margin-bottom:-.6em}.ui-slider-vertical .ui-slider-range{left:0;width:100%}.ui-slider-vertical .ui-slider-range-min{bottom:0}.ui-slider-vertical .ui-slider-range-max{top:0}.ui-spinner{position:relative;display:inline-block;overflow:hidden;padding:0;vertical-align:middle}.ui-spinner-input{border:none;background:none;color:inherit;padding:0;margin:.2em 0;vertical-align:middle;margin-left:.4em;margin-right:22px}.ui-spinner-button{width:16px;height:50%;font-size:.5em;padding:0;margin:0;text-align:center;position:absolute;cursor:default;display:block;overflow:hidden;right:0}.ui-spinner a.ui-spinner-button{border-top:none;border-bottom:none;border-right:none}.ui-spinner .ui-icon{position:absolute;margin-top:-8px;top:50%;left:0}.ui-spinner-up{top:0}.ui-spinner-down{bottom:0}.ui-spinner .ui-icon-triangle-1-s{background-position:-65px -16px}.ui-tabs{position:relative;padding:.2em}.ui-tabs .ui-tabs-nav{margin:0;padding:.2em .2em 0}.ui-tabs .ui-tabs-nav li{list-style:none;float:left;position:relative;top:0;margin:1px .2em 0 0;border-bottom-width:0;padding:0;white-space:nowrap}.ui-tabs .ui-tabs-nav .ui-tabs-anchor{float:left;padding:.5em 1em;text-decoration:none}.ui-tabs .ui-tabs-nav li.ui-tabs-active{margin-bottom:-1px;padding-bottom:1px}.ui-tabs .ui-tabs-nav li.ui-tabs-active .ui-tabs-anchor,.ui-tabs .ui-tabs-nav li.ui-state-disabled .ui-tabs-anchor,.ui-tabs .ui-tabs-nav li.ui-tabs-loading .ui-tabs-anchor{cursor:text}.ui-tabs-collapsible .ui-tabs-nav li.ui-tabs-active .ui-tabs-anchor{cursor:pointer}.ui-tabs .ui-tabs-panel{display:block;border-width:0;padding:1em 1.4em;background:none}.ui-tooltip{padding:8px;position:absolute;z-index:9999;max-width:300px;-webkit-box-shadow:0 0 5px #aaa;box-shadow:0 0 5px #aaa}body .ui-tooltip{border-width:2px}.ui-widget{font-family:Arial,Helvetica,sans-serif;font-size:1em}.ui-widget .ui-widget{font-size:1em}.ui-widget input,.ui-widget select,.ui-widget textarea,.ui-widget button{font-family:Arial,Helvetica,sans-serif;font-size:1em}.ui-widget-content{border:1px solid #66c2ff;background:#fff;color:#333}.ui-widget-content a{color:#333}.ui-widget-header{border:1px solid #fff;background:#fff;color:#333;font-weight:bold}.ui-widget-header a{color:#333}.ui-state-default,.ui-widget-content .ui-state-default,.ui-widget-header .ui-state-default{border:1px solid #c5c5c5;background:#fff;font-weight:normal;color:#454545}.ui-state-default a,.ui-state-default a:link,.ui-state-default a:visited{color:#454545;text-decoration:none}.ui-state-hover,.ui-widget-content .ui-state-hover,.ui-widget-header .ui-state-hover,.ui-state-focus,.ui-widget-content .ui-state-focus,.ui-widget-header .ui-state-focus{border:1px solid #ccc;background:#ededed;font-weight:normal;color:#2b2b2b}.ui-state-hover a,.ui-state-hover a:hover,.ui-state-hover a:link,.ui-state-hover a:visited,.ui-state-focus a,.ui-state-focus a:hover,.ui-state-focus a:link,.ui-state-focus a:visited{color:#2b2b2b;text-decoration:none}.ui-state-active,.ui-widget-content .ui-state-active,.ui-widget-header .ui-state-active{border:1px solid #66c2ff;background:#66c2ff;font-weight:normal;color:#fff}.ui-state-active a,.ui-state-active a:link,.ui-state-active a:visited{color:#fff;text-decoration:none}.ui-state-highlight,.ui-widget-content .ui-state-highlight,.ui-widget-header .ui-state-highlight{border:1px solid #dad55e;background:#fffa90;color:#777620}.ui-state-highlight a,.ui-widget-content .ui-state-highlight a,.ui-widget-header .ui-state-highlight a{color:#777620}.ui-state-error,.ui-widget-content .ui-state-error,.ui-widget-header .ui-state-error{border:1px solid #f1a899;background:#fddfdf;color:#5f3f3f}.ui-state-error a,.ui-widget-content .ui-state-error a,.ui-widget-header .ui-state-error a{color:#5f3f3f}.ui-state-error-text,.ui-widget-content .ui-state-error-text,.ui-widget-header .ui-state-error-text{color:#5f3f3f}.ui-priority-primary,.ui-widget-content .ui-priority-primary,.ui-widget-header .ui-priority-primary{font-weight:bold}.ui-priority-secondary,.ui-widget-content .ui-priority-secondary,.ui-widget-header .ui-priority-secondary{opacity:.7;filter:Alpha(Opacity=70);font-weight:normal}.ui-state-disabled,.ui-widget-content .ui-state-disabled,.ui-widget-header .ui-state-disabled{opacity:.35;filter:Alpha(Opacity=35);background-image:none}.ui-state-disabled .ui-icon{filter:Alpha(Opacity=35)}.ui-icon{width:16px;height:16px}.ui-icon,.ui-widget-content .ui-icon{background-image:url("images/ui-icons_444444_256x240.png")}.ui-widget-header .ui-icon{background-image:url("images/ui-icons_444444_256x240.png")}.ui-state-default .ui-icon{background-image:url("images/ui-icons_777777_256x240.png")}.ui-state-hover .ui-icon,.ui-state-focus .ui-icon{background-image:url("images/ui-icons_555555_256x240.png")}.ui-state-active .ui-icon{background-image:url("images/ui-icons_ffffff_256x240.png")}.ui-state-highlight .ui-icon{background-image:url("images/ui-icons_777620_256x240.png")}.ui-state-error .ui-icon,.ui-state-error-text .ui-icon{background-image:url("images/ui-icons_cc0000_256x240.png")}.ui-icon-blank{background-position:16px 16px}.ui-icon-carat-1-n{background-position:0 0}.ui-icon-carat-1-ne{background-position:-16px 0}.ui-icon-carat-1-e{background-position:-32px 0}.ui-icon-carat-1-se{background-position:-48px 0}.ui-icon-carat-1-s{background-position:-64px 0}.ui-icon-carat-1-sw{background-position:-80px 0}.ui-icon-carat-1-w{background-position:-96px 0}.ui-icon-carat-1-nw{background-position:-112px 0}.ui-icon-carat-2-n-s{background-position:-128px 0}.ui-icon-carat-2-e-w{background-position:-144px 0}.ui-icon-triangle-1-n{background-position:0 -16px}.ui-icon-triangle-1-ne{background-position:-16px -16px}.ui-icon-triangle-1-e{background-position:-32px -16px}.ui-icon-triangle-1-se{background-position:-48px -16px}.ui-icon-triangle-1-s{background-position:-64px -16px}.ui-icon-triangle-1-sw{background-position:-80px -16px}.ui-icon-triangle-1-w{background-position:-96px -16px}.ui-icon-triangle-1-nw{background-position:-112px -16px}.ui-icon-triangle-2-n-s{background-position:-128px -16px}.ui-icon-triangle-2-e-w{background-position:-144px -16px}.ui-icon-arrow-1-n{background-position:0 -32px}.ui-icon-arrow-1-ne{background-position:-16px -32px}.ui-icon-arrow-1-e{background-position:-32px -32px}.ui-icon-arrow-1-se{background-position:-48px -32px}.ui-icon-arrow-1-s{background-position:-64px -32px}.ui-icon-arrow-1-sw{background-position:-80px -32px}.ui-icon-arrow-1-w{background-position:-96px -32px}.ui-icon-arrow-1-nw{background-position:-112px -32px}.ui-icon-arrow-2-n-s{background-position:-128px -32px}.ui-icon-arrow-2-ne-sw{background-position:-144px -32px}.ui-icon-arrow-2-e-w{background-position:-160px -32px}.ui-icon-arrow-2-se-nw{background-position:-176px -32px}.ui-icon-arrowstop-1-n{background-position:-192px -32px}.ui-icon-arrowstop-1-e{background-position:-208px -32px}.ui-icon-arrowstop-1-s{background-position:-224px -32px}.ui-icon-arrowstop-1-w{background-position:-240px -32px}.ui-icon-arrowthick-1-n{background-position:0 -48px}.ui-icon-arrowthick-1-ne{background-position:-16px -48px}.ui-icon-arrowthick-1-e{background-position:-32px -48px}.ui-icon-arrowthick-1-se{background-position:-48px -48px}.ui-icon-arrowthick-1-s{background-position:-64px -48px}.ui-icon-arrowthick-1-sw{background-position:-80px -48px}.ui-icon-arrowthick-1-w{background-position:-96px -48px}.ui-icon-arrowthick-1-nw{background-position:-112px -48px}.ui-icon-arrowthick-2-n-s{background-position:-128px -48px}.ui-icon-arrowthick-2-ne-sw{background-position:-144px -48px}.ui-icon-arrowthick-2-e-w{background-position:-160px -48px}.ui-icon-arrowthick-2-se-nw{background-position:-176px -48px}.ui-icon-arrowthickstop-1-n{background-position:-192px -48px}.ui-icon-arrowthickstop-1-e{background-position:-208px -48px}.ui-icon-arrowthickstop-1-s{background-position:-224px -48px}.ui-icon-arrowthickstop-1-w{background-position:-240px -48px}.ui-icon-arrowreturnthick-1-w{background-position:0 -64px}.ui-icon-arrowreturnthick-1-n{background-position:-16px -64px}.ui-icon-arrowreturnthick-1-e{background-position:-32px -64px}.ui-icon-arrowreturnthick-1-s{background-position:-48px -64px}.ui-icon-arrowreturn-1-w{background-position:-64px -64px}.ui-icon-arrowreturn-1-n{background-position:-80px -64px}.ui-icon-arrowreturn-1-e{background-position:-96px -64px}.ui-icon-arrowreturn-1-s{background-position:-112px -64px}.ui-icon-arrowrefresh-1-w{background-position:-128px -64px}.ui-icon-arrowrefresh-1-n{background-position:-144px -64px}.ui-icon-arrowrefresh-1-e{background-position:-160px -64px}.ui-icon-arrowrefresh-1-s{background-position:-176px -64px}.ui-icon-arrow-4{background-position:0 -80px}.ui-icon-arrow-4-diag{background-position:-16px -80px}.ui-icon-extlink{background-position:-32px -80px}.ui-icon-newwin{background-position:-48px -80px}.ui-icon-refresh{background-position:-64px -80px}.ui-icon-shuffle{background-position:-80px -80px}.ui-icon-transfer-e-w{background-position:-96px -80px}.ui-icon-transferthick-e-w{background-position:-112px -80px}.ui-icon-folder-collapsed{background-position:0 -96px}.ui-icon-folder-open{background-position:-16px -96px}.ui-icon-document{background-position:-32px -96px}.ui-icon-document-b{background-position:-48px -96px}.ui-icon-note{background-position:-64px -96px}.ui-icon-mail-closed{background-position:-80px -96px}.ui-icon-mail-open{background-position:-96px -96px}.ui-icon-suitcase{background-position:-112px -96px}.ui-icon-comment{background-position:-128px -96px}.ui-icon-person{background-position:-144px -96px}.ui-icon-print{background-position:-160px -96px}.ui-icon-trash{background-position:-176px -96px}.ui-icon-locked{background-position:-192px -96px}.ui-icon-unlocked{background-position:-208px -96px}.ui-icon-bookmark{background-position:-224px -96px}.ui-icon-tag{background-position:-240px -96px}.ui-icon-home{background-position:0 -112px}.ui-icon-flag{background-position:-16px -112px}.ui-icon-calendar{background-position:-32px -112px}.ui-icon-cart{background-position:-48px -112px}.ui-icon-pencil{background-position:-64px -112px}.ui-icon-clock{background-position:-80px -112px}.ui-icon-disk{background-position:-96px -112px}.ui-icon-calculator{background-position:-112px -112px}.ui-icon-zoomin{background-position:-128px -112px}.ui-icon-zoomout{background-position:-144px -112px}.ui-icon-search{background-position:-160px -112px}.ui-icon-wrench{background-position:-176px -112px}.ui-icon-gear{background-position:-192px -112px}.ui-icon-heart{background-position:-208px -112px}.ui-icon-star{background-position:-224px -112px}.ui-icon-link{background-position:-240px -112px}.ui-icon-cancel{background-position:0 -128px}.ui-icon-plus{background-position:-16px -128px}.ui-icon-plusthick{background-position:-32px -128px}.ui-icon-minus{background-position:-48px -128px}.ui-icon-minusthick{background-position:-64px -128px}.ui-icon-close{background-position:-80px -128px}.ui-icon-closethick{background-position:-96px -128px}.ui-icon-key{background-position:-112px -128px}.ui-icon-lightbulb{background-position:-128px -128px}.ui-icon-scissors{background-position:-144px -128px}.ui-icon-clipboard{background-position:-160px -128px}.ui-icon-copy{background-position:-176px -128px}.ui-icon-contact{background-position:-192px -128px}.ui-icon-image{background-position:-208px -128px}.ui-icon-video{background-position:-224px -128px}.ui-icon-script{background-position:-240px -128px}.ui-icon-alert{background-position:0 -144px}.ui-icon-info{background-position:-16px -144px}.ui-icon-notice{background-position:-32px -144px}.ui-icon-help{background-position:-48px -144px}.ui-icon-check{background-position:-64px -144px}.ui-icon-bullet{background-position:-80px -144px}.ui-icon-radio-on{background-position:-96px -144px}.ui-icon-radio-off{background-position:-112px -144px}.ui-icon-pin-w{background-position:-128px -144px}.ui-icon-pin-s{background-position:-144px -144px}.ui-icon-play{background-position:0 -160px}.ui-icon-pause{background-position:-16px -160px}.ui-icon-seek-next{background-position:-32px -160px}.ui-icon-seek-prev{background-position:-48px -160px}.ui-icon-seek-end{background-position:-64px -160px}.ui-icon-seek-start{background-position:-80px -160px}.ui-icon-seek-first{background-position:-80px -160px}.ui-icon-stop{background-position:-96px -160px}.ui-icon-eject{background-position:-112px -160px}.ui-icon-volume-off{background-position:-128px -160px}.ui-icon-volume-on{background-position:-144px -160px}.ui-icon-power{background-position:0 -176px}.ui-icon-signal-diag{background-position:-16px -176px}.ui-icon-signal{background-position:-32px -176px}.ui-icon-battery-0{background-position:-48px -176px}.ui-icon-battery-1{background-position:-64px -176px}.ui-icon-battery-2{background-position:-80px -176px}.ui-icon-battery-3{background-position:-96px -176px}.ui-icon-circle-plus{background-position:0 -192px}.ui-icon-circle-minus{background-position:-16px -192px}.ui-icon-circle-close{background-position:-32px -192px}.ui-icon-circle-triangle-e{background-position:-48px -192px}.ui-icon-circle-triangle-s{background-position:-64px -192px}.ui-icon-circle-triangle-w{background-position:-80px -192px}.ui-icon-circle-triangle-n{background-position:-96px -192px}.ui-icon-circle-arrow-e{background-position:-112px -192px}.ui-icon-circle-arrow-s{background-position:-128px -192px}.ui-icon-circle-arrow-w{background-position:-144px -192px}.ui-icon-circle-arrow-n{background-position:-160px -192px}.ui-icon-circle-zoomin{background-position:-176px -192px}.ui-icon-circle-zoomout{background-position:-192px -192px}.ui-icon-circle-check{background-position:-208px -192px}.ui-icon-circlesmall-plus{background-position:0 -208px}.ui-icon-circlesmall-minus{background-position:-16px -208px}.ui-icon-circlesmall-close{background-position:-32px -208px}.ui-icon-squaresmall-plus{background-position:-48px -208px}.ui-icon-squaresmall-minus{background-position:-64px -208px}.ui-icon-squaresmall-close{background-position:-80px -208px}.ui-icon-grip-dotted-vertical{background-position:0 -224px}.ui-icon-grip-dotted-horizontal{background-position:-16px -224px}.ui-icon-grip-solid-vertical{background-position:-32px -224px}.ui-icon-grip-solid-horizontal{background-position:-48px -224px}.ui-icon-gripsmall-diagonal-se{background-position:-64px -224px}.ui-icon-grip-diagonal-se{background-position:-80px -224px}.ui-corner-all,.ui-corner-top,.ui-corner-left,.ui-corner-tl{border-top-left-radius:3px}.ui-corner-all,.ui-corner-top,.ui-corner-right,.ui-corner-tr{border-top-right-radius:3px}.ui-corner-all,.ui-corner-bottom,.ui-corner-left,.ui-corner-bl{border-bottom-left-radius:3px}.ui-corner-all,.ui-corner-bottom,.ui-corner-right,.ui-corner-br{border-bottom-right-radius:3px}.ui-widget-overlay{background:#aaa;opacity:.3;filter:Alpha(Opacity=30)}.ui-widget-shadow{margin:0 0 0 0;padding:5px;background:#666;opacity:.3;filter:Alpha(Opacity=30);border-radius:8px}
+.ui-helper-hidden{display:none}.ui-helper-hidden-accessible{border:0;clip:rect(0 0 0 0);height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;width:1px}.ui-helper-reset{margin:0;padding:0;border:0;outline:0;line-height:1.3;text-decoration:none;font-size:100%;list-style:none}.ui-helper-clearfix:before,.ui-helper-clearfix:after{content:"";display:table;border-collapse:collapse}.ui-helper-clearfix:after{clear:both}.ui-helper-clearfix{min-height:0}.ui-helper-zfix{width:100%;height:100%;top:0;left:0;position:absolute;opacity:0;filter:Alpha(Opacity=0)}.ui-front{z-index:100}.ui-state-disabled{cursor:default!important}.ui-icon{display:block;text-indent:-99999px;overflow:hidden;background-repeat:no-repeat}.ui-widget-overlay{position:fixed;top:0;left:0;width:100%;height:100%}.ui-draggable-handle{-ms-touch-action:none;touch-action:none}.ui-resizable{position:relative}.ui-resizable-handle{position:absolute;font-size:0.1px;display:block;-ms-touch-action:none;touch-action:none}.ui-resizable-disabled .ui-resizable-handle,.ui-resizable-autohide .ui-resizable-handle{display:none}.ui-resizable-n{cursor:n-resize;height:7px;width:100%;top:-5px;left:0}.ui-resizable-s{cursor:s-resize;height:7px;width:100%;bottom:-5px;left:0}.ui-resizable-e{cursor:e-resize;width:7px;right:-5px;top:0;height:100%}.ui-resizable-w{cursor:w-resize;width:7px;left:-5px;top:0;height:100%}.ui-resizable-se{cursor:se-resize;width:12px;height:12px;right:1px;bottom:1px}.ui-resizable-sw{cursor:sw-resize;width:9px;height:9px;left:-5px;bottom:-5px}.ui-resizable-nw{cursor:nw-resize;width:9px;height:9px;left:-5px;top:-5px}.ui-resizable-ne{cursor:ne-resize;width:9px;height:9px;right:-5px;top:-5px}.ui-selectable{-ms-touch-action:none;touch-action:none}.ui-selectable-helper{position:absolute;z-index:100;border:1px dotted black}.ui-sortable-handle{-ms-touch-action:none;touch-action:none}.ui-accordion .ui-accordion-header{display:block;cursor:pointer;position:relative;margin:2px 0 0 0;padding:.5em .5em .5em .7em;min-height:0;font-size:100%}.ui-accordion .ui-accordion-icons{padding-left:2.2em}.ui-accordion .ui-accordion-icons .ui-accordion-icons{padding-left:2.2em}.ui-accordion .ui-accordion-header .ui-accordion-header-icon{position:absolute;left:.5em;top:50%;margin-top:-8px}.ui-accordion .ui-accordion-content{padding:1em 2.2em;border-top:0;overflow:auto}.ui-autocomplete{position:absolute;top:0;left:0;cursor:default}.ui-button{display:inline-block;position:relative;padding:0;line-height:normal;margin-right:.1em;cursor:pointer;vertical-align:middle;text-align:center;overflow:visible}.ui-button,.ui-button:link,.ui-button:visited,.ui-button:hover,.ui-button:active{text-decoration:none}.ui-button-icon-only{width:2.2em}button.ui-button-icon-only{width:2.4em}.ui-button-icons-only{width:3.4em}button.ui-button-icons-only{width:3.7em}.ui-button .ui-button-text{display:block;line-height:normal}.ui-button-text-only .ui-button-text{padding:.4em 1em}.ui-button-icon-only .ui-button-text,.ui-button-icons-only .ui-button-text{padding:.4em;text-indent:-9999999px}.ui-button-text-icon-primary .ui-button-text,.ui-button-text-icons .ui-button-text{padding:.4em 1em .4em 2.1em}.ui-button-text-icon-secondary .ui-button-text,.ui-button-text-icons .ui-button-text{padding:.4em 2.1em .4em 1em}.ui-button-text-icons .ui-button-text{padding-left:2.1em;padding-right:2.1em}input.ui-button{padding:.4em 1em}.ui-button-icon-only .ui-icon,.ui-button-text-icon-primary .ui-icon,.ui-button-text-icon-secondary .ui-icon,.ui-button-text-icons .ui-icon,.ui-button-icons-only .ui-icon{position:absolute;top:50%;margin-top:-8px}.ui-button-icon-only .ui-icon{left:50%;margin-left:-8px}.ui-button-text-icon-primary .ui-button-icon-primary,.ui-button-text-icons .ui-button-icon-primary,.ui-button-icons-only .ui-button-icon-primary{left:.5em}.ui-button-text-icon-secondary .ui-button-icon-secondary,.ui-button-text-icons .ui-button-icon-secondary,.ui-button-icons-only .ui-button-icon-secondary{right:.5em}.ui-buttonset{margin-right:7px}.ui-buttonset .ui-button{margin-left:0;margin-right:-.3em}input.ui-button::-moz-focus-inner,button.ui-button::-moz-focus-inner{border:0;padding:0}.ui-datepicker{width:17em;padding:.2em .2em 0;display:none}.ui-datepicker .ui-datepicker-header{position:relative;padding:.2em 0}.ui-datepicker .ui-datepicker-prev,.ui-datepicker .ui-datepicker-next{position:absolute;top:2px;width:1.8em;height:1.8em}.ui-datepicker .ui-datepicker-prev-hover,.ui-datepicker .ui-datepicker-next-hover{top:1px}.ui-datepicker .ui-datepicker-prev{left:2px}.ui-datepicker .ui-datepicker-next{right:2px}.ui-datepicker .ui-datepicker-prev-hover{left:1px}.ui-datepicker .ui-datepicker-next-hover{right:1px}.ui-datepicker .ui-datepicker-prev span,.ui-datepicker .ui-datepicker-next span{display:block;position:absolute;left:50%;margin-left:-8px;top:50%;margin-top:-8px}.ui-datepicker .ui-datepicker-title{margin:0 2.3em;line-height:1.8em;text-align:center}.ui-datepicker .ui-datepicker-title select{font-size:1em;margin:1px 0}.ui-datepicker select.ui-datepicker-month,.ui-datepicker select.ui-datepicker-year{width:45%}.ui-datepicker table{width:100%;font-size:.9em;border-collapse:collapse;margin:0 0 .4em}.ui-datepicker th{padding:.7em .3em;text-align:center;font-weight:bold;border:0}.ui-datepicker td{border:0;padding:1px}.ui-datepicker td span,.ui-datepicker td a{display:block;padding:.2em;text-align:right;text-decoration:none}.ui-datepicker .ui-datepicker-buttonpane{background-image:none;margin:.7em 0 0 0;padding:0 .2em;border-left:0;border-right:0;border-bottom:0}.ui-datepicker .ui-datepicker-buttonpane button{float:right;margin:.5em .2em .4em;cursor:pointer;padding:.2em .6em .3em .6em;width:auto;overflow:visible}.ui-datepicker .ui-datepicker-buttonpane button.ui-datepicker-current{float:left}.ui-datepicker.ui-datepicker-multi{width:auto}.ui-datepicker-multi .ui-datepicker-group{float:left}.ui-datepicker-multi .ui-datepicker-group table{width:95%;margin:0 auto .4em}.ui-datepicker-multi-2 .ui-datepicker-group{width:50%}.ui-datepicker-multi-3 .ui-datepicker-group{width:33.3%}.ui-datepicker-multi-4 .ui-datepicker-group{width:25%}.ui-datepicker-multi .ui-datepicker-group-last .ui-datepicker-header,.ui-datepicker-multi .ui-datepicker-group-middle .ui-datepicker-header{border-left-width:0}.ui-datepicker-multi .ui-datepicker-buttonpane{clear:left}.ui-datepicker-row-break{clear:both;width:100%;font-size:0}.ui-datepicker-rtl{direction:rtl}.ui-datepicker-rtl .ui-datepicker-prev{right:2px;left:auto}.ui-datepicker-rtl .ui-datepicker-next{left:2px;right:auto}.ui-datepicker-rtl .ui-datepicker-prev:hover{right:1px;left:auto}.ui-datepicker-rtl .ui-datepicker-next:hover{left:1px;right:auto}.ui-datepicker-rtl .ui-datepicker-buttonpane{clear:right}.ui-datepicker-rtl .ui-datepicker-buttonpane button{float:left}.ui-datepicker-rtl .ui-datepicker-buttonpane button.ui-datepicker-current,.ui-datepicker-rtl .ui-datepicker-group{float:right}.ui-datepicker-rtl .ui-datepicker-group-last .ui-datepicker-header,.ui-datepicker-rtl .ui-datepicker-group-middle .ui-datepicker-header{border-right-width:0;border-left-width:1px}.ui-dialog{overflow:hidden;position:absolute;top:0;left:0;padding:.2em;outline:0}.ui-dialog .ui-dialog-titlebar{padding:.4em 1em;position:relative}.ui-dialog .ui-dialog-title{float:left;margin:.1em 0;white-space:nowrap;width:90%;overflow:hidden;text-overflow:ellipsis}.ui-dialog .ui-dialog-titlebar-close{position:absolute;right:.3em;top:50%;width:20px;margin:-10px 0 0 0;padding:1px;height:20px}.ui-dialog .ui-dialog-content{position:relative;border:0;padding:.5em 1em;background:none;overflow:auto}.ui-dialog .ui-dialog-buttonpane{text-align:left;border-width:1px 0 0 0;background-image:none;margin-top:.5em;padding:.3em 1em .5em .4em}.ui-dialog .ui-dialog-buttonpane .ui-dialog-buttonset{float:right}.ui-dialog .ui-dialog-buttonpane button{margin:.5em .4em .5em 0;cursor:pointer}.ui-dialog .ui-resizable-se{width:12px;height:12px;right:-5px;bottom:-5px;background-position:16px 16px}.ui-draggable .ui-dialog-titlebar{cursor:move}.ui-menu{list-style:none;padding:0;margin:0;display:block;outline:none}.ui-menu .ui-menu{position:absolute}.ui-menu .ui-menu-item{position:relative;margin:0;padding:3px 1em 3px .4em;cursor:pointer;min-height:0;list-style-image:url("data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7")}.ui-menu .ui-menu-divider{margin:5px 0;height:0;font-size:0;line-height:0;border-width:1px 0 0 0}.ui-menu .ui-state-focus,.ui-menu .ui-state-active{margin:-1px}.ui-menu-icons{position:relative}.ui-menu-icons .ui-menu-item{padding-left:2em}.ui-menu .ui-icon{position:absolute;top:0;bottom:0;left:.2em;margin:auto 0}.ui-menu .ui-menu-icon{left:auto;right:0}.ui-progressbar{height:2em;text-align:left;overflow:hidden}.ui-progressbar .ui-progressbar-value{margin:-1px;height:100%}.ui-progressbar .ui-progressbar-overlay{background:url("data:image/gif;base64,R0lGODlhKAAoAIABAAAAAP///yH/C05FVFNDQVBFMi4wAwEAAAAh+QQJAQABACwAAAAAKAAoAAACkYwNqXrdC52DS06a7MFZI+4FHBCKoDeWKXqymPqGqxvJrXZbMx7Ttc+w9XgU2FB3lOyQRWET2IFGiU9m1frDVpxZZc6bfHwv4c1YXP6k1Vdy292Fb6UkuvFtXpvWSzA+HycXJHUXiGYIiMg2R6W459gnWGfHNdjIqDWVqemH2ekpObkpOlppWUqZiqr6edqqWQAAIfkECQEAAQAsAAAAACgAKAAAApSMgZnGfaqcg1E2uuzDmmHUBR8Qil95hiPKqWn3aqtLsS18y7G1SzNeowWBENtQd+T1JktP05nzPTdJZlR6vUxNWWjV+vUWhWNkWFwxl9VpZRedYcflIOLafaa28XdsH/ynlcc1uPVDZxQIR0K25+cICCmoqCe5mGhZOfeYSUh5yJcJyrkZWWpaR8doJ2o4NYq62lAAACH5BAkBAAEALAAAAAAoACgAAAKVDI4Yy22ZnINRNqosw0Bv7i1gyHUkFj7oSaWlu3ovC8GxNso5fluz3qLVhBVeT/Lz7ZTHyxL5dDalQWPVOsQWtRnuwXaFTj9jVVh8pma9JjZ4zYSj5ZOyma7uuolffh+IR5aW97cHuBUXKGKXlKjn+DiHWMcYJah4N0lYCMlJOXipGRr5qdgoSTrqWSq6WFl2ypoaUAAAIfkECQEAAQAsAAAAACgAKAAAApaEb6HLgd/iO7FNWtcFWe+ufODGjRfoiJ2akShbueb0wtI50zm02pbvwfWEMWBQ1zKGlLIhskiEPm9R6vRXxV4ZzWT2yHOGpWMyorblKlNp8HmHEb/lCXjcW7bmtXP8Xt229OVWR1fod2eWqNfHuMjXCPkIGNileOiImVmCOEmoSfn3yXlJWmoHGhqp6ilYuWYpmTqKUgAAIfkECQEAAQAsAAAAACgAKAAAApiEH6kb58biQ3FNWtMFWW3eNVcojuFGfqnZqSebuS06w5V80/X02pKe8zFwP6EFWOT1lDFk8rGERh1TTNOocQ61Hm4Xm2VexUHpzjymViHrFbiELsefVrn6XKfnt2Q9G/+Xdie499XHd2g4h7ioOGhXGJboGAnXSBnoBwKYyfioubZJ2Hn0RuRZaflZOil56Zp6iioKSXpUAAAh+QQJAQABACwAAAAAKAAoAAACkoQRqRvnxuI7kU1a1UU5bd5tnSeOZXhmn5lWK3qNTWvRdQxP8qvaC+/yaYQzXO7BMvaUEmJRd3TsiMAgswmNYrSgZdYrTX6tSHGZO73ezuAw2uxuQ+BbeZfMxsexY35+/Qe4J1inV0g4x3WHuMhIl2jXOKT2Q+VU5fgoSUI52VfZyfkJGkha6jmY+aaYdirq+lQAACH5BAkBAAEALAAAAAAoACgAAAKWBIKpYe0L3YNKToqswUlvznigd4wiR4KhZrKt9Upqip61i9E3vMvxRdHlbEFiEXfk9YARYxOZZD6VQ2pUunBmtRXo1Lf8hMVVcNl8JafV38aM2/Fu5V16Bn63r6xt97j09+MXSFi4BniGFae3hzbH9+hYBzkpuUh5aZmHuanZOZgIuvbGiNeomCnaxxap2upaCZsq+1kAACH5BAkBAAEALAAAAAAoACgAAAKXjI8By5zf4kOxTVrXNVlv1X0d8IGZGKLnNpYtm8Lr9cqVeuOSvfOW79D9aDHizNhDJidFZhNydEahOaDH6nomtJjp1tutKoNWkvA6JqfRVLHU/QUfau9l2x7G54d1fl995xcIGAdXqMfBNadoYrhH+Mg2KBlpVpbluCiXmMnZ2Sh4GBqJ+ckIOqqJ6LmKSllZmsoq6wpQAAAh+QQJAQABACwAAAAAKAAoAAAClYx/oLvoxuJDkU1a1YUZbJ59nSd2ZXhWqbRa2/gF8Gu2DY3iqs7yrq+xBYEkYvFSM8aSSObE+ZgRl1BHFZNr7pRCavZ5BW2142hY3AN/zWtsmf12p9XxxFl2lpLn1rseztfXZjdIWIf2s5dItwjYKBgo9yg5pHgzJXTEeGlZuenpyPmpGQoKOWkYmSpaSnqKileI2FAAACH5BAkBAAEALAAAAAAoACgAAAKVjB+gu+jG4kORTVrVhRlsnn2dJ3ZleFaptFrb+CXmO9OozeL5VfP99HvAWhpiUdcwkpBH3825AwYdU8xTqlLGhtCosArKMpvfa1mMRae9VvWZfeB2XfPkeLmm18lUcBj+p5dnN8jXZ3YIGEhYuOUn45aoCDkp16hl5IjYJvjWKcnoGQpqyPlpOhr3aElaqrq56Bq7VAAAOw==");height:100%;filter:alpha(opacity=25);opacity:0.25}.ui-progressbar-indeterminate .ui-progressbar-value{background-image:none}.ui-selectmenu-menu{padding:0;margin:0;position:absolute;top:0;left:0;display:none}.ui-selectmenu-menu .ui-menu{overflow:auto;overflow-x:hidden;padding-bottom:1px}.ui-selectmenu-menu .ui-menu .ui-selectmenu-optgroup{font-size:1em;font-weight:bold;line-height:1.5;padding:2px 0.4em;margin:0.5em 0 0 0;height:auto;border:0}.ui-selectmenu-open{display:block}.ui-selectmenu-button{display:inline-block;overflow:hidden;position:relative;text-decoration:none;cursor:pointer}.ui-selectmenu-button span.ui-icon{right:0.5em;left:auto;margin-top:-8px;position:absolute;top:50%}.ui-selectmenu-button span.ui-selectmenu-text{text-align:left;padding:0.4em 2.1em 0.4em 1em;display:block;line-height:1.4;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.ui-slider{position:relative;text-align:left}.ui-slider .ui-slider-handle{position:absolute;z-index:2;width:1.2em;height:1.2em;cursor:default;-ms-touch-action:none;touch-action:none}.ui-slider .ui-slider-range{position:absolute;z-index:1;font-size:.7em;display:block;border:0;background-position:0 0}.ui-slider.ui-state-disabled .ui-slider-handle,.ui-slider.ui-state-disabled .ui-slider-range{filter:inherit}.ui-slider-horizontal{height:.8em}.ui-slider-horizontal .ui-slider-handle{top:-.3em;margin-left:-.6em}.ui-slider-horizontal .ui-slider-range{top:0;height:100%}.ui-slider-horizontal .ui-slider-range-min{left:0}.ui-slider-horizontal .ui-slider-range-max{right:0}.ui-slider-vertical{width:.8em;height:100px}.ui-slider-vertical .ui-slider-handle{left:-.3em;margin-left:0;margin-bottom:-.6em}.ui-slider-vertical .ui-slider-range{left:0;width:100%}.ui-slider-vertical .ui-slider-range-min{bottom:0}.ui-slider-vertical .ui-slider-range-max{top:0}.ui-spinner{position:relative;display:inline-block;overflow:hidden;padding:0;vertical-align:middle}.ui-spinner-input{border:none;background:none;color:inherit;padding:0;margin:.2em 0;vertical-align:middle;margin-left:.4em;margin-right:22px}.ui-spinner-button{width:16px;height:50%;font-size:.5em;padding:0;margin:0;text-align:center;position:absolute;cursor:default;display:block;overflow:hidden;right:0}.ui-spinner a.ui-spinner-button{border-top:none;border-bottom:none;border-right:none}.ui-spinner .ui-icon{position:absolute;margin-top:-8px;top:50%;left:0}.ui-spinner-up{top:0}.ui-spinner-down{bottom:0}.ui-spinner .ui-icon-triangle-1-s{background-position:-65px -16px}.ui-tabs{position:relative;padding:.2em}.ui-tabs .ui-tabs-nav{margin:0;padding:.2em .2em 0}.ui-tabs .ui-tabs-nav li{list-style:none;float:left;position:relative;top:0;margin:1px .2em 0 0;border-bottom-width:0;padding:0;white-space:nowrap}.ui-tabs .ui-tabs-nav .ui-tabs-anchor{float:left;padding:.5em 1em;text-decoration:none}.ui-tabs .ui-tabs-nav li.ui-tabs-active{margin-bottom:-1px;padding-bottom:1px}.ui-tabs .ui-tabs-nav li.ui-tabs-active .ui-tabs-anchor,.ui-tabs .ui-tabs-nav li.ui-state-disabled .ui-tabs-anchor,.ui-tabs .ui-tabs-nav li.ui-tabs-loading .ui-tabs-anchor{cursor:text}.ui-tabs-collapsible .ui-tabs-nav li.ui-tabs-active .ui-tabs-anchor{cursor:pointer}.ui-tabs .ui-tabs-panel{display:block;border-width:0;padding:1em 1.4em;background:none}.ui-tooltip{padding:8px;position:absolute;z-index:9999;max-width:300px;-webkit-box-shadow:0 0 5px #aaa;box-shadow:0 0 5px #aaa}body .ui-tooltip{border-width:2px}.ui-widget{font-family:Arial,Helvetica,sans-serif;font-size:1em}.ui-widget .ui-widget{font-size:1em}.ui-widget input,.ui-widget select,.ui-widget textarea,.ui-widget button{font-family:Arial,Helvetica,sans-serif;font-size:1em}.ui-widget-content{border:1px solid #66c2ff;background:#fff;color:#333}.ui-widget-content a{color:#333}.ui-widget-header{border:1px solid #fff;background:#fff;color:#333;font-weight:bold}.ui-widget-header a{color:#333}.ui-state-default,.ui-widget-content .ui-state-default,.ui-widget-header .ui-state-default{border:1px solid #c5c5c5;background:#fff;font-weight:normal;color:#454545}.ui-state-default a,.ui-state-default a:link,.ui-state-default a:visited{color:#454545;text-decoration:none}.ui-state-hover,.ui-widget-content .ui-state-hover,.ui-widget-header .ui-state-hover,.ui-state-focus,.ui-widget-content .ui-state-focus,.ui-widget-header .ui-state-focus{border:1px solid #ccc;background:#ededed;font-weight:normal;color:#2b2b2b}.ui-state-hover a,.ui-state-hover a:hover,.ui-state-hover a:link,.ui-state-hover a:visited,.ui-state-focus a,.ui-state-focus a:hover,.ui-state-focus a:link,.ui-state-focus a:visited{color:#2b2b2b;text-decoration:none}.ui-state-active,.ui-widget-content .ui-state-active,.ui-widget-header .ui-state-active{border:1px solid #66c2ff;background:#66c2ff;font-weight:normal;color:#fff}.ui-state-active a,.ui-state-active a:link,.ui-state-active a:visited{color:#fff;text-decoration:none}.ui-state-highlight,.ui-widget-content .ui-state-highlight,.ui-widget-header .ui-state-highlight{border:1px solid #dad55e;background:#fffa90;color:#777620}.ui-state-highlight a,.ui-widget-content .ui-state-highlight a,.ui-widget-header .ui-state-highlight a{color:#777620}.ui-state-error,.ui-widget-content .ui-state-error,.ui-widget-header .ui-state-error{border:1px solid #f1a899;background:#fddfdf;color:#5f3f3f}.ui-state-error a,.ui-widget-content .ui-state-error a,.ui-widget-header .ui-state-error a{color:#5f3f3f}.ui-state-error-text,.ui-widget-content .ui-state-error-text,.ui-widget-header .ui-state-error-text{color:#5f3f3f}.ui-priority-primary,.ui-widget-content .ui-priority-primary,.ui-widget-header .ui-priority-primary{font-weight:bold}.ui-priority-secondary,.ui-widget-content .ui-priority-secondary,.ui-widget-header .ui-priority-secondary{opacity:.7;filter:Alpha(Opacity=70);font-weight:normal}.ui-state-disabled,.ui-widget-content .ui-state-disabled,.ui-widget-header .ui-state-disabled{opacity:.35;filter:Alpha(Opacity=35);background-image:none}.ui-state-disabled .ui-icon{filter:Alpha(Opacity=35)}.ui-icon{width:16px;height:16px}.ui-icon,.ui-widget-content .ui-icon{background-image:url("images/ui-icons_444444_256x240.png")}.ui-widget-header .ui-icon{background-image:url("images/ui-icons_444444_256x240.png")}.ui-state-default .ui-icon{background-image:url("images/ui-icons_777777_256x240.png")}.ui-state-hover .ui-icon,.ui-state-focus .ui-icon{background-image:url("images/ui-icons_555555_256x240.png")}.ui-state-active .ui-icon{background-image:url("images/ui-icons_ffffff_256x240.png")}.ui-state-highlight .ui-icon{background-image:url("images/ui-icons_777620_256x240.png")}.ui-state-error .ui-icon,.ui-state-error-text .ui-icon{background-image:url("images/ui-icons_cc0000_256x240.png")}.ui-icon-blank{background-position:16px 16px}.ui-icon-carat-1-n{background-position:0 0}.ui-icon-carat-1-ne{background-position:-16px 0}.ui-icon-carat-1-e{background-position:-32px 0}.ui-icon-carat-1-se{background-position:-48px 0}.ui-icon-carat-1-s{background-position:-64px 0}.ui-icon-carat-1-sw{background-position:-80px 0}.ui-icon-carat-1-w{background-position:-96px 0}.ui-icon-carat-1-nw{background-position:-112px 0}.ui-icon-carat-2-n-s{background-position:-128px 0}.ui-icon-carat-2-e-w{background-position:-144px 0}.ui-icon-triangle-1-n{background-position:0 -16px}.ui-icon-triangle-1-ne{background-position:-16px -16px}.ui-icon-triangle-1-e{background-position:-32px -16px}.ui-icon-triangle-1-se{background-position:-48px -16px}.ui-icon-triangle-1-s{background-position:-64px -16px}.ui-icon-triangle-1-sw{background-position:-80px -16px}.ui-icon-triangle-1-w{background-position:-96px -16px}.ui-icon-triangle-1-nw{background-position:-112px -16px}.ui-icon-triangle-2-n-s{background-position:-128px -16px}.ui-icon-triangle-2-e-w{background-position:-144px -16px}.ui-icon-arrow-1-n{background-position:0 -32px}.ui-icon-arrow-1-ne{background-position:-16px -32px}.ui-icon-arrow-1-e{background-position:-32px -32px}.ui-icon-arrow-1-se{background-position:-48px -32px}.ui-icon-arrow-1-s{background-position:-64px -32px}.ui-icon-arrow-1-sw{background-position:-80px -32px}.ui-icon-arrow-1-w{background-position:-96px -32px}.ui-icon-arrow-1-nw{background-position:-112px -32px}.ui-icon-arrow-2-n-s{background-position:-128px -32px}.ui-icon-arrow-2-ne-sw{background-position:-144px -32px}.ui-icon-arrow-2-e-w{background-position:-160px -32px}.ui-icon-arrow-2-se-nw{background-position:-176px -32px}.ui-icon-arrowstop-1-n{background-position:-192px -32px}.ui-icon-arrowstop-1-e{background-position:-208px -32px}.ui-icon-arrowstop-1-s{background-position:-224px -32px}.ui-icon-arrowstop-1-w{background-position:-240px -32px}.ui-icon-arrowthick-1-n{background-position:0 -48px}.ui-icon-arrowthick-1-ne{background-position:-16px -48px}.ui-icon-arrowthick-1-e{background-position:-32px -48px}.ui-icon-arrowthick-1-se{background-position:-48px -48px}.ui-icon-arrowthick-1-s{background-position:-64px -48px}.ui-icon-arrowthick-1-sw{background-position:-80px -48px}.ui-icon-arrowthick-1-w{background-position:-96px -48px}.ui-icon-arrowthick-1-nw{background-position:-112px -48px}.ui-icon-arrowthick-2-n-s{background-position:-128px -48px}.ui-icon-arrowthick-2-ne-sw{background-position:-144px -48px}.ui-icon-arrowthick-2-e-w{background-position:-160px -48px}.ui-icon-arrowthick-2-se-nw{background-position:-176px -48px}.ui-icon-arrowthickstop-1-n{background-position:-192px -48px}.ui-icon-arrowthickstop-1-e{background-position:-208px -48px}.ui-icon-arrowthickstop-1-s{background-position:-224px -48px}.ui-icon-arrowthickstop-1-w{background-position:-240px -48px}.ui-icon-arrowreturnthick-1-w{background-position:0 -64px}.ui-icon-arrowreturnthick-1-n{background-position:-16px -64px}.ui-icon-arrowreturnthick-1-e{background-position:-32px -64px}.ui-icon-arrowreturnthick-1-s{background-position:-48px -64px}.ui-icon-arrowreturn-1-w{background-position:-64px -64px}.ui-icon-arrowreturn-1-n{background-position:-80px -64px}.ui-icon-arrowreturn-1-e{background-position:-96px -64px}.ui-icon-arrowreturn-1-s{background-position:-112px -64px}.ui-icon-arrowrefresh-1-w{background-position:-128px -64px}.ui-icon-arrowrefresh-1-n{background-position:-144px -64px}.ui-icon-arrowrefresh-1-e{background-position:-160px -64px}.ui-icon-arrowrefresh-1-s{background-position:-176px -64px}.ui-icon-arrow-4{background-position:0 -80px}.ui-icon-arrow-4-diag{background-position:-16px -80px}.ui-icon-extlink{background-position:-32px -80px}.ui-icon-newwin{background-position:-48px -80px}.ui-icon-refresh{background-position:-64px -80px}.ui-icon-shuffle{background-position:-80px -80px}.ui-icon-transfer-e-w{background-position:-96px -80px}.ui-icon-transferthick-e-w{background-position:-112px -80px}.ui-icon-folder-collapsed{background-position:0 -96px}.ui-icon-folder-open{background-position:-16px -96px}.ui-icon-document{background-position:-32px -96px}.ui-icon-document-b{background-position:-48px -96px}.ui-icon-note{background-position:-64px -96px}.ui-icon-mail-closed{background-position:-80px -96px}.ui-icon-mail-open{background-position:-96px -96px}.ui-icon-suitcase{background-position:-112px -96px}.ui-icon-comment{background-position:-128px -96px}.ui-icon-person{background-position:-144px -96px}.ui-icon-print{background-position:-160px -96px}.ui-icon-trash{background-position:-176px -96px}.ui-icon-locked{background-position:-192px -96px}.ui-icon-unlocked{background-position:-208px -96px}.ui-icon-bookmark{background-position:-224px -96px}.ui-icon-tag{background-position:-240px -96px}.ui-icon-home{background-position:0 -112px}.ui-icon-flag{background-position:-16px -112px}.ui-icon-calendar{background-position:-32px -112px}.ui-icon-cart{background-position:-48px -112px}.ui-icon-pencil{background-position:-64px -112px}.ui-icon-clock{background-position:-80px -112px}.ui-icon-disk{background-position:-96px -112px}.ui-icon-calculator{background-position:-112px -112px}.ui-icon-zoomin{background-position:-128px -112px}.ui-icon-zoomout{background-position:-144px -112px}.ui-icon-search{background-position:-160px -112px}.ui-icon-wrench{background-position:-176px -112px}.ui-icon-gear{background-position:-192px -112px}.ui-icon-heart{background-position:-208px -112px}.ui-icon-star{background-position:-224px -112px}.ui-icon-link{background-position:-240px -112px}.ui-icon-cancel{background-position:0 -128px}.ui-icon-plus{background-position:-16px -128px}.ui-icon-plusthick{background-position:-32px -128px}.ui-icon-minus{background-position:-48px -128px}.ui-icon-minusthick{background-position:-64px -128px}.ui-icon-close{background-position:-80px -128px}.ui-icon-closethick{background-position:-96px -128px}.ui-icon-key{background-position:-112px -128px}.ui-icon-lightbulb{background-position:-128px -128px}.ui-icon-scissors{background-position:-144px -128px}.ui-icon-clipboard{background-position:-160px -128px}.ui-icon-copy{background-position:-176px -128px}.ui-icon-contact{background-position:-192px -128px}.ui-icon-image{background-position:-208px -128px}.ui-icon-video{background-position:-224px -128px}.ui-icon-script{background-position:-240px -128px}.ui-icon-alert{background-position:0 -144px}.ui-icon-info{background-position:-16px -144px}.ui-icon-notice{background-position:-32px -144px}.ui-icon-help{background-position:-48px -144px}.ui-icon-check{background-position:-64px -144px}.ui-icon-bullet{background-position:-80px -144px}.ui-icon-radio-on{background-position:-96px -144px}.ui-icon-radio-off{background-position:-112px -144px}.ui-icon-pin-w{background-position:-128px -144px}.ui-icon-pin-s{background-position:-144px -144px}.ui-icon-play{background-position:0 -160px}.ui-icon-pause{background-position:-16px -160px}.ui-icon-seek-next{background-position:-32px -160px}.ui-icon-seek-prev{background-position:-48px -160px}.ui-icon-seek-end{background-position:-64px -160px}.ui-icon-seek-start{background-position:-80px -160px}.ui-icon-seek-first{background-position:-80px -160px}.ui-icon-stop{background-position:-96px -160px}.ui-icon-eject{background-position:-112px -160px}.ui-icon-volume-off{background-position:-128px -160px}.ui-icon-volume-on{background-position:-144px -160px}.ui-icon-power{background-position:0 -176px}.ui-icon-signal-diag{background-position:-16px -176px}.ui-icon-signal{background-position:-32px -176px}.ui-icon-battery-0{background-position:-48px -176px}.ui-icon-battery-1{background-position:-64px -176px}.ui-icon-battery-2{background-position:-80px -176px}.ui-icon-battery-3{background-position:-96px -176px}.ui-icon-circle-plus{background-position:0 -192px}.ui-icon-circle-minus{background-position:-16px -192px}.ui-icon-circle-close{background-position:-32px -192px}.ui-icon-circle-triangle-e{background-position:-48px -192px}.ui-icon-circle-triangle-s{background-position:-64px -192px}.ui-icon-circle-triangle-w{background-position:-80px -192px}.ui-icon-circle-triangle-n{background-position:-96px -192px}.ui-icon-circle-arrow-e{background-position:-112px -192px}.ui-icon-circle-arrow-s{background-position:-128px -192px}.ui-icon-circle-arrow-w{background-position:-144px -192px}.ui-icon-circle-arrow-n{background-position:-160px -192px}.ui-icon-circle-zoomin{background-position:-176px -192px}.ui-icon-circle-zoomout{background-position:-192px -192px}.ui-icon-circle-check{background-position:-208px -192px}.ui-icon-circlesmall-plus{background-position:0 -208px}.ui-icon-circlesmall-minus{background-position:-16px -208px}.ui-icon-circlesmall-close{background-position:-32px -208px}.ui-icon-squaresmall-plus{background-position:-48px -208px}.ui-icon-squaresmall-minus{background-position:-64px -208px}.ui-icon-squaresmall-close{background-position:-80px -208px}.ui-icon-grip-dotted-vertical{background-position:0 -224px}.ui-icon-grip-dotted-horizontal{background-position:-16px -224px}.ui-icon-grip-solid-vertical{background-position:-32px -224px}.ui-icon-grip-solid-horizontal{background-position:-48px -224px}.ui-icon-gripsmall-diagonal-se{background-position:-64px -224px}.ui-icon-grip-diagonal-se{background-position:-80px -224px}.ui-corner-all,.ui-corner-top,.ui-corner-left,.ui-corner-tl{border-top-left-radius:3px}.ui-corner-all,.ui-corner-top,.ui-corner-right,.ui-corner-tr{border-top-right-radius:3px}.ui-corner-all,.ui-corner-bottom,.ui-corner-left,.ui-corner-bl{border-bottom-left-radius:3px}.ui-corner-all,.ui-corner-bottom,.ui-corner-right,.ui-corner-br{border-bottom-right-radius:3px}.ui-widget-overlay{background:#aaa;opacity:.3;filter:Alpha(Opacity=30)}.ui-widget-shadow{margin:0 0 0 0;padding:5px;background:#666;opacity:.3;filter:Alpha(Opacity=30);border-radius:8px}
```

### Comparing `evv4esm-0.5.0/evv4esm/resources/css/lightbox.min.css` & `evv4esm-0.5.1/evv4esm/resources/css/lightbox.min.css`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/resources/css/livv.css` & `evv4esm-0.5.1/evv4esm/resources/css/livv.css`

 * *Files 0% similar despite different names*

```diff
@@ -54,18 +54,18 @@
 }
 
 #header a{
     text-decoration: none;
 }
 
 #header-icon {
-    float: left; 
-    padding: 12px; 
+    float: left;
+    padding: 12px;
     padding-left: 15px;
-    width: 70px; 
+    width: 70px;
 }
 
 #header-home {
 	float: left;
     color: #F26C3A;
     height: 1.25em;
    	line-height: 1.25em;
@@ -145,15 +145,15 @@
 }
 
 .testCase {
     text-align: right;
 }
 
 /******************************************************************************
-  Element Styling 
+  Element Styling
 ******************************************************************************/
 .error {}
 
 .error p {
     color: red;
 }
```

### Comparing `evv4esm-0.5.0/evv4esm/resources/css/normalize.css` & `evv4esm-0.5.1/evv4esm/resources/css/normalize.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -342,8 +342,8 @@
 
 /**
  * Add the correct display in IE 10.
  */
 
 [hidden] {
   display: none;
-}
+}
```

### Comparing `evv4esm-0.5.0/evv4esm/resources/favicon.ico` & `evv4esm-0.5.1/evv4esm/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/resources/imgs/DOE-BER-logo.png` & `evv4esm-0.5.1/evv4esm/resources/imgs/DOE-BER-logo.png`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/resources/imgs/DOE-logo.png` & `evv4esm-0.5.1/evv4esm/resources/imgs/DOE-logo.png`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/resources/imgs/ORNL-logo.png` & `evv4esm-0.5.1/evv4esm/resources/imgs/ORNL-logo.png`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/resources/imgs/background.jpg` & `evv4esm-0.5.1/evv4esm/resources/imgs/background.jpg`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/resources/imgs/icon.svg` & `evv4esm-0.5.1/evv4esm/resources/imgs/icon.svg`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/resources/imgs/loading.gif` & `evv4esm-0.5.1/evv4esm/resources/imgs/loading.gif`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/resources/imgs/next.png` & `evv4esm-0.5.1/evv4esm/resources/imgs/next.png`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/resources/imgs/prev.png` & `evv4esm-0.5.1/evv4esm/resources/imgs/prev.png`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/resources/index.html` & `evv4esm-0.5.1/evv4esm/resources/index.html`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/resources/js/common.js` & `evv4esm-0.5.1/evv4esm/resources/js/common.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 /*
 / Copyright (c) 2015-2023, UT-BATTELLE, LLC
 / All rights reserved.
-/ 
+/
 / Redistribution and use in source and binary forms, with or without
 / modification, are permitted provided that the following conditions are met:
-/ 
+/
 / 1. Redistributions of source code must retain the above copyright notice, this
 / list of conditions and the following disclaimer.
-/ 
+/
 / 2. Redistributions in binary form must reproduce the above copyright notice,
 / this list of conditions and the following disclaimer in the documentation
 / and/or other materials provided with the distribution.
-/ 
+/
 / 3. Neither the name of the copyright holder nor the names of its contributors
 / may be used to endorse or promote products derived from this software without
 / specific prior written permission.
-/ 
+/
 / THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
 / ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 / WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 / DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 / FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 / DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 / SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
@@ -61,15 +61,15 @@
             )
         )
     );
 });
 
 
 /**
- * Draws the navigation sidebar by looking at the index.json data and appends the 
+ * Draws the navigation sidebar by looking at the index.json data and appends the
  * list of resultant pages to the nav div.
  */
 function drawNav() {
     // Get the dataset, to do so the html page must have the `indexPath` variable defined
     var html = "";
     var getUrl = window.location.href.substr(0, window.location.href.lastIndexOf('/') + 1);
     var data = loadJSON(getUrl + indexPath + '/index.json');
@@ -86,15 +86,15 @@
         }
     }
     $("#nav").append(html);
 }
 
 
 /**
- * Draws content to the page by looking at the name of the page and loading the 
+ * Draws content to the page by looking at the name of the page and loading the
  * appropriate dataset.
  */
 function drawContent() {
     // Load the data and add header information
     var html_file = window.location.href.substr(
         window.location.href.lastIndexOf("/") + 1).split("#")[0].replace(".html", "");
     // Assume index.html if empty page name
```

### Comparing `evv4esm-0.5.0/evv4esm/resources/js/jquery-ui.min.js` & `evv4esm-0.5.1/evv4esm/resources/js/jquery-ui.min.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with very long lines (32035)*

 * *Files 0% similar despite different names*

```diff
@@ -15020,8 +15020,8 @@
 0003aab0: 7474 7228 2274 6974 6c65 2229 7c7c 612e  ttr("title")||a.
 0003aac0: 6174 7472 2822 7469 746c 6522 2c61 2e64  attr("title",a.d
 0003aad0: 6174 6128 2275 692d 746f 6f6c 7469 702d  ata("ui-tooltip-
 0003aae0: 7469 746c 6522 2929 2c61 2e72 656d 6f76  title")),a.remov
 0003aaf0: 6544 6174 6128 2275 692d 746f 6f6c 7469  eData("ui-toolti
 0003ab00: 702d 7469 746c 6522 2929 7d29 2c74 6869  p-title"))}),thi
 0003ab10: 732e 6c69 7665 5265 6769 6f6e 2e72 656d  s.liveRegion.rem
-0003ab20: 6f76 6528 297d 7d29 7d29 3b              ove()}})});
+0003ab20: 6f76 6528 297d 7d29 7d29 3b0a            ove()}})});.
```

### Comparing `evv4esm-0.5.0/evv4esm/resources/js/jquery.caption.min.js` & `evv4esm-0.5.1/evv4esm/resources/js/jquery.caption.min.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, Unicode text, UTF-8 text, with very long lines (2033)*

 * *Files 0% similar despite different names*

```diff
@@ -138,8 +138,8 @@
 00000890: 616e 696d 6174 6564 223d 3d3d 732e 6d6f  animated"===s.mo
 000008a0: 6465 2626 722e 6373 7328 7b62 6f74 746f  de&&r.css({botto
 000008b0: 6d3a 2d69 7d29 2c22 6869 6464 656e 223d  m:-i}),"hidden"=
 000008c0: 3d3d 732e 6d6f 6465 2626 722e 6373 7328  ==s.mode&&r.css(
 000008d0: 7b22 6d61 7267 696e 2d62 6f74 746f 6d22  {"margin-bottom"
 000008e0: 3a69 2c62 6f74 746f 6d3a 2d69 7d29 7d29  :i,bottom:-i})})
 000008f0: 7d29 7d7d 286a 5175 6572 792c 7769 6e64  })}}(jQuery,wind
-00000900: 6f77 293b                                ow);
+00000900: 6f77 293b 0a                             ow);.
```

### Comparing `evv4esm-0.5.0/evv4esm/resources/js/jquery.min.js` & `evv4esm-0.5.1/evv4esm/resources/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `evv4esm-0.5.0/evv4esm/resources/js/lightbox.min.js` & `evv4esm-0.5.1/evv4esm/resources/js/lightbox.min.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with very long lines (9089)*

 * *Files 0% similar despite different names*

```diff
@@ -579,8 +579,8 @@
 00002420: 7468 6973 2e6f 7074 696f 6e73 2e64 6973  this.options.dis
 00002430: 6162 6c65 5363 726f 6c6c 696e 6726 2661  ableScrolling&&a
 00002440: 2822 626f 6479 2229 2e72 656d 6f76 6543  ("body").removeC
 00002450: 6c61 7373 2822 6c62 2d64 6973 6162 6c65  lass("lb-disable
 00002460: 2d73 6372 6f6c 6c69 6e67 2229 7d2c 6e65  -scrolling")},ne
 00002470: 7720 627d 293b 0a2f 2f23 2073 6f75 7263  w b});.//# sourc
 00002480: 654d 6170 7069 6e67 5552 4c3d 6c69 6768  eMappingURL=ligh
-00002490: 7462 6f78 2e6d 696e 2e6d 6170            tbox.min.map
+00002490: 7462 6f78 2e6d 696e 2e6d 6170 0a         tbox.min.map.
```

### Comparing `evv4esm-0.5.0/evv4esm/resources/js/lightbox.min.map` & `evv4esm-0.5.1/evv4esm/resources/js/lightbox.min.map`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -604,8 +604,8 @@
 000025b0: 4151 552c 6341 436e 435a 2c45 4141 452c  AQU,cACnCZ,EAAE,
 000025c0: 7942 4141 7942 3843 2c4b 4143 7a42 7742  yBAAyB8C,KACzBwB
 000025d0: 2c57 4141 592c 5941 4556 7645 2c4b 4141  ,WAAY,YAEVvE,KAA
 000025e0: 4b47 2c51 4141 5169 422c 6b42 4143 666e  KG,QAAQiB,kBACfn
 000025f0: 422c 4541 4145 2c51 4141 5134 482c 5941  B,EAAE,QAAQ4H,YA
 00002600: 4159 2c79 4241 496e 422c 4741 4149 3348  AY,yBAInB,GAAI3H
 00002610: 222c 2266 696c 6522 3a22 6c69 6768 7462  ","file":"lightb
-00002620: 6f78 2e6d 696e 2e6a 7322 7d              ox.min.js"}
+00002620: 6f78 2e6d 696e 2e6a 7322 7d0a            ox.min.js"}.
```

### Comparing `evv4esm-0.5.0/evv4esm/resources/validation.html` & `evv4esm-0.5.1/evv4esm/resources/validation.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -61,8 +61,8 @@
             <h3 style="text-align: center;">
                 <a href="https://github.com/LIVVkit/evv4esm/issues" target=_blank>Contact us on github</a>
             </h3>
         </div>
 
     <script src="../js/lightbox.min.js"></script>
     </body>
-</html>
+</html>
```

### Comparing `evv4esm-0.5.0/evv4esm/utils.py` & `evv4esm-0.5.1/evv4esm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 # coding=utf-8
 
-import six
-
 import pybtex.database
 import pybtex.io
-
+import six
 from pybtex.backends.html import Backend as BaseBackend
 from pybtex.style.formatting.plain import Style as PlainStyle
 
 
 class HTMLBackend(BaseBackend):
     def __init__(self, *args, **kwargs):
         super(HTMLBackend, self).__init__(*args, **kwargs)
-        self._html = ''
+        self._html = ""
 
     def output(self, html):
         self._html += html
 
     def format_protected(self, text):
-        if text[:4] == 'http':
+        if text[:4] == "http":
             return self.format_href(text, text)
         else:
             return r'<span class="bibtex-protected">{}</span>'.format(text)
 
     def write_prologue(self):
         self.output('<div class="bibliography"><dl>')
 
     def write_epilogue(self):
-        self.output('</dl></div>')
+        self.output("</dl></div>")
 
     def _repr_html(self, formatted_bibliography):
         self.write_prologue()
         for entry in formatted_bibliography:
             self.write_entry(entry.key, entry.label, entry.text.render(self))
         self.write_epilogue()
 
-        return self._html.replace('\n', ' ').replace('\\url <a', '<a')
+        return self._html.replace("\n", " ").replace("\\url <a", "<a")
 
 
 # FIXME: For python 3.7+ only...
 # from functools import singledispatch
 # from collections.abc import Iterable
 #
 # # noinspection PyUnusedLocal
@@ -50,15 +48,17 @@
     if isinstance(bib, six.string_types):
         return _bib2html_string(bib, style=style, backend=backend)
     if isinstance(bib, (list, set, tuple)):
         return _bib2html_list(bib, style=style, backend=backend)
     if isinstance(bib, pybtex.database.BibliographyData):
         return _bib2html_bibdata(bib, style=style, backend=backend)
     else:
-        raise NotImplementedError('I do not now how to convert a {} type to a bibliography'.format(type(bib)))
+        raise NotImplementedError(
+            "I do not now how to convert a {} type to a bibliography".format(type(bib))
+        )
 
 
 # FIXME: For python 3.7+ only...
 # @bib2html.register
 # def _bib2html_string(bib: str, style=None, backend=None):
 def _bib2html_string(bib, style=None, backend=None):
     if style is None:
```

### Comparing `evv4esm-0.5.0/evv4esm.egg-info/PKG-INFO` & `evv4esm-0.5.1/evv4esm.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 Metadata-Version: 2.1
 Name: evv4esm
-Version: 0.5.0
+Version: 0.5.1
 Summary: Extended verification and validation for earth system models
-Home-page: https://github.com/LIVVkit/evv4esm
-Author: Joseph H. Kennedy
-Author-email: kennedyjh@ornl.gov
-Maintainer: Michael Kelleher
-Maintainer-email: kelleherme@ornl.gov
-License: BSD
+Author-email: Michael Kelleher <kelleherme@ornl.gov>, "Joseph H. Kennedy" <kennedyjh@ornl.gov>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/LIVVkit/evv4esm
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools
 Requires-Dist: six
 Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: pandas
+Requires-Dist: pandas>=2.1.0
 Requires-Dist: livvkit>=3.0.1
 Requires-Dist: netCDF4
 Requires-Dist: matplotlib
-Requires-Dist: pybtex
-Requires-Dist: statsmodels==0.14.0
+Requires-Dist: pybtex>=0.24.0
+Requires-Dist: statsmodels>=0.14.0
+Provides-Extra: dev
+Requires-Dist: modelmimic; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
   Extended Verification and Validation for Earth System Models
 ===============================================================================
 
 EVV is a python-based toolkit for extended verification and validation of Earth
 system models (ESMs). Currently, it provides a number tests to determine if
 modifications to an ESM is *climate changing.*
@@ -48,10 +58,10 @@
 Want to send us a private message?
 
 
 **Michael Kelleher**
 * github: @mkstratos
 * email: <a href="mailto:kelleherme@ornl.gov">kelleherme [at] ornl.gov</a>
 
-**Joseph H. Kennedy** 
+**Joseph H. Kennedy**
 * github: @jhkennedy
 * email: <a href="mailto:kennedyjh@ornl.gov">kennedyjh [at] ornl.gov</a>
```

#### html2text {}

```diff
@@ -1,23 +1,31 @@
-Metadata-Version: 2.1 Name: evv4esm Version: 0.5.0 Summary: Extended
-verification and validation for earth system models Home-page: https://
-github.com/LIVVkit/evv4esm Author: Joseph H. Kennedy Author-email:
-kennedyjh@ornl.gov Maintainer: Michael Kelleher Maintainer-email:
-kelleherme@ornl.gov License: BSD Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
-Topic :: Scientific/Engineering Classifier: Topic :: Software Development ::
-Testing Classifier: License :: OSI Approved :: BSD License Classifier:
+Metadata-Version: 2.1 Name: evv4esm Version: 0.5.1 Summary: Extended
+verification and validation for earth system models Author-email: Michael
+Kelleher
+ornl.gov>, "Joseph H. Kennedy"
+ornl.gov> License: BSD-3-Clause Project-URL: Homepage, https://github.com/
+LIVVkit/evv4esm Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Software Development :: Testing
+Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
+:: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: six Requires-Dist: numpy Requires-Dist: scipy Requires-Dist:
-pandas Requires-Dist: livvkit>=3.0.1 Requires-Dist: netCDF4 Requires-Dist:
-matplotlib Requires-Dist: pybtex Requires-Dist: statsmodels==0.14.0 Extended
-Verification and Validation for Earth System Models
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Requires-Python: >=3.6 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: setuptools Requires-Dist: six Requires-
+Dist: numpy Requires-Dist: scipy Requires-Dist: pandas>=2.1.0 Requires-Dist:
+livvkit>=3.0.1 Requires-Dist: netCDF4 Requires-Dist: matplotlib Requires-Dist:
+pybtex>=0.24.0 Requires-Dist: statsmodels>=0.14.0 Provides-Extra: dev Requires-
+Dist: modelmimic; extra == "dev" Requires-Dist: ruff; extra == "dev" Requires-
+Dist: black; extra == "dev" Requires-Dist: isort; extra == "dev" Requires-Dist:
+pytest; extra == "dev" Extended Verification and Validation for Earth System
+Models
 ===============================================================================
 EVV is a python-based toolkit for extended verification and validation of Earth
 system models (ESMs). Currently, it provides a number tests to determine if
 modifications to an ESM is *climate changing.* Contact =========== If you would
 like to suggest features, request tests, discuss contributions, report bugs,
 ask questions, or contact us for any reason, use the [Issue Tracker](https://
 github.com/LIVVkit/evv4esm/issues). Want to send us a private message?
```

### Comparing `evv4esm-0.5.0/evv4esm.egg-info/SOURCES.txt` & `evv4esm-0.5.1/evv4esm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+.git-blame-ignore-revs
+.gitignore
+.pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+.github/workflows/pre-commit.yml
+.github/workflows/python-package.yml
+.github/workflows/python-publish.yml
 evv4esm/__init__.py
 evv4esm/__main__.py
 evv4esm/utils.py
 evv4esm.egg-info/PKG-INFO
 evv4esm.egg-info/SOURCES.txt
 evv4esm.egg-info/dependency_links.txt
 evv4esm.egg-info/entry_points.txt
-evv4esm.egg-info/not-zip-safe
 evv4esm.egg-info/requires.txt
 evv4esm.egg-info/top_level.txt
 evv4esm/ensembles/__init__.py
 evv4esm/ensembles/e3sm.py
 evv4esm/ensembles/tools.py
 evv4esm/extensions/__init__.py
 evv4esm/extensions/ks.bib
@@ -46,8 +51,11 @@
 evv4esm/resources/imgs/next.png
 evv4esm/resources/imgs/prev.png
 evv4esm/resources/js/common.js
 evv4esm/resources/js/jquery-ui.min.js
 evv4esm/resources/js/jquery.caption.min.js
 evv4esm/resources/js/jquery.min.js
 evv4esm/resources/js/lightbox.min.js
-evv4esm/resources/js/lightbox.min.map
+evv4esm/resources/js/lightbox.min.map
+test/MVK_template.json
+test/TSC_template.json
+test/test_evv.py
```

