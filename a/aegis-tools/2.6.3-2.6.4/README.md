# Comparing `tmp/aegis-tools-2.6.3.tar.gz` & `tmp/aegis-tools-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.6.3.tar", last modified: Mon May  6 18:49:45 2024, max compression
+gzip compressed data, was "aegis-tools-2.6.4.tar", last modified: Wed May 15 02:29:26 2024, max compression
```

## Comparing `aegis-tools-2.6.3.tar` & `aegis-tools-2.6.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-06 18:49:45.329288 aegis-tools-2.6.3/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-05-06 18:49:45.329288 aegis-tools-2.6.3/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-06 18:49:45.305288 aegis-tools-2.6.3/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    20802 2024-04-30 00:13:47.000000 aegis-tools-2.6.3/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    19087 2024-04-30 00:19:28.000000 aegis-tools-2.6.3/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2831 2024-02-09 21:33:25.000000 aegis-tools-2.6.3/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25607 2024-04-30 01:24:43.000000 aegis-tools-2.6.3/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    27302 2024-04-22 18:29:41.000000 aegis-tools-2.6.3/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.6.3/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    46355 2024-05-06 18:46:46.000000 aegis-tools-2.6.3/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-06 18:49:45.321288 aegis-tools-2.6.3/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.6.3/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4611 2024-01-31 22:04:42.000000 aegis-tools-2.6.3/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.6.3/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.6.3/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.6.3/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    37012 2024-04-18 02:54:56.000000 aegis-tools-2.6.3/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-06 18:49:45.325288 aegis-tools-2.6.3/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3071 2023-09-30 03:49:20.000000 aegis-tools-2.6.3/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.6.3/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.6.3/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.6.3/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3377 2023-08-14 03:31:20.000000 aegis-tools-2.6.3/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2238 2023-09-30 03:49:39.000000 aegis-tools-2.6.3/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.6.3/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1857 2023-09-30 03:52:25.000000 aegis-tools-2.6.3/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.6.3/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.6.3/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.6.3/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.6.3/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.6.3/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.6.3/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    78528 2024-04-30 00:13:28.000000 aegis-tools-2.6.3/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-06 18:49:45.329288 aegis-tools-2.6.3/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-05-06 18:49:45.000000 aegis-tools-2.6.3/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2024-05-06 18:49:45.000000 aegis-tools-2.6.3/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2024-05-06 18:49:45.000000 aegis-tools-2.6.3/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2024-05-06 18:49:45.000000 aegis-tools-2.6.3/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2024-05-06 18:49:45.000000 aegis-tools-2.6.3/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2024-05-06 18:49:45.000000 aegis-tools-2.6.3/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2024-05-06 18:49:45.329288 aegis-tools-2.6.3/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1716 2023-09-26 15:24:50.000000 aegis-tools-2.6.3/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-15 02:29:26.555724 aegis-tools-2.6.4/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-05-15 02:29:26.555724 aegis-tools-2.6.4/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-15 02:29:26.539724 aegis-tools-2.6.4/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    20802 2024-04-30 00:13:47.000000 aegis-tools-2.6.4/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    19087 2024-04-30 00:19:28.000000 aegis-tools-2.6.4/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2831 2024-02-09 21:33:25.000000 aegis-tools-2.6.4/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    26399 2024-05-15 02:29:17.000000 aegis-tools-2.6.4/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    27302 2024-04-22 18:29:41.000000 aegis-tools-2.6.4/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.6.4/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    46365 2024-05-15 02:29:17.000000 aegis-tools-2.6.4/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-15 02:29:26.547724 aegis-tools-2.6.4/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.6.4/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4611 2024-01-31 22:04:42.000000 aegis-tools-2.6.4/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.6.4/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.6.4/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.6.4/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    37012 2024-04-18 02:54:56.000000 aegis-tools-2.6.4/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-15 02:29:26.551725 aegis-tools-2.6.4/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3071 2023-09-30 03:49:20.000000 aegis-tools-2.6.4/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.6.4/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.6.4/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.6.4/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3377 2023-08-14 03:31:20.000000 aegis-tools-2.6.4/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2238 2023-09-30 03:49:39.000000 aegis-tools-2.6.4/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.6.4/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1857 2023-09-30 03:52:25.000000 aegis-tools-2.6.4/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.6.4/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.6.4/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.6.4/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.6.4/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.6.4/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.6.4/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    78528 2024-04-30 00:13:28.000000 aegis-tools-2.6.4/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-05-15 02:29:26.555724 aegis-tools-2.6.4/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-05-15 02:29:26.000000 aegis-tools-2.6.4/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2024-05-15 02:29:26.000000 aegis-tools-2.6.4/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2024-05-15 02:29:26.000000 aegis-tools-2.6.4/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2024-05-15 02:29:26.000000 aegis-tools-2.6.4/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2024-05-15 02:29:26.000000 aegis-tools-2.6.4/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2024-05-15 02:29:26.000000 aegis-tools-2.6.4/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2024-05-15 02:29:26.555724 aegis-tools-2.6.4/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1716 2023-09-26 15:24:50.000000 aegis-tools-2.6.4/setup.py
```

### Comparing `aegis-tools-2.6.3/LICENSE` & `aegis-tools-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/PKG-INFO` & `aegis-tools-2.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.6.3
+Version: 2.6.4
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.6.3/README.md` & `aegis-tools-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/aegis_.py` & `aegis-tools-2.6.4/aegis/aegis_.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/build.py` & `aegis-tools-2.6.4/aegis/build.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/config.py` & `aegis-tools-2.6.4/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/database.py` & `aegis-tools-2.6.4/aegis/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -555,15 +555,15 @@
             cls.logw("SCAN", cls.scan_id(where_col, row_id), row_id)
             logging.warning("")
             cls.logw("ITEMS", items, row_id)
         return items
 
     @classmethod
     def get_id(cls, column_id_val, member_id=None, dbconn=None):
