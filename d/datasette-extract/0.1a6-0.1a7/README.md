# Comparing `tmp/datasette_extract-0.1a6.tar.gz` & `tmp/datasette_extract-0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_extract-0.1a6.tar", last modified: Thu Apr 25 19:06:30 2024, max compression
+gzip compressed data, was "datasette_extract-0.1a7.tar", last modified: Wed May 15 04:32:14 2024, max compression
```

## Comparing `datasette_extract-0.1a6.tar` & `datasette_extract-0.1a7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:06:30.742569 datasette_extract-0.1a6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-25 19:06:30.742569 datasette_extract-0.1a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:06:30.734569 datasette_extract-0.1a6/datasette_extract/
--rw-r--r--   0 runner    (1001) docker     (127)    16004 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/datasette_extract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:06:30.742569 datasette_extract-0.1a6/datasette_extract/static/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/datasette_extract/static/extract.css
--rw-r--r--   0 runner    (1001) docker     (127)  1352452 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/datasette_extract/static/heic2any-0.0.4.min.js
--rw-r--r--   0 runner    (1001) docker     (127)  1875780 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/datasette_extract/static/pdf.worker.mjs
--rw-r--r--   0 runner    (1001) docker     (127)   317819 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/datasette_extract/static/pdfjs-dist-4-0-379.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:06:30.742569 datasette_extract-0.1a6/datasette_extract/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/datasette_extract/templates/_extract_drop_handler.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/datasette_extract/templates/extract.html
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/datasette_extract/templates/extract_create_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/datasette_extract/templates/extract_progress.html
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/datasette_extract/templates/extract_to_table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:06:30.742569 datasette_extract-0.1a6/datasette_extract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-25 19:06:30.000000 datasette_extract-0.1a6/datasette_extract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-25 19:06:30.000000 datasette_extract-0.1a6/datasette_extract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:06:30.000000 datasette_extract-0.1a6/datasette_extract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 19:06:30.000000 datasette_extract-0.1a6/datasette_extract.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-25 19:06:30.000000 datasette_extract-0.1a6/datasette_extract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 19:06:30.000000 datasette_extract-0.1a6/datasette_extract.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:06:30.742569 datasette_extract-0.1a6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:06:30.742569 datasette_extract-0.1a6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-25 19:06:24.000000 datasette_extract-0.1a6/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:32:14.681072 datasette_extract-0.1a7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-15 04:32:14.681072 datasette_extract-0.1a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:32:14.673072 datasette_extract-0.1a7/datasette_extract/
+-rw-r--r--   0 runner    (1001) docker     (127)    15999 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/datasette_extract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:32:14.681072 datasette_extract-0.1a7/datasette_extract/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/datasette_extract/static/extract.css
+-rw-r--r--   0 runner    (1001) docker     (127)  1352452 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/datasette_extract/static/heic2any-0.0.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1875780 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/datasette_extract/static/pdf.worker.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)   317819 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/datasette_extract/static/pdfjs-dist-4-0-379.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:32:14.681072 datasette_extract-0.1a7/datasette_extract/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/datasette_extract/templates/_extract_drop_handler.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/datasette_extract/templates/extract.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/datasette_extract/templates/extract_create_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/datasette_extract/templates/extract_progress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/datasette_extract/templates/extract_to_table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:32:14.681072 datasette_extract-0.1a7/datasette_extract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-15 04:32:14.000000 datasette_extract-0.1a7/datasette_extract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-15 04:32:14.000000 datasette_extract-0.1a7/datasette_extract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 04:32:14.000000 datasette_extract-0.1a7/datasette_extract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 04:32:14.000000 datasette_extract-0.1a7/datasette_extract.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-15 04:32:14.000000 datasette_extract-0.1a7/datasette_extract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 04:32:14.000000 datasette_extract-0.1a7/datasette_extract.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:32:14.681072 datasette_extract-0.1a7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:32:14.681072 datasette_extract-0.1a7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-15 04:32:02.000000 datasette_extract-0.1a7/tests/test_web.py
```

### Comparing `datasette_extract-0.1a6/LICENSE` & `datasette_extract-0.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette_extract-0.1a6/PKG-INFO` & `datasette_extract-0.1a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-extract
-Version: 0.1a6
+Version: 0.1a7
 Summary: Import unstructured data (text and images) into structured tables
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-extract
 Project-URL: Changelog, https://github.com/datasette/datasette-extract/releases
 Project-URL: Issues, https://github.com/datasette/datasette-extract/issues
 Project-URL: CI, https://github.com/datasette/datasette-extract/actions
