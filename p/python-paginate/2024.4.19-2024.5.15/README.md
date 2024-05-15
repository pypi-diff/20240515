# Comparing `tmp/python_paginate-2024.4.19.tar.gz` & `tmp/python_paginate-2024.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_paginate-2024.4.19.tar", last modified: Fri Apr 19 08:19:46 2024, max compression
+gzip compressed data, was "python_paginate-2024.5.15.tar", last modified: Wed May 15 07:51:59 2024, max compression
```

## Comparing `python_paginate-2024.4.19.tar` & `python_paginate-2024.5.15.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:19:46.838268 python_paginate-2024.4.19/
--rw-rw-rw-   0        0        0     1449 2022-03-22 00:47:44.000000 python_paginate-2024.4.19/LICENSE
--rw-rw-rw-   0        0        0     1023 2024-04-19 08:19:46.838268 python_paginate-2024.4.19/PKG-INFO
--rw-rw-rw-   0        0        0     1330 2023-10-12 01:37:48.000000 python_paginate-2024.4.19/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 08:19:46.771499 python_paginate-2024.4.19/python_paginate/
--rw-rw-rw-   0        0        0      322 2024-04-19 08:13:52.000000 python_paginate-2024.4.19/python_paginate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:19:46.813944 python_paginate-2024.4.19/python_paginate/css/
--rw-rw-rw-   0        0        0        0 2022-03-17 06:48:01.000000 python_paginate-2024.4.19/python_paginate/css/__init__.py
--rw-rw-rw-   0        0        0     2431 2022-03-22 00:47:44.000000 python_paginate-2024.4.19/python_paginate/css/basecss.py
--rw-rw-rw-   0        0        0     2502 2022-03-22 00:47:44.000000 python_paginate-2024.4.19/python_paginate/css/bootstrap.py
--rw-rw-rw-   0        0        0     1195 2022-03-22 00:47:44.000000 python_paginate-2024.4.19/python_paginate/css/foundation.py
--rw-rw-rw-   0        0        0      820 2022-03-22 00:47:44.000000 python_paginate-2024.4.19/python_paginate/css/ink.py
--rw-rw-rw-   0        0        0     1105 2022-03-22 00:47:44.000000 python_paginate-2024.4.19/python_paginate/css/metro.py
--rw-rw-rw-   0        0        0      854 2022-03-22 00:47:44.000000 python_paginate-2024.4.19/python_paginate/css/semantic.py
--rw-rw-rw-   0        0        0      876 2022-03-22 00:47:44.000000 python_paginate-2024.4.19/python_paginate/css/uikit.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:19:46.828215 python_paginate-2024.4.19/python_paginate/web/
--rw-rw-rw-   0        0        0        0 2022-03-17 06:48:01.000000 python_paginate-2024.4.19/python_paginate/web/__init__.py
--rw-rw-rw-   0        0        0    12589 2024-04-19 08:13:52.000000 python_paginate-2024.4.19/python_paginate/web/base_paginate.py
--rw-rw-rw-   0        0        0     2183 2024-04-19 08:13:52.000000 python_paginate-2024.4.19/python_paginate/web/flask_paginate.py
--rw-rw-rw-   0        0        0     2443 2024-03-28 03:04:03.000000 python_paginate-2024.4.19/python_paginate/web/sanic_paginate.py
--rw-rw-rw-   0        0        0      879 2022-03-22 00:47:44.000000 python_paginate-2024.4.19/python_paginate/web/tornado_paginate.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:19:46.835275 python_paginate-2024.4.19/python_paginate.egg-info/
--rw-rw-rw-   0        0        0     1023 2024-04-19 08:19:46.000000 python_paginate-2024.4.19/python_paginate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      728 2024-04-19 08:19:46.000000 python_paginate-2024.4.19/python_paginate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:19:46.000000 python_paginate-2024.4.19/python_paginate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-12 01:38:21.000000 python_paginate-2024.4.19/python_paginate.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2024-04-19 08:19:46.000000 python_paginate-2024.4.19/python_paginate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-19 08:19:46.000000 python_paginate-2024.4.19/python_paginate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      118 2024-04-19 08:19:46.840364 python_paginate-2024.4.19/setup.cfg
--rw-rw-rw-   0        0        0     1558 2023-10-12 01:37:48.000000 python_paginate-2024.4.19/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:51:59.865622 python_paginate-2024.5.15/
+-rw-rw-rw-   0        0        0     1449 2022-03-22 00:47:44.000000 python_paginate-2024.5.15/LICENSE
+-rw-rw-rw-   0        0        0     1023 2024-05-15 07:51:59.864622 python_paginate-2024.5.15/PKG-INFO
+-rw-rw-rw-   0        0        0     1330 2023-10-12 01:37:48.000000 python_paginate-2024.5.15/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 07:51:59.800431 python_paginate-2024.5.15/python_paginate/
+-rw-rw-rw-   0        0        0      322 2024-05-15 07:27:23.000000 python_paginate-2024.5.15/python_paginate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:51:59.843228 python_paginate-2024.5.15/python_paginate/css/
+-rw-rw-rw-   0        0        0        0 2022-03-17 06:48:01.000000 python_paginate-2024.5.15/python_paginate/css/__init__.py
+-rw-rw-rw-   0        0        0     2431 2022-03-22 00:47:44.000000 python_paginate-2024.5.15/python_paginate/css/basecss.py
+-rw-rw-rw-   0        0        0     2502 2022-03-22 00:47:44.000000 python_paginate-2024.5.15/python_paginate/css/bootstrap.py
+-rw-rw-rw-   0        0        0     1195 2022-03-22 00:47:44.000000 python_paginate-2024.5.15/python_paginate/css/foundation.py
+-rw-rw-rw-   0        0        0      820 2022-03-22 00:47:44.000000 python_paginate-2024.5.15/python_paginate/css/ink.py
+-rw-rw-rw-   0        0        0     1105 2022-03-22 00:47:44.000000 python_paginate-2024.5.15/python_paginate/css/metro.py
+-rw-rw-rw-   0        0        0      854 2022-03-22 00:47:44.000000 python_paginate-2024.5.15/python_paginate/css/semantic.py
+-rw-rw-rw-   0        0        0      876 2022-03-22 00:47:44.000000 python_paginate-2024.5.15/python_paginate/css/uikit.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:51:59.857258 python_paginate-2024.5.15/python_paginate/web/
+-rw-rw-rw-   0        0        0        0 2022-03-17 06:48:01.000000 python_paginate-2024.5.15/python_paginate/web/__init__.py
+-rw-rw-rw-   0        0        0    12472 2024-05-15 07:27:23.000000 python_paginate-2024.5.15/python_paginate/web/base_paginate.py
+-rw-rw-rw-   0        0        0     2186 2024-05-15 07:27:23.000000 python_paginate-2024.5.15/python_paginate/web/flask_paginate.py
+-rw-rw-rw-   0        0        0     2443 2024-03-28 03:04:03.000000 python_paginate-2024.5.15/python_paginate/web/sanic_paginate.py
+-rw-rw-rw-   0        0        0      879 2022-03-22 00:47:44.000000 python_paginate-2024.5.15/python_paginate/web/tornado_paginate.py
+drwxrwxrwx   0        0        0        0 2024-05-15 07:51:59.861621 python_paginate-2024.5.15/python_paginate.egg-info/
+-rw-rw-rw-   0        0        0     1023 2024-05-15 07:51:59.000000 python_paginate-2024.5.15/python_paginate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      728 2024-05-15 07:51:59.000000 python_paginate-2024.5.15/python_paginate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 07:51:59.000000 python_paginate-2024.5.15/python_paginate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-10-12 01:38:21.000000 python_paginate-2024.5.15/python_paginate.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2024-05-15 07:51:59.000000 python_paginate-2024.5.15/python_paginate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-15 07:51:59.000000 python_paginate-2024.5.15/python_paginate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      118 2024-05-15 07:51:59.867129 python_paginate-2024.5.15/setup.cfg
+-rw-rw-rw-   0        0        0     1558 2023-10-12 01:37:48.000000 python_paginate-2024.5.15/setup.py
```

### Comparing `python_paginate-2024.4.19/LICENSE` & `python_paginate-2024.5.15/LICENSE`

 * *Files identical despite different names*

### Comparing `python_paginate-2024.4.19/PKG-INFO` & `python_paginate-2024.5.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-paginate
-Version: 2024.4.19
+Version: 2024.5.15
 Summary: Simple paginate support for python web frameworks
 Home-page: https://github.com/lixxu/python-paginate
 Author: Lix Xu
 Author-email: xuzenglin@gmail.com
 License: BSD-3-Clause
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `python_paginate-2024.4.19/README.md` & `python_paginate-2024.5.15/README.md`

 * *Files identical despite different names*

