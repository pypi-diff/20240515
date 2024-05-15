# Comparing `tmp/airtable_pg_sync-0.0.8.tar.gz` & `tmp/airtable_pg_sync-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtable_pg_sync-0.0.8.tar", last modified: Wed Aug  9 16:12:17 2023, max compression
+gzip compressed data, was "airtable_pg_sync-0.0.9.tar", last modified: Wed Aug  9 16:20:03 2023, max compression
```

## Comparing `airtable_pg_sync-0.0.8.tar` & `airtable_pg_sync-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:12:17.749457 airtable_pg_sync-0.0.8/
--rw-r--r--   0 benurwin   (501) staff       (20)     1071 2023-07-31 09:55:19.000000 airtable_pg_sync-0.0.8/LICENSE
--rw-r--r--   0 benurwin   (501) staff       (20)       37 2023-08-01 00:26:02.000000 airtable_pg_sync-0.0.8/MANIFEST.in
--rw-r--r--   0 benurwin   (501) staff       (20)     5638 2023-08-09 16:12:17.749237 airtable_pg_sync-0.0.8/PKG-INFO
--rw-r--r--   0 benurwin   (501) staff       (20)     3962 2023-08-01 09:33:58.000000 airtable_pg_sync-0.0.8/README.md
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:12:17.743442 airtable_pg_sync-0.0.8/airtable_pg_sync/
--rw-r--r--   0 benurwin   (501) staff       (20)       45 2023-08-01 00:18:57.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2770 2023-08-09 15:03:52.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/cli.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:12:17.744815 airtable_pg_sync-0.0.8/airtable_pg_sync/core/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:05:55.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/core/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     5027 2023-08-09 15:13:35.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/core/change_handler.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:12:17.745833 airtable_pg_sync-0.0.8/airtable_pg_sync/core/clients/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:08:13.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/core/clients/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     4310 2023-08-09 15:40:32.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/core/clients/airtable.py
--rw-r--r--   0 benurwin   (501) staff       (20)     8487 2023-08-09 15:36:39.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/core/clients/postgres.py
--rw-r--r--   0 benurwin   (501) staff       (20)     7562 2023-08-09 16:11:08.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/core/clients/response_parser.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1175 2023-08-09 15:36:39.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/core/env.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:12:17.746850 airtable_pg_sync-0.0.8/airtable_pg_sync/core/types/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:06:33.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/core/types/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)      597 2023-08-09 14:36:22.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/core/types/bridges.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1993 2023-08-09 15:42:59.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/core/types/changes.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2977 2023-07-30 23:13:28.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/core/types/concepts.py
--rw-r--r--   0 benurwin   (501) staff       (20)      893 2023-08-09 15:42:59.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/core/types/env_types.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:12:17.748046 airtable_pg_sync-0.0.8/airtable_pg_sync/initial_sync/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:07:03.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/initial_sync/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)      793 2023-08-09 15:37:32.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/initial_sync/initial_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     3669 2023-08-09 14:12:50.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/initial_sync/row_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2624 2023-08-09 14:12:18.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/initial_sync/schema_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2752 2023-08-09 14:12:18.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/initial_sync/table_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1580 2023-08-09 15:35:08.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/initial_sync/view_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)      328 2023-07-30 12:27:45.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/logging.conf
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:12:17.748613 airtable_pg_sync-0.0.8/airtable_pg_sync/perpetual_sync/
--rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:10:23.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/perpetual_sync/__init__.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1385 2023-08-09 15:43:40.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/perpetual_sync/perpetual_syncer.py
--rw-r--r--   0 benurwin   (501) staff       (20)     2754 2023-08-09 14:45:43.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/perpetual_sync/webhook_listener.py
--rw-r--r--   0 benurwin   (501) staff       (20)     1365 2023-08-09 14:14:23.000000 airtable_pg_sync-0.0.8/airtable_pg_sync/sync.py
-drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:12:17.744285 airtable_pg_sync-0.0.8/airtable_pg_sync.egg-info/
--rw-r--r--   0 benurwin   (501) staff       (20)     5638 2023-08-09 16:12:17.000000 airtable_pg_sync-0.0.8/airtable_pg_sync.egg-info/PKG-INFO
--rw-r--r--   0 benurwin   (501) staff       (20)     1291 2023-08-09 16:12:17.000000 airtable_pg_sync-0.0.8/airtable_pg_sync.egg-info/SOURCES.txt
--rw-r--r--   0 benurwin   (501) staff       (20)        1 2023-08-09 16:12:17.000000 airtable_pg_sync-0.0.8/airtable_pg_sync.egg-info/dependency_links.txt
--rw-r--r--   0 benurwin   (501) staff       (20)       59 2023-08-09 16:12:17.000000 airtable_pg_sync-0.0.8/airtable_pg_sync.egg-info/entry_points.txt
--rw-r--r--   0 benurwin   (501) staff       (20)       69 2023-08-09 16:12:17.000000 airtable_pg_sync-0.0.8/airtable_pg_sync.egg-info/requires.txt
--rw-r--r--   0 benurwin   (501) staff       (20)       17 2023-08-09 16:12:17.000000 airtable_pg_sync-0.0.8/airtable_pg_sync.egg-info/top_level.txt
--rw-r--r--   0 benurwin   (501) staff       (20)      847 2023-08-09 16:12:00.000000 airtable_pg_sync-0.0.8/pyproject.toml
--rw-r--r--   0 benurwin   (501) staff       (20)       38 2023-08-09 16:12:17.749503 airtable_pg_sync-0.0.8/setup.cfg
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:20:03.267172 airtable_pg_sync-0.0.9/
+-rw-r--r--   0 benurwin   (501) staff       (20)     1071 2023-07-31 09:55:19.000000 airtable_pg_sync-0.0.9/LICENSE
+-rw-r--r--   0 benurwin   (501) staff       (20)       37 2023-08-01 00:26:02.000000 airtable_pg_sync-0.0.9/MANIFEST.in
+-rw-r--r--   0 benurwin   (501) staff       (20)     5637 2023-08-09 16:20:03.267012 airtable_pg_sync-0.0.9/PKG-INFO
+-rw-r--r--   0 benurwin   (501) staff       (20)     3962 2023-08-01 09:33:58.000000 airtable_pg_sync-0.0.9/README.md
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:20:03.261415 airtable_pg_sync-0.0.9/airtable_pg_sync/
+-rw-r--r--   0 benurwin   (501) staff       (20)       45 2023-08-01 00:18:57.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2770 2023-08-09 15:03:52.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/cli.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:20:03.262683 airtable_pg_sync-0.0.9/airtable_pg_sync/core/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:05:55.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/core/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     5027 2023-08-09 15:13:35.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/core/change_handler.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:20:03.263486 airtable_pg_sync-0.0.9/airtable_pg_sync/core/clients/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:08:13.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/core/clients/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     4222 2023-08-09 16:19:37.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/core/clients/airtable.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     8487 2023-08-09 15:36:39.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/core/clients/postgres.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     7536 2023-08-09 16:19:37.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/core/clients/response_parser.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1175 2023-08-09 15:36:39.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/core/env.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:20:03.264528 airtable_pg_sync-0.0.9/airtable_pg_sync/core/types/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:06:33.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/core/types/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      597 2023-08-09 14:36:22.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/core/types/bridges.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1993 2023-08-09 15:42:59.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/core/types/changes.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2977 2023-07-30 23:13:28.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/core/types/concepts.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      893 2023-08-09 15:42:59.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/core/types/env_types.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:20:03.265969 airtable_pg_sync-0.0.9/airtable_pg_sync/initial_sync/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:07:03.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/initial_sync/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      793 2023-08-09 15:37:32.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/initial_sync/initial_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     3669 2023-08-09 14:12:50.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/initial_sync/row_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2624 2023-08-09 14:12:18.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/initial_sync/schema_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2752 2023-08-09 14:12:18.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/initial_sync/table_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1580 2023-08-09 15:35:08.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/initial_sync/view_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)      328 2023-07-30 12:27:45.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/logging.conf
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:20:03.266638 airtable_pg_sync-0.0.9/airtable_pg_sync/perpetual_sync/
+-rw-r--r--   0 benurwin   (501) staff       (20)        0 2023-08-01 00:10:23.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/perpetual_sync/__init__.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1385 2023-08-09 15:43:40.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/perpetual_sync/perpetual_syncer.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     2754 2023-08-09 14:45:43.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/perpetual_sync/webhook_listener.py
+-rw-r--r--   0 benurwin   (501) staff       (20)     1365 2023-08-09 14:14:23.000000 airtable_pg_sync-0.0.9/airtable_pg_sync/sync.py
+drwxr-xr-x   0 benurwin   (501) staff       (20)        0 2023-08-09 16:20:03.262245 airtable_pg_sync-0.0.9/airtable_pg_sync.egg-info/
+-rw-r--r--   0 benurwin   (501) staff       (20)     5637 2023-08-09 16:20:03.000000 airtable_pg_sync-0.0.9/airtable_pg_sync.egg-info/PKG-INFO
+-rw-r--r--   0 benurwin   (501) staff       (20)     1291 2023-08-09 16:20:03.000000 airtable_pg_sync-0.0.9/airtable_pg_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)        1 2023-08-09 16:20:03.000000 airtable_pg_sync-0.0.9/airtable_pg_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)       59 2023-08-09 16:20:03.000000 airtable_pg_sync-0.0.9/airtable_pg_sync.egg-info/entry_points.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)       69 2023-08-09 16:20:03.000000 airtable_pg_sync-0.0.9/airtable_pg_sync.egg-info/requires.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)       17 2023-08-09 16:20:03.000000 airtable_pg_sync-0.0.9/airtable_pg_sync.egg-info/top_level.txt
+-rw-r--r--   0 benurwin   (501) staff       (20)      846 2023-08-09 16:19:55.000000 airtable_pg_sync-0.0.9/pyproject.toml
+-rw-r--r--   0 benurwin   (501) staff       (20)       38 2023-08-09 16:20:03.267215 airtable_pg_sync-0.0.9/setup.cfg
```

### Comparing `airtable_pg_sync-0.0.8/LICENSE` & `airtable_pg_sync-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/PKG-INFO` & `airtable_pg_sync-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: airtable_pg_sync
-Version: 0.0.8
-Summary: Sync an Airtable base to a Postgres schema in real time
+Version: 0.0.9
+Summary: Sync Airtable bases to a Postgres schemas in real time
 Author-email: Benjamin Urwin <benurwin@outlook.com>
 License: Copyright 2023 Benjamin Urwin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `airtable_pg_sync-0.0.8/README.md` & `airtable_pg_sync-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/cli.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/cli.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/core/change_handler.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/core/change_handler.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/core/clients/airtable.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/core/clients/airtable.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,14 @@
     def delete_webhook(self, webhook_id: concepts.WebhookId):
         self.session().delete(
             url=f'{self.API_URL}/bases/{self.base}/webhooks/{webhook_id}',
             headers={'Authorization': f'Bearer {self.pat}'}
         )
 
     def setup_webhook(self, replication: env_types.Replication):
-        print('Setting up webhook', f'{env.value.webhook_url}{replication.endpoint}', )
         response = self.session().post(
             url=f'{self.API_URL}/bases/{self.base}/webhooks',
             headers={'Authorization': f'Bearer {self.pat}', 'Content-Type': 'application/json'},
             data=json.dumps({
                 'notificationUrl': f'{env.value.webhook_url}{replication.endpoint}',
                 'specification': {
                     'options': {
```

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/core/clients/postgres.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/core/clients/postgres.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/core/clients/response_parser.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/core/clients/response_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                                        name=field['name'],
                                        type=field['type']
                                    ) for field in table['fields']
                                ]
                                ) for table in response]
 
     def parse_field_value(self, field_value: str | list | dict) -> str | list:
