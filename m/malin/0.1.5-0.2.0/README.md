# Comparing `tmp/malin-0.1.5.tar.gz` & `tmp/malin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malin-0.1.5.tar", max compression
+gzip compressed data, was "malin-0.2.0.tar", max compression
```

## Comparing `malin-0.1.5.tar` & `malin-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       67 2024-05-14 13:27:31.227071 malin-0.1.5/malin/__init__.py
--rw-r--r--   0        0        0       32 2024-05-14 13:35:40.951891 malin-0.1.5/malin/actions/__init__.py
--rw-r--r--   0        0        0     1229 2024-05-14 15:26:00.528701 malin-0.1.5/malin/actions/scan.py
--rw-r--r--   0        0        0       80 2024-05-14 13:35:54.355565 malin-0.1.5/malin/errors/__init__.py
--rw-r--r--   0        0        0       29 2024-05-13 14:35:22.657421 malin-0.1.5/malin/errors/engine_error.py
--rw-r--r--   0        0        0      298 2024-05-14 11:46:30.922977 malin-0.1.5/malin/errors/parser_error.py
--rw-r--r--   0        0        0      582 2024-05-14 15:44:09.880226 malin-0.1.5/malin/malin.py
--rw-r--r--   0        0        0       88 2024-05-14 13:34:26.915707 malin-0.1.5/malin/models/__init__.py
--rw-r--r--   0        0        0       83 2024-05-13 14:32:45.847772 malin-0.1.5/malin/models/scan_error.py
--rw-r--r--   0        0        0      141 2024-05-13 14:24:13.581645 malin-0.1.5/malin/models/scan_summary.py
--rw-r--r--   0        0        0      303 2024-05-14 15:44:14.491012 malin-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 07:54:08.000000 malin-0.1.5/README.md
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 malin-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       67 2024-05-14 13:27:31.227071 malin-0.2.0/malin/__init__.py
+-rw-r--r--   0        0        0       32 2024-05-14 13:35:40.951891 malin-0.2.0/malin/actions/__init__.py
+-rw-r--r--   0        0        0     1229 2024-05-14 15:26:00.528701 malin-0.2.0/malin/actions/scan.py
+-rw-r--r--   0        0        0       80 2024-05-14 13:35:54.355565 malin-0.2.0/malin/errors/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-13 14:35:22.657421 malin-0.2.0/malin/errors/engine_error.py
+-rw-r--r--   0        0        0      298 2024-05-14 11:46:30.922977 malin-0.2.0/malin/errors/parser_error.py
+-rw-r--r--   0        0        0      582 2024-05-14 15:44:09.880226 malin-0.2.0/malin/malin.py
+-rw-r--r--   0        0        0       88 2024-05-14 13:34:26.915707 malin-0.2.0/malin/models/__init__.py
+-rw-r--r--   0        0        0       83 2024-05-13 14:32:45.847772 malin-0.2.0/malin/models/scan_error.py
+-rw-r--r--   0        0        0      258 2024-05-14 15:58:07.126804 malin-0.2.0/malin/models/scan_summary.py
+-rw-r--r--   0        0        0      303 2024-05-14 15:59:11.709071 malin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-22 07:54:08.000000 malin-0.2.0/README.md
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 malin-0.2.0/PKG-INFO
```

### Comparing `malin-0.1.5/malin/actions/scan.py` & `malin-0.2.0/malin/actions/scan.py`

 * *Files identical despite different names*

### Comparing `malin-0.1.5/malin/malin.py` & `malin-0.2.0/malin/malin.py`

 * *Files identical despite different names*

