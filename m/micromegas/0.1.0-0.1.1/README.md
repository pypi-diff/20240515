# Comparing `tmp/micromegas-0.1.0.tar.gz` & `tmp/micromegas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micromegas-0.1.0.tar", max compression
+gzip compressed data, was "micromegas-0.1.1.tar", max compression
```

## Comparing `micromegas-0.1.0.tar` & `micromegas-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       22 2024-05-10 17:53:36.441886 micromegas-0.1.0/micromegas/__init__.py
--rw-r--r--   0        0        0      474 2024-05-10 17:53:36.445960 micromegas-0.1.0/micromegas/request.py
--rw-r--r--   0        0        0      435 2024-05-10 17:53:36.467627 micromegas-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       85 2024-05-10 17:53:36.432884 micromegas-0.1.0/README.md
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 micromegas-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2024-05-15 17:16:29.525121 micromegas-0.1.1/micromegas/__init__.py
+-rw-r--r--   0        0        0     1613 2024-05-15 17:16:29.533300 micromegas-0.1.1/micromegas/client.py
+-rw-r--r--   0        0        0      512 2024-05-15 17:16:29.545716 micromegas-0.1.1/micromegas/request.py
+-rw-r--r--   0        0        0      505 2024-05-15 17:20:16.453544 micromegas-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-05-10 17:53:36.432884 micromegas-0.1.1/README.md
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 micromegas-0.1.1/PKG-INFO
```

### Comparing `micromegas-0.1.0/PKG-INFO` & `micromegas-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: micromegas
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Python analytics client for https://github.com/madesroches/micromegas/
 Author: Marc-Antoine Desroches
 Author-email: madesroches@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

