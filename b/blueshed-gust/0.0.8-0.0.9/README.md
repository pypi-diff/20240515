# Comparing `tmp/blueshed_gust-0.0.8.tar.gz` & `tmp/blueshed_gust-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueshed_gust-0.0.8.tar", last modified: Wed May  8 15:27:30 2024, max compression
+gzip compressed data, was "blueshed_gust-0.0.9.tar", last modified: Wed May  8 17:10:52 2024, max compression
```

## Comparing `blueshed_gust-0.0.8.tar` & `blueshed_gust-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 15:27:30.935524 blueshed_gust-0.0.8/
--rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-08 15:27:30.935353 blueshed_gust-0.0.8/PKG-INFO
--rw-r--r--   0 peterb     (501) staff       (20)      320 2024-05-06 13:29:02.000000 blueshed_gust-0.0.8/README.md
--rw-r--r--   0 peterb     (501) staff       (20)     1879 2024-05-08 15:27:27.000000 blueshed_gust-0.0.8/pyproject.toml
--rw-r--r--   0 peterb     (501) staff       (20)       38 2024-05-08 15:27:30.935562 blueshed_gust-0.0.8/setup.cfg
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 15:27:30.932225 blueshed_gust-0.0.8/src/
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 15:27:30.932163 blueshed_gust-0.0.8/src/blueshed/
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 15:27:30.933956 blueshed_gust-0.0.8/src/blueshed/gust/
--rw-r--r--   0 peterb     (501) staff       (20)      145 2024-05-08 15:27:27.000000 blueshed_gust-0.0.8/src/blueshed/gust/__init__.py
--rw-r--r--   0 peterb     (501) staff       (20)      754 2024-05-06 10:00:21.000000 blueshed_gust-0.0.8/src/blueshed/gust/configs.py
--rw-r--r--   0 peterb     (501) staff       (20)      801 2024-05-07 21:45:19.000000 blueshed_gust-0.0.8/src/blueshed/gust/context.py
--rw-r--r--   0 peterb     (501) staff       (20)     1416 2024-05-06 10:00:21.000000 blueshed_gust-0.0.8/src/blueshed/gust/json_utils.py
--rw-r--r--   0 peterb     (501) staff       (20)     2494 2024-05-08 15:26:10.000000 blueshed_gust-0.0.8/src/blueshed/gust/main.py
--rw-r--r--   0 peterb     (501) staff       (20)     3829 2024-05-06 14:08:50.000000 blueshed_gust-0.0.8/src/blueshed/gust/routes.py
--rw-r--r--   0 peterb     (501) staff       (20)      919 2024-05-06 10:00:21.000000 blueshed_gust-0.0.8/src/blueshed/gust/static_file_handler.py
--rw-r--r--   0 peterb     (501) staff       (20)     2599 2024-05-06 13:33:43.000000 blueshed_gust-0.0.8/src/blueshed/gust/utils.py
--rw-r--r--   0 peterb     (501) staff       (20)       67 2024-05-06 13:33:43.000000 blueshed_gust-0.0.8/src/blueshed/gust/web.py
--rw-r--r--   0 peterb     (501) staff       (20)     2269 2024-05-07 21:46:04.000000 blueshed_gust-0.0.8/src/blueshed/gust/web_handler.py
--rw-r--r--   0 peterb     (501) staff       (20)     5676 2024-05-07 21:46:16.000000 blueshed_gust-0.0.8/src/blueshed/gust/websocket.py
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 15:27:30.934847 blueshed_gust-0.0.8/src/blueshed_gust.egg-info/
--rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-08 15:27:30.000000 blueshed_gust-0.0.8/src/blueshed_gust.egg-info/PKG-INFO
--rw-r--r--   0 peterb     (501) staff       (20)      559 2024-05-08 15:27:30.000000 blueshed_gust-0.0.8/src/blueshed_gust.egg-info/SOURCES.txt
--rw-r--r--   0 peterb     (501) staff       (20)        1 2024-05-08 15:27:30.000000 blueshed_gust-0.0.8/src/blueshed_gust.egg-info/dependency_links.txt
--rw-r--r--   0 peterb     (501) staff       (20)      124 2024-05-08 15:27:30.000000 blueshed_gust-0.0.8/src/blueshed_gust.egg-info/requires.txt
--rw-r--r--   0 peterb     (501) staff       (20)        9 2024-05-08 15:27:30.000000 blueshed_gust-0.0.8/src/blueshed_gust.egg-info/top_level.txt
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 17:10:52.633855 blueshed_gust-0.0.9/
+-rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-08 17:10:52.633680 blueshed_gust-0.0.9/PKG-INFO
+-rw-r--r--   0 peterb     (501) staff       (20)      320 2024-05-06 13:29:02.000000 blueshed_gust-0.0.9/README.md
+-rw-r--r--   0 peterb     (501) staff       (20)     1879 2024-05-08 17:10:49.000000 blueshed_gust-0.0.9/pyproject.toml
+-rw-r--r--   0 peterb     (501) staff       (20)       38 2024-05-08 17:10:52.633900 blueshed_gust-0.0.9/setup.cfg
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 17:10:52.630550 blueshed_gust-0.0.9/src/
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 17:10:52.630490 blueshed_gust-0.0.9/src/blueshed/
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 17:10:52.632303 blueshed_gust-0.0.9/src/blueshed/gust/
+-rw-r--r--   0 peterb     (501) staff       (20)      145 2024-05-08 17:10:49.000000 blueshed_gust-0.0.9/src/blueshed/gust/__init__.py
+-rw-r--r--   0 peterb     (501) staff       (20)      754 2024-05-06 10:00:21.000000 blueshed_gust-0.0.9/src/blueshed/gust/configs.py
+-rw-r--r--   0 peterb     (501) staff       (20)      801 2024-05-07 21:45:19.000000 blueshed_gust-0.0.9/src/blueshed/gust/context.py
+-rw-r--r--   0 peterb     (501) staff       (20)     1416 2024-05-06 10:00:21.000000 blueshed_gust-0.0.9/src/blueshed/gust/json_utils.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2526 2024-05-08 17:10:32.000000 blueshed_gust-0.0.9/src/blueshed/gust/main.py
+-rw-r--r--   0 peterb     (501) staff       (20)     3829 2024-05-06 14:08:50.000000 blueshed_gust-0.0.9/src/blueshed/gust/routes.py
+-rw-r--r--   0 peterb     (501) staff       (20)      919 2024-05-06 10:00:21.000000 blueshed_gust-0.0.9/src/blueshed/gust/static_file_handler.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2599 2024-05-06 13:33:43.000000 blueshed_gust-0.0.9/src/blueshed/gust/utils.py
+-rw-r--r--   0 peterb     (501) staff       (20)       67 2024-05-06 13:33:43.000000 blueshed_gust-0.0.9/src/blueshed/gust/web.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2269 2024-05-07 21:46:04.000000 blueshed_gust-0.0.9/src/blueshed/gust/web_handler.py
+-rw-r--r--   0 peterb     (501) staff       (20)     5676 2024-05-07 21:46:16.000000 blueshed_gust-0.0.9/src/blueshed/gust/websocket.py
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 17:10:52.633127 blueshed_gust-0.0.9/src/blueshed_gust.egg-info/
+-rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-08 17:10:52.000000 blueshed_gust-0.0.9/src/blueshed_gust.egg-info/PKG-INFO
+-rw-r--r--   0 peterb     (501) staff       (20)      559 2024-05-08 17:10:52.000000 blueshed_gust-0.0.9/src/blueshed_gust.egg-info/SOURCES.txt
+-rw-r--r--   0 peterb     (501) staff       (20)        1 2024-05-08 17:10:52.000000 blueshed_gust-0.0.9/src/blueshed_gust.egg-info/dependency_links.txt
+-rw-r--r--   0 peterb     (501) staff       (20)      124 2024-05-08 17:10:52.000000 blueshed_gust-0.0.9/src/blueshed_gust.egg-info/requires.txt
+-rw-r--r--   0 peterb     (501) staff       (20)        9 2024-05-08 17:10:52.000000 blueshed_gust-0.0.9/src/blueshed_gust.egg-info/top_level.txt
```

### Comparing `blueshed_gust-0.0.8/PKG-INFO` & `blueshed_gust-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueshed-gust
-Version: 0.0.8
+Version: 0.0.9
 Summary: a library.
 Author-email: Peter Bunyan <pete@blueshed.co.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
