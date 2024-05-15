# Comparing `tmp/elm_messenger-0.3.1.tar.gz` & `tmp/elm_messenger-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm_messenger-0.3.1.tar", last modified: Tue May 14 03:11:52 2024, max compression
+gzip compressed data, was "elm_messenger-0.3.2.tar", last modified: Tue May 14 21:24:32 2024, max compression
```

## Comparing `elm_messenger-0.3.1.tar` & `elm_messenger-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-14 03:11:52.007553 elm_messenger-0.3.1/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2024-05-04 14:47:23.000000 elm_messenger-0.3.1/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)     7467 2024-05-14 03:11:52.007553 elm_messenger-0.3.1/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)     7181 2024-05-04 14:47:23.000000 elm_messenger-0.3.1/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-14 03:11:52.007553 elm_messenger-0.3.1/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)     7467 2024-05-14 03:11:52.000000 elm_messenger-0.3.1/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2024-05-14 03:11:52.000000 elm_messenger-0.3.1/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2024-05-14 03:11:52.000000 elm_messenger-0.3.1/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2024-05-14 03:11:52.000000 elm_messenger-0.3.1/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2024-05-14 03:11:52.000000 elm_messenger-0.3.1/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2024-05-14 03:11:52.000000 elm_messenger-0.3.1/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-14 03:11:52.007553 elm_messenger-0.3.1/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-04 14:47:23.000000 elm_messenger-0.3.1/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2024-05-04 14:47:23.000000 elm_messenger-0.3.1/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)     8028 2024-05-13 18:59:35.000000 elm_messenger-0.3.1/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2024-05-04 14:47:23.000000 elm_messenger-0.3.1/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2024-05-14 03:11:52.007553 elm_messenger-0.3.1/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2024-05-04 14:47:23.000000 elm_messenger-0.3.1/setup.py
+drwxr-xr-x   0 wayland   (1000) wayland   (1000)        0 2024-05-14 21:24:32.310885 elm_messenger-0.3.2/
+-rw-r--r--   0 wayland   (1000) wayland   (1000)       18 2024-05-12 21:23:16.000000 elm_messenger-0.3.2/MANIFEST.in
+-rw-r--r--   0 wayland   (1000) wayland   (1000)     7452 2024-05-14 21:24:32.310885 elm_messenger-0.3.2/PKG-INFO
+-rw-r--r--   0 wayland   (1000) wayland   (1000)     7181 2024-05-12 21:23:16.000000 elm_messenger-0.3.2/Readme.md
+drwxr-xr-x   0 wayland   (1000) wayland   (1000)        0 2024-05-14 21:24:32.310885 elm_messenger-0.3.2/elm_messenger.egg-info/
+-rw-r--r--   0 wayland   (1000) wayland   (1000)     7452 2024-05-14 21:24:32.000000 elm_messenger-0.3.2/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 wayland   (1000) wayland   (1000)      368 2024-05-14 21:24:32.000000 elm_messenger-0.3.2/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 wayland   (1000) wayland   (1000)        1 2024-05-14 21:24:32.000000 elm_messenger-0.3.2/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 wayland   (1000) wayland   (1000)       61 2024-05-14 21:24:32.000000 elm_messenger-0.3.2/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 wayland   (1000) wayland   (1000)        6 2024-05-14 21:24:32.000000 elm_messenger-0.3.2/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 wayland   (1000) wayland   (1000)       13 2024-05-14 21:24:32.000000 elm_messenger-0.3.2/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 wayland   (1000) wayland   (1000)        0 2024-05-14 21:24:32.310885 elm_messenger-0.3.2/messengercli/
+-rwxr-xr-x   0 wayland   (1000) wayland   (1000)        0 2024-05-12 21:23:17.000000 elm_messenger-0.3.2/messengercli/__init__.py
+-rwxr-xr-x   0 wayland   (1000) wayland   (1000)      120 2024-05-12 21:23:17.000000 elm_messenger-0.3.2/messengercli/command_line.py
+-rwxr-xr-x   0 wayland   (1000) wayland   (1000)    13990 2024-05-14 21:15:13.000000 elm_messenger-0.3.2/messengercli/messenger.py
+-rw-r--r--   0 wayland   (1000) wayland   (1000)     1170 2024-05-12 21:23:17.000000 elm_messenger-0.3.2/messengercli/updater.py
+-rw-r--r--   0 wayland   (1000) wayland   (1000)      392 2024-05-14 21:24:32.314885 elm_messenger-0.3.2/setup.cfg
+-rw-r--r--   0 wayland   (1000) wayland   (1000)      161 2024-05-12 21:23:17.000000 elm_messenger-0.3.2/setup.py
```

### Comparing `elm_messenger-0.3.1/PKG-INFO` & `elm_messenger-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: elm-messenger
-Version: 0.3.1
-Summary: The Messenger game framework toolkit for Elm
+Version: 0.3.2
+Summary: The Messenger toolkit for Elm
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: typer
```

### Comparing `elm_messenger-0.3.1/Readme.md` & `elm_messenger-0.3.2/Readme.md`

 * *Files identical despite different names*

### Comparing `elm_messenger-0.3.1/elm_messenger.egg-info/PKG-INFO` & `elm_messenger-0.3.2/elm_messenger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: elm-messenger
-Version: 0.3.1
-Summary: The Messenger game framework toolkit for Elm
+Version: 0.3.2
+Summary: The Messenger toolkit for Elm
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: typer
```

### Comparing `elm_messenger-0.3.1/messengercli/updater.py` & `elm_messenger-0.3.2/messengercli/updater.py`

 * *Files identical despite different names*

