# Comparing `tmp/google_sheets_sdk-0.1.5.tar.gz` & `tmp/google_sheets_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_sheets_sdk-0.1.5.tar", max compression
+gzip compressed data, was "google_sheets_sdk-0.1.6.tar", max compression
```

## Comparing `google_sheets_sdk-0.1.5.tar` & `google_sheets_sdk-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2024-05-08 20:40:25.393452 google_sheets_sdk-0.1.5/README.md
--rw-r--r--   0        0        0       31 2024-05-09 22:05:15.890493 google_sheets_sdk-0.1.5/google_sheets_sdk/__init__.py
--rw-r--r--   0        0        0       81 2024-05-09 21:26:16.192570 google_sheets_sdk-0.1.5/google_sheets_sdk/entities/__init__.py
--rw-r--r--   0        0        0      317 2024-05-09 19:37:37.022530 google_sheets_sdk-0.1.5/google_sheets_sdk/entities/settings.py
--rw-r--r--   0        0        0      153 2024-05-09 21:45:00.913001 google_sheets_sdk-0.1.5/google_sheets_sdk/entities/sheet.py
--rw-r--r--   0        0        0       14 2024-05-09 21:45:18.630595 google_sheets_sdk-0.1.5/google_sheets_sdk/entities/spreadsheet.py
--rw-r--r--   0        0        0     1393 2024-05-09 21:16:10.790753 google_sheets_sdk-0.1.5/google_sheets_sdk/entities/token.py
--rw-r--r--   0        0        0      347 2024-05-09 21:56:10.068794 google_sheets_sdk-0.1.5/google_sheets_sdk/example.py
--rw-r--r--   0        0        0       27 2024-05-09 20:14:03.310461 google_sheets_sdk-0.1.5/google_sheets_sdk/frameworks/__init__.py
--rw-r--r--   0        0        0     2990 2024-05-09 22:35:23.386386 google_sheets_sdk-0.1.5/google_sheets_sdk/frameworks/client/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 19:32:08.899991 google_sheets_sdk-0.1.5/google_sheets_sdk/interfaces/controllers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 19:32:06.270051 google_sheets_sdk-0.1.5/google_sheets_sdk/interfaces/repositories/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 19:32:11.271937 google_sheets_sdk-0.1.5/google_sheets_sdk/interfaces/services/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 21:30:12.963346 google_sheets_sdk-0.1.5/google_sheets_sdk/use_cases/__init__.py
--rw-r--r--   0        0        0      407 2024-05-09 22:35:34.393131 google_sheets_sdk-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 google_sheets_sdk-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/README.md
+-rw-r--r--   0        0        0       31 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/__init__.py
+-rw-r--r--   0        0        0       81 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/entities/__init__.py
+-rw-r--r--   0        0        0      317 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/entities/settings.py
+-rw-r--r--   0        0        0      153 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/entities/sheet.py
+-rw-r--r--   0        0        0     1115 2024-05-14 21:09:42.861349 google_sheets_sdk-0.1.6/google_sheets_sdk/entities/spreadsheet.py
+-rw-r--r--   0        0        0     1393 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/entities/token.py
+-rw-r--r--   0        0        0      347 2024-05-14 21:08:12.115313 google_sheets_sdk-0.1.6/google_sheets_sdk/example.py
+-rw-r--r--   0        0        0       27 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/frameworks/__init__.py
+-rw-r--r--   0        0        0     2407 2024-05-14 21:10:17.764592 google_sheets_sdk-0.1.6/google_sheets_sdk/frameworks/client/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/interfaces/controllers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/interfaces/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/interfaces/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/use_cases/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-14 21:11:39.794810 google_sheets_sdk-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 google_sheets_sdk-0.1.6/PKG-INFO
```

### Comparing `google_sheets_sdk-0.1.5/google_sheets_sdk/entities/token.py` & `google_sheets_sdk-0.1.6/google_sheets_sdk/entities/token.py`

 * *Files identical despite different names*

### Comparing `google_sheets_sdk-0.1.5/PKG-INFO` & `google_sheets_sdk-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-sheets-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Marco Carmona
 Author-email: marcocarmonapy@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

