# Comparing `tmp/socketsecurity-0.0.47.tar.gz` & `tmp/socketsecurity-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.47.tar", last modified: Mon May 13 20:48:12 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.48.tar", last modified: Wed May 15 04:14:27 2024, max compression
```

## Comparing `socketsecurity-0.0.47.tar` & `socketsecurity-0.0.48.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:48:12.755473 socketsecurity-0.0.47/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      157 2024-05-13 20:48:12.755266 socketsecurity-0.0.47/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-13 20:48:12.755510 socketsecurity-0.0.47/setup.cfg
--rw-r--r--   0 douglascoburn   (501) staff       (20)      330 2024-05-13 20:48:06.000000 socketsecurity-0.0.47/setup.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:48:12.745590 socketsecurity-0.0.47/socketsecurity/
--rw-r--r--   0 douglascoburn   (501) staff       (20)       48 2024-05-13 20:30:22.000000 socketsecurity-0.0.47/socketsecurity/__init__.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:48:12.754825 socketsecurity-0.0.47/socketsecurity/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    25969 2024-05-13 20:48:06.000000 socketsecurity-0.0.47/socketsecurity/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     8665 2024-05-07 20:28:21.000000 socketsecurity-0.0.47/socketsecurity/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.47/socketsecurity/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11251 2024-05-08 17:15:58.000000 socketsecurity-0.0.47/socketsecurity/core/github.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11208 2024-05-05 18:30:58.000000 socketsecurity-0.0.47/socketsecurity/core/glitlab.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    67547 2024-05-05 17:36:53.000000 socketsecurity-0.0.47/socketsecurity/core/issues.py
--rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.47/socketsecurity/core/licenses.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11834 2024-05-08 17:02:42.000000 socketsecurity-0.0.47/socketsecurity/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     5457 2024-05-13 20:47:47.000000 socketsecurity-0.0.47/socketsecurity/socketcli.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:48:12.755054 socketsecurity-0.0.47/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      157 2024-05-13 20:48:12.000000 socketsecurity-0.0.47/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      545 2024-05-13 20:48:12.000000 socketsecurity-0.0.47/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-13 20:48:12.000000 socketsecurity-0.0.47/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-13 20:48:12.000000 socketsecurity-0.0.47/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-13 20:48:12.000000 socketsecurity-0.0.47/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-13 20:48:12.000000 socketsecurity-0.0.47/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-15 04:14:27.906189 socketsecurity-0.0.48/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      182 2024-05-15 04:14:27.905991 socketsecurity-0.0.48/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-15 04:14:27.906220 socketsecurity-0.0.48/setup.cfg
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      360 2024-05-15 04:13:31.000000 socketsecurity-0.0.48/setup.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-15 04:14:27.883848 socketsecurity-0.0.48/socketsecurity/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       48 2024-05-15 04:13:44.000000 socketsecurity-0.0.48/socketsecurity/__init__.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-15 04:14:27.905159 socketsecurity-0.0.48/socketsecurity/core/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    25969 2024-05-15 04:13:31.000000 socketsecurity-0.0.48/socketsecurity/core/__init__.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     8606 2024-05-13 22:21:02.000000 socketsecurity-0.0.48/socketsecurity/core/classes.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.48/socketsecurity/core/exceptions.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11251 2024-05-08 17:15:58.000000 socketsecurity-0.0.48/socketsecurity/core/github.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11208 2024-05-05 18:30:58.000000 socketsecurity-0.0.48/socketsecurity/core/glitlab.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    67547 2024-05-05 17:36:53.000000 socketsecurity-0.0.48/socketsecurity/core/issues.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.48/socketsecurity/core/licenses.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11834 2024-05-08 17:02:42.000000 socketsecurity-0.0.48/socketsecurity/core/messages.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     5457 2024-05-13 20:47:47.000000 socketsecurity-0.0.48/socketsecurity/socketcli.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-15 04:14:27.905676 socketsecurity-0.0.48/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      182 2024-05-15 04:14:27.000000 socketsecurity-0.0.48/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      545 2024-05-15 04:14:27.000000 socketsecurity-0.0.48/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-15 04:14:27.000000 socketsecurity-0.0.48/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-15 04:14:27.000000 socketsecurity-0.0.48/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-15 04:14:27.000000 socketsecurity-0.0.48/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-15 04:14:27.000000 socketsecurity-0.0.48/socketsecurity.egg-info/top_level.txt
```

### Comparing `socketsecurity-0.0.47/socketsecurity/core/__init__.py` & `socketsecurity-0.0.48/socketsecurity/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.47'
+__version__ = '0.0.48'
 __all__ = [
     "Core",
     "log"
 ]
 
 
 global encoded_key
```

### Comparing `socketsecurity-0.0.47/socketsecurity/core/classes.py` & `socketsecurity-0.0.48/socketsecurity/core/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,11 +363,7 @@
                 setattr(self, key, value)
         if not hasattr(self, "body_list"):
             self.body_list = []
 
     def __str__(self):
         return json.dumps(self.__dict__)
 
-class LicenseOutput(Purl):
-    licenses: list
-    license
-
```

### Comparing `socketsecurity-0.0.47/socketsecurity/core/exceptions.py` & `socketsecurity-0.0.48/socketsecurity/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.47/socketsecurity/core/github.py` & `socketsecurity-0.0.48/socketsecurity/core/github.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.47/socketsecurity/core/glitlab.py` & `socketsecurity-0.0.48/socketsecurity/core/glitlab.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.47/socketsecurity/core/issues.py` & `socketsecurity-0.0.48/socketsecurity/core/issues.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.47/socketsecurity/core/licenses.py` & `socketsecurity-0.0.48/socketsecurity/core/licenses.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.47/socketsecurity/core/messages.py` & `socketsecurity-0.0.48/socketsecurity/core/messages.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.47/socketsecurity/socketcli.py` & `socketsecurity-0.0.48/socketsecurity/socketcli.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.47/socketsecurity.egg-info/SOURCES.txt` & `socketsecurity-0.0.48/socketsecurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