```

### Comparing `blueshed_gust-0.0.8/pyproject.toml` & `blueshed_gust-0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,14 @@
 
 [tool.coverage.run]
 data_file = ".venv/cache/.coverage"
 [tool.coverage.report]
 data_file = ".venv/cache/.coverage"
 
 [tool.bumpversion]
-current_version = "0.0.8"
+current_version = "0.0.9"
 commit = false
 tag = true
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "src/blueshed/gust/__init__.py"
```

### Comparing `blueshed_gust-0.0.8/src/blueshed/gust/configs.py` & `blueshed_gust-0.0.9/src/blueshed/gust/configs.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.8/src/blueshed/gust/context.py` & `blueshed_gust-0.0.9/src/blueshed/gust/context.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.8/src/blueshed/gust/json_utils.py` & `blueshed_gust-0.0.9/src/blueshed/gust/json_utils.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.8/src/blueshed/gust/main.py` & `blueshed_gust-0.0.9/src/blueshed/gust/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,11 +70,11 @@
         if self.settings.get('debug') is True:
             log.info('running in debug mode')
 
         await asyncio.Event().wait()
 
     def run(self):  # pragma: no cover
         try:
-            asyncio.run(self._run_())
+            asyncio.get_event_loop().run_until_complete(self._run_())
         except (KeyboardInterrupt, SystemExit):
             # graceful shutdown
             pass
```

### Comparing `blueshed_gust-0.0.8/src/blueshed/gust/routes.py` & `blueshed_gust-0.0.9/src/blueshed/gust/routes.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.8/src/blueshed/gust/static_file_handler.py` & `blueshed_gust-0.0.9/src/blueshed/gust/static_file_handler.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.8/src/blueshed/gust/utils.py` & `blueshed_gust-0.0.9/src/blueshed/gust/utils.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.8/src/blueshed/gust/web_handler.py` & `blueshed_gust-0.0.9/src/blueshed/gust/web_handler.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.8/src/blueshed/gust/websocket.py` & `blueshed_gust-0.0.9/src/blueshed/gust/websocket.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.8/src/blueshed_gust.egg-info/PKG-INFO` & `blueshed_gust-0.0.9/src/blueshed_gust.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueshed-gust
-Version: 0.0.8
+Version: 0.0.9
 Summary: a library.
 Author-email: Peter Bunyan <pete@blueshed.co.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
```

### Comparing `blueshed_gust-0.0.8/src/blueshed_gust.egg-info/SOURCES.txt` & `blueshed_gust-0.0.9/src/blueshed_gust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

