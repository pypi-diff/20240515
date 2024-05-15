# Comparing `tmp/afl-ai-utils-0.4.7.tar.gz` & `tmp/afl-ai-utils-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afl-ai-utils-0.4.7.tar", last modified: Mon Mar  4 10:25:51 2024, max compression
+gzip compressed data, was "afl-ai-utils-0.4.8.tar", last modified: Wed May 15 07:16:57 2024, max compression
```

## Comparing `afl-ai-utils-0.4.7.tar` & `afl-ai-utils-0.4.8.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 abhaykumar   (502) staff       (20)        0 2024-03-04 10:25:51.288904 afl-ai-utils-0.4.7/
--rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2023-10-19 13:42:39.000000 afl-ai-utils-0.4.7/LICENSE
--rw-r--r--   0 abhaykumar   (502) staff       (20)     2729 2024-03-04 10:25:51.288646 afl-ai-utils-0.4.7/PKG-INFO
--rw-r--r--   0 abhaykumar   (502) staff       (20)     2407 2023-11-10 08:42:51.000000 afl-ai-utils-0.4.7/README.md
-drwxr-xr-x   0 abhaykumar   (502) staff       (20)        0 2024-03-04 10:25:51.286780 afl-ai-utils-0.4.7/afl_ai_utils/
--rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2023-10-20 08:02:33.000000 afl-ai-utils-0.4.7/afl_ai_utils/__init__.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)     7013 2024-03-04 10:23:21.000000 afl-ai-utils-0.4.7/afl_ai_utils/bigquery_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)       36 2023-10-19 13:42:39.000000 afl-ai-utils-0.4.7/afl_ai_utils/consts.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)     4991 2023-12-22 11:43:29.000000 afl-ai-utils-0.4.7/afl_ai_utils/drive_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)     4996 2023-11-29 16:38:37.000000 afl-ai-utils-0.4.7/afl_ai_utils/email_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)    11045 2023-12-22 11:43:29.000000 afl-ai-utils-0.4.7/afl_ai_utils/outlook_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)     3357 2024-03-04 10:23:21.000000 afl-ai-utils-0.4.7/afl_ai_utils/selenium_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)     2063 2023-11-10 08:39:25.000000 afl-ai-utils-0.4.7/afl_ai_utils/slack_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)    16225 2023-12-22 11:43:29.000000 afl-ai-utils-0.4.7/afl_ai_utils/text_utils.py
-drwxr-xr-x   0 abhaykumar   (502) staff       (20)        0 2024-03-04 10:25:51.288306 afl-ai-utils-0.4.7/afl_ai_utils.egg-info/
--rw-r--r--   0 abhaykumar   (502) staff       (20)     2729 2024-03-04 10:25:51.000000 afl-ai-utils-0.4.7/afl_ai_utils.egg-info/PKG-INFO
--rw-r--r--   0 abhaykumar   (502) staff       (20)      456 2024-03-04 10:25:51.000000 afl-ai-utils-0.4.7/afl_ai_utils.egg-info/SOURCES.txt
--rw-r--r--   0 abhaykumar   (502) staff       (20)        1 2024-03-04 10:25:51.000000 afl-ai-utils-0.4.7/afl_ai_utils.egg-info/dependency_links.txt
--rw-r--r--   0 abhaykumar   (502) staff       (20)       88 2024-03-04 10:25:51.000000 afl-ai-utils-0.4.7/afl_ai_utils.egg-info/requires.txt
--rw-r--r--   0 abhaykumar   (502) staff       (20)       13 2024-03-04 10:25:51.000000 afl-ai-utils-0.4.7/afl_ai_utils.egg-info/top_level.txt
--rw-r--r--   0 abhaykumar   (502) staff       (20)       38 2024-03-04 10:25:51.288952 afl-ai-utils-0.4.7/setup.cfg
--rw-r--r--   0 abhaykumar   (502) staff       (20)      612 2024-03-04 10:23:21.000000 afl-ai-utils-0.4.7/setup.py
+drwxr-xr-x   0 abhaykumar   (502) staff       (20)        0 2024-05-15 07:16:57.373898 afl-ai-utils-0.4.8/
+-rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2023-10-19 13:42:39.000000 afl-ai-utils-0.4.8/LICENSE
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     2729 2024-05-15 07:16:57.373628 afl-ai-utils-0.4.8/PKG-INFO
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     2407 2023-11-10 08:42:51.000000 afl-ai-utils-0.4.8/README.md
+drwxr-xr-x   0 abhaykumar   (502) staff       (20)        0 2024-05-15 07:16:57.371581 afl-ai-utils-0.4.8/afl_ai_utils/
+-rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2023-10-20 08:02:33.000000 afl-ai-utils-0.4.8/afl_ai_utils/__init__.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     7308 2024-05-15 07:16:24.000000 afl-ai-utils-0.4.8/afl_ai_utils/bigquery_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)       36 2023-10-19 13:42:39.000000 afl-ai-utils-0.4.8/afl_ai_utils/consts.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     4991 2023-12-22 11:43:29.000000 afl-ai-utils-0.4.8/afl_ai_utils/drive_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     4996 2023-11-29 16:38:37.000000 afl-ai-utils-0.4.8/afl_ai_utils/email_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     1132 2024-03-28 12:10:06.000000 afl-ai-utils-0.4.8/afl_ai_utils/microsoft_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2024-04-01 09:52:23.000000 afl-ai-utils-0.4.8/afl_ai_utils/ms_api.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2024-03-28 14:25:52.000000 afl-ai-utils-0.4.8/afl_ai_utils/office365_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)    11871 2024-04-01 08:50:54.000000 afl-ai-utils-0.4.8/afl_ai_utils/outlook_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     3357 2024-03-04 10:23:21.000000 afl-ai-utils-0.4.8/afl_ai_utils/selenium_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     1375 2024-04-08 08:08:34.000000 afl-ai-utils-0.4.8/afl_ai_utils/sftp_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     2063 2023-11-10 08:39:25.000000 afl-ai-utils-0.4.8/afl_ai_utils/slack_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)    16225 2023-12-22 11:43:29.000000 afl-ai-utils-0.4.8/afl_ai_utils/text_utils.py
+drwxr-xr-x   0 abhaykumar   (502) staff       (20)        0 2024-05-15 07:16:57.373197 afl-ai-utils-0.4.8/afl_ai_utils.egg-info/
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     2729 2024-05-15 07:16:57.000000 afl-ai-utils-0.4.8/afl_ai_utils.egg-info/PKG-INFO
+-rw-r--r--   0 abhaykumar   (502) staff       (20)      570 2024-05-15 07:16:57.000000 afl-ai-utils-0.4.8/afl_ai_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 abhaykumar   (502) staff       (20)        1 2024-05-15 07:16:57.000000 afl-ai-utils-0.4.8/afl_ai_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 abhaykumar   (502) staff       (20)       88 2024-05-15 07:16:57.000000 afl-ai-utils-0.4.8/afl_ai_utils.egg-info/requires.txt
+-rw-r--r--   0 abhaykumar   (502) staff       (20)       13 2024-05-15 07:16:57.000000 afl-ai-utils-0.4.8/afl_ai_utils.egg-info/top_level.txt
+-rw-r--r--   0 abhaykumar   (502) staff       (20)       38 2024-05-15 07:16:57.373954 afl-ai-utils-0.4.8/setup.cfg
+-rw-r--r--   0 abhaykumar   (502) staff       (20)      612 2024-05-15 07:16:45.000000 afl-ai-utils-0.4.8/setup.py
```

### Comparing `afl-ai-utils-0.4.7/PKG-INFO` & `afl-ai-utils-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afl-ai-utils
-Version: 0.4.7
+Version: 0.4.8
 Summary: A sample test package
 Home-page: https://github.com/gituser/test-tackage
 Author: Abhay Kumar
 Author-email: abhay.kumar@arvindbrands.co.in
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `afl-ai-utils-0.4.7/README.md` & `afl-ai-utils-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.7/afl_ai_utils/bigquery_utils.py` & `afl-ai-utils-0.4.8/afl_ai_utils/bigquery_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import time
 import traceback
 
 from google.cloud import bigquery
 from google.oauth2.service_account import Credentials
-
+from google.api_core.exceptions import NotFound
 import logging
 import pandas as pd
 
 logging.basicConfig(format='%(name)s - %(levelname)s -%(asctime)s- %(message)s', level=logging.INFO)
 
 
 class BigQuery():
@@ -62,34 +62,41 @@
                 schema.append(
                     bigquery.SchemaField(col, bigquery.enums.SqlTypeNames.TIMESTAMP)
                 )
 
         table = bigquery.Table(table_id, schema=schema)
         table.clustering_fields = clustering_fields
 
-        if len(partitioning_field_type.keys()) == 1:
+        if partitioning_field_type and len(partitioning_field_type.keys()) == 1:
             for field, field_type in partitioning_field_type.items():
                 if partitioning_field_type[field] == "day":
                     table.time_partitioning = bigquery.TimePartitioning(
                         type_=bigquery.TimePartitioningType.DAY,
                         field=field
                     )
                 elif partitioning_field_type[field] == "integer":
                     table.range_partitioning = bigquery.RangePartitioning(
                         # To use integer range partitioning, select a top-level REQUIRED /
                         # NULLABLE column with INTEGER / INT64 data type.
                         field=field,
                         range_=bigquery.PartitionRange(start=0, end=1000000000, interval=100000),
                     )
-        table = self.client.create_table(table)  # Make an API request.
-        print(
-            "Created clustered table {}.{}.{}".format(
-                table.project, table.dataset_id, table.table_id
+
+        try:
+            # Try to get the table
+            self.client.get_table(table_id)
+            print(f"Table {table_id} already exists.")
+        except NotFound:
+            # If table is not found, create it
+            table = self.client.create_table(table)
+            print(
+                "Created clustered table {}.{}.{}".format(
+                    table.project, table.dataset_id, table.table_id
+                )
             )
-        )
 
     def execute_query(self, query: str):
         query_job = self.client.query(query)
         results_df = query_job.result().to_dataframe()  # Waits for job to complete.
         return results_df
 
     def dump_dataframe_to_bq_table(self, dataframe: pd.DataFrame, schema_cols_type: dict, table_id: str, mode: str):
```