### Comparing `python_paginate-2024.4.19/python_paginate/css/basecss.py` & `python_paginate-2024.5.15/python_paginate/css/basecss.py`

 * *Files identical despite different names*

### Comparing `python_paginate-2024.4.19/python_paginate/css/bootstrap.py` & `python_paginate-2024.5.15/python_paginate/css/bootstrap.py`

 * *Files identical despite different names*

### Comparing `python_paginate-2024.4.19/python_paginate/css/foundation.py` & `python_paginate-2024.5.15/python_paginate/css/foundation.py`

 * *Files identical despite different names*

### Comparing `python_paginate-2024.4.19/python_paginate/css/ink.py` & `python_paginate-2024.5.15/python_paginate/css/ink.py`

 * *Files identical despite different names*

### Comparing `python_paginate-2024.4.19/python_paginate/css/metro.py` & `python_paginate-2024.5.15/python_paginate/css/metro.py`

 * *Files identical despite different names*

### Comparing `python_paginate-2024.4.19/python_paginate/css/semantic.py` & `python_paginate-2024.5.15/python_paginate/css/semantic.py`

 * *Files identical despite different names*

### Comparing `python_paginate-2024.4.19/python_paginate/css/uikit.py` & `python_paginate-2024.5.15/python_paginate/css/uikit.py`

 * *Files identical despite different names*