-        print(field_value)
+
         if isinstance(field_value, list):
             return [self.parse_field_value(value) for value in field_value]
 
         if isinstance(field_value, dict):
             if 'linkedRecordIds' in field_value:
                 return next(iter(field_value['valuesByLinkedRecordId'].values()))
```

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/core/env.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/core/env.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/core/types/bridges.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/core/types/bridges.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/core/types/changes.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/core/types/changes.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/core/types/concepts.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/core/types/concepts.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/core/types/env_types.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/core/types/env_types.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/initial_sync/initial_syncer.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/initial_sync/initial_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/initial_sync/row_syncer.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/initial_sync/row_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/initial_sync/schema_syncer.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/initial_sync/schema_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/initial_sync/table_syncer.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/initial_sync/table_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/initial_sync/view_syncer.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/initial_sync/view_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/perpetual_sync/perpetual_syncer.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/perpetual_sync/perpetual_syncer.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/perpetual_sync/webhook_listener.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/perpetual_sync/webhook_listener.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync/sync.py` & `airtable_pg_sync-0.0.9/airtable_pg_sync/sync.py`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync.egg-info/PKG-INFO` & `airtable_pg_sync-0.0.9/airtable_pg_sync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: airtable-pg-sync
-Version: 0.0.8
-Summary: Sync an Airtable base to a Postgres schema in real time
+Version: 0.0.9
+Summary: Sync Airtable bases to a Postgres schemas in real time
 Author-email: Benjamin Urwin <benurwin@outlook.com>
 License: Copyright 2023 Benjamin Urwin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `airtable_pg_sync-0.0.8/airtable_pg_sync.egg-info/SOURCES.txt` & `airtable_pg_sync-0.0.9/airtable_pg_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airtable_pg_sync-0.0.8/pyproject.toml` & `airtable_pg_sync-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airtable_pg_sync"
-version = "0.0.8"
-description = "Sync an Airtable base to a Postgres schema in real time"
+version = "0.0.9"
+description = "Sync Airtable bases to a Postgres schemas in real time"
 readme = "README.md"
 authors = [{ name = "Benjamin Urwin", email = "benurwin@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

