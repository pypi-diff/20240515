# Comparing `tmp/surrealist-0.4.1.tar.gz` & `tmp/surrealist-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surrealist-0.4.1.tar", last modified: Sat Apr 20 09:06:33 2024, max compression
+gzip compressed data, was "surrealist-0.5.0.tar", last modified: Wed May 15 11:06:42 2024, max compression
```

## Comparing `surrealist-0.4.1.tar` & `surrealist-0.5.0.tar`

### file list

```diff
@@ -1,57 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.703699 surrealist-0.4.1/
--rw-rw-rw-   0        0        0     1091 2024-02-04 05:55:53.000000 surrealist-0.4.1/LICENSE
--rw-rw-rw-   0        0        0    31030 2024-04-20 09:06:33.702699 surrealist-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0    29020 2024-04-20 09:05:50.000000 surrealist-0.4.1/README.md
--rw-rw-rw-   0        0        0      905 2024-04-20 09:05:50.000000 surrealist-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-20 09:06:33.703699 surrealist-0.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.606738 surrealist-0.4.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.619746 surrealist-0.4.1/src/surrealist/
--rw-rw-rw-   0        0        0      849 2024-04-20 09:05:50.000000 surrealist-0.4.1/src/surrealist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.632737 surrealist-0.4.1/src/surrealist/clients/
--rw-rw-rw-   0        0        0      124 2024-02-04 05:55:53.000000 surrealist-0.4.1/src/surrealist/clients/__init__.py
--rw-rw-rw-   0        0        0     5044 2024-02-16 16:27:45.000000 surrealist-0.4.1/src/surrealist/clients/http_client.py
--rw-rw-rw-   0        0        0     8117 2024-02-16 16:26:19.000000 surrealist-0.4.1/src/surrealist/clients/ws_client.py
-drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.650740 surrealist-0.4.1/src/surrealist/connections/
--rw-rw-rw-   0        0        0      198 2024-02-04 05:55:53.000000 surrealist-0.4.1/src/surrealist/connections/__init__.py
--rw-rw-rw-   0        0        0    18589 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/connections/connection.py
--rw-rw-rw-   0        0        0    27023 2024-03-14 16:05:03.000000 surrealist-0.4.1/src/surrealist/connections/http_connection.py
--rw-rw-rw-   0        0        0     8023 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/connections/pool.py
--rw-rw-rw-   0        0        0    29659 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/connections/ws_connection.py
--rw-rw-rw-   0        0        0     2439 2024-03-14 15:59:51.000000 surrealist-0.4.1/src/surrealist/errors.py
-drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.657740 surrealist-0.4.1/src/surrealist/ql/
--rw-rw-rw-   0        0        0      231 2024-03-02 11:31:18.000000 surrealist-0.4.1/src/surrealist/ql/__init__.py
--rw-rw-rw-   0        0        0    15690 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/ql/database.py
--rw-rw-rw-   0        0        0     3135 2024-03-02 11:31:18.000000 surrealist-0.4.1/src/surrealist/ql/pool_database.py
-drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.700670 surrealist-0.4.1/src/surrealist/ql/statements/
--rw-rw-rw-   0        0        0      473 2024-02-11 10:03:17.000000 surrealist-0.4.1/src/surrealist/ql/statements/__init__.py
--rw-rw-rw-   0        0        0     2909 2024-02-11 13:05:41.000000 surrealist-0.4.1/src/surrealist/ql/statements/common_statements.py
--rw-rw-rw-   0        0        0     1518 2024-02-12 10:41:24.000000 surrealist-0.4.1/src/surrealist/ql/statements/create.py
--rw-rw-rw-   0        0        0     1345 2024-02-11 10:03:17.000000 surrealist-0.4.1/src/surrealist/ql/statements/create_statements.py
--rw-rw-rw-   0        0        0    15710 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/ql/statements/define.py
--rw-rw-rw-   0        0        0     1213 2024-02-19 06:12:19.000000 surrealist-0.4.1/src/surrealist/ql/statements/delete.py
--rw-rw-rw-   0        0        0     2409 2024-02-19 06:14:54.000000 surrealist-0.4.1/src/surrealist/ql/statements/insert.py
--rw-rw-rw-   0        0        0      496 2024-02-09 12:21:48.000000 surrealist-0.4.1/src/surrealist/ql/statements/insert_statements.py
--rw-rw-rw-   0        0        0     2967 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/ql/statements/live.py
--rw-rw-rw-   0        0        0     1289 2024-02-12 10:41:24.000000 surrealist-0.4.1/src/surrealist/ql/statements/live_statements.py
--rw-rw-rw-   0        0        0     1749 2024-02-19 06:06:05.000000 surrealist-0.4.1/src/surrealist/ql/statements/permissions.py
--rw-rw-rw-   0        0        0     1377 2024-02-12 10:41:24.000000 surrealist-0.4.1/src/surrealist/ql/statements/relate.py
--rw-rw-rw-   0        0        0     1792 2024-03-13 09:08:42.000000 surrealist-0.4.1/src/surrealist/ql/statements/remove.py
--rw-rw-rw-   0        0        0      825 2024-02-12 10:41:24.000000 surrealist-0.4.1/src/surrealist/ql/statements/returns.py
--rw-rw-rw-   0        0        0     3190 2024-02-19 06:14:54.000000 surrealist-0.4.1/src/surrealist/ql/statements/select.py
--rw-rw-rw-   0        0        0     8006 2024-02-11 12:57:39.000000 surrealist-0.4.1/src/surrealist/ql/statements/select_statements.py
--rw-rw-rw-   0        0        0     1860 2024-04-20 09:05:50.000000 surrealist-0.4.1/src/surrealist/ql/statements/show.py
--rw-rw-rw-   0        0        0     1510 2024-02-19 06:06:05.000000 surrealist-0.4.1/src/surrealist/ql/statements/simple_statements.py
--rw-rw-rw-   0        0        0     3436 2024-02-16 16:23:17.000000 surrealist-0.4.1/src/surrealist/ql/statements/statement.py
--rw-rw-rw-   0        0        0      924 2024-02-19 06:12:19.000000 surrealist-0.4.1/src/surrealist/ql/statements/transaction.py
--rw-rw-rw-   0        0        0     1273 2024-02-19 06:12:19.000000 surrealist-0.4.1/src/surrealist/ql/statements/update.py
--rw-rw-rw-   0        0        0     2079 2024-02-09 12:21:48.000000 surrealist-0.4.1/src/surrealist/ql/statements/update_statements.py
--rw-rw-rw-   0        0        0     8908 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/ql/table.py
--rw-rw-rw-   0        0        0     8695 2024-04-14 06:04:00.000000 surrealist-0.4.1/src/surrealist/result.py
--rw-rw-rw-   0        0        0     9831 2024-03-29 07:04:55.000000 surrealist-0.4.1/src/surrealist/surreal.py
--rw-rw-rw-   0        0        0     2221 2024-04-20 09:05:50.000000 surrealist-0.4.1/src/surrealist/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 09:06:33.701699 surrealist-0.4.1/src/surrealist.egg-info/
--rw-rw-rw-   0        0        0    31030 2024-04-20 09:06:33.000000 surrealist-0.4.1/src/surrealist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1729 2024-04-20 09:06:33.000000 surrealist-0.4.1/src/surrealist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 09:06:33.000000 surrealist-0.4.1/src/surrealist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-20 09:06:33.000000 surrealist-0.4.1/src/surrealist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-20 09:06:33.000000 surrealist-0.4.1/src/surrealist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.564814 surrealist-0.5.0/
+-rw-rw-rw-   0        0        0     1091 2024-02-04 05:55:53.000000 surrealist-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0    31030 2024-05-15 11:06:42.563815 surrealist-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    29020 2024-05-15 11:06:07.000000 surrealist-0.5.0/README.md
+-rw-rw-rw-   0        0        0      905 2024-05-15 11:06:07.000000 surrealist-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 11:06:42.564814 surrealist-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.495815 surrealist-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.507815 surrealist-0.5.0/src/surrealist/
+-rw-rw-rw-   0        0        0      849 2024-04-20 09:05:50.000000 surrealist-0.5.0/src/surrealist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.518814 surrealist-0.5.0/src/surrealist/clients/
+-rw-rw-rw-   0        0        0      124 2024-02-04 05:55:53.000000 surrealist-0.5.0/src/surrealist/clients/__init__.py
+-rw-rw-rw-   0        0        0     5044 2024-02-16 16:27:45.000000 surrealist-0.5.0/src/surrealist/clients/http_client.py
+-rw-rw-rw-   0        0        0     8117 2024-02-16 16:26:19.000000 surrealist-0.5.0/src/surrealist/clients/ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.525815 surrealist-0.5.0/src/surrealist/connections/
+-rw-rw-rw-   0        0        0      198 2024-02-04 05:55:53.000000 surrealist-0.5.0/src/surrealist/connections/__init__.py
+-rw-rw-rw-   0        0        0    19339 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/connections/connection.py
+-rw-rw-rw-   0        0        0    27023 2024-03-14 16:05:03.000000 surrealist-0.5.0/src/surrealist/connections/http_connection.py
+-rw-rw-rw-   0        0        0     8023 2024-04-14 06:04:00.000000 surrealist-0.5.0/src/surrealist/connections/pool.py
+-rw-rw-rw-   0        0        0    29659 2024-04-14 06:04:00.000000 surrealist-0.5.0/src/surrealist/connections/ws_connection.py
+-rw-rw-rw-   0        0        0     2439 2024-03-14 15:59:51.000000 surrealist-0.5.0/src/surrealist/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.530815 surrealist-0.5.0/src/surrealist/ql/
+-rw-rw-rw-   0        0        0      231 2024-03-02 11:31:18.000000 surrealist-0.5.0/src/surrealist/ql/__init__.py
+-rw-rw-rw-   0        0        0    16349 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/database.py
+-rw-rw-rw-   0        0        0     3135 2024-03-02 11:31:18.000000 surrealist-0.5.0/src/surrealist/ql/pool_database.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.561815 surrealist-0.5.0/src/surrealist/ql/statements/
+-rw-rw-rw-   0        0        0      530 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/__init__.py
+-rw-rw-rw-   0        0        0     2909 2024-02-11 13:05:41.000000 surrealist-0.5.0/src/surrealist/ql/statements/common_statements.py
+-rw-rw-rw-   0        0        0     1518 2024-02-12 10:41:24.000000 surrealist-0.5.0/src/surrealist/ql/statements/create.py
+-rw-rw-rw-   0        0        0     1282 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/create_statements.py
+-rw-rw-rw-   0        0        0    15142 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/define.py
+-rw-rw-rw-   0        0        0     5465 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/define_index_statements.py
+-rw-rw-rw-   0        0        0     1213 2024-02-19 06:12:19.000000 surrealist-0.5.0/src/surrealist/ql/statements/delete.py
+-rw-rw-rw-   0        0        0     2409 2024-02-19 06:14:54.000000 surrealist-0.5.0/src/surrealist/ql/statements/insert.py
+-rw-rw-rw-   0        0        0      496 2024-02-09 12:21:48.000000 surrealist-0.5.0/src/surrealist/ql/statements/insert_statements.py
+-rw-rw-rw-   0        0        0     2967 2024-04-14 06:04:00.000000 surrealist-0.5.0/src/surrealist/ql/statements/live.py
+-rw-rw-rw-   0        0        0     1289 2024-02-12 10:41:24.000000 surrealist-0.5.0/src/surrealist/ql/statements/live_statements.py
+-rw-rw-rw-   0        0        0     1749 2024-02-19 06:06:05.000000 surrealist-0.5.0/src/surrealist/ql/statements/permissions.py
+-rw-rw-rw-   0        0        0      962 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/rebuild_index.py
+-rw-rw-rw-   0        0        0     1377 2024-02-12 10:41:24.000000 surrealist-0.5.0/src/surrealist/ql/statements/relate.py
+-rw-rw-rw-   0        0        0     1792 2024-03-13 09:08:42.000000 surrealist-0.5.0/src/surrealist/ql/statements/remove.py
+-rw-rw-rw-   0        0        0      825 2024-02-12 10:41:24.000000 surrealist-0.5.0/src/surrealist/ql/statements/returns.py
+-rw-rw-rw-   0        0        0     3190 2024-02-19 06:14:54.000000 surrealist-0.5.0/src/surrealist/ql/statements/select.py
+-rw-rw-rw-   0        0        0     8006 2024-02-11 12:57:39.000000 surrealist-0.5.0/src/surrealist/ql/statements/select_statements.py
+-rw-rw-rw-   0        0        0     2167 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/show.py
+-rw-rw-rw-   0        0        0     1457 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/simple_statements.py
+-rw-rw-rw-   0        0        0     3436 2024-02-16 16:23:17.000000 surrealist-0.5.0/src/surrealist/ql/statements/statement.py
+-rw-rw-rw-   0        0        0      924 2024-02-19 06:12:19.000000 surrealist-0.5.0/src/surrealist/ql/statements/transaction.py
+-rw-rw-rw-   0        0        0     1273 2024-02-19 06:12:19.000000 surrealist-0.5.0/src/surrealist/ql/statements/update.py
+-rw-rw-rw-   0        0        0     2016 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/update_statements.py
+-rw-rw-rw-   0        0        0      621 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/utils.py
+-rw-rw-rw-   0        0        0     9582 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/table.py
+-rw-rw-rw-   0        0        0     8695 2024-04-14 06:04:00.000000 surrealist-0.5.0/src/surrealist/result.py
+-rw-rw-rw-   0        0        0     9831 2024-03-29 07:04:55.000000 surrealist-0.5.0/src/surrealist/surreal.py
+-rw-rw-rw-   0        0        0     2221 2024-04-20 09:05:50.000000 surrealist-0.5.0/src/surrealist/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.562814 surrealist-0.5.0/src/surrealist.egg-info/
+-rw-rw-rw-   0        0        0    31030 2024-05-15 11:06:42.000000 surrealist-0.5.0/src/surrealist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1869 2024-05-15 11:06:42.000000 surrealist-0.5.0/src/surrealist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 11:06:42.000000 surrealist-0.5.0/src/surrealist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 11:06:42.000000 surrealist-0.5.0/src/surrealist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 11:06:42.000000 surrealist-0.5.0/src/surrealist.egg-info/top_level.txt
```

### Comparing `surrealist-0.4.1/LICENSE` & `surrealist-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/PKG-INFO` & `surrealist-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surrealist
-Version: 0.4.1
+Version: 0.5.0
 Summary: Python client for SurrealDB, latest SurrealDB version compatible, all features supported
 Author-email: kotolex <farofwell@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -45,15 +45,15 @@
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
  * only one small dependency (websocket-client), no need to pull a lot of libraries to your project
  * fully documented
  * well tested (on the latest Ubuntu, macOS and Windows 10)