### Comparing `python_paginate-2024.4.19/python_paginate/web/base_paginate.py` & `python_paginate-2024.5.15/python_paginate/web/base_paginate.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     _hide_page_one = True
     _inner_window = 2
     _outer_window = 1
     _format_total = False
     _format_number = False
     _show_prev = True
     _show_next = True
-    _include_first_page_numberinclude_first_page_number = False
+    _include_first_page_number = False
     _record_name = "records"
     _href = None
     _search = False
     _show_single_page = False
     _display_msg = "displaying <b>{start} - {end}</b> {record_name} in \
     total <b>{total}</b>"
     _search_msg = "found <b>{total}</b> {record_name} \
@@ -85,15 +85,15 @@
 
         **size**: font size of page links
 
         **show_prev**: show previous page or not
 
         **show_next**: show next page or not
 
-        **include_first_page_numberinclude_first_page_number**: show page number for first page or not
+        **include_first_page_number**: show page number for first page or not
 
         **others**: other parameters startswith css_ will be accepted by \
         css_framework
         """
         self.page_name = kwargs.get("page_name", self._page_name)
         self.per_page_name = kwargs.get("per_page_name", self._per_page_name)
         self.page = int(kwargs.get(self.page_name, 1))
@@ -117,17 +117,17 @@
         self.info_end = kwargs.get("info_end", self._info_end)
 
         self.show_prev = kwargs.get("show_prev", self._show_prev)
         self.show_next = kwargs.get("show_next", self._show_next)
         self.record_name = kwargs.get("record_name", self._record_name)
         self.href = kwargs.get("href", self._href)
         self.show_single_page = kwargs.get("show_single_page", self._show_single_page)
-        self.include_first_page_numberinclude_first_page_number = kwargs.get(
-            "include_first_page_numberinclude_first_page_number",
-            self._include_first_page_numberinclude_first_page_number,
+        self.include_first_page_number = kwargs.get(
+            "include_first_page_number",
+            self._include_first_page_number,
         )
         self.css = self.get_css(kwargs.pop("css_framework", None), **kwargs)
         self.url = kwargs.get("url") or self.get_url()
         self.init_values()
 
     def init_values(self):
         self._cached = {}
@@ -243,16 +243,17 @@
     @property
     def single_link(self):
         """You can do markup here, such as flask has Markup(links_text)."""
         return self.raw_single_link
 
     @property
     def raw_links(self):
-        if "links" in self._cached:
-            return self._cached["links"]
+        links = self._cached.get("links")
+        if links:
+            return links
 
         if self.total_pages <= 1:
             if self.show_single_page:
                 self._cached["links"] = self.raw_single_link
             else:
                 self._cached["links"] = ""
```

### Comparing `python_paginate-2024.4.19/python_paginate/web/flask_paginate.py` & `python_paginate-2024.5.15/python_paginate/web/flask_paginate.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def get_href(self, page=1):
         if self.href:
             url = self.href.format(page or 1)
         else:
             url_args = self.url_args.copy()
             url_args[self.page_name] = page
             self.url_args[self.page_name] = page
-            if page == 1 and not self.show_first_page_number:
+            if page == 1 and not self.include_first_page_number:
                 url_args[self.page_name] = None
 
             url = url_for(self.endpoint, **url_args)
 
         # Need to return a unicode object
         return url.decode("utf8") if PY2 else url
```

### Comparing `python_paginate-2024.4.19/python_paginate/web/sanic_paginate.py` & `python_paginate-2024.5.15/python_paginate/web/sanic_paginate.py`

 * *Files identical despite different names*

### Comparing `python_paginate-2024.4.19/python_paginate/web/tornado_paginate.py` & `python_paginate-2024.5.15/python_paginate/web/tornado_paginate.py`

 * *Files identical despite different names*

### Comparing `python_paginate-2024.4.19/python_paginate.egg-info/PKG-INFO` & `python_paginate-2024.5.15/python_paginate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-paginate
-Version: 2024.4.19
+Version: 2024.5.15
 Summary: Simple paginate support for python web frameworks
 Home-page: https://github.com/lixxu/python-paginate
 Author: Lix Xu
 Author-email: xuzenglin@gmail.com
 License: BSD-3-Clause
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `python_paginate-2024.4.19/python_paginate.egg-info/SOURCES.txt` & `python_paginate-2024.5.15/python_paginate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_paginate-2024.4.19/setup.py` & `python_paginate-2024.5.15/setup.py`

 * *Files identical despite different names*

