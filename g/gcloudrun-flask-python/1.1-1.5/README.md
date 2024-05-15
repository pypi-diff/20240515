# Comparing `tmp/gcloudrun_flask_python-1.1.tar.gz` & `tmp/gcloudrun_flask_python-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloudrun_flask_python-1.1.tar", last modified: Wed May 15 06:33:45 2024, max compression
+gzip compressed data, was "gcloudrun_flask_python-1.5.tar", last modified: Wed May 15 06:30:09 2024, max compression
```

## Comparing `gcloudrun_flask_python-1.1.tar` & `gcloudrun_flask_python-1.5.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 06:33:45.214231 gcloudrun_flask_python-1.1/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      155 2024-05-15 06:33:45.214231 gcloudrun_flask_python-1.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1654 2024-05-14 17:41:17.000000 gcloudrun_flask_python-1.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 06:33:45.214231 gcloudrun_flask_python-1.1/gcloudrun_flask_python/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-15 06:33:26.000000 gcloudrun_flask_python-1.1/gcloudrun_flask_python/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3857 2024-05-15 06:21:29.000000 gcloudrun_flask_python-1.1/gcloudrun_flask_python/main.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 06:33:45.214231 gcloudrun_flask_python-1.1/gcloudrun_flask_python.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      155 2024-05-15 06:33:45.000000 gcloudrun_flask_python-1.1/gcloudrun_flask_python.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      362 2024-05-15 06:33:45.000000 gcloudrun_flask_python-1.1/gcloudrun_flask_python.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-15 06:33:45.000000 gcloudrun_flask_python-1.1/gcloudrun_flask_python.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-15 06:33:45.000000 gcloudrun_flask_python-1.1/gcloudrun_flask_python.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       46 2024-05-15 06:33:45.000000 gcloudrun_flask_python-1.1/gcloudrun_flask_python.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2024-05-15 06:33:45.000000 gcloudrun_flask_python-1.1/gcloudrun_flask_python.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-15 06:33:45.214231 gcloudrun_flask_python-1.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      414 2024-05-15 06:33:35.000000 gcloudrun_flask_python-1.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 06:30:09.882239 gcloudrun_flask_python-1.5/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      155 2024-05-15 06:30:09.882239 gcloudrun_flask_python-1.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1654 2024-05-14 17:41:17.000000 gcloudrun_flask_python-1.5/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-15 06:30:09.882239 gcloudrun_flask_python-1.5/gcloudrun_flask_python.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      155 2024-05-15 06:30:09.000000 gcloudrun_flask_python-1.5/gcloudrun_flask_python.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      296 2024-05-15 06:30:09.000000 gcloudrun_flask_python-1.5/gcloudrun_flask_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-15 06:30:09.000000 gcloudrun_flask_python-1.5/gcloudrun_flask_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-15 06:30:09.000000 gcloudrun_flask_python-1.5/gcloudrun_flask_python.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       46 2024-05-15 06:30:09.000000 gcloudrun_flask_python-1.5/gcloudrun_flask_python.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-15 06:30:09.000000 gcloudrun_flask_python-1.5/gcloudrun_flask_python.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-15 06:30:09.882239 gcloudrun_flask_python-1.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      414 2024-05-15 06:29:02.000000 gcloudrun_flask_python-1.5/setup.py
```

### Comparing `gcloudrun_flask_python-1.1/README.md` & `gcloudrun_flask_python-1.5/README.md`

 * *Files identical despite different names*