- * fully compatible with the latest version of SurrealDB (1.4.2), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
+ * fully compatible with the latest version of SurrealDB (1.5.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
  * debug mode to see all that goes in and out if you need
  * iterator to handle big select queries
  * QL-builder to explore, generate and use SurrealDB queries (explain, transaction etc.)
  * connections pool for use at a high load
  * http or websocket transport to use
  * always up to date with SurrealDB features and changes
```

### Comparing `surrealist-0.4.1/README.md` & `surrealist-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
  * only one small dependency (websocket-client), no need to pull a lot of libraries to your project
  * fully documented
  * well tested (on the latest Ubuntu, macOS and Windows 10)
- * fully compatible with the latest version of SurrealDB (1.4.2), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
+ * fully compatible with the latest version of SurrealDB (1.5.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
  * debug mode to see all that goes in and out if you need
  * iterator to handle big select queries
  * QL-builder to explore, generate and use SurrealDB queries (explain, transaction etc.)
  * connections pool for use at a high load
  * http or websocket transport to use
  * always up to date with SurrealDB features and changes
```

### Comparing `surrealist-0.4.1/pyproject.toml` & `surrealist-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "surrealist"
-version = "0.4.1"
+version = "0.5.0"
 description = "Python client for SurrealDB, latest SurrealDB version compatible, all features supported"
 readme = "README.md"
 authors = [{ name = "kotolex", email = "farofwell@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
```

### Comparing `surrealist-0.4.1/src/surrealist/__init__.py` & `surrealist-0.5.0/src/surrealist/__init__.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/clients/http_client.py` & `surrealist-0.5.0/src/surrealist/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/clients/ws_client.py` & `surrealist-0.5.0/src/surrealist/clients/ws_client.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/connections/connection.py` & `surrealist-0.5.0/src/surrealist/connections/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,66 +96,73 @@
         logger.info("Query-Operation: COUNT. Table: %s", crop_data(table_name))
         result = self.query(f"SELECT count() FROM {table_name} GROUP ALL;")
         if not result.is_error():
             result.result = self._get_count(result.result)
         return result
 
     @connected
-    def table_info(self, table_name: str) -> SurrealResult:
+    def table_info(self, table_name: str, structured: bool = False) -> SurrealResult:
         """
         Returns info about specified table. You should have permissions for this action.
 
         Actually converts to QL "INFO FOR TABLE table_name" to use in **query** method.
 
         Refer to: https://docs.surrealdb.com/docs/surrealql/statements/info
 
+        :param table_name: name of the table
+        :param structured: if True returns data in structured view (use STRUCTURE statement). Note: experimental!
         :return: full table information
         """
-        return self._info(f"TABLE {table_name}")
+        return self._info(f"TABLE {table_name}", structured)
 
     @connected
-    def db_info(self) -> SurrealResult:
+    def db_info(self, structured: bool = False) -> SurrealResult:
         """
         Returns info about a current database. You should have permissions for this action.
 
         Actually converts to QL "INFO FOR DB" to use in **query** method.
 
         Refer to: https://docs.surrealdb.com/docs/surrealql/statements/info
 
+        :param structured: if True returns data in structured view (use STRUCTURE statement). Note: experimental!
         :return: full database information
         """
-        return self._info("DB")
+        return self._info("DB", structured)
 
     @connected
-    def ns_info(self) -> SurrealResult:
+    def ns_info(self, structured: bool = False) -> SurrealResult:
         """
         Returns info about current namespace. You should have permissions for this action.
 
         Actually converts to QL "INFO FOR NS" to use in **query** method.
 
         Refer to: https://docs.surrealdb.com/docs/surrealql/statements/info
 
+        :param structured: if True returns data in structured view (use STRUCTURE statement). Note: experimental!
         :return: full namespace information
         """
-        return self._info("NS")
+        return self._info("NS", structured)
 
     @connected
-    def root_info(self) -> SurrealResult:
+    def root_info(self, structured: bool = False) -> SurrealResult:
         """
         Returns info about root. You should have permissions for this action.
 
         Actually converts to QL "INFO FOR ROOT" to use in **query** method.
 
         Refer to: https://docs.surrealdb.com/docs/surrealql/statements/info
 
+        :param structured: if True returns data in structured view (use STRUCTURE statement). Note: experimental!
         :return: information about root
         """
-        return self._info("ROOT")
+        return self._info("ROOT", structured)
 
-    def _info(self, type_: str) -> SurrealResult:
+    def _info(self, type_: str, structured: bool = False) -> SurrealResult:
+        if structured:
+            type_ = f"{type_} STRUCTURE"
         logger.info("Query-Operation: %s_INFO", type_)
         return self.query(f"INFO FOR {type_};")
 
     @connected
     def session_info(self) -> SurrealResult:
         """
         Returns info about the current session. You should have permissions for this action.
```

### Comparing `surrealist-0.4.1/src/surrealist/connections/http_connection.py` & `surrealist-0.5.0/src/surrealist/connections/http_connection.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/connections/pool.py` & `surrealist-0.5.0/src/surrealist/connections/pool.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/connections/ws_connection.py` & `surrealist-0.5.0/src/surrealist/connections/ws_connection.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/errors.py` & `surrealist-0.5.0/src/surrealist/errors.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/database.py` & `surrealist-0.5.0/src/surrealist/ql/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from typing import Optional, Tuple, List, Dict, Union, Any, Callable
 
 from surrealist.ql.statements import Select, Remove, Live
 from surrealist.ql.statements.define import (DefineEvent, DefineUser, DefineParam, DefineAnalyzer, DefineScope,
                                              DefineIndex, DefineToken, DefineTable, DefineField)
+from surrealist.ql.statements.rebuild_index import RebuildIndex
 from surrealist.ql.statements.relate import Relate
 from surrealist.ql.statements.returns import Return
 from surrealist.ql.statements.statement import Statement
 from surrealist.ql.statements.transaction import Transaction
 from surrealist.ql.table import Table
 from surrealist.result import SurrealResult
 from surrealist.surreal import Surreal
@@ -282,14 +283,27 @@
 
         :param name: name for the index
         :param table_name: name of table to work with
         :return: DefineINdex object
         """
         return DefineIndex(self._connection, name, table_name)
 
+    def rebuild_index(self, index_name: str, table_name: str, if_exists: bool = False) -> RebuildIndex:
+        """
+        Represents REBUILD INDEX object, used to rebuild resources.
+
+        Refer to: https://surrealdb.com/docs/surrealdb/surrealql/statements/rebuild
+
+        :param index_name: name of the index
+        :param table_name: name of the table
+        :param if_exists: use IF EXISTS statement if True
+        :return: RebuildIndex object
+        """
+        return RebuildIndex(self._connection, index_name=index_name, table_name=table_name, if_exists=if_exists)
+
     def remove_index(self, name: str, table_name: str) -> Remove:
         """
         Remove index by name on the table
 
         :param name: name og the index
         :param table_name: name of the table
         :return: Remove object
```

### Comparing `surrealist-0.4.1/src/surrealist/ql/pool_database.py` & `surrealist-0.5.0/src/surrealist/ql/pool_database.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/common_statements.py` & `surrealist-0.5.0/src/surrealist/ql/statements/common_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/create.py` & `surrealist-0.5.0/src/surrealist/ql/statements/create.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/create_statements.py` & `surrealist-0.5.0/src/surrealist/ql/statements/create_statements.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import json
 from typing import Dict, Optional
 
 from surrealist.ql.statements.common_statements import CanUseReturn
 from surrealist.ql.statements.statement import FinishedStatement, Statement
+from surrealist.ql.statements.utils import combine
 
 
 class Set(FinishedStatement, CanUseReturn):
     def __init__(self, statement: Statement, result: Optional[str] = None, **kwargs):
         super().__init__(statement)
         self._kw = kwargs
         self._result = result
 
     def _clean_str(self):
         if not self._kw and not self._result:
             return self._statement._clean_str()
-        if not self._result:
-            args = ", ".join(f"{k} = {json.dumps(v)}" for k, v in self._kw.items())
-        else:
-            args = self._result
+        args = combine(self._result, self._kw)
         return f"{self._statement._clean_str()} SET {args}"
 
 
 class Content(FinishedStatement, CanUseReturn):
     def __init__(self, statement: Statement, content: Dict):
         super().__init__(statement)
         self._content = content
```

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/define.py` & `surrealist-0.5.0/src/surrealist/ql/statements/define.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC
 from typing import List, Union, Any, Optional, Tuple
 
 from surrealist.connections import Connection
+from surrealist.ql.statements.define_index_statements import CanUseIndexTypes
 from surrealist.ql.statements.permissions import CanUsePermissions
 from surrealist.ql.statements.statement import Statement
 from surrealist.utils import OK
 
 
 class Define(Statement, ABC):
     """
@@ -202,15 +203,15 @@
         return [OK]
 
     def _clean_str(self):
         return f"DEFINE SCOPE{self._exists()} {self._name} SESSION {self._duration} \nSIGNUP {self._signup} " \
                f"\nSIGNIN {self._signin}"
 
 
-class DefineIndex(Define):
+class DefineIndex(Define, CanUseIndexTypes):
     """
     Represents DEFINE INDEX statement
 
     Refer to: https://docs.surrealdb.com/docs/surrealql/statements/define/indexes
 
     Example: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/database.py
     """
@@ -241,43 +242,21 @@
         Represents fields for index, COLUMNS statement
 
         :param columns: fields to index
         """
         self._fields = f"COLUMNS {columns}"
         return self
 
-    def unique(self) -> "DefineIndex":
-        """
-        Represents UNIQUE statement
-        """
-        self._analyzer = None
-        self._uni = True
-        return self
-
-    def search_analyzer(self, name: str, use: str = "BM25", highlights: bool = True) -> "DefineIndex":
-        """
-        Represents SEARCH ANALYZER statement
-        """
-        self._uni = False
-        hl = "" if not highlights else " HIGHLIGHTS"
-        self._analyzer = f" SEARCH ANALYZER {name} {use}{hl}"
-        return self
-
     def validate(self) -> List[str]:
         if not self._fields:
             return ["You need to specify FIELDS or COLUMNS"]
         return [OK]
 
     def _clean_str(self):
-        add = ""
-        if self._uni:
-            add = " UNIQUE"
-        elif self._analyzer:
-            add = self._analyzer
-        return f"DEFINE INDEX{self._exists()} {self._name} ON TABLE {self._table_name} {self._fields}{add}"
+        return f"DEFINE INDEX{self._exists()} {self._name} ON TABLE {self._table_name} {self._fields}"
 
 
 class DefineToken(Define):
     """
     Represents DEFINE TOKEN statement
 
     Refer to: https://docs.surrealdb.com/docs/surrealql/statements/define/token
```

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/delete.py` & `surrealist-0.5.0/src/surrealist/ql/statements/delete.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/insert.py` & `surrealist-0.5.0/src/surrealist/ql/statements/insert.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/live.py` & `surrealist-0.5.0/src/surrealist/ql/statements/live.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/live_statements.py` & `surrealist-0.5.0/src/surrealist/ql/statements/live_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/permissions.py` & `surrealist-0.5.0/src/surrealist/ql/statements/permissions.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/relate.py` & `surrealist-0.5.0/src/surrealist/ql/statements/relate.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/remove.py` & `surrealist-0.5.0/src/surrealist/ql/statements/remove.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/returns.py` & `surrealist-0.5.0/src/surrealist/ql/statements/returns.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/select.py` & `surrealist-0.5.0/src/surrealist/ql/statements/select.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/select_statements.py` & `surrealist-0.5.0/src/surrealist/ql/statements/select_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/show.py` & `surrealist-0.5.0/src/surrealist/ql/statements/show.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,18 +30,28 @@
             except ValueError:
                 result.append("Timestamp in the wrong format, you need iso-date like 2024-01-01T10:10:10.000001Z")
         if self._limit and self._limit < 1:
             result.append("Limit should not be less than 1")
         return [OK] if not result else result
 
     def limit(self, limit: int) -> "Show":
+        """
+        Limits number of results to show (LIMIT statement)
+        :param limit: number of results
+        :return: Show object
+        """
         self._limit = limit
         return self
 
     def since(self, timestamp: str) -> "Show":
+        """
+        Init timestamp since is to show updates
+        :param timestamp: surreal timestamp
+        :return: Show object
+        """
         self._since = timestamp
         return self
 
     def _clean_str(self):
         if not self._since:
             self._since = to_surreal_datetime_str(datetime.now(timezone.utc))  # default value
         limit = f" LIMIT {self._limit}" if self._limit else ""
```

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/simple_statements.py` & `surrealist-0.5.0/src/surrealist/ql/statements/simple_statements.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Optional
+from surrealist.ql.statements.utils import combine
 
 
 class Where:
     """
     Represents simple WHERE statement for DEFINE FIELD and DEFINE TABLE
     """
     def __init__(self, raw_string: Optional[str] = None, **kwargs):
         self._raw = raw_string
         self._kw = kwargs
-        self._body = raw_string if raw_string else ", ".join(f"{k} = {v}" for k, v in kwargs.items())
+        self._body = combine(self._raw, self._kw)
         self._body = f"WHERE {self._body}"
 
     def __str__(self):
         return self._body
 
     def __repr__(self):
         return f"Where({self._raw=}, {self._kw=})"
@@ -31,13 +32,13 @@
 
 
 class OrAnd(Where):
     def __init__(self, parent: Where, use_or: bool = True, raw_string: Optional[str] = None, **kwargs):
         super().__init__(raw_string, **kwargs)
         self._or = use_or
         self._parent = parent
-        self._cur_body = raw_string if raw_string else ", ".join(f"{k} = {v}" for k, v in kwargs.items())
+        self._cur_body = combine(raw_string, kwargs)
         self._type = "OR" if self._or else "AND"
         self._body = f"{parent} {self._type} {self._cur_body}"
 
     def __repr__(self):
         return f"{self._type}({self._raw=}, {self._kw=}, {self._parent:!r})"
```

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/statement.py` & `surrealist-0.5.0/src/surrealist/ql/statements/statement.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/transaction.py` & `surrealist-0.5.0/src/surrealist/ql/statements/transaction.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/update.py` & `surrealist-0.5.0/src/surrealist/ql/statements/update.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/ql/statements/update_statements.py` & `surrealist-0.5.0/src/surrealist/ql/statements/update_statements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import json
 from typing import Dict, List, Optional
 
 from surrealist.ql.statements.common_statements import CanUseWhere
 from surrealist.ql.statements.statement import FinishedStatement, Statement
+from surrealist.ql.statements.utils import combine
 
 
 class Set(FinishedStatement, CanUseWhere):
     def __init__(self, statement: Statement, result: Optional[str] = None, **kwargs):
         super().__init__(statement)
         self._kw = kwargs
         self._result = result
 
     def _clean_str(self):
         if not self._kw and not self._result:
             return self._statement._clean_str()
-        if not self._result:
-            args = ", ".join(f"{k} = {json.dumps(v)}" for k, v in self._kw.items())
-        else:
-            args = self._result
+        args = combine(self._result, self._kw)
         return f"{self._statement._clean_str()} SET {args}"
 
 
 class Patch(FinishedStatement, CanUseWhere):
     def __init__(self, statement: Statement, operations: List[Dict]):
         super().__init__(statement)
         self._value = operations
```

### Comparing `surrealist-0.4.1/src/surrealist/ql/table.py` & `surrealist-0.5.0/src/surrealist/ql/table.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Optional, Callable, Dict, Tuple, Union, List
 
-from surrealist.errors import WrongCallError
 from surrealist.connections import Connection
+from surrealist.errors import WrongCallError
 from surrealist.ql.statements.create import Create
 from surrealist.ql.statements.delete import Delete
 from surrealist.ql.statements.insert import Insert
 from surrealist.ql.statements.live import Live
+from surrealist.ql.statements.rebuild_index import RebuildIndex
 from surrealist.ql.statements.remove import Remove
 from surrealist.ql.statements.select import Select
 from surrealist.ql.statements.show import Show
 from surrealist.ql.statements.statement import Statement
 from surrealist.ql.statements.update import Update
 from surrealist.result import SurrealResult
 
@@ -220,13 +221,28 @@
         Examples: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/ql_update_examples.py
 
         :param record_id: optional, if specified transform to 'table_name:record_id'
         :return: Update object
         """
         return Update(self._connection, self._name, record_id)
 
+    def rebuild_index(self, index_name: str, if_exists: bool = False) -> RebuildIndex:
+        """
+        Represents REBUILD INDEX object, used to rebuild resources.
+
+        Example:
+        db.table("user").rebuild_index("my_index").run()
+
+        Refer to: https://surrealdb.com/docs/surrealdb/surrealql/statements/rebuild
+
+        :param index_name: name of the index
+        :param if_exists: use IF EXISTS statement if True
+        :return: RebuildIndex object
+        """
+        return RebuildIndex(self._connection, index_name=index_name, table_name=self._name, if_exists=if_exists)
+
     def __repr__(self):
         return f"Table(name={self._name})"
 
     def __call__(self, *args, **kwargs):
         raise WrongCallError(f"Table object is not callable. \n"
                              f"It looks like you misspelled the method name of Database({self._name})")
```

### Comparing `surrealist-0.4.1/src/surrealist/result.py` & `surrealist-0.5.0/src/surrealist/result.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/surreal.py` & `surrealist-0.5.0/src/surrealist/surreal.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist/utils.py` & `surrealist-0.5.0/src/surrealist/utils.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.4.1/src/surrealist.egg-info/PKG-INFO` & `surrealist-0.5.0/src/surrealist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surrealist
-Version: 0.4.1
+Version: 0.5.0
 Summary: Python client for SurrealDB, latest SurrealDB version compatible, all features supported
 Author-email: kotolex <farofwell@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -45,15 +45,15 @@
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
  * only one small dependency (websocket-client), no need to pull a lot of libraries to your project
  * fully documented
  * well tested (on the latest Ubuntu, macOS and Windows 10)
- * fully compatible with the latest version of SurrealDB (1.4.2), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
+ * fully compatible with the latest version of SurrealDB (1.5.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
  * debug mode to see all that goes in and out if you need
  * iterator to handle big select queries
  * QL-builder to explore, generate and use SurrealDB queries (explain, transaction etc.)
  * connections pool for use at a high load
  * http or websocket transport to use
  * always up to date with SurrealDB features and changes
```

### Comparing `surrealist-0.4.1/src/surrealist.egg-info/SOURCES.txt` & `surrealist-0.5.0/src/surrealist.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,24 +24,27 @@
 src/surrealist/ql/pool_database.py
 src/surrealist/ql/table.py
 src/surrealist/ql/statements/__init__.py
 src/surrealist/ql/statements/common_statements.py
 src/surrealist/ql/statements/create.py
 src/surrealist/ql/statements/create_statements.py
 src/surrealist/ql/statements/define.py
+src/surrealist/ql/statements/define_index_statements.py
 src/surrealist/ql/statements/delete.py
 src/surrealist/ql/statements/insert.py
 src/surrealist/ql/statements/insert_statements.py
 src/surrealist/ql/statements/live.py
 src/surrealist/ql/statements/live_statements.py
 src/surrealist/ql/statements/permissions.py
+src/surrealist/ql/statements/rebuild_index.py
 src/surrealist/ql/statements/relate.py
 src/surrealist/ql/statements/remove.py
 src/surrealist/ql/statements/returns.py
 src/surrealist/ql/statements/select.py
 src/surrealist/ql/statements/select_statements.py
 src/surrealist/ql/statements/show.py
 src/surrealist/ql/statements/simple_statements.py
 src/surrealist/ql/statements/statement.py
 src/surrealist/ql/statements/transaction.py
 src/surrealist/ql/statements/update.py
-src/surrealist/ql/statements/update_statements.py
+src/surrealist/ql/statements/update_statements.py
+src/surrealist/ql/statements/utils.py
```

