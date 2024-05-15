# Comparing `tmp/google_sheets_sdk-0.1.7.tar.gz` & `tmp/google_sheets_sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_sheets_sdk-0.1.7.tar", max compression
+gzip compressed data, was "google_sheets_sdk-0.1.8.tar", max compression
```

## Comparing `google_sheets_sdk-0.1.7.tar` & `google_sheets_sdk-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.7/README.md
--rw-r--r--   0        0        0       27 2024-05-15 17:21:02.673376 google_sheets_sdk-0.1.7/google_sheets_sdk/__init__.py
--rw-r--r--   0        0        0     2325 2024-05-15 17:39:34.521315 google_sheets_sdk-0.1.7/google_sheets_sdk/client/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 17:30:15.109120 google_sheets_sdk-0.1.7/google_sheets_sdk/common/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 17:30:20.273045 google_sheets_sdk-0.1.7/google_sheets_sdk/common/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-15 17:22:49.403931 google_sheets_sdk-0.1.7/google_sheets_sdk/core/__init__.py
--rw-r--r--   0        0        0     2977 2024-05-15 17:38:38.566077 google_sheets_sdk-0.1.7/google_sheets_sdk/core/models.py
--rw-r--r--   0        0        0      407 2024-05-15 17:42:36.950851 google_sheets_sdk-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 google_sheets_sdk-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.8/README.md
+-rw-r--r--   0        0        0       48 2024-05-15 17:45:20.372660 google_sheets_sdk-0.1.8/google_sheets_sdk/__init__.py
+-rw-r--r--   0        0        0     2329 2024-05-15 17:44:47.449101 google_sheets_sdk-0.1.8/google_sheets_sdk/client/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:30:15.109120 google_sheets_sdk-0.1.8/google_sheets_sdk/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:30:20.273045 google_sheets_sdk-0.1.8/google_sheets_sdk/common/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:22:49.403931 google_sheets_sdk-0.1.8/google_sheets_sdk/core/__init__.py
+-rw-r--r--   0        0        0     2977 2024-05-15 17:38:38.566077 google_sheets_sdk-0.1.8/google_sheets_sdk/core/models.py
+-rw-r--r--   0        0        0      407 2024-05-15 17:45:41.028385 google_sheets_sdk-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 google_sheets_sdk-0.1.8/PKG-INFO
```

### Comparing `google_sheets_sdk-0.1.7/google_sheets_sdk/client/__init__.py` & `google_sheets_sdk-0.1.8/google_sheets_sdk/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import InitVar, dataclass, field
 from typing import ClassVar
 
 from httpx import AsyncClient, HTTPStatusError
 
-from google_sheets.core import models
+from google_sheets_sdk.core import models
 
 
 @dataclass
 class Client:
     _BASE_URL: ClassVar[str] = "https://sheets.googleapis.com/"
 
     _http_client: AsyncClient
```

### Comparing `google_sheets_sdk-0.1.7/google_sheets_sdk/core/models.py` & `google_sheets_sdk-0.1.8/google_sheets_sdk/core/models.py`

 * *Files identical despite different names*

### Comparing `google_sheets_sdk-0.1.7/PKG-INFO` & `google_sheets_sdk-0.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-sheets-sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Marco Carmona
 Author-email: marcocarmonapy@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

