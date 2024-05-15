# Comparing `tmp/google_sheets_sdk-0.1.6.tar.gz` & `tmp/google_sheets_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_sheets_sdk-0.1.6.tar", max compression
+gzip compressed data, was "google_sheets_sdk-0.1.7.tar", max compression
```

## Comparing `google_sheets_sdk-0.1.6.tar` & `google_sheets_sdk-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,9 @@
--rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/README.md
--rw-r--r--   0        0        0       31 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/__init__.py
--rw-r--r--   0        0        0       81 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/entities/__init__.py
--rw-r--r--   0        0        0      317 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/entities/settings.py
--rw-r--r--   0        0        0      153 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/entities/sheet.py
--rw-r--r--   0        0        0     1115 2024-05-14 21:09:42.861349 google_sheets_sdk-0.1.6/google_sheets_sdk/entities/spreadsheet.py
--rw-r--r--   0        0        0     1393 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/entities/token.py
--rw-r--r--   0        0        0      347 2024-05-14 21:08:12.115313 google_sheets_sdk-0.1.6/google_sheets_sdk/example.py
--rw-r--r--   0        0        0       27 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/frameworks/__init__.py
--rw-r--r--   0        0        0     2407 2024-05-14 21:10:17.764592 google_sheets_sdk-0.1.6/google_sheets_sdk/frameworks/client/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/interfaces/controllers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/interfaces/repositories/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/interfaces/services/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.6/google_sheets_sdk/use_cases/__init__.py
--rw-r--r--   0        0        0      407 2024-05-14 21:11:39.794810 google_sheets_sdk-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 google_sheets_sdk-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.7/README.md
+-rw-r--r--   0        0        0       27 2024-05-15 17:21:02.673376 google_sheets_sdk-0.1.7/google_sheets_sdk/__init__.py
+-rw-r--r--   0        0        0     2325 2024-05-15 17:39:34.521315 google_sheets_sdk-0.1.7/google_sheets_sdk/client/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:30:15.109120 google_sheets_sdk-0.1.7/google_sheets_sdk/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:30:20.273045 google_sheets_sdk-0.1.7/google_sheets_sdk/common/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:22:49.403931 google_sheets_sdk-0.1.7/google_sheets_sdk/core/__init__.py
+-rw-r--r--   0        0        0     2977 2024-05-15 17:38:38.566077 google_sheets_sdk-0.1.7/google_sheets_sdk/core/models.py
+-rw-r--r--   0        0        0      407 2024-05-15 17:42:36.950851 google_sheets_sdk-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 google_sheets_sdk-0.1.7/PKG-INFO
```

### Comparing `google_sheets_sdk-0.1.6/google_sheets_sdk/frameworks/client/__init__.py` & `google_sheets_sdk-0.1.7/google_sheets_sdk/client/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 from dataclasses import InitVar, dataclass, field
 from typing import ClassVar
 
-
-from google_sheets_sdk.entities import spreadsheet as spreadsheet_entity
-from google_sheets_sdk.entities import Settings, Sheet, Token
-
 from httpx import AsyncClient, HTTPStatusError
 
+from google_sheets.core import models
+
 
 @dataclass
 class Client:
-    _base_url: ClassVar[str] = "https://sheets.googleapis.com/"
+    _BASE_URL: ClassVar[str] = "https://sheets.googleapis.com/"
 
-    _http_client: "AsyncClient"
-    _token: Token = field(
+    _http_client: AsyncClient
+    _token: models.Token = field(
         init=False,
     )
-    settings: InitVar[Settings]
+    settings: InitVar[models.Settings]
 
     def __post_init__(
         self,
-        settings: Settings,
+        settings: models.Settings,
     ):
-        self._token = Token(
+        self._token = models.Token(
             email=settings.CLIENT_EMAIL,
-            base_url=self._base_url,
+            base_url=self._BASE_URL,
             scope=settings.SCOPE.unicode_string(),
             private_key=settings.PRIVATE_KEY.replace(r"\n", "\n"),
             private_key_id=settings.PRIVATE_KEY_ID,
         )
 
     async def batch_clear_values(
         self,
-        spreadsheet_id: spreadsheet_entity.Id,
-        ranges: list[str],
+        spreadsheet_id: models.SpreadsheetId,
+        ranges: list[models.Range],
     ) -> None:
         try:
             response = await self._http_client.post(
-                url=f"{self._base_url}v4/spreadsheets/{spreadsheet_id}/values:batchClear",
+                url=f"{self._BASE_URL}v4/spreadsheets/{spreadsheet_id}/values:batchClear",
                 json={
                     "ranges": ranges,
                 },
                 headers={
                     "Authorization": f"Bearer {self._token.encoded}",
                 },
             )
             response.raise_for_status()
         except HTTPStatusError as exc:
             raise exc
 
     async def batch_update_values(
         self,
-        spreadsheet_id: spreadsheet_entity.Id,
-        sheets: list[Sheet],
-    ) -> spreadsheet_entity.BatchUpdateValuesResponse:
+        spreadsheet_id: models.SpreadsheetId,
+        sheets: list[models.Sheet],
+    ) -> models.BatchUpdateValuesResponse:
         try:
             response = await self._http_client.post(
-                url=f"{self._base_url}v4/spreadsheets/{spreadsheet_id}/values:batchUpdate",
+                url=f"{self._BASE_URL}v4/spreadsheets/{spreadsheet_id}/values:batchUpdate",
                 json={
                     "valueInputOption": "USER_ENTERED",
                     "data": [
                         sheet.model_dump(
                             mode="json",
                         )
                         for sheet in sheets
@@ -70,8 +68,8 @@
                     "Authorization": f"Bearer {self._token.encoded}",
                 },
             )
             response.raise_for_status()
         except HTTPStatusError as exc:
             raise exc
         else:
-            return spreadsheet_entity.BatchUpdateValuesResponse(**response.json())
+            return models.BatchUpdateValuesResponse(**response.json())
```

### Comparing `google_sheets_sdk-0.1.6/PKG-INFO` & `google_sheets_sdk-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-sheets-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Marco Carmona
 Author-email: marcocarmonapy@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

