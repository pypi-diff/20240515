# Comparing `tmp/tinygui-1.0.1.tar.gz` & `tmp/tinygui-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinygui-1.0.1.tar", last modified: Tue May 14 11:03:55 2024, max compression
+gzip compressed data, was "tinygui-1.0.2.tar", last modified: Wed May 15 05:48:08 2024, max compression
```

## Comparing `tinygui-1.0.1.tar` & `tinygui-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 11:03:55.046754 tinygui-1.0.1/
--rw-rw-rw-   0        0        0     1093 2024-05-13 06:57:48.000000 tinygui-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      511 2024-05-14 11:03:55.044742 tinygui-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      620 2024-05-14 10:36:13.000000 tinygui-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 11:03:55.046754 tinygui-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 11:03:55.027590 tinygui-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 11:03:55.033692 tinygui-1.0.1/src/tinygui/
--rw-rw-rw-   0        0        0       21 2024-04-29 06:18:34.000000 tinygui-1.0.1/src/tinygui/__init__.py
--rw-rw-rw-   0        0        0     1809 2024-05-09 03:08:39.000000 tinygui-1.0.1/src/tinygui/tinygui.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:03:55.043223 tinygui-1.0.1/src/tinygui.egg-info/
--rw-rw-rw-   0        0        0      511 2024-05-14 11:03:55.000000 tinygui-1.0.1/src/tinygui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-05-14 11:03:55.000000 tinygui-1.0.1/src/tinygui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 11:03:55.000000 tinygui-1.0.1/src/tinygui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 11:03:55.000000 tinygui-1.0.1/src/tinygui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 05:48:08.209490 tinygui-1.0.2/
+-rw-rw-rw-   0        0        0      488 2024-05-15 05:48:08.208484 tinygui-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2024-05-15 05:46:13.000000 tinygui-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 05:48:08.209490 tinygui-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 05:48:08.192509 tinygui-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 05:48:08.197532 tinygui-1.0.2/src/tinygui/
+-rw-rw-rw-   0        0        0       21 2024-04-29 06:18:34.000000 tinygui-1.0.2/src/tinygui/__init__.py
+-rw-rw-rw-   0        0        0     2889 2024-05-15 05:44:44.000000 tinygui-1.0.2/src/tinygui/tinygui.py
+drwxrwxrwx   0        0        0        0 2024-05-15 05:48:08.206484 tinygui-1.0.2/src/tinygui.egg-info/
+-rw-rw-rw-   0        0        0      488 2024-05-15 05:48:08.000000 tinygui-1.0.2/src/tinygui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-15 05:48:08.000000 tinygui-1.0.2/src/tinygui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 05:48:08.000000 tinygui-1.0.2/src/tinygui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 05:48:08.000000 tinygui-1.0.2/src/tinygui.egg-info/top_level.txt
```

### Comparing `tinygui-1.0.1/pyproject.toml` & `tinygui-1.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tinygui"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name = "xiaoheli", email = "1173324325@qq.com" },
 ]
 dependencies = []
 description = "A small example package for gui"
 readme = "README.md"
 requires-python = ">=3.8"
```

