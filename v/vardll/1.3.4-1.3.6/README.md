# Comparing `tmp/vardll-1.3.4.tar.gz` & `tmp/vardll-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vardll-1.3.4.tar", last modified: Tue May 14 21:31:58 2024, max compression
+gzip compressed data, was "vardll-1.3.6.tar", last modified: Tue May 14 21:54:05 2024, max compression
```

## Comparing `vardll-1.3.4.tar` & `vardll-1.3.6.tar`

### file list

```diff
@@ -1,16 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 21:31:58.203422 vardll-1.3.4/
--rw-rw-rw-   0        0        0      280 2024-05-14 21:31:58.199077 vardll-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1109 2024-05-13 19:52:21.000000 vardll-1.3.4/license
--rw-rw-rw-   0        0        0       42 2024-05-14 21:31:58.203534 vardll-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      507 2024-05-14 21:26:57.000000 vardll-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:31:58.166190 vardll-1.3.4/vardll/
--rw-rw-rw-   0        0        0       60 2024-05-13 19:47:11.000000 vardll-1.3.4/vardll/__init__.py
--rw-rw-rw-   0        0        0      306 2024-05-13 18:24:47.000000 vardll-1.3.4/vardll/dllvariable.py
--rw-rw-rw-   0        0        0      402 2024-05-13 18:49:06.000000 vardll-1.3.4/vardll/loader.py
--rw-rw-rw-   0        0        0      534 2024-05-13 20:10:21.000000 vardll-1.3.4/vardll/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:31:58.196617 vardll-1.3.4/vardll.egg-info/
--rw-rw-rw-   0        0        0      280 2024-05-14 21:31:57.000000 vardll-1.3.4/vardll.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-05-14 21:31:57.000000 vardll-1.3.4/vardll.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 21:31:57.000000 vardll-1.3.4/vardll.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-14 21:31:57.000000 vardll-1.3.4/vardll.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 21:31:57.000000 vardll-1.3.4/vardll.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 21:54:05.640129 vardll-1.3.6/
+-rw-rw-rw-   0        0        0      280 2024-05-14 21:54:05.638130 vardll-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1109 2024-05-13 19:52:21.000000 vardll-1.3.6/license
+-rw-rw-rw-   0        0        0       42 2024-05-14 21:54:05.645129 vardll-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      507 2024-05-14 21:53:10.000000 vardll-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 21:54:05.636129 vardll-1.3.6/vardll.egg-info/
+-rw-rw-rw-   0        0        0      280 2024-05-14 21:54:05.000000 vardll-1.3.6/vardll.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-05-14 21:54:05.000000 vardll-1.3.6/vardll.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 21:54:05.000000 vardll-1.3.6/vardll.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-14 21:54:05.000000 vardll-1.3.6/vardll.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 21:54:05.000000 vardll-1.3.6/vardll.egg-info/top_level.txt
```

### Comparing `vardll-1.3.4/license` & `vardll-1.3.6/license`

 * *Files identical despite different names*

