# Comparing `tmp/transistorfm-1.0.0.tar.gz` & `tmp/transistorfm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transistorfm-1.0.0.tar", last modified: Wed May 15 20:14:30 2024, max compression
+gzip compressed data, was "transistorfm-1.0.1.tar", last modified: Wed May 15 20:16:07 2024, max compression
```

## Comparing `transistorfm-1.0.0.tar` & `transistorfm-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-15 20:14:30.396715 transistorfm-1.0.0/
--rw-r--r--   0 josh       (501) staff       (20)     1070 2024-05-15 19:46:17.000000 transistorfm-1.0.0/LICENSE
--rw-r--r--   0 josh       (501) staff       (20)      491 2024-05-15 20:14:30.396487 transistorfm-1.0.0/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)      234 2024-05-15 20:10:04.000000 transistorfm-1.0.0/README.md
--rw-r--r--   0 josh       (501) staff       (20)       38 2024-05-15 20:14:30.396766 transistorfm-1.0.0/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)      426 2024-05-15 20:14:23.000000 transistorfm-1.0.0/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-15 20:14:30.395264 transistorfm-1.0.0/transistor/
--rw-r--r--   0 josh       (501) staff       (20)        0 2024-05-15 19:42:17.000000 transistorfm-1.0.0/transistor/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     3133 2024-05-15 19:42:48.000000 transistorfm-1.0.0/transistor/client.py
--rw-r--r--   0 josh       (501) staff       (20)     1769 2024-05-15 19:42:24.000000 transistorfm-1.0.0/transistor/objects.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-15 20:14:30.396223 transistorfm-1.0.0/transistorfm.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)      491 2024-05-15 20:14:30.000000 transistorfm-1.0.0/transistorfm.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)      236 2024-05-15 20:14:30.000000 transistorfm-1.0.0/transistorfm.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2024-05-15 20:14:30.000000 transistorfm-1.0.0/transistorfm.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)       11 2024-05-15 20:14:30.000000 transistorfm-1.0.0/transistorfm.egg-info/top_level.txt
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-15 20:16:07.142834 transistorfm-1.0.1/
+-rw-r--r--   0 josh       (501) staff       (20)     1070 2024-05-15 19:46:17.000000 transistorfm-1.0.1/LICENSE
+-rw-r--r--   0 josh       (501) staff       (20)      474 2024-05-15 20:16:07.142569 transistorfm-1.0.1/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)      217 2024-05-15 20:15:12.000000 transistorfm-1.0.1/README.md
+-rw-r--r--   0 josh       (501) staff       (20)       38 2024-05-15 20:16:07.142893 transistorfm-1.0.1/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      426 2024-05-15 20:16:01.000000 transistorfm-1.0.1/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-15 20:16:07.141242 transistorfm-1.0.1/transistor/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2024-05-15 19:42:17.000000 transistorfm-1.0.1/transistor/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     3133 2024-05-15 19:42:48.000000 transistorfm-1.0.1/transistor/client.py
+-rw-r--r--   0 josh       (501) staff       (20)     1769 2024-05-15 19:42:24.000000 transistorfm-1.0.1/transistor/objects.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2024-05-15 20:16:07.142242 transistorfm-1.0.1/transistorfm.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)      474 2024-05-15 20:16:07.000000 transistorfm-1.0.1/transistorfm.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)      236 2024-05-15 20:16:07.000000 transistorfm-1.0.1/transistorfm.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2024-05-15 20:16:07.000000 transistorfm-1.0.1/transistorfm.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)       11 2024-05-15 20:16:07.000000 transistorfm-1.0.1/transistorfm.egg-info/top_level.txt
```

### Comparing `transistorfm-1.0.0/LICENSE` & `transistorfm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transistorfm-1.0.0/transistor/client.py` & `transistorfm-1.0.1/transistor/client.py`

 * *Files identical despite different names*

### Comparing `transistorfm-1.0.0/transistor/objects.py` & `transistorfm-1.0.1/transistor/objects.py`

 * *Files identical despite different names*