-        if not column_id_val:
+        if not aegis.stdlib.validate_int(column_id_val):
             return None
         sql = 'SELECT * FROM %s WHERE %s=%%s'
         args = [int(column_id_val)]
         if member_id:
             sql = sql + ' AND member_id=%%s'
             args.append(int(member_id))
         sql = sql % (cls._table_name(), cls.id_column)
@@ -644,7 +644,27 @@
         args += args2
         where_clause = ' AND '.join(['%s=%s' % (key, value) for key, value in zip(keys, values)])
         # SQL statement
         sql = 'UPDATE %s SET %s WHERE %s' % (db_table, set_clause, where_clause)
         #aegis.stdlib.logw(sql, "SQL")
         #aegis.stdlib.logw(args, "ARGS")
         return dbconn.execute_rowcount(sql, *args)
+
+    @classmethod
+    def set_row(cls, data, dbconn):
+        # INSERT or UPDATE
+        data_row = cls.get_id(data[cls.id_column])
+        if data_row:
+            # compare everything in **data to data_row and don't update if there's no update
+            cols = {}
+            where = {cls.id_column: data_row[cls.id_column]}
+            for key, value in data.items():
+                if key in data_row and data_row[key] != value:
+                    cols[key] = value
+            if cols:
+                return cls.update_columns(cols, where, dbconn=dbconn)
+            else:
+                # 0 rows updated when no columns to update
+                return 0
+        else:
+            row_id = cls.insert_columns(**data, dbconn=dbconn)
+            return 1
```

### Comparing `aegis-tools-2.6.3/aegis/hydra.py` & `aegis-tools-2.6.4/aegis/hydra.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/mailer.py` & `aegis-tools-2.6.4/aegis/mailer.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/model.py` & `aegis-tools-2.6.4/aegis/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #-*- coding: utf-8 -*-
 #
-# Core common Data Model that will applies to a lot of applications
+# Core common Data Model that will apply to many applications
 
 
 # Python Imports
 import datetime
 import hashlib
 import json
 import logging
@@ -540,15 +540,15 @@
             sql += ' RETURNING pageview_id'
         return db().execute(sql, user_id, member_id, url_path, url_query, url_tx, request_name)
 
 
 class HydraType(aegis.database.Row):
     table_name = 'hydra_type'
     id_column = 'hydra_type_id'
-    data_columns = ('hydra_type_name', 'hydra_type_desc', 'priority_ndx', 'next_run_sql', 'claimed_dttm', 'run_host', 'run_env')
+    data_columns = ('hydra_type_id', 'hydra_type_name', 'hydra_type_desc', 'priority_ndx', 'next_run_sql', 'claimed_dttm', 'run_host', 'run_env')
 
     @classmethod
     def get_name(cls, hydra_type_name, dbconn=None):
         dbconn = dbconn if dbconn else db()
         sql = "SELECT * FROM hydra_type WHERE hydra_type_name=%s"
         return dbconn.get(sql, hydra_type_name, cls=cls)
 
@@ -941,15 +941,15 @@
     @classmethod
     def get_cache(cls, cache_key):
         # It's important to make sure this only does SELECT. It can't UPDATE or DELETE to maintain the cache or can be surprising in real usage.
         cache_obj = cls.get_key(cache_key)
         if not cache_obj:
             return None
         if cache_obj['cache_expiry'] <= datetime.datetime.utcnow():
-            return False
+            return None
         if type(cache_obj['cache_json']) is str:
             return json.loads(cache_obj['cache_json'])
         else:
             return cache_obj['cache_json']
 
     @classmethod
     def set_cache(cls, cache_key, cache_json_str, duration_s):
```

### Comparing `aegis-tools-2.6.3/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.6.4/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.6.4/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/sql/build-mysql.sql` & `aegis-tools-2.6.4/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/sql/build-pgsql.sql` & `aegis-tools-2.6.4/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.6.4/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/sql/google_signin.sql` & `aegis-tools-2.6.4/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.6.4/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.6.4/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/sql/member_auth.sql` & `aegis-tools-2.6.4/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.6.4/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/sql/reports.sql` & `aegis-tools-2.6.4/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/stdlib.py` & `aegis-tools-2.6.4/aegis/stdlib.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/templates/build.html` & `aegis-tools-2.6.4/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/templates/build_confirm.html` & `aegis-tools-2.6.4/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/templates/build_form.html` & `aegis-tools-2.6.4/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/templates/build_view.html` & `aegis-tools-2.6.4/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/templates/frame.html` & `aegis-tools-2.6.4/aegis/templates/frame.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/templates/hydra.html` & `aegis-tools-2.6.4/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/templates/hydra_form.html` & `aegis-tools-2.6.4/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/templates/hydra_queue.html` & `aegis-tools-2.6.4/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/templates/report.html` & `aegis-tools-2.6.4/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/templates/report_form.html` & `aegis-tools-2.6.4/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/templates/reports.html` & `aegis-tools-2.6.4/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/templates/w3.css` & `aegis-tools-2.6.4/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/threadpool.py` & `aegis-tools-2.6.4/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis/webapp.py` & `aegis-tools-2.6.4/aegis/webapp.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.6.4/aegis_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.6.3
+Version: 2.6.4
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.6.3/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.6.4/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.6.3/setup.py` & `aegis-tools-2.6.4/setup.py`

 * *Files identical despite different names*

