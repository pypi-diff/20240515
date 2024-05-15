# Comparing `tmp/yplib-5.7.4.tar.gz` & `tmp/yplib-5.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yplib-5.7.4.tar", last modified: Tue May 14 10:04:45 2024, max compression
+gzip compressed data, was "yplib-5.7.5.tar", last modified: Wed May 15 02:29:40 2024, max compression
```

## Comparing `yplib-5.7.4.tar` & `yplib-5.7.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 10:04:45.331562 yplib-5.7.4/
--rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.7.4/LICENSE
--rw-rw-rw-   0        0        0      355 2024-05-14 10:04:45.330551 yplib-5.7.4/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.7.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 10:04:45.331562 yplib-5.7.4/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-05-14 10:04:30.000000 yplib-5.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 10:04:45.322703 yplib-5.7.4/yplib/
--rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.7.4/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.7.4/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.7.4/yplib/chart_html.py
--rw-rw-rw-   0        0        0    12335 2024-05-14 10:02:00.000000 yplib-5.7.4/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.7.4/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.7.4/yplib/http_util.py
--rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.7.4/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.7.4/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.7.4/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.7.4/yplib/markdown.py
--rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.7.4/yplib/multi_thread.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.7.4/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-05-14 10:04:45.329551 yplib-5.7.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      355 2024-05-14 10:04:44.000000 yplib-5.7.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-14 10:04:44.000000 yplib-5.7.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 10:04:44.000000 yplib-5.7.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-14 10:04:44.000000 yplib-5.7.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 02:29:40.514764 yplib-5.7.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.7.5/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-15 02:29:40.514764 yplib-5.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.7.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 02:29:40.514764 yplib-5.7.5/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-05-15 02:29:20.000000 yplib-5.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 02:29:40.499135 yplib-5.7.5/yplib/
+-rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.7.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.7.5/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.7.5/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    12764 2024-05-15 02:28:58.000000 yplib-5.7.5/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.7.5/yplib/file.py
+-rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.7.5/yplib/http_util.py
+-rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.7.5/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.7.5/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.7.5/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.7.5/yplib/markdown.py
+-rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.7.5/yplib/multi_thread.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.7.5/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-05-15 02:29:40.499135 yplib-5.7.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-15 02:29:40.000000 yplib-5.7.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-15 02:29:40.000000 yplib-5.7.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 02:29:40.000000 yplib-5.7.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 02:29:40.000000 yplib-5.7.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.7.4/LICENSE` & `yplib-5.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-5.7.4/setup.py` & `yplib-5.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.7.4",
+    version="5.7.5",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.7.4/yplib/__init__.py` & `yplib-5.7.5/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.4/yplib/chart.py` & `yplib-5.7.5/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.4/yplib/chart_html.py` & `yplib-5.7.5/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.4/yplib/db.py` & `yplib-5.7.5/yplib/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,33 +24,38 @@
     port = port if port is not None else config_db['port'] if 'port' in config_db else 3306
     charset = charset if charset is not None else config_db['charset'] if 'charset' in config_db else 'utf8mb4'
     return get_connect(database=database, user=user, password=password, charset=charset, port=port, host=host)
 
 
 # 执行 sql 语句, 并且提交, 默认值提交的了
 def exec_sql(sql='', db_conn=None, db_config='stock_db', commit=True, is_log=False, database=None):
-    db_conn = db_conn if db_conn is not None else get_connect_from_config(db_config, database=database)
-    if sql is None or sql == '':
-        if is_log:
-            to_log_file("db_conn is None or sql is None or sql == '', so return")
-        return
-    db_cursor = db_conn.cursor()
-    if isinstance(sql, list) or isinstance(sql, set):
-        for s in sql:
+    db_cursor = None
+    try:
+        db_conn = db_conn if db_conn is not None else get_connect_from_config(db_config, database=database)
+        if sql is None or sql == '':
             if is_log:
-                to_log_file(s)
-            db_cursor.execute(s)
-    else:
-        if is_log:
-            to_log_file(sql)
-        db_cursor.execute(str(sql))
-    if commit:
-        db_conn.commit()
-    db_cursor.close()
-    db_conn.close()
+                to_log_file("db_conn is None or sql is None or sql == '', so return")
+            return
+        db_cursor = db_conn.cursor()
+        if isinstance(sql, list) or isinstance(sql, set):
+            for s in sql:
+                if is_log:
+                    to_log_file(s)
+                db_cursor.execute(s)
+        else:
+            if is_log:
+                to_log_file(sql)
+            db_cursor.execute(str(sql))
+        if commit:
+            db_conn.commit()
+    finally:
+        if db_cursor is not None:
+            db_cursor.close()
+        if db_conn is not None:
+            db_conn.close()
 
 
 def get_doris_conn(db_config='doris'):
     config_db = get_config_data(db_config)
     my_uri = config_db['uri']
     my_db_kwargs = {
         adbc_driver_manager.DatabaseOptions.USERNAME.value: config_db['username'],
@@ -96,24 +101,32 @@
 # 执行 sql 语句, 不提交
 def exec_sql_un_commit(sql='', db_conn=None, database=None):
     exec_sql(sql=sql, db_conn=db_conn, commit=False, database=database)
 
 
 # 执行 sql 获得 数据
 def get_data_from_sql(sql='', db_conn=None, db_config='stock_db', is_log=False, database=None):
-    db_conn = db_conn if db_conn is not None else get_connect_from_config(db_config, database=database)
-    if sql is None or sql == '':
+    db_cursor = None
+    try:
+        db_conn = db_conn if db_conn is not None else get_connect_from_config(db_config, database=database)
+        if sql is None or sql == '':
+            if is_log:
+                to_log_file("db_conn is None or sql is None or sql == '', so return")
+            return
+        db_cursor = db_conn.cursor()
         if is_log:
-            to_log_file("db_conn is None or sql is None or sql == '', so return")
-        return
-    db_cursor = db_conn.cursor()
-    if is_log:
-        to_log_file(sql)
-    db_cursor.execute(str(sql))
-    return db_cursor.fetchall()
+            to_log_file(sql)
+        db_cursor.execute(str(sql))
+        data = db_cursor.fetchall()
+    finally:
+        if db_cursor is not None:
+            db_cursor.close()
+        if db_conn is not None:
+            db_conn.close()
+    return data
 
 
 # table_name, column_name_list, type_list, comment_list, column_name_type_comment_list, info_list
 def get_table_sql(file_path):
     table_list = []
     r_list = []
     # 普通文件的解析
```

### Comparing `yplib-5.7.4/yplib/file.py` & `yplib-5.7.5/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.4/yplib/http_util.py` & `yplib-5.7.5/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.4/yplib/index.py` & `yplib-5.7.5/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.4/yplib/mail.py` & `yplib-5.7.5/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.4/yplib/mail_html.py` & `yplib-5.7.5/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.4/yplib/markdown.py` & `yplib-5.7.5/yplib/markdown.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.4/yplib/multi_thread.py` & `yplib-5.7.5/yplib/multi_thread.py`

 * *Files identical despite different names*

