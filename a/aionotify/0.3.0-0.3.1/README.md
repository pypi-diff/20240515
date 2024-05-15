# Comparing `tmp/aionotify-0.3.0.tar.gz` & `tmp/aionotify-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aionotify-0.3.0.tar", last modified: Fri Feb  2 13:22:47 2024, max compression
+gzip compressed data, was "aionotify-0.3.1.tar", last modified: Wed May 15 17:05:23 2024, max compression
```

## Comparing `aionotify-0.3.0.tar` & `aionotify-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2024-02-02 13:22:47.312731 aionotify-0.3.0/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)       55 2024-02-02 13:22:46.000000 aionotify-0.3.0/.flake8
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      399 2024-02-02 13:22:46.000000 aionotify-0.3.0/CHANGES
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1610 2024-02-02 13:22:46.000000 aionotify-0.3.0/CREDITS
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      130 2024-02-02 13:22:46.000000 aionotify-0.3.0/INSTALL
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1304 2024-02-02 13:22:46.000000 aionotify-0.3.0/LICENSE
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      177 2024-02-02 13:22:46.000000 aionotify-0.3.0/MANIFEST.in
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1717 2024-02-02 13:22:46.000000 aionotify-0.3.0/Makefile
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3525 2024-02-02 13:22:47.312731 aionotify-0.3.0/PKG-INFO
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2218 2024-02-02 13:22:46.000000 aionotify-0.3.0/README.rst
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2024-02-02 13:22:47.309731 aionotify-0.3.0/aionotify/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      343 2024-02-02 13:22:46.000000 aionotify-0.3.0/aionotify/__init__.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     4410 2024-02-02 13:22:46.000000 aionotify-0.3.0/aionotify/aioutils.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     4075 2024-02-02 13:22:46.000000 aionotify-0.3.0/aionotify/base.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1388 2024-02-02 13:22:46.000000 aionotify-0.3.0/aionotify/enums.py
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2024-02-02 13:22:47.311731 aionotify-0.3.0/aionotify.egg-info/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3525 2024-02-02 13:22:47.000000 aionotify-0.3.0/aionotify.egg-info/PKG-INFO
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      478 2024-02-02 13:22:47.000000 aionotify-0.3.0/aionotify.egg-info/SOURCES.txt
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        1 2024-02-02 13:22:47.000000 aionotify-0.3.0/aionotify.egg-info/dependency_links.txt
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        1 2024-02-02 13:22:47.000000 aionotify-0.3.0/aionotify.egg-info/not-zip-safe
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      134 2024-02-02 13:22:47.000000 aionotify-0.3.0/aionotify.egg-info/requires.txt
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)       10 2024-02-02 13:22:47.000000 aionotify-0.3.0/aionotify.egg-info/top_level.txt
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2024-02-02 13:22:47.310731 aionotify-0.3.0/examples/
--rwxr-xr-x   0 xelnor    (1000) xelnet    (1000)     2035 2024-02-02 13:22:46.000000 aionotify-0.3.0/examples/print.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1291 2024-02-02 13:22:47.313731 aionotify-0.3.0/setup.cfg
--rwxr-xr-x   0 xelnor    (1000) xelnet    (1000)      171 2024-02-02 13:22:46.000000 aionotify-0.3.0/setup.py
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2024-02-02 13:22:47.311731 aionotify-0.3.0/tests/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2024-02-02 13:22:46.000000 aionotify-0.3.0/tests/__init__.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      412 2024-02-02 13:22:46.000000 aionotify-0.3.0/tests/test_enums.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     7046 2024-02-02 13:22:46.000000 aionotify-0.3.0/tests/test_usage.py
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2024-02-02 13:22:47.311731 aionotify-0.3.0/tests/testevents/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2024-02-02 13:22:46.000000 aionotify-0.3.0/tests/testevents/.keep_dir
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      272 2024-02-02 13:22:46.000000 aionotify-0.3.0/tox.ini
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2024-05-15 17:05:23.703376 aionotify-0.3.1/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)       55 2024-05-15 17:05:23.000000 aionotify-0.3.1/.flake8
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      506 2024-05-15 17:05:23.000000 aionotify-0.3.1/CHANGES
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1610 2024-05-15 17:05:23.000000 aionotify-0.3.1/CREDITS
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      130 2024-05-15 17:05:23.000000 aionotify-0.3.1/INSTALL
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1304 2024-05-15 17:05:23.000000 aionotify-0.3.1/LICENSE
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      177 2024-05-15 17:05:23.000000 aionotify-0.3.1/MANIFEST.in
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1717 2024-05-15 17:05:23.000000 aionotify-0.3.1/Makefile
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3525 2024-05-15 17:05:23.703376 aionotify-0.3.1/PKG-INFO
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2218 2024-05-15 17:05:23.000000 aionotify-0.3.1/README.rst
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2024-05-15 17:05:23.700376 aionotify-0.3.1/aionotify/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      343 2024-05-15 17:05:23.000000 aionotify-0.3.1/aionotify/__init__.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     4410 2024-05-15 17:05:23.000000 aionotify-0.3.1/aionotify/aioutils.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     4081 2024-05-15 17:05:23.000000 aionotify-0.3.1/aionotify/base.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1388 2024-05-15 17:05:23.000000 aionotify-0.3.1/aionotify/enums.py
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2024-05-15 17:05:23.701376 aionotify-0.3.1/aionotify.egg-info/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3525 2024-05-15 17:05:23.000000 aionotify-0.3.1/aionotify.egg-info/PKG-INFO
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      478 2024-05-15 17:05:23.000000 aionotify-0.3.1/aionotify.egg-info/SOURCES.txt
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        1 2024-05-15 17:05:23.000000 aionotify-0.3.1/aionotify.egg-info/dependency_links.txt
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        1 2024-05-15 17:05:23.000000 aionotify-0.3.1/aionotify.egg-info/not-zip-safe
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      134 2024-05-15 17:05:23.000000 aionotify-0.3.1/aionotify.egg-info/requires.txt
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)       10 2024-05-15 17:05:23.000000 aionotify-0.3.1/aionotify.egg-info/top_level.txt
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2024-05-15 17:05:23.700376 aionotify-0.3.1/examples/
+-rwxr-xr-x   0 xelnor    (1000) xelnet    (1000)     2035 2024-05-15 17:05:23.000000 aionotify-0.3.1/examples/print.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1291 2024-05-15 17:05:23.703376 aionotify-0.3.1/setup.cfg
+-rwxr-xr-x   0 xelnor    (1000) xelnet    (1000)      171 2024-05-15 17:05:23.000000 aionotify-0.3.1/setup.py
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2024-05-15 17:05:23.701376 aionotify-0.3.1/tests/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2024-05-15 17:05:23.000000 aionotify-0.3.1/tests/__init__.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      412 2024-05-15 17:05:23.000000 aionotify-0.3.1/tests/test_enums.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     7481 2024-05-15 17:05:23.000000 aionotify-0.3.1/tests/test_usage.py
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2024-05-15 17:05:23.701376 aionotify-0.3.1/tests/testevents/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2024-05-15 17:05:23.000000 aionotify-0.3.1/tests/testevents/.keep_dir
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      272 2024-05-15 17:05:23.000000 aionotify-0.3.1/tox.ini
```

### Comparing `aionotify-0.3.0/CREDITS` & `aionotify-0.3.1/CREDITS`

 * *Files identical despite different names*

### Comparing `aionotify-0.3.0/LICENSE` & `aionotify-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aionotify-0.3.0/Makefile` & `aionotify-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `aionotify-0.3.0/PKG-INFO` & `aionotify-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aionotify
-Version: 0.3.0
+Version: 0.3.1
 Summary: Asyncio-powered inotify library
 Home-page: https://github.com/rbarrois/aionotify
 Author: Raphaël Barrois
 Author-email: raphael.barrois+aionotify@polytechnique.org
 License: BSD
 Keywords: asyncio,inotify
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aionotify-0.3.0/README.rst` & `aionotify-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `aionotify-0.3.0/aionotify/aioutils.py` & `aionotify-0.3.1/aionotify/aioutils.py`

 * *Files identical despite different names*

### Comparing `aionotify-0.3.0/aionotify/base.py` & `aionotify-0.3.1/aionotify/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         self._loop = loop or asyncio.get_running_loop()
 
         self._fd = LibC.inotify_init()
         for alias, (path, flags) in self.requests.items():
             self._setup_watch(alias, path, flags)
 
         # We pass ownership of the fd to the transport; it will close it.
