# Comparing `tmp/squiral-0.4.4.tar.gz` & `tmp/squiral-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squiral-0.4.4.tar", max compression
+gzip compressed data, was "squiral-0.4.5.tar", max compression
```

## Comparing `squiral-0.4.4.tar` & `squiral-0.4.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2024-04-23 20:01:47.169035 squiral-0.4.4/LICENSE
--rw-r--r--   0        0        0     3182 2024-04-23 20:01:47.173035 squiral-0.4.4/README.md
--rw-r--r--   0        0        0      531 2024-04-23 20:01:47.173035 squiral-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      185 2024-04-23 20:01:47.173035 squiral-0.4.4/squiral/__init__.py
--rw-r--r--   0        0        0      152 2024-04-23 20:01:47.173035 squiral-0.4.4/squiral/__main__.py
--rw-r--r--   0        0        0      744 2024-04-23 20:01:47.173035 squiral-0.4.4/squiral/main.py
--rw-r--r--   0        0        0     2464 2024-04-23 20:01:47.173035 squiral-0.4.4/squiral/squiral.py
--rw-r--r--   0        0        0     3854 1970-01-01 00:00:00.000000 squiral-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-14 22:42:51.823231 squiral-0.4.5/LICENSE
+-rw-r--r--   0        0        0     3367 2024-05-14 22:42:51.823231 squiral-0.4.5/README.md
+-rw-r--r--   0        0        0      531 2024-05-14 22:42:51.823231 squiral-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      185 2024-05-14 22:42:51.823231 squiral-0.4.5/squiral/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-14 22:42:51.823231 squiral-0.4.5/squiral/__main__.py
+-rw-r--r--   0        0        0      744 2024-05-14 22:42:51.823231 squiral-0.4.5/squiral/main.py
+-rw-r--r--   0        0        0     2464 2024-05-14 22:42:51.823231 squiral-0.4.5/squiral/squiral.py
+-rw-r--r--   0        0        0     4039 1970-01-01 00:00:00.000000 squiral-0.4.5/PKG-INFO
```

### Comparing `squiral-0.4.4/LICENSE` & `squiral-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `squiral-0.4.4/README.md` & `squiral-0.4.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -89,7 +89,13 @@
 >>>
 ```
 
 ### Contributing
 
 To learn more about making a contribution to squiral, please see our
 [Contributing guide](CONTRIBUTING.md)
+
+#### Many Thanks To Our Contributors
+
+ <a href = "https://github.com/sadikkuzu/squiral/graphs/contributors">
+   <img src = "https://contrib.rocks/image?repo=sadikkuzu/squiral"/>
+ </a>
```

### Comparing `squiral-0.4.4/pyproject.toml` & `squiral-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squiral"
-version = "0.4.4"
+version = "0.4.5"
 description = "squiral - square spiral"
 authors = ["SADIK KUZU <sadikkuzu@hotmail.com>"]
 homepage = "https://github.com/sadikkuzu/squiral"
 readme = "README.md"
 license = "MIT"
 packages = [{include = "squiral"}]
```

### Comparing `squiral-0.4.4/squiral/main.py` & `squiral-0.4.5/squiral/main.py`

 * *Files identical despite different names*

### Comparing `squiral-0.4.4/squiral/squiral.py` & `squiral-0.4.5/squiral/squiral.py`

 * *Files identical despite different names*

### Comparing `squiral-0.4.4/PKG-INFO` & `squiral-0.4.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squiral
-Version: 0.4.4
+Version: 0.4.5
 Summary: squiral - square spiral
 Home-page: https://github.com/sadikkuzu/squiral
 License: MIT
 Author: SADIK KUZU
 Author-email: sadikkuzu@hotmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -109,7 +109,13 @@
 ```
 
 ### Contributing
 
 To learn more about making a contribution to squiral, please see our
 [Contributing guide](CONTRIBUTING.md)
 
+#### Many Thanks To Our Contributors
+
+ <a href = "https://github.com/sadikkuzu/squiral/graphs/contributors">
+   <img src = "https://contrib.rocks/image?repo=sadikkuzu/squiral"/>
+ </a>
+
```

