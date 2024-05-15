# Comparing `tmp/signal_export-2.3.2.tar.gz` & `tmp/signal_export-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal_export-2.3.2.tar", last modified: Mon May 13 15:18:21 2024, max compression
+gzip compressed data, was "signal_export-2.3.3.tar", last modified: Wed May 15 07:39:41 2024, max compression
```

## Comparing `signal_export-2.3.2.tar` & `signal_export-2.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1170 2024-05-13 15:18:17.715710 signal_export-2.3.2/LICENSE
--rw-r--r--   0        0        0     6921 2024-05-13 15:18:17.715710 signal_export-2.3.2/README.md
--rw-r--r--   0        0        0     2006 2024-05-13 15:18:21.031731 signal_export-2.3.2/pyproject.toml
--rw-r--r--   0        0        0        1 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/__init__.py
--rw-r--r--   0        0        0       69 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/__main__.py
--rw-r--r--   0        0        0     3173 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/create.py
--rw-r--r--   0        0        0     3017 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/data.py
--rw-r--r--   0        0        0     3209 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/files.py
--rw-r--r--   0        0        0     3451 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/html.py
--rw-r--r--   0        0        0      144 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/logging.py
--rwxr-xr-x   0        0        0     8356 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/main.py
--rw-r--r--   0        0        0     2722 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/merge.py
--rw-r--r--   0        0        0     4548 2024-05-13 15:18:17.719710 signal_export-2.3.2/sigexport/models.py
--rw-r--r--   0        0        0     1846 2024-05-13 15:18:17.719710 signal_export-2.3.2/sigexport/style.css
--rw-r--r--   0        0        0     1271 2024-05-13 15:18:17.719710 signal_export-2.3.2/sigexport/templates.py
--rw-r--r--   0        0        0     2467 2024-05-13 15:18:17.719710 signal_export-2.3.2/sigexport/utils.py
--rw-r--r--   0        0        0     2546 2024-05-13 15:18:17.719710 signal_export-2.3.2/tests/data/attachments.noindex/image.jpeg
--rw-r--r--   0        0        0    17641 2024-05-13 15:18:17.719710 signal_export-2.3.2/tests/data/attachments.noindex/voicenote.m4a
--rw-r--r--   0        0        0       22 2024-05-13 15:18:17.719710 signal_export-2.3.2/tests/data/config.json
--rw-r--r--   0        0        0    16384 2024-05-13 15:18:17.719710 signal_export-2.3.2/tests/data/sql/db.sqlite
--rw-r--r--   0        0        0     5125 2024-05-13 15:18:17.719710 signal_export-2.3.2/tests/test_integration.py
--rw-r--r--   0        0        0       86 2024-05-13 15:18:17.719710 signal_export-2.3.2/tests/test_utils.py
--rw-r--r--   0        0        0     7846 1970-01-01 00:00:00.000000 signal_export-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1170 2024-05-15 07:39:37.985367 signal_export-2.3.3/LICENSE
+-rw-r--r--   0        0        0     6921 2024-05-15 07:39:37.985367 signal_export-2.3.3/README.md
+-rw-r--r--   0        0        0     2006 2024-05-15 07:39:41.157382 signal_export-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/__init__.py
+-rw-r--r--   0        0        0       69 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/__main__.py
+-rw-r--r--   0        0        0     3173 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/create.py
+-rw-r--r--   0        0        0     3017 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/data.py
+-rw-r--r--   0        0        0     3209 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/files.py
+-rw-r--r--   0        0        0     3451 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/html.py
+-rw-r--r--   0        0        0      144 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/logging.py
+-rwxr-xr-x   0        0        0     8356 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/main.py
+-rw-r--r--   0        0        0     2722 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/merge.py
+-rw-r--r--   0        0        0     4548 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/models.py
+-rw-r--r--   0        0        0     1846 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/style.css
+-rw-r--r--   0        0        0     1271 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/templates.py
+-rw-r--r--   0        0        0     2467 2024-05-15 07:39:37.985367 signal_export-2.3.3/sigexport/utils.py
+-rw-r--r--   0        0        0     2546 2024-05-15 07:39:37.989367 signal_export-2.3.3/tests/data/attachments.noindex/image.jpeg
+-rw-r--r--   0        0        0    17641 2024-05-15 07:39:37.989367 signal_export-2.3.3/tests/data/attachments.noindex/voicenote.m4a
+-rw-r--r--   0        0        0       22 2024-05-15 07:39:37.989367 signal_export-2.3.3/tests/data/config.json
+-rw-r--r--   0        0        0    16384 2024-05-15 07:39:37.989367 signal_export-2.3.3/tests/data/sql/db.sqlite
+-rw-r--r--   0        0        0     5125 2024-05-15 07:39:37.989367 signal_export-2.3.3/tests/test_integration.py
+-rw-r--r--   0        0        0       86 2024-05-15 07:39:37.989367 signal_export-2.3.3/tests/test_utils.py
+-rw-r--r--   0        0        0     7846 1970-01-01 00:00:00.000000 signal_export-2.3.3/PKG-INFO
```

### Comparing `signal_export-2.3.2/LICENSE` & `signal_export-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/README.md` & `signal_export-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/pyproject.toml` & `signal_export-2.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 ]
 dependencies = [
     "beautifulsoup4 ~= 4.11",
     "emoji ~= 2.0",
     "Markdown ~= 3.4",
     "typer[all] ~= 0.7",
 ]
