# Comparing `tmp/database_creator-0.0.tar.gz` & `tmp/database_creator-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_creator-0.0.tar", last modified: Mon May 13 15:45:04 2024, max compression
+gzip compressed data, was "database_creator-1.0.tar", last modified: Wed May 15 14:54:55 2024, max compression
```

## Comparing `database_creator-0.0.tar` & `database_creator-1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 15:45:04.700672 database_creator-0.0/
--rw-rw-rw-   0        0        0       95 2024-05-13 15:45:04.700672 database_creator-0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 15:45:04.682637 database_creator-0.0/database_creator/
--rw-rw-rw-   0        0        0       31 2024-05-13 15:39:56.000000 database_creator-0.0/database_creator/__init__.py
--rw-rw-rw-   0        0        0     2794 2024-05-12 11:15:54.000000 database_creator-0.0/database_creator/db_module.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:45:04.699669 database_creator-0.0/database_creator.egg-info/
--rw-rw-rw-   0        0        0       95 2024-05-13 15:45:04.000000 database_creator-0.0/database_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-05-13 15:45:04.000000 database_creator-0.0/database_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 15:45:04.000000 database_creator-0.0/database_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-13 15:45:04.000000 database_creator-0.0/database_creator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2024-05-13 15:45:04.000000 database_creator-0.0/database_creator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 15:45:04.701671 database_creator-0.0/setup.cfg
--rw-rw-rw-   0        0        0      204 2024-05-13 15:38:59.000000 database_creator-0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:54:55.557436 database_creator-1.0/
+-rw-rw-rw-   0        0        0      383 2024-05-15 14:54:55.557436 database_creator-1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 14:54:55.547417 database_creator-1.0/database_creator/
+-rw-rw-rw-   0        0        0       31 2024-05-13 15:39:56.000000 database_creator-1.0/database_creator/__init__.py
+-rw-rw-rw-   0        0        0     2828 2024-05-15 14:45:51.000000 database_creator-1.0/database_creator/db_module.py
+drwxrwxrwx   0        0        0        0 2024-05-15 14:54:55.557436 database_creator-1.0/database_creator.egg-info/
+-rw-rw-rw-   0        0        0      383 2024-05-15 14:54:55.000000 database_creator-1.0/database_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-05-15 14:54:55.000000 database_creator-1.0/database_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 14:54:55.000000 database_creator-1.0/database_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-15 14:54:55.000000 database_creator-1.0/database_creator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-05-15 14:54:55.000000 database_creator-1.0/database_creator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 14:54:55.559947 database_creator-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      481 2024-05-15 14:54:45.000000 database_creator-1.0/setup.py
```

### Comparing `database_creator-0.0/database_creator/db_module.py` & `database_creator-1.0/database_creator/db_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,9 @@
             database.cursor.execute(f"SELECT {columns} FROM {table} {request}")
 
             return database.cursor.fetchone() if fetchone else database.cursor.fetchall()
 
         def delete(database: object, table: str, request: str) -> None:
             "Delete data in table with request sorting"
 
-            database.cursor.execute(f"DELETE FROM {table} Where {request}")
+            database.cursor.execute(f"DELETE FROM {table} Where {request}")
+            database.db.commit()
```

