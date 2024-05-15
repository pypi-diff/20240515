# Comparing `tmp/hstream-0.1.51.tar.gz` & `tmp/hstream-0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstream-0.1.51.tar", max compression
+gzip compressed data, was "hstream-0.1.52.tar", max compression
```

## Comparing `hstream-0.1.51.tar` & `hstream-0.1.52.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1927 2024-05-15 12:59:21.249808 hstream-0.1.51/README.md
--rw-r--r--   0        0        0       53 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/__init__.py
--rw-r--r--   0        0        0       66 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/__main__.py
--rw-r--r--   0        0        0     3522 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/cli.py
--rw-r--r--   0        0        0    19076 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/components/components.py
--rw-r--r--   0        0        0     4625 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/components/styling_components.py
--rw-r--r--   0        0        0        0 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/django_server/hs/__init__.py
--rw-r--r--   0        0        0      136 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/django_server/hs/apps.py
--rw-r--r--   0        0        0      749 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/django_server/hs/session_utils.py
--rw-r--r--   0        0        0      424 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/django_server/hs/urls.py
--rw-r--r--   0        0        0     7990 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/django_server/hs/views.py
--rwxr-xr-x   0        0        0      661 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/django_server/manage.py
--rw-r--r--   0        0        0        0 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/django_server/root/__init__.py
--rw-r--r--   0        0        0      381 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/django_server/root/asgi.py
--rw-r--r--   0        0        0     3218 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/django_server/root/settings.py
--rw-r--r--   0        0        0      802 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/django_server/root/urls.py
--rw-r--r--   0        0        0      381 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/django_server/root/wsgi.py
--rw-r--r--   0        0        0      683 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/hs.py
--rw-r--r--   0        0        0      638 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/run.py
--rw-r--r--   0        0        0      394 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/template.py
--rw-r--r--   0        0        0      162 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/templates/error_html.html
--rw-r--r--   0        0        0     2446 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/templates/format_html.html
--rw-r--r--   0        0        0     2466 2024-05-15 12:59:21.261808 hstream-0.1.51/hstream/utils.py
--rw-r--r--   0        0        0      646 2024-05-15 12:59:21.261808 hstream-0.1.51/pyproject.toml
--rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 hstream-0.1.51/PKG-INFO
+-rw-r--r--   0        0        0     1927 2024-05-15 13:07:46.821292 hstream-0.1.52/README.md
+-rw-r--r--   0        0        0       53 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/__main__.py
+-rw-r--r--   0        0        0     3522 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/cli.py
+-rw-r--r--   0        0        0    19076 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/components/components.py
+-rw-r--r--   0        0        0     4625 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/components/styling_components.py
+-rw-r--r--   0        0        0        0 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/django_server/hs/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/django_server/hs/apps.py
+-rw-r--r--   0        0        0      749 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/django_server/hs/session_utils.py
+-rw-r--r--   0        0        0      424 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/django_server/hs/urls.py
+-rw-r--r--   0        0        0     7990 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/django_server/hs/views.py
+-rwxr-xr-x   0        0        0      661 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/django_server/manage.py
+-rw-r--r--   0        0        0        0 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/django_server/root/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/django_server/root/asgi.py
+-rw-r--r--   0        0        0     3218 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/django_server/root/settings.py
+-rw-r--r--   0        0        0      802 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/django_server/root/urls.py
+-rw-r--r--   0        0        0      381 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/django_server/root/wsgi.py
+-rw-r--r--   0        0        0      683 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/hs.py
+-rw-r--r--   0        0        0      638 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/run.py
+-rw-r--r--   0        0        0      394 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/template.py
+-rw-r--r--   0        0        0      162 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/templates/error_html.html
+-rw-r--r--   0        0        0     2446 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/templates/format_html.html
+-rw-r--r--   0        0        0     2466 2024-05-15 13:07:46.829292 hstream-0.1.52/hstream/utils.py
+-rw-r--r--   0        0        0      677 2024-05-15 13:07:46.829292 hstream-0.1.52/pyproject.toml
+-rw-r--r--   0        0        0     2509 1970-01-01 00:00:00.000000 hstream-0.1.52/PKG-INFO
```

### Comparing `hstream-0.1.51/README.md` & `hstream-0.1.52/README.md`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/hstream/cli.py` & `hstream-0.1.52/hstream/cli.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/hstream/components/components.py` & `hstream-0.1.52/hstream/components/components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/hstream/components/styling_components.py` & `hstream-0.1.52/hstream/components/styling_components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/hstream/django_server/hs/session_utils.py` & `hstream-0.1.52/hstream/django_server/hs/session_utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/hstream/django_server/hs/views.py` & `hstream-0.1.52/hstream/django_server/hs/views.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/hstream/django_server/manage.py` & `hstream-0.1.52/hstream/django_server/manage.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/hstream/django_server/root/settings.py` & `hstream-0.1.52/hstream/django_server/root/settings.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/hstream/django_server/root/urls.py` & `hstream-0.1.52/hstream/django_server/root/urls.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/hstream/hs.py` & `hstream-0.1.52/hstream/hs.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/hstream/run.py` & `hstream-0.1.52/hstream/run.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/hstream/templates/format_html.html` & `hstream-0.1.52/hstream/templates/format_html.html`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/hstream/utils.py` & `hstream-0.1.52/hstream/utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.51/pyproject.toml` & `hstream-0.1.52/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hstream"
-version = "0.1.51"
+version = "0.1.52"
 description = ""
 authors = ["Conrad <conradbez1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 hstream = "hstream.cli:cli"
 
@@ -23,11 +23,12 @@
 ipdb = "^0.13.13"
 isort = "^5.13.2"
 pre-commit = "^3.7.1"
 ruff = "^0.4.4"
 pytest = "^8.2.0"
 python-dotenv = "^1.0.1"
 playwright = "^1.43.0"
+pytest-rerunfailures = "^14.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hstream-0.1.51/PKG-INFO` & `hstream-0.1.52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstream
-Version: 0.1.51
+Version: 0.1.52
 Summary: 
 Author: Conrad
 Author-email: conradbez1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