-version = "2.3.2"
+version = "2.3.3"
 
 [project.license]
 text = "MIT License"
 
 [project.optional-dependencies]
 sql = [
     "pysqlcipher3 == 1.1.0; python_version <  \"3.11\"",
```

### Comparing `signal_export-2.3.2/sigexport/create.py` & `signal_export-2.3.3/sigexport/create.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/sigexport/data.py` & `signal_export-2.3.3/sigexport/data.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/sigexport/files.py` & `signal_export-2.3.3/sigexport/files.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/sigexport/html.py` & `signal_export-2.3.3/sigexport/html.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/sigexport/main.py` & `signal_export-2.3.3/sigexport/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     chats: str = Option(
         "", help="Comma-separated chat names to include: contact names or group names"
     ),
     json_output: bool = Option(
         False, "--json/--no-json", "-j", help="Whether to create JSON output"
     ),
     html_output: bool = Option(
-        False, "--html/--no-html", "-j", help="Whether to create HTML output"
+        False, "--html/--no-html", "-h", help="Whether to create HTML output"
     ),
     list_chats: bool = Option(
         False, "--list-chats", "-l", help="List available chats and exit"
     ),
     include_empty: bool = Option(
         False, "--include-empty", help="Whether to include empty chats"
     ),
```

### Comparing `signal_export-2.3.2/sigexport/merge.py` & `signal_export-2.3.3/sigexport/merge.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/sigexport/models.py` & `signal_export-2.3.3/sigexport/models.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/sigexport/style.css` & `signal_export-2.3.3/sigexport/style.css`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/sigexport/templates.py` & `signal_export-2.3.3/sigexport/templates.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/sigexport/utils.py` & `signal_export-2.3.3/sigexport/utils.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/tests/data/attachments.noindex/image.jpeg` & `signal_export-2.3.3/tests/data/attachments.noindex/image.jpeg`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/tests/data/attachments.noindex/voicenote.m4a` & `signal_export-2.3.3/tests/data/attachments.noindex/voicenote.m4a`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/tests/data/sql/db.sqlite` & `signal_export-2.3.3/tests/data/sql/db.sqlite`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/tests/test_integration.py` & `signal_export-2.3.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.2/PKG-INFO` & `signal_export-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-export
-Version: 2.3.2
+Version: 2.3.3
 Summary: Export Signal conversations to Markdown and HTML
 Keywords: backup,chat,export
 Home-page: https://github.com/carderne/signal-export
 Author-Email: Chris Arderne <chris@rdrn.me>
 License: MIT License
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

