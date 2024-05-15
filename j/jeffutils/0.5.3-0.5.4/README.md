# Comparing `tmp/jeffutils-0.5.3.tar.gz` & `tmp/jeffutils-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.5.3.tar", last modified: Wed May  8 21:33:56 2024, max compression
+gzip compressed data, was "jeffutils-0.5.4.tar", last modified: Wed May 15 15:17:20 2024, max compression
```

## Comparing `jeffutils-0.5.3.tar` & `jeffutils-0.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-08 21:33:56.065231 jeffutils-0.5.3/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.3/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-08 21:33:56.065231 jeffutils-0.5.3/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.3/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.3/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-08 21:33:56.065231 jeffutils-0.5.3/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-08 21:33:52.000000 jeffutils-0.5.3/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-08 21:33:56.061231 jeffutils-0.5.3/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-08 21:33:56.065231 jeffutils-0.5.3/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.3/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    16498 2024-05-08 21:33:36.000000 jeffutils-0.5.3/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-08 21:33:56.065231 jeffutils-0.5.3/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-08 21:33:56.000000 jeffutils-0.5.3/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-08 21:33:56.000000 jeffutils-0.5.3/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-08 21:33:56.000000 jeffutils-0.5.3/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-08 21:33:56.000000 jeffutils-0.5.3/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 15:17:20.189269 jeffutils-0.5.4/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.4/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-15 15:17:20.189269 jeffutils-0.5.4/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.4/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.4/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-15 15:17:20.189269 jeffutils-0.5.4/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-15 15:17:16.000000 jeffutils-0.5.4/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 15:17:20.189269 jeffutils-0.5.4/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 15:17:20.189269 jeffutils-0.5.4/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.4/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    19988 2024-05-15 15:16:36.000000 jeffutils-0.5.4/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-15 15:17:20.189269 jeffutils-0.5.4/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-15 15:17:20.000000 jeffutils-0.5.4/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-15 15:17:20.000000 jeffutils-0.5.4/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-15 15:17:20.000000 jeffutils-0.5.4/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-15 15:17:20.000000 jeffutils-0.5.4/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.5.3/LICENSE.txt` & `jeffutils-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.5.3/setup.py` & `jeffutils-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.5.3',
+    version='0.5.4',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.5.3/src/jeffutils/utils.py` & `jeffutils-0.5.4/src/jeffutils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from time import perf_counter
 import time
 from datetime import datetime, timezone
+from collections import defaultdict
+import sqlite3 as sql
 import json
 import numpy as np
 import pandas as pd
 import io
 import os
 import pstats
 import cProfile
@@ -495,8 +497,92 @@
             # if the thread is no longer running, then the thread entry will
             # just have the last time that the thread was running
             else:
                 pass
             
         # sleep for 1 minute, so that it only checks all of the threads
         # every minute
-        time.sleep(60)
+        time.sleep(60)
+        
+############################################################
+#                       SQL FUNCTIONS                      #
+############################################################
+
+def get_sql_tables_info(db_path, verbose=True):
+    """
+    Retrieve and print all table names and their respective column names from a SQLite database.
+
+    Args:
+        db_path (str): The file path to the SQLite database.
+        verbose (bool): If True, prints the table names and columns to the console. Default is True.
+
+    Returns:
+        dict: A dictionary where the keys are table names and the values are lists of column names for each table.
+    
+    Example:
+        >>> sql_table_names_and_cols('example.db', verbose=True)
+        table1: id, name, age
+        table2: id, department, salary
+        {
+            'table1': {
+                'id': {'cid': 0, 'name': 'id', 'type': 'INTEGER', 'notnull': 0, 'dflt_value': None, 'pk': 0},
+                'name': {'cid': 1, 'name': 'name', 'type': 'TEXT', 'notnull': 0, 'dflt_value': None, 'pk': 0},
+                'age': {'cid': 2, 'name': 'age', 'type': 'INTEGER', 'notnull': 0, 'dflt_value': None, 'pk': 0}
+            }
+            'table2': {
+                'id': {'cid': 0, 'name': 'id', 'type': 'INTEGER', 'notnull'},
+                'departmet': {'cid': 1, 'name': 'department', 'type': 'TEXT', 'notnull': 0, 'dflt_value': None, 'pk': 0},
+                'salary': {'cid': 2, 'name': 'salary', 'type': 'INTEGER', 'notnull': 0, 'dflt_value': None, 'pk': 0}
+            }
+        }
+    
+    Note:
+        Ensure the database file exists at the specified path before calling this function.
+    """
+    # make sure the db_path exists and is a sqlite .db file
+    if not os.path.exists(db_path):
+        raise FileNotFoundError(f"Database file not found at path: {db_path}")
+    if not db_path.endswith('.db'):
+        raise ValueError("Database file must be a SQLite file with a .db extension.")
+    
+    try:
+        table_info = defaultdict(dict)
+        
+        with sql.connect(db_path) as conn:
+            cur = conn.cursor()
+            
+            # extrac each of the table names
+            query = '''
+            SELECT name FROM sqlite_master WHERE type='table'
+            '''
+            result = cur.execute(query).fetchall()
+            
+            # fore each table extract the table column information
+            for row in result:
+                table_name = row[0]
+                
+                # use PRAGMA table_info to get the column names
+                # and all of the information for each column
+                query = (
+                    f"PRAGMA table_info({table_name}) "
+                )
+                result = cur.execute(query).fetchall()
+                for row in result:
+                    cid, name, type, notnull, dflt_value, pk = row
+                    entry = {
+                        'cid': cid,
+                        'name': name,
+                        'type': type,
+                        'notnull': notnull,
+                        'dflt_value': dflt_value,
+                        'pk': pk
+                    }
+                    table_info[table_name][name] = entry
+            
+    finally:
+        conn.close()
+        
+    if verbose:
+        for table_name, col_names in table_info.items():
+            print(f'{table_name}:', ", ".join(map(str, col_names)))
+            
+    return table_info
```

