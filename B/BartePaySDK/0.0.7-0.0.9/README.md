# Comparing `tmp/BartePaySDK-0.0.7.tar.gz` & `tmp/BartePaySDK-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BartePaySDK-0.0.7.tar", last modified: Tue May 14 17:57:14 2024, max compression
+gzip compressed data, was "BartePaySDK-0.0.9.tar", last modified: Tue May 14 19:25:27 2024, max compression
```

## Comparing `BartePaySDK-0.0.7.tar` & `BartePaySDK-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 17:57:14.309171 BartePaySDK-0.0.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 17:57:14.309171 BartePaySDK-0.0.7/BartePaySDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)      215 2024-05-14 17:57:14.000000 BartePaySDK-0.0.7/BartePaySDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2024-05-14 17:57:14.000000 BartePaySDK-0.0.7/BartePaySDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 17:57:14.000000 BartePaySDK-0.0.7/BartePaySDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-14 17:57:14.000000 BartePaySDK-0.0.7/BartePaySDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 17:57:14.000000 BartePaySDK-0.0.7/BartePaySDK.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      215 2024-05-14 17:57:14.309171 BartePaySDK-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 17:57:14.309171 BartePaySDK-0.0.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      384 2024-05-14 17:57:01.000000 BartePaySDK-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:25:27.180861 BartePaySDK-0.0.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:25:27.176861 BartePaySDK-0.0.9/BarteChargesAPI/
+-rw-rw-r--   0 root         (0) root         (0)       34 2024-05-14 19:22:52.000000 BartePaySDK-0.0.9/BarteChargesAPI/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      405 2024-05-14 19:22:52.000000 BartePaySDK-0.0.9/BarteChargesAPI/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:25:27.176861 BartePaySDK-0.0.9/BartePaySDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-14 19:25:27.000000 BartePaySDK-0.0.9/BartePaySDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-14 19:25:27.000000 BartePaySDK-0.0.9/BartePaySDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 19:25:27.000000 BartePaySDK-0.0.9/BartePaySDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-14 19:25:27.000000 BartePaySDK-0.0.9/BartePaySDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-14 19:25:27.000000 BartePaySDK-0.0.9/BartePaySDK.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:25:27.176861 BartePaySDK-0.0.9/BarteReportAPI/
+-rw-rw-r--   0 root         (0) root         (0)       33 2024-05-14 19:22:52.000000 BartePaySDK-0.0.9/BarteReportAPI/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      718 2024-05-14 19:22:52.000000 BartePaySDK-0.0.9/BarteReportAPI/main.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-14 19:22:52.000000 BartePaySDK-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-14 19:25:27.176861 BartePaySDK-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 19:25:27.180861 BartePaySDK-0.0.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      384 2024-05-14 19:25:14.000000 BartePaySDK-0.0.9/setup.py
```

