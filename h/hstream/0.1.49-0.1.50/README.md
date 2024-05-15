# Comparing `tmp/hstream-0.1.49.tar.gz` & `tmp/hstream-0.1.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstream-0.1.49.tar", max compression
+gzip compressed data, was "hstream-0.1.50.tar", max compression
```

## Comparing `hstream-0.1.49.tar` & `hstream-0.1.50.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     4232 2024-05-15 11:59:56.595400 hstream-0.1.49/README.md
--rw-r--r--   0        0        0       53 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/__init__.py
--rw-r--r--   0        0        0       66 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/__main__.py
--rw-r--r--   0        0        0     3522 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/cli.py
--rw-r--r--   0        0        0    19076 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/components/components.py
--rw-r--r--   0        0        0     4625 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/components/styling_components.py
--rw-r--r--   0        0        0        0 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/hs/__init__.py
--rw-r--r--   0        0        0      136 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/hs/apps.py
--rw-r--r--   0        0        0      749 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/hs/session_utils.py
--rw-r--r--   0        0        0      424 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/hs/urls.py
--rw-r--r--   0        0        0     7990 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/hs/views.py
--rwxr-xr-x   0        0        0      661 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/manage.py
--rw-r--r--   0        0        0        0 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/root/__init__.py
--rw-r--r--   0        0        0      381 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/root/asgi.py
--rw-r--r--   0        0        0     3218 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/root/settings.py
--rw-r--r--   0        0        0      802 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/root/urls.py
--rw-r--r--   0        0        0      381 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/django_server/root/wsgi.py
--rw-r--r--   0        0        0      683 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/hs.py
--rw-r--r--   0        0        0      638 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/run.py
--rw-r--r--   0        0        0      394 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/template.py
--rw-r--r--   0        0        0      162 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/templates/error_html.html
--rw-r--r--   0        0        0     2446 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/templates/format_html.html
--rw-r--r--   0        0        0     2466 2024-05-15 11:59:56.607400 hstream-0.1.49/hstream/utils.py
--rw-r--r--   0        0        0      646 2024-05-15 11:59:56.607400 hstream-0.1.49/pyproject.toml
--rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 hstream-0.1.49/PKG-INFO
+-rw-r--r--   0        0        0     4317 2024-05-15 12:35:42.090185 hstream-0.1.50/README.md
+-rw-r--r--   0        0        0       53 2024-05-15 12:35:42.098185 hstream-0.1.50/hstream/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-15 12:35:42.098185 hstream-0.1.50/hstream/__main__.py
+-rw-r--r--   0        0        0     3522 2024-05-15 12:35:42.098185 hstream-0.1.50/hstream/cli.py
+-rw-r--r--   0        0        0    19076 2024-05-15 12:35:42.098185 hstream-0.1.50/hstream/components/components.py
+-rw-r--r--   0        0        0     4625 2024-05-15 12:35:42.098185 hstream-0.1.50/hstream/components/styling_components.py
+-rw-r--r--   0        0        0        0 2024-05-15 12:35:42.098185 hstream-0.1.50/hstream/django_server/hs/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-15 12:35:42.098185 hstream-0.1.50/hstream/django_server/hs/apps.py
+-rw-r--r--   0        0        0      749 2024-05-15 12:35:42.098185 hstream-0.1.50/hstream/django_server/hs/session_utils.py
+-rw-r--r--   0        0        0      424 2024-05-15 12:35:42.098185 hstream-0.1.50/hstream/django_server/hs/urls.py
+-rw-r--r--   0        0        0     7990 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/django_server/hs/views.py
+-rwxr-xr-x   0        0        0      661 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/django_server/manage.py
+-rw-r--r--   0        0        0        0 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/django_server/root/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/django_server/root/asgi.py
+-rw-r--r--   0        0        0     3218 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/django_server/root/settings.py
+-rw-r--r--   0        0        0      802 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/django_server/root/urls.py
+-rw-r--r--   0        0        0      381 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/django_server/root/wsgi.py
+-rw-r--r--   0        0        0      683 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/hs.py
+-rw-r--r--   0        0        0      638 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/run.py
+-rw-r--r--   0        0        0      394 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/template.py
+-rw-r--r--   0        0        0      162 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/templates/error_html.html
+-rw-r--r--   0        0        0     2446 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/templates/format_html.html
+-rw-r--r--   0        0        0     2466 2024-05-15 12:35:42.102185 hstream-0.1.50/hstream/utils.py
+-rw-r--r--   0        0        0      646 2024-05-15 12:35:42.102185 hstream-0.1.50/pyproject.toml
+-rw-r--r--   0        0        0     4899 1970-01-01 00:00:00.000000 hstream-0.1.50/PKG-INFO
```

### Comparing `hstream-0.1.49/README.md` & `hstream-0.1.50/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -104,18 +104,21 @@
         hs.markdown('Thanks to: ')
         with hs.html('a', href='https://picocss.com'):
             hs.markdown('pico css')
 ```
 
 ![hstream card demo](demo/card_example.png)
 
+`hstream eject`: gives a dockerfile and step by step commands to deploy to Railway
+
 # Technologies
 
 Big thanks to the following libraries in particular
 
+
 - Streamlit
 - htmx
 - Yattag
 - pico css
 - Django
 
 # Features (WIP)
```

### Comparing `hstream-0.1.49/hstream/cli.py` & `hstream-0.1.50/hstream/cli.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.49/hstream/components/components.py` & `hstream-0.1.50/hstream/components/components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.49/hstream/components/styling_components.py` & `hstream-0.1.50/hstream/components/styling_components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.49/hstream/django_server/hs/session_utils.py` & `hstream-0.1.50/hstream/django_server/hs/session_utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.49/hstream/django_server/hs/views.py` & `hstream-0.1.50/hstream/django_server/hs/views.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.49/hstream/django_server/manage.py` & `hstream-0.1.50/hstream/django_server/manage.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.49/hstream/django_server/root/settings.py` & `hstream-0.1.50/hstream/django_server/root/settings.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.49/hstream/django_server/root/urls.py` & `hstream-0.1.50/hstream/django_server/root/urls.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.49/hstream/hs.py` & `hstream-0.1.50/hstream/hs.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.49/hstream/run.py` & `hstream-0.1.50/hstream/run.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.49/hstream/templates/format_html.html` & `hstream-0.1.50/hstream/templates/format_html.html`

 * *Files identical despite different names*

### Comparing `hstream-0.1.49/hstream/utils.py` & `hstream-0.1.50/hstream/utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.49/pyproject.toml` & `hstream-0.1.50/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hstream"
-version = "0.1.49"
+version = "0.1.50"
 description = ""
 authors = ["Conrad <conradbez1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 hstream = "hstream.cli:cli"
```

### Comparing `hstream-0.1.49/PKG-INFO` & `hstream-0.1.50/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstream
-Version: 0.1.49
+Version: 0.1.50
 Summary: 
 Author: Conrad
 Author-email: conradbez1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -122,18 +122,21 @@
         hs.markdown('Thanks to: ')
         with hs.html('a', href='https://picocss.com'):
             hs.markdown('pico css')
 ```
 
 ![hstream card demo](demo/card_example.png)
 
+`hstream eject`: gives a dockerfile and step by step commands to deploy to Railway
+
 # Technologies
 
 Big thanks to the following libraries in particular
 
+
 - Streamlit
 - htmx
 - Yattag
 - pico css
 - Django
 
 # Features (WIP)
```