```

### Comparing `datasette_extract-0.1a6/README.md` & `datasette_extract-0.1a7/README.md`

 * *Files identical despite different names*

### Comparing `datasette_extract-0.1a6/datasette_extract/__init__.py` & `datasette_extract-0.1a7/datasette_extract/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
                 }
             )
         if content:
             messages.append({"role": "user", "content": content})
 
         async for chunk in await async_client.chat.completions.create(
             stream=True,
-            model="gpt-4-turbo",
+            model="gpt-4o",
             messages=messages,
             tools=[
                 {
                     "type": "function",
                     "function": {
                         "name": "extract_data",
                         "description": "Extract data matching this schema",
```

### Comparing `datasette_extract-0.1a6/datasette_extract/static/heic2any-0.0.4.min.js` & `datasette_extract-0.1a7/datasette_extract/static/heic2any-0.0.4.min.js`

 * *Files identical despite different names*

### Comparing `datasette_extract-0.1a6/datasette_extract/static/pdf.worker.mjs` & `datasette_extract-0.1a7/datasette_extract/static/pdf.worker.mjs`

 * *Files identical despite different names*

### Comparing `datasette_extract-0.1a6/datasette_extract/static/pdfjs-dist-4-0-379.js` & `datasette_extract-0.1a7/datasette_extract/static/pdfjs-dist-4-0-379.js`

 * *Files identical despite different names*

### Comparing `datasette_extract-0.1a6/datasette_extract/templates/_extract_drop_handler.html` & `datasette_extract-0.1a7/datasette_extract/templates/_extract_drop_handler.html`

 * *Files identical despite different names*

### Comparing `datasette_extract-0.1a6/datasette_extract/templates/extract_create_table.html` & `datasette_extract-0.1a7/datasette_extract/templates/extract_create_table.html`

 * *Files identical despite different names*

### Comparing `datasette_extract-0.1a6/datasette_extract/templates/extract_progress.html` & `datasette_extract-0.1a7/datasette_extract/templates/extract_progress.html`

 * *Files identical despite different names*

### Comparing `datasette_extract-0.1a6/datasette_extract/templates/extract_to_table.html` & `datasette_extract-0.1a7/datasette_extract/templates/extract_to_table.html`

 * *Files identical despite different names*

### Comparing `datasette_extract-0.1a6/datasette_extract.egg-info/PKG-INFO` & `datasette_extract-0.1a7/datasette_extract.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-extract
-Version: 0.1a6
+Version: 0.1a7
 Summary: Import unstructured data (text and images) into structured tables
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-extract
 Project-URL: Changelog, https://github.com/datasette/datasette-extract/releases
 Project-URL: Issues, https://github.com/datasette/datasette-extract/issues
 Project-URL: CI, https://github.com/datasette/datasette-extract/actions
```

### Comparing `datasette_extract-0.1a6/datasette_extract.egg-info/SOURCES.txt` & `datasette_extract-0.1a7/datasette_extract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datasette_extract-0.1a6/pyproject.toml` & `datasette_extract-0.1a7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datasette-extract"
-version = "0.1a6"
+version = "0.1a7"
 description = "Import unstructured data (text and images) into structured tables"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
```

### Comparing `datasette_extract-0.1a6/tests/test_web.py` & `datasette_extract-0.1a7/tests/test_web.py`

 * *Files identical despite different names*