### Comparing `afl-ai-utils-0.4.7/afl_ai_utils/drive_utils.py` & `afl-ai-utils-0.4.8/afl_ai_utils/drive_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.7/afl_ai_utils/email_utils.py` & `afl-ai-utils-0.4.8/afl_ai_utils/email_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.7/afl_ai_utils/outlook_utils.py` & `afl-ai-utils-0.4.8/afl_ai_utils/outlook_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,26 +8,49 @@
 from datetime import datetime, timezone, timedelta
 import pytz
 
 logging.basicConfig(format='[%(asctime)s]:[%(levelname)s]:[%(filename)s %(lineno)d]:[%(funcName)s]:%(message)s')
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
+def get_resource_access_token(client_id=None, client_secret=None, tenant_id=None, resource=None):
+    token_url = f"https://login.microsoftonline.com/{tenant_id}/oauth2/token"
 
-def get_access_token(client_id, client_secret, refresh_token):
+    # Token request parameters
+    token_data = {
+        "grant_type": "client_credentials",
+        "client_id": client_id,
+        "client_secret": client_secret,
+        "resource": resource
+    }
+
+    # Request access token
+    token_response = requests.post(token_url, data=token_data)
+
+    # Check if token request was successful
+    if token_response.status_code == 200:
+        # Extract access token from response
+        access_token = token_response.json()["access_token"]
+        print("Access Token:", access_token)
+        return access_token
+    else:
+        print("Error:", token_response.text)
+
+def get_access_token(client_id, client_secret, refresh_token,scopes="offline_access%20Mail.ReadWrite%20Mail.send"):
     url = "https://login.microsoftonline.com/d6454b9f-4ca2-4392-b62f-20e21e54335a/oauth2/v2.0/token"
 
