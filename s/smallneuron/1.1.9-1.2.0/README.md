# Comparing `tmp/smallneuron-1.1.9.tar.gz` & `tmp/smallneuron-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallneuron-1.1.9.tar", last modified: Wed May 15 20:34:01 2024, max compression
+gzip compressed data, was "smallneuron-1.2.0.tar", last modified: Wed May 15 20:51:46 2024, max compression
```

## Comparing `smallneuron-1.1.9.tar` & `smallneuron-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:34:01.484450 smallneuron-1.1.9/
--rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.9/.gitignore
--rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.9/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 20:34:01.484450 smallneuron-1.1.9/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.1.9/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.9/example.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-15 20:32:09.000000 smallneuron-1.1.9/pyproject.toml
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-15 20:34:01.484450 smallneuron-1.1.9/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:34:01.480450 smallneuron-1.1.9/src/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:34:01.480450 smallneuron-1.1.9/src/smallneuron/
--rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron/__init__.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron/build
--rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron/gpio_h3.c
--rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron/gpio_h3.h
--rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron/gpio_h3.so
--rw-rw-r--   0 andres    (1000) andres    (1000)     1608 2024-05-15 20:33:23.000000 smallneuron-1.1.9/src/smallneuron/logger.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    14106 2024-05-15 20:33:23.000000 smallneuron-1.1.9/src/smallneuron/smallneuron.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.1.9/src/smallneuron/snapi.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.9/src/smallneuron/sndummy.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.9/src/smallneuron/sngpio.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.9/src/smallneuron/sninput.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.9/src/smallneuron/snmqtt.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3382 2024-05-15 20:33:23.000000 smallneuron-1.1.9/src/smallneuron/snserial.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.9/src/smallneuron/sntimer.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:34:01.484450 smallneuron-1.1.9/src/smallneuron.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 20:34:01.000000 smallneuron-1.1.9/src/smallneuron.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-15 20:34:01.000000 smallneuron-1.1.9/src/smallneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-15 20:34:01.000000 smallneuron-1.1.9/src/smallneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-15 20:34:01.000000 smallneuron-1.1.9/src/smallneuron.egg-info/top_level.txt
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:34:01.484450 smallneuron-1.1.9/src/smallneuron_pelainux.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron_pelainux.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron_pelainux.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron_pelainux.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron_pelainux.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:51:46.263034 smallneuron-1.2.0/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.2.0/.gitignore
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.2.0/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 20:51:46.263034 smallneuron-1.2.0/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.2.0/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.2.0/example.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-15 20:51:06.000000 smallneuron-1.2.0/pyproject.toml
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-15 20:51:46.263034 smallneuron-1.2.0/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:51:46.259034 smallneuron-1.2.0/src/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:51:46.263034 smallneuron-1.2.0/src/smallneuron/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron/__init__.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron/build
+-rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron/gpio_h3.c
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron/gpio_h3.h
+-rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron/gpio_h3.so
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1733 2024-05-15 20:50:25.000000 smallneuron-1.2.0/src/smallneuron/logger.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    14106 2024-05-15 20:33:23.000000 smallneuron-1.2.0/src/smallneuron/smallneuron.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.2.0/src/smallneuron/snapi.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.2.0/src/smallneuron/sndummy.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.2.0/src/smallneuron/sngpio.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.2.0/src/smallneuron/sninput.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.2.0/src/smallneuron/snmqtt.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3334 2024-05-15 20:50:25.000000 smallneuron-1.2.0/src/smallneuron/snserial.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.2.0/src/smallneuron/sntimer.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:51:46.263034 smallneuron-1.2.0/src/smallneuron.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 20:51:46.000000 smallneuron-1.2.0/src/smallneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-15 20:51:46.000000 smallneuron-1.2.0/src/smallneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-15 20:51:46.000000 smallneuron-1.2.0/src/smallneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-15 20:51:46.000000 smallneuron-1.2.0/src/smallneuron.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:51:46.263034 smallneuron-1.2.0/src/smallneuron_pelainux.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron_pelainux.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron_pelainux.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron_pelainux.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron_pelainux.egg-info/top_level.txt
```

### Comparing `smallneuron-1.1.9/LICENSE` & `smallneuron-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/PKG-INFO` & `smallneuron-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.9
+Version: 1.2.0
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.1.9/README.md` & `smallneuron-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/example.py` & `smallneuron-1.2.0/example.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/pyproject.toml` & `smallneuron-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "smallneuron"
-version = "1.1.9"
+version = "1.2.0"
 authors = [
   { name="Andres Artigas", email="andres@artigas.cl" },
 ]
 description = "Small Neuron Workflow"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smallneuron-1.1.9/src/smallneuron/gpio_h3.c` & `smallneuron-1.2.0/src/smallneuron/gpio_h3.c`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/src/smallneuron/gpio_h3.h` & `smallneuron-1.2.0/src/smallneuron/gpio_h3.h`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/src/smallneuron/gpio_h3.so` & `smallneuron-1.2.0/src/smallneuron/gpio_h3.so`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/src/smallneuron/logger.py` & `smallneuron-1.2.0/src/smallneuron/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import syslog
 from datetime import datetime
 from time import time
 import sys
 
 class Logger:
-    prev_log=time()
+    perf_enable=False
+    prev_time=time()
     logLevel=syslog.LOG_DEBUG
     def __init__(self, service_name):
         self.service_name = service_name
         self.prefix=""
 
     def error(self, *args):
         if syslog.LOG_ERR <= Logger.logLevel:
@@ -29,18 +30,22 @@
     def debug(self, *args):
         if syslog.LOG_DEBUG <= Logger.logLevel:
             self.__logger(syslog.LOG_DEBUG, *args)
 
     def set_level(level):
         Logger.logLevel=level
 
+    def set_perf(setOn):
+        Logger.perf_enable=setOn
+
     def perfMark(self,text):
-        t=time()
-        print(self.service_name, t, t-Logger.prev_time, text, file=sys.stderr)
-        Logger.prev_time=t
+        if Logger.perf_enable:
+            t=time()
+            print(self.service_name, t, t-Logger.prev_time, text, file=sys.stderr)
+            Logger.prev_time=t
         
     def __logger(self, severity, *args):
         try:
             syslog.openlog(self.service_name, syslog.LOG_CONS | syslog.LOG_PID | syslog.LOG_NDELAY, syslog.LOG_LOCAL1)
             msg = ""
             for a in args:
                 msg = msg + " " + str(a)
```

