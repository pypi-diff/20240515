# Comparing `tmp/yplib-5.7.3.tar.gz` & `tmp/yplib-5.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yplib-5.7.3.tar", last modified: Wed May  8 07:04:49 2024, max compression
+gzip compressed data, was "yplib-5.7.4.tar", last modified: Tue May 14 10:04:45 2024, max compression
```

## Comparing `yplib-5.7.3.tar` & `yplib-5.7.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 07:04:49.258207 yplib-5.7.3/
--rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.7.3/LICENSE
--rw-rw-rw-   0        0        0      355 2024-05-08 07:04:49.258207 yplib-5.7.3/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.7.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 07:04:49.258207 yplib-5.7.3/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-05-08 07:04:37.000000 yplib-5.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:04:49.258207 yplib-5.7.3/yplib/
--rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.7.3/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.7.3/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.7.3/yplib/chart_html.py
--rw-rw-rw-   0        0        0    12173 2024-05-08 07:04:26.000000 yplib-5.7.3/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.7.3/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.7.3/yplib/http_util.py
--rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.7.3/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.7.3/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.7.3/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.7.3/yplib/markdown.py
--rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.7.3/yplib/multi_thread.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.7.3/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:04:49.258207 yplib-5.7.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      355 2024-05-08 07:04:49.000000 yplib-5.7.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-08 07:04:49.000000 yplib-5.7.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 07:04:49.000000 yplib-5.7.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-08 07:04:49.000000 yplib-5.7.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 10:04:45.331562 yplib-5.7.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.7.4/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-14 10:04:45.330551 yplib-5.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.7.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 10:04:45.331562 yplib-5.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-05-14 10:04:30.000000 yplib-5.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:04:45.322703 yplib-5.7.4/yplib/
+-rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.7.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.7.4/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.7.4/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    12335 2024-05-14 10:02:00.000000 yplib-5.7.4/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.7.4/yplib/file.py
+-rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.7.4/yplib/http_util.py
+-rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.7.4/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.7.4/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.7.4/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.7.4/yplib/markdown.py
+-rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.7.4/yplib/multi_thread.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.7.4/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:04:45.329551 yplib-5.7.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-14 10:04:44.000000 yplib-5.7.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-14 10:04:44.000000 yplib-5.7.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 10:04:44.000000 yplib-5.7.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-14 10:04:44.000000 yplib-5.7.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.7.3/LICENSE` & `yplib-5.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-5.7.3/setup.py` & `yplib-5.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.7.3",
+    version="5.7.4",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.7.3/yplib/__init__.py` & `yplib-5.7.4/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.3/yplib/chart.py` & `yplib-5.7.4/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.3/yplib/chart_html.py` & `yplib-5.7.4/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.3/yplib/db.py` & `yplib-5.7.4/yplib/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,22 +67,28 @@
     # cursor = conn.cursor()
     # cursor.execute(sql)
     # cursor.close()
     # conn.close()
 
 
 def get_data_from_doris(sql='', db_config='doris'):
-    conn = get_doris_conn(db_config)
-    cursor = conn.cursor()
-    cursor.execute(sql)
-    arrow_data = cursor.fetchallarrow()
-    dataframe = arrow_data.to_pandas()
-    json_data = dataframe.to_json(orient='records')
-    cursor.close()
-    conn.close()
+    conn = None
+    cursor = None
+    try:
+        conn = get_doris_conn(db_config)
+        cursor = conn.cursor()
+        cursor.execute(sql)
+        arrow_data = cursor.fetchallarrow()
+        dataframe = arrow_data.to_pandas()
+        json_data = dataframe.to_json(orient='records')
+    finally:
+        if cursor is not None:
+            cursor.close()
+        if conn is not None:
+            conn.close()
     return json.loads(json_data)
 
 
 def get_data_line_one_from_doris(sql='', db_config='doris'):
     data_list = get_data_from_doris(sql, db_config=db_config)
     return list(data_list[0].values())
```

### Comparing `yplib-5.7.3/yplib/file.py` & `yplib-5.7.4/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.3/yplib/http_util.py` & `yplib-5.7.4/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.3/yplib/index.py` & `yplib-5.7.4/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.3/yplib/mail.py` & `yplib-5.7.4/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.3/yplib/mail_html.py` & `yplib-5.7.4/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.3/yplib/markdown.py` & `yplib-5.7.4/yplib/markdown.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.3/yplib/multi_thread.py` & `yplib-5.7.4/yplib/multi_thread.py`

 * *Files identical despite different names*

