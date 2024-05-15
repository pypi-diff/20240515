# Comparing `tmp/playpty-0.1.0.tar.gz` & `tmp/playpty-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playpty-0.1.0.tar", last modified: Thu May  9 16:08:50 2024, max compression
+gzip compressed data, was "playpty-0.1.1.tar", last modified: Wed May 15 12:23:14 2024, max compression
```

## Comparing `playpty-0.1.0.tar` & `playpty-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-05-09 16:08:50.127932 playpty-0.1.0/
--rw-r--r--   0 zsm        (501) staff       (20)     1070 2024-05-09 12:50:47.000000 playpty-0.1.0/LICENSE
--rw-r--r--   0 zsm        (501) staff       (20)     2210 2024-05-09 16:08:50.127732 playpty-0.1.0/PKG-INFO
--rw-r--r--   0 zsm        (501) staff       (20)      167 2024-05-09 14:42:26.000000 playpty-0.1.0/README.md
--rw-r--r--   0 zsm        (501) staff       (20)     1384 2024-05-09 15:55:36.000000 playpty-0.1.0/pyproject.toml
--rw-r--r--   0 zsm        (501) staff       (20)       38 2024-05-09 16:08:50.127974 playpty-0.1.0/setup.cfg
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-05-09 16:08:50.126398 playpty-0.1.0/src/
--rw-r--r--   0 zsm        (501) staff       (20)        0 2024-05-09 14:00:01.000000 playpty-0.1.0/src/__init__.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-05-09 16:08:50.126647 playpty-0.1.0/src/playpty/
--rw-r--r--   0 zsm        (501) staff       (20)       23 2024-05-09 13:39:06.000000 playpty-0.1.0/src/playpty/__init__.py
--rw-r--r--   0 zsm        (501) staff       (20)     3863 2024-05-09 15:54:35.000000 playpty-0.1.0/src/playpty/playpty.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-05-09 16:08:50.127531 playpty-0.1.0/src/playpty.egg-info/
--rw-r--r--   0 zsm        (501) staff       (20)     2210 2024-05-09 16:08:50.000000 playpty-0.1.0/src/playpty.egg-info/PKG-INFO
--rw-r--r--   0 zsm        (501) staff       (20)      273 2024-05-09 16:08:50.000000 playpty-0.1.0/src/playpty.egg-info/SOURCES.txt
--rw-r--r--   0 zsm        (501) staff       (20)        1 2024-05-09 16:08:50.000000 playpty-0.1.0/src/playpty.egg-info/dependency_links.txt
--rw-r--r--   0 zsm        (501) staff       (20)       41 2024-05-09 16:08:50.000000 playpty-0.1.0/src/playpty.egg-info/entry_points.txt
--rw-r--r--   0 zsm        (501) staff       (20)       17 2024-05-09 16:08:50.000000 playpty-0.1.0/src/playpty.egg-info/top_level.txt
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-05-15 12:23:14.899574 playpty-0.1.1/
+-rw-r--r--   0 zsm        (501) staff       (20)     1070 2024-05-09 12:50:47.000000 playpty-0.1.1/LICENSE
+-rw-r--r--   0 zsm        (501) staff       (20)     2210 2024-05-15 12:23:14.899362 playpty-0.1.1/PKG-INFO
+-rw-r--r--   0 zsm        (501) staff       (20)      167 2024-05-09 14:42:26.000000 playpty-0.1.1/README.md
+-rw-r--r--   0 zsm        (501) staff       (20)     1384 2024-05-15 12:20:01.000000 playpty-0.1.1/pyproject.toml
+-rw-r--r--   0 zsm        (501) staff       (20)       38 2024-05-15 12:23:14.899625 playpty-0.1.1/setup.cfg
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-05-15 12:23:14.898029 playpty-0.1.1/src/
+-rw-r--r--   0 zsm        (501) staff       (20)        0 2024-05-09 14:00:01.000000 playpty-0.1.1/src/__init__.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-05-15 12:23:14.898260 playpty-0.1.1/src/playpty/
+-rw-r--r--   0 zsm        (501) staff       (20)       23 2024-05-09 13:39:06.000000 playpty-0.1.1/src/playpty/__init__.py
+-rw-r--r--   0 zsm        (501) staff       (20)     3842 2024-05-09 17:19:24.000000 playpty-0.1.1/src/playpty/playpty.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2024-05-15 12:23:14.899135 playpty-0.1.1/src/playpty.egg-info/
+-rw-r--r--   0 zsm        (501) staff       (20)     2210 2024-05-15 12:23:14.000000 playpty-0.1.1/src/playpty.egg-info/PKG-INFO
+-rw-r--r--   0 zsm        (501) staff       (20)      273 2024-05-15 12:23:14.000000 playpty-0.1.1/src/playpty.egg-info/SOURCES.txt
+-rw-r--r--   0 zsm        (501) staff       (20)        1 2024-05-15 12:23:14.000000 playpty-0.1.1/src/playpty.egg-info/dependency_links.txt
+-rw-r--r--   0 zsm        (501) staff       (20)       41 2024-05-15 12:23:14.000000 playpty-0.1.1/src/playpty.egg-info/entry_points.txt
+-rw-r--r--   0 zsm        (501) staff       (20)       17 2024-05-15 12:23:14.000000 playpty-0.1.1/src/playpty.egg-info/top_level.txt
```

### Comparing `playpty-0.1.0/LICENSE` & `playpty-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `playpty-0.1.0/PKG-INFO` & `playpty-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playpty
-Version: 0.1.0
+Version: 0.1.1
 Summary: Play script in pty
 Author-email: wzshiming <wzshiming@foxmail.com>
 License: MIT License
         
         Copyright (c) 2024 Shiming Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `playpty-0.1.0/pyproject.toml` & `playpty-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "playpty"
-version = "0.1.0"
+version = "0.1.1"
 description = "Play script in pty"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["playpty"]
 authors = [
   {name = "wzshiming", email = "wzshiming@foxmail.com" }
```

### Comparing `playpty-0.1.0/src/playpty/playpty.py` & `playpty-0.1.1/src/playpty/playpty.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         time.sleep(0.1)
 
 
 def write_with_delay(fd: int, content: str, delay: float):
     global last_typing
     for idx, c in enumerate(content):
         os.write(fd, c.encode())
-        os.fsync(fd)
         if idx == len(content) - 1:
             last_typing = time.time()
         time.sleep(delay)
 
 
 def clear_header(fd: int):
     while True:
```

### Comparing `playpty-0.1.0/src/playpty.egg-info/PKG-INFO` & `playpty-0.1.1/src/playpty.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playpty
-Version: 0.1.0
+Version: 0.1.1
 Summary: Play script in pty
 Author-email: wzshiming <wzshiming@foxmail.com>
 License: MIT License
         
         Copyright (c) 2024 Shiming Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