-    payload = f'client_id={client_id}&scope=offline_access%20Mail.ReadWrite%20Mail.send&grant_type=refresh_token&client_secret={client_secret}&redirect_uri=https%3A%2F%2Flocalhost&refresh_token={refresh_token}'
+    payload = f'client_id={client_id}&scope={scopes}&grant_type=refresh_token&client_secret={client_secret}&redirect_uri=https%3A%2F%2Flocalhost&refresh_token={refresh_token}'
     headers = {
         'Content-Type': 'application/x-www-form-urlencoded',
         'Cookie': 'buid=0.AXIAn0tF1qJMkkO2LyDiHlQzWv8X8zrAVMtPqebAWud5G3tyAAA.AQABAAEAAAAmoFfGtYxvRrNriQdPKIZ-kZ5EkppMdTFRuYfniN_3y8-Xd4UdnOxoj73wJ1eZZCaKAT8JgDNpeqo0oFp59_urEfHRgAmxblfrvqZtteL87F0uVuBqo0iR-vyvN064OsAgAA; esctx=PAQABAAEAAAAmoFfGtYxvRrNriQdPKIZ-P8XcBu5-Z0yzoAJsYjHRoOrKnytCJJQZgtooKwI6-pwI0SH2MDCLXDXZbbdMx66FO30bZMF3OHeT5bL1TAdiQ4VV253aXWPOxep_3bDQ51hSp_8t3O5-_onUpGnU8RcuxnipsDXB1JojtTrJv8z5wQjGcGTbcAT1ttYODVqDMgIgAA; esctx-FbQVuPalhqg=AQABAAEAAAAmoFfGtYxvRrNriQdPKIZ-3CuntieqvcMk6UUaMPDkg0albmtVMGDKcYBLElzQlZY5BuS8kjO13PYFuvM631jlMLKFAtIxhAhe-6ffmXxJ7FIvp6zkgdlCdjY3zoSgYxAmMXLDc8II0tV8QHkyO8MN_C-kClYgVW8qHbel_H_FjCAA; fpc=Am86eFjVZTxGmw3t5Z7iqnHZjOJlAQAAAAuHAt0OAAAAlaghQQEAAABQhwLdDgAAAP8yaQoCAAAA5IgC3Q4AAAA; stsservicecookie=estsfd; x-ms-gateway-slice=estsfd'
     }
 
     response = requests.request("POST", url, headers=headers, data=payload)
     result = json.loads(response.text)
