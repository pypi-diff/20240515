# Comparing `tmp/pih-web-0.11.tar.gz` & `tmp/pih-web-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-web-0.11.tar", last modified: Wed Apr 10 02:31:54 2024, max compression
+gzip compressed data, was "pih-web-0.12.tar", last modified: Wed May 15 04:30:02 2024, max compression
```

## Comparing `pih-web-0.11.tar` & `pih-web-0.12.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:31:54.388451 pih-web-0.11/
--rw-rw-rw-   0        0        0      377 2024-04-10 02:31:54.357202 pih-web-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 02:31:54.013465 pih-web-0.11/WebServerService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-web-0.11/WebServerService/__init__.py
--rw-rw-rw-   0        0        0      151 2024-02-14 00:18:05.000000 pih-web-0.11/WebServerService/__main__.py
--rw-rw-rw-   0        0        0    76962 2024-04-09 05:06:36.000000 pih-web-0.11/WebServerService/const.py
--rw-rw-rw-   0        0        0     4960 2024-04-09 05:06:40.000000 pih-web-0.11/WebServerService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:31:54.325954 pih-web-0.11/pih_web.egg-info/
--rw-rw-rw-   0        0        0      377 2024-04-10 02:31:53.000000 pih-web-0.11/pih_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-04-10 02:31:53.000000 pih-web-0.11/pih_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:31:53.000000 pih-web-0.11/pih_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-10 02:31:53.000000 pih-web-0.11/pih_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-04-10 02:31:53.000000 pih-web-0.11/pih_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-10 02:31:53.000000 pih-web-0.11/pih_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 02:31:54.388451 pih-web-0.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:02.866446 pih-web-0.12/
+-rw-rw-rw-   0        0        0      377 2024-05-15 04:30:02.788307 pih-web-0.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:02.146662 pih-web-0.12/WebServerService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-web-0.12/WebServerService/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-02-14 00:18:05.000000 pih-web-0.12/WebServerService/__main__.py
+-rw-rw-rw-   0        0        0      523 2024-05-15 04:23:07.000000 pih-web-0.12/WebServerService/const.py
+-rw-rw-rw-   0        0        0     4960 2024-05-15 04:23:16.000000 pih-web-0.12/WebServerService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:30:02.757174 pih-web-0.12/pih_web.egg-info/
+-rw-rw-rw-   0        0        0      377 2024-05-15 04:30:01.000000 pih-web-0.12/pih_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-05-15 04:30:01.000000 pih-web-0.12/pih_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 04:30:01.000000 pih-web-0.12/pih_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-15 04:30:01.000000 pih-web-0.12/pih_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-05-15 04:30:01.000000 pih-web-0.12/pih_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-15 04:30:01.000000 pih-web-0.12/pih_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 04:30:02.866446 pih-web-0.12/setup.cfg
```

### Comparing `pih-web-0.11/WebServerService/service.py` & `pih-web-0.12/WebServerService/service.py`

 * *Files identical despite different names*

