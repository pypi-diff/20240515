# Comparing `tmp/yplib-5.7.5.tar.gz` & `tmp/yplib-5.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yplib-5.7.5.tar", last modified: Wed May 15 02:29:40 2024, max compression
+gzip compressed data, was "yplib-5.7.6.tar", last modified: Wed May 15 06:50:06 2024, max compression
```

## Comparing `yplib-5.7.5.tar` & `yplib-5.7.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 02:29:40.514764 yplib-5.7.5/
--rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.7.5/LICENSE
--rw-rw-rw-   0        0        0      355 2024-05-15 02:29:40.514764 yplib-5.7.5/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.7.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 02:29:40.514764 yplib-5.7.5/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-05-15 02:29:20.000000 yplib-5.7.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 02:29:40.499135 yplib-5.7.5/yplib/
--rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.7.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.7.5/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.7.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0    12764 2024-05-15 02:28:58.000000 yplib-5.7.5/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.7.5/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.7.5/yplib/http_util.py
--rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.7.5/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.7.5/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.7.5/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.7.5/yplib/markdown.py
--rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.7.5/yplib/multi_thread.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.7.5/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-05-15 02:29:40.499135 yplib-5.7.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      355 2024-05-15 02:29:40.000000 yplib-5.7.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-15 02:29:40.000000 yplib-5.7.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 02:29:40.000000 yplib-5.7.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-15 02:29:40.000000 yplib-5.7.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 06:50:06.104162 yplib-5.7.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.7.6/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-15 06:50:06.104162 yplib-5.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.7.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 06:50:06.104162 yplib-5.7.6/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-05-15 06:49:47.000000 yplib-5.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:50:06.104162 yplib-5.7.6/yplib/
+-rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.7.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.7.6/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.7.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    12806 2024-05-15 06:49:06.000000 yplib-5.7.6/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.7.6/yplib/file.py
+-rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.7.6/yplib/http_util.py
+-rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.7.6/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.7.6/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.7.6/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.7.6/yplib/markdown.py
+-rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.7.6/yplib/multi_thread.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.7.6/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:50:06.104162 yplib-5.7.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-15 06:50:06.000000 yplib-5.7.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-15 06:50:06.000000 yplib-5.7.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 06:50:06.000000 yplib-5.7.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 06:50:06.000000 yplib-5.7.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.7.5/LICENSE` & `yplib-5.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-5.7.5/setup.py` & `yplib-5.7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.7.5",
+    version="5.7.6",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.7.5/yplib/__init__.py` & `yplib-5.7.6/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.5/yplib/chart.py` & `yplib-5.7.6/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.5/yplib/chart_html.py` & `yplib-5.7.6/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.5/yplib/db.py` & `yplib-5.7.6/yplib/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,29 +71,32 @@
     # conn = get_doris_conn(db_config)
     # cursor = conn.cursor()
     # cursor.execute(sql)
     # cursor.close()
     # conn.close()
 
 
+conn_doris = None
+
+
 def get_data_from_doris(sql='', db_config='doris'):
-    conn = None
-    cursor = None
-    try:
-        conn = get_doris_conn(db_config)
-        cursor = conn.cursor()
-        cursor.execute(sql)
-        arrow_data = cursor.fetchallarrow()
-        dataframe = arrow_data.to_pandas()
-        json_data = dataframe.to_json(orient='records')
-    finally:
-        if cursor is not None:
-            cursor.close()
-        if conn is not None:
-            conn.close()
+    global conn_doris
+    # try:
+    if conn_doris is None:
+        conn_doris = get_doris_conn(db_config)
+    cursor = conn_doris.cursor()
+    cursor.execute(sql)
+    arrow_data = cursor.fetchallarrow()
+    dataframe = arrow_data.to_pandas()
+    json_data = dataframe.to_json(orient='records')
+    # finally:
+    #     if cursor is not None:
+    #         cursor.close()
+    #     if conn is not None:
+    #         conn.close()
     return json.loads(json_data)
 
 
 def get_data_line_one_from_doris(sql='', db_config='doris'):
     data_list = get_data_from_doris(sql, db_config=db_config)
     return list(data_list[0].values())
```

### Comparing `yplib-5.7.5/yplib/file.py` & `yplib-5.7.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.5/yplib/http_util.py` & `yplib-5.7.6/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.5/yplib/index.py` & `yplib-5.7.6/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.5/yplib/mail.py` & `yplib-5.7.6/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.5/yplib/mail_html.py` & `yplib-5.7.6/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.5/yplib/markdown.py` & `yplib-5.7.6/yplib/markdown.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.5/yplib/multi_thread.py` & `yplib-5.7.6/yplib/multi_thread.py`

 * *Files identical despite different names*