+    print(result)
     return result['access_token']
 
 
 def read_mail(access_token=None, from_email=None, top=1):
     subject = r"Arvind Fashions Limited: Storewise Inventory Report - ODIN"
     endpoint = f'https://graph.microsoft.com/v1.0/me/messages'
     params = {"$search": f'"from:{from_email}"', "top": top}
```

### Comparing `afl-ai-utils-0.4.7/afl_ai_utils/selenium_utils.py` & `afl-ai-utils-0.4.8/afl_ai_utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.7/afl_ai_utils/slack_utils.py` & `afl-ai-utils-0.4.8/afl_ai_utils/slack_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.7/afl_ai_utils/text_utils.py` & `afl-ai-utils-0.4.8/afl_ai_utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.7/afl_ai_utils.egg-info/PKG-INFO` & `afl-ai-utils-0.4.8/afl_ai_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afl-ai-utils
-Version: 0.4.7
+Version: 0.4.8
 Summary: A sample test package
 Home-page: https://github.com/gituser/test-tackage
 Author: Abhay Kumar
 Author-email: abhay.kumar@arvindbrands.co.in
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `afl-ai-utils-0.4.7/setup.py` & `afl-ai-utils-0.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setuptools.setup(
     name="afl-ai-utils",
-    version="0.4.7",
+    version="0.4.8",
     author="Abhay Kumar",
     author_email="abhay.kumar@arvindbrands.co.in",
     packages=["afl_ai_utils"],
     description="A sample test package",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/gituser/test-tackage",
```