### Comparing `smallneuron-1.1.9/src/smallneuron/smallneuron.py` & `smallneuron-1.2.0/src/smallneuron/smallneuron.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/src/smallneuron/snapi.py` & `smallneuron-1.2.0/src/smallneuron/snapi.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/src/smallneuron/sndummy.py` & `smallneuron-1.2.0/src/smallneuron/sndummy.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/src/smallneuron/sngpio.py` & `smallneuron-1.2.0/src/smallneuron/sngpio.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/src/smallneuron/sninput.py` & `smallneuron-1.2.0/src/smallneuron/sninput.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/src/smallneuron/snmqtt.py` & `smallneuron-1.2.0/src/smallneuron/snmqtt.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/src/smallneuron/snserial.py` & `smallneuron-1.2.0/src/smallneuron/snserial.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         self.events.append((event, pattern))
 
     def read_until(self, end_of_read_byte: bytes = b"\r"):
         line = b""
         c = b""
         while c != end_of_read_byte:
             c = self.read()
-            log.perfMark("read_until readChar")
             line += c
         return line[:-1].decode("utf-8")
 
     def start(self):
         log.debug("SnSerial started")
         threading.Thread(target=lambda: eventWait(self)).start()
```

### Comparing `smallneuron-1.1.9/src/smallneuron/sntimer.py` & `smallneuron-1.2.0/src/smallneuron/sntimer.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/src/smallneuron.egg-info/PKG-INFO` & `smallneuron-1.2.0/src/smallneuron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.9
+Version: 1.2.0
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.1.9/src/smallneuron.egg-info/SOURCES.txt` & `smallneuron-1.2.0/src/smallneuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.9/src/smallneuron_pelainux.egg-info/PKG-INFO` & `smallneuron-1.2.0/src/smallneuron_pelainux.egg-info/PKG-INFO`

 * *Files identical despite different names*

