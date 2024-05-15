# Comparing `tmp/okta_graph-0.1.0.tar.gz` & `tmp/okta_graph-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okta_graph-0.1.0.tar", max compression
+gzip compressed data, was "okta_graph-0.2.0.tar", max compression
```

## Comparing `okta_graph-0.1.0.tar` & `okta_graph-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2024-02-07 18:40:54.573320 okta_graph-0.1.0/README.md
--rw-r--r--   0        0        0      668 2024-02-09 21:19:50.684097 okta_graph-0.1.0/okta_graph/README.md
--rw-r--r--   0        0        0       28 2024-02-07 18:07:57.982496 okta_graph-0.1.0/okta_graph/__init__.py
--rw-r--r--   0        0        0     3918 2024-05-06 14:22:40.212816 okta_graph-0.1.0/okta_graph/api.py
--rw-r--r--   0        0        0     8805 2024-02-20 17:35:37.933994 okta_graph-0.1.0/okta_graph/cache.py
--rwxr-xr-x   0        0        0     9534 2024-02-14 04:20:17.585916 okta_graph-0.1.0/okta_graph/graph.py
--rwxr-xr-x   0        0        0     1411 2024-02-02 23:03:41.749538 okta_graph-0.1.0/okta_graph/install.sh
--rw-r--r--   0        0        0     1382 2024-02-08 17:18:15.658980 okta_graph-0.1.0/okta_graph/logging.py
--rw-r--r--   0        0        0     2090 2024-02-09 17:49:02.469683 okta_graph-0.1.0/okta_graph/models.py
--rw-r--r--   0        0        0     9991 2024-02-09 19:28:49.773376 okta_graph-0.1.0/okta_graph/plugins.py
--rwxr-xr-x   0        0        0     8913 2024-02-09 18:21:45.952287 okta_graph-0.1.0/okta_graph/rule_parser.py
--rw-r--r--   0        0        0    41965 2024-02-02 18:56:17.516403 okta_graph-0.1.0/okta_graph/static/css/jsoneditor.css
--rw-r--r--   0        0        0     3269 2024-02-06 20:52:26.354538 okta_graph-0.1.0/okta_graph/static/css/main.css
--rw-r--r--   0        0        0     2916 2024-01-29 21:53:26.525847 okta_graph-0.1.0/okta_graph/static/icons/aws.png
--rw-r--r--   0        0        0     6784 2024-01-29 20:09:01.195559 okta_graph-0.1.0/okta_graph/static/icons/group.png
--rw-r--r--   0        0        0      825 2024-02-06 06:04:36.231237 okta_graph-0.1.0/okta_graph/static/icons/manual_group.png
--rw-r--r--   0        0        0     1373 2024-01-29 22:03:10.821084 okta_graph-0.1.0/okta_graph/static/icons/rule.png
--rw-r--r--   0        0        0     6788 2024-01-30 21:29:05.663316 okta_graph-0.1.0/okta_graph/static/icons/user.png
--rw-r--r--   0        0        0    31482 2024-02-02 17:35:11.632475 okta_graph-0.1.0/okta_graph/static/img/jsoneditor-icons.svg
--rw-r--r--   0        0        0     3464 2024-02-06 22:24:31.704943 okta_graph-0.1.0/okta_graph/static/index.html
--rw-r--r--   0        0        0    10601 2024-05-13 16:19:37.153291 okta_graph-0.1.0/okta_graph/static/js/graph.js
--rw-r--r--   0        0        0  2104113 2024-02-02 17:21:57.050505 okta_graph-0.1.0/okta_graph/static/js/jsoneditor.js
--rw-r--r--   0        0        0     2807 2024-02-06 20:20:21.160181 okta_graph-0.1.0/okta_graph/static/js/profile-editor.js
--rw-r--r--   0        0        0      689 2024-05-13 16:21:17.729583 okta_graph-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 okta_graph-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-07 18:40:54.573320 okta_graph-0.2.0/README.md
+-rw-r--r--   0        0        0      668 2024-02-09 21:19:50.684097 okta_graph-0.2.0/okta_graph/README.md
+-rw-r--r--   0        0        0       28 2024-02-07 18:07:57.982496 okta_graph-0.2.0/okta_graph/__init__.py
+-rw-r--r--   0        0        0     3918 2024-05-06 14:22:40.212816 okta_graph-0.2.0/okta_graph/api.py
+-rw-r--r--   0        0        0     8805 2024-02-20 17:35:37.933994 okta_graph-0.2.0/okta_graph/cache.py
+-rwxr-xr-x   0        0        0     9534 2024-02-14 04:20:17.585916 okta_graph-0.2.0/okta_graph/graph.py
+-rwxr-xr-x   0        0        0     1411 2024-02-02 23:03:41.749538 okta_graph-0.2.0/okta_graph/install.sh
+-rw-r--r--   0        0        0     1382 2024-02-08 17:18:15.658980 okta_graph-0.2.0/okta_graph/logging.py
+-rw-r--r--   0        0        0     2090 2024-02-09 17:49:02.469683 okta_graph-0.2.0/okta_graph/models.py
+-rw-r--r--   0        0        0     9991 2024-02-09 19:28:49.773376 okta_graph-0.2.0/okta_graph/plugins.py
+-rwxr-xr-x   0        0        0     8913 2024-02-09 18:21:45.952287 okta_graph-0.2.0/okta_graph/rule_parser.py
+-rw-r--r--   0        0        0    41965 2024-02-02 18:56:17.516403 okta_graph-0.2.0/okta_graph/static/css/jsoneditor.css
+-rw-r--r--   0        0        0     3269 2024-02-06 20:52:26.354538 okta_graph-0.2.0/okta_graph/static/css/main.css
+-rw-r--r--   0        0        0     2916 2024-01-29 21:53:26.525847 okta_graph-0.2.0/okta_graph/static/icons/aws.png
+-rw-r--r--   0        0        0     6784 2024-01-29 20:09:01.195559 okta_graph-0.2.0/okta_graph/static/icons/group.png
+-rw-r--r--   0        0        0      825 2024-02-06 06:04:36.231237 okta_graph-0.2.0/okta_graph/static/icons/manual_group.png
+-rw-r--r--   0        0        0     1373 2024-01-29 22:03:10.821084 okta_graph-0.2.0/okta_graph/static/icons/rule.png
+-rw-r--r--   0        0        0     6788 2024-01-30 21:29:05.663316 okta_graph-0.2.0/okta_graph/static/icons/user.png
+-rw-r--r--   0        0        0    31482 2024-02-02 17:35:11.632475 okta_graph-0.2.0/okta_graph/static/img/jsoneditor-icons.svg
+-rw-r--r--   0        0        0     3464 2024-02-06 22:24:31.704943 okta_graph-0.2.0/okta_graph/static/index.html
+-rw-r--r--   0        0        0    10601 2024-05-13 16:19:37.153291 okta_graph-0.2.0/okta_graph/static/js/graph.js
+-rw-r--r--   0        0        0  2104113 2024-02-02 17:21:57.050505 okta_graph-0.2.0/okta_graph/static/js/jsoneditor.js
+-rw-r--r--   0        0        0     2807 2024-02-06 20:20:21.160181 okta_graph-0.2.0/okta_graph/static/js/profile-editor.js
+-rw-r--r--   0        0        0      689 2024-05-15 19:55:51.366225 okta_graph-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 okta_graph-0.2.0/PKG-INFO
```

### Comparing `okta_graph-0.1.0/okta_graph/README.md` & `okta_graph-0.2.0/okta_graph/README.md`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/api.py` & `okta_graph-0.2.0/okta_graph/api.py`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/cache.py` & `okta_graph-0.2.0/okta_graph/cache.py`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/graph.py` & `okta_graph-0.2.0/okta_graph/graph.py`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/install.sh` & `okta_graph-0.2.0/okta_graph/install.sh`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/logging.py` & `okta_graph-0.2.0/okta_graph/logging.py`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/models.py` & `okta_graph-0.2.0/okta_graph/models.py`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/plugins.py` & `okta_graph-0.2.0/okta_graph/plugins.py`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/rule_parser.py` & `okta_graph-0.2.0/okta_graph/rule_parser.py`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/static/css/jsoneditor.css` & `okta_graph-0.2.0/okta_graph/static/css/jsoneditor.css`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/static/css/main.css` & `okta_graph-0.2.0/okta_graph/static/css/main.css`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/static/icons/aws.png` & `okta_graph-0.2.0/okta_graph/static/icons/aws.png`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/static/icons/group.png` & `okta_graph-0.2.0/okta_graph/static/icons/group.png`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/static/icons/manual_group.png` & `okta_graph-0.2.0/okta_graph/static/icons/manual_group.png`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/static/icons/rule.png` & `okta_graph-0.2.0/okta_graph/static/icons/rule.png`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/static/icons/user.png` & `okta_graph-0.2.0/okta_graph/static/icons/user.png`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/static/img/jsoneditor-icons.svg` & `okta_graph-0.2.0/okta_graph/static/img/jsoneditor-icons.svg`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/static/index.html` & `okta_graph-0.2.0/okta_graph/static/index.html`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/static/js/graph.js` & `okta_graph-0.2.0/okta_graph/static/js/graph.js`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/static/js/jsoneditor.js` & `okta_graph-0.2.0/okta_graph/static/js/jsoneditor.js`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/okta_graph/static/js/profile-editor.js` & `okta_graph-0.2.0/okta_graph/static/js/profile-editor.js`

 * *Files identical despite different names*

### Comparing `okta_graph-0.1.0/pyproject.toml` & `okta_graph-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "okta-graph"
-version = "0.1.0"
+version = "0.2.0"
 description = "An ASGI web application that provides tools for graphing uset groups based on user attributes and group rules in Okta."
 authors = ["Mathew Moon <me@mathewmoon.net>"]
 readme = "README.md"
 packages = [{include = "okta_graph", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.109.2"
 okta = "^2.9.5"
 pydot = "^2.0.0"
 pydantic = "^2.6.1"
-okta-expression-parser = "^0.2.0"
+okta-expression-parser = "^0.3.0"
 uvicorn = "^0.27.0"
 loguru = "^0.7.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "7.4.3"
 
 [tool.pytest.ini_options]
```

### Comparing `okta_graph-0.1.0/PKG-INFO` & `okta_graph-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: okta-graph
-Version: 0.1.0
+Version: 0.2.0
 Summary: An ASGI web application that provides tools for graphing uset groups based on user attributes and group rules in Okta.
 Author: Mathew Moon
 Author-email: me@mathewmoon.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: okta (>=2.9.5,<3.0.0)
-Requires-Dist: okta-expression-parser (>=0.2.0,<0.3.0)
+Requires-Dist: okta-expression-parser (>=0.3.0,<0.4.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: pydot (>=2.0.0,<3.0.0)
 Requires-Dist: uvicorn (>=0.27.0,<0.28.0)
 Description-Content-Type: text/markdown
```

