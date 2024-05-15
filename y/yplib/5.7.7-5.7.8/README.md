# Comparing `tmp/yplib-5.7.7.tar.gz` & `tmp/yplib-5.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yplib-5.7.7.tar", last modified: Wed May 15 06:55:12 2024, max compression
+gzip compressed data, was "yplib-5.7.8.tar", last modified: Wed May 15 06:56:54 2024, max compression
```

## Comparing `yplib-5.7.7.tar` & `yplib-5.7.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 06:55:12.499112 yplib-5.7.7/
--rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.7.7/LICENSE
--rw-rw-rw-   0        0        0      355 2024-05-15 06:55:12.499112 yplib-5.7.7/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.7.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 06:55:12.499112 yplib-5.7.7/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-05-15 06:55:07.000000 yplib-5.7.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:55:12.499112 yplib-5.7.7/yplib/
--rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.7.7/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.7.7/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.7.7/yplib/chart_html.py
--rw-rw-rw-   0        0        0    12924 2024-05-15 06:55:04.000000 yplib-5.7.7/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.7.7/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.7.7/yplib/http_util.py
--rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.7.7/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.7.7/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.7.7/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.7.7/yplib/markdown.py
--rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.7.7/yplib/multi_thread.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.7.7/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:55:12.499112 yplib-5.7.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      355 2024-05-15 06:55:12.000000 yplib-5.7.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-15 06:55:12.000000 yplib-5.7.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 06:55:12.000000 yplib-5.7.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-15 06:55:12.000000 yplib-5.7.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 06:56:54.714008 yplib-5.7.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.7.8/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-15 06:56:54.698998 yplib-5.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.7.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 06:56:54.714008 yplib-5.7.8/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-05-15 06:56:39.000000 yplib-5.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:56:54.698998 yplib-5.7.8/yplib/
+-rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.7.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.7.8/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.7.8/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    12806 2024-05-15 06:56:33.000000 yplib-5.7.8/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.7.8/yplib/file.py
+-rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.7.8/yplib/http_util.py
+-rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.7.8/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.7.8/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.7.8/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.7.8/yplib/markdown.py
+-rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.7.8/yplib/multi_thread.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.7.8/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:56:54.698998 yplib-5.7.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-15 06:56:54.000000 yplib-5.7.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-15 06:56:54.000000 yplib-5.7.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 06:56:54.000000 yplib-5.7.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 06:56:54.000000 yplib-5.7.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.7.7/LICENSE` & `yplib-5.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-5.7.7/setup.py` & `yplib-5.7.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.7.7",
+    version="5.7.8",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.7.7/yplib/__init__.py` & `yplib-5.7.8/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.7/yplib/chart.py` & `yplib-5.7.8/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.7/yplib/chart_html.py` & `yplib-5.7.8/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.7/yplib/db.py` & `yplib-5.7.8/yplib/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,18 +78,15 @@
 conn_doris = None
 
 
 def get_data_from_doris(sql='', db_config='doris'):
     global conn_doris
     # try:
     if conn_doris is None:
-        print('conn_doris is None and get_doris_conn')
         conn_doris = get_doris_conn(db_config)
-    else:
-        print('conn_doris is not None and reuse')
     cursor = conn_doris.cursor()
     cursor.execute(sql)
     arrow_data = cursor.fetchallarrow()
     dataframe = arrow_data.to_pandas()
     json_data = dataframe.to_json(orient='records')
     # finally:
     #     if cursor is not None:
```

### Comparing `yplib-5.7.7/yplib/file.py` & `yplib-5.7.8/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.7/yplib/http_util.py` & `yplib-5.7.8/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.7/yplib/index.py` & `yplib-5.7.8/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.7/yplib/mail.py` & `yplib-5.7.8/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.7/yplib/mail_html.py` & `yplib-5.7.8/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.7/yplib/markdown.py` & `yplib-5.7.8/yplib/markdown.py`

 * *Files identical despite different names*

### Comparing `yplib-5.7.7/yplib/multi_thread.py` & `yplib-5.7.8/yplib/multi_thread.py`

 * *Files identical despite different names*