-        self._stream, self._transport = await aioutils.stream_from_fd(self._fd, loop)
+        self._stream, self._transport = await aioutils.stream_from_fd(self._fd, self._loop)
 
     def close(self):
         """Schedule closure.
 
         This will close the transport and all related resources.
         """
         self._transport.close()
```

### Comparing `aionotify-0.3.0/aionotify/enums.py` & `aionotify-0.3.1/aionotify/enums.py`

 * *Files identical despite different names*

### Comparing `aionotify-0.3.0/aionotify.egg-info/PKG-INFO` & `aionotify-0.3.1/aionotify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aionotify
-Version: 0.3.0
+Version: 0.3.1
 Summary: Asyncio-powered inotify library
 Home-page: https://github.com/rbarrois/aionotify
 Author: Raphaël Barrois
 Author-email: raphael.barrois+aionotify@polytechnique.org
 License: BSD
 Keywords: asyncio,inotify
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aionotify-0.3.0/examples/print.py` & `aionotify-0.3.1/examples/print.py`

 * *Files identical despite different names*

### Comparing `aionotify-0.3.0/setup.cfg` & `aionotify-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aionotify
-version = 0.3.0
+version = 0.3.1
 description = Asyncio-powered inotify library
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Raphaël Barrois
 author_email = raphael.barrois+aionotify@polytechnique.org
 url = https://github.com/rbarrois/aionotify
 keywords = asyncio, inotify
```

### Comparing `aionotify-0.3.0/tests/test_usage.py` & `aionotify-0.3.1/tests/test_usage.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,14 +97,27 @@
         self._touch('a')
         event = await self.watcher.get_event()
         self._assert_file_event(event, 'a')
 
         # And it's over.
         await self._assert_no_events()
 
+    async def test_watch_before_start_default_loop(self):
+        """A watch call is valid before startup."""
+        self.watcher.watch(self.testdir, aionotify.Flags.CREATE)
+        await self.watcher.setup()
+
+        # Touch a file: we get the event.
+        self._touch('a')
+        event = await self.watcher.get_event()
+        self._assert_file_event(event, 'a')
+
+        # And it's over.
+        await self._assert_no_events()
+
     async def test_watch_after_start(self):
         """A watch call is valid after startup."""
         await self.watcher.setup(self.loop)
         self.watcher.watch(self.testdir, aionotify.Flags.CREATE)
 
         # Touch a file: we get the event.
         self._touch('a')
```

