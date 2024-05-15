# Comparing `tmp/deltalake_ipython_extensions-0.1.0.tar.gz` & `tmp/deltalake_ipython_extensions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltalake_ipython_extensions-0.1.0.tar", max compression
+gzip compressed data, was "deltalake_ipython_extensions-0.1.1.tar", max compression
```

## Comparing `deltalake_ipython_extensions-0.1.0.tar` & `deltalake_ipython_extensions-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-10 14:15:03.662501 deltalake_ipython_extensions-0.1.0/README.md
--rw-r--r--   0        0        0      166 2024-05-10 14:18:11.762868 deltalake_ipython_extensions-0.1.0/deltalake_ipython_extensions/__init__.py
--rw-r--r--   0        0        0     1849 2024-05-10 14:17:43.794449 deltalake_ipython_extensions-0.1.0/deltalake_ipython_extensions/duckdb_extensions.py
--rw-r--r--   0        0        0      370 2024-05-15 14:20:31.723443 deltalake_ipython_extensions-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 deltalake_ipython_extensions-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 14:15:03.662501 deltalake_ipython_extensions-0.1.1/README.md
+-rw-r--r--   0        0        0      166 2024-05-10 14:18:11.762868 deltalake_ipython_extensions-0.1.1/deltalake_ipython_extensions/__init__.py
+-rw-r--r--   0        0        0     1849 2024-05-10 14:17:43.794449 deltalake_ipython_extensions-0.1.1/deltalake_ipython_extensions/duckdb_extensions.py
+-rw-r--r--   0        0        0      369 2024-05-15 14:47:09.611642 deltalake_ipython_extensions-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 deltalake_ipython_extensions-0.1.1/PKG-INFO
```

### Comparing `deltalake_ipython_extensions-0.1.0/deltalake_ipython_extensions/duckdb_extensions.py` & `deltalake_ipython_extensions-0.1.1/deltalake_ipython_extensions/duckdb_extensions.py`

 * *Files identical despite different names*

