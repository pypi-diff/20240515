# Comparing `tmp/smallneuron-1.1.8.tar.gz` & `tmp/smallneuron-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallneuron-1.1.8.tar", last modified: Wed May 15 20:23:17 2024, max compression
+gzip compressed data, was "smallneuron-1.1.9.tar", last modified: Wed May 15 20:34:01 2024, max compression
```

## Comparing `smallneuron-1.1.8.tar` & `smallneuron-1.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:23:17.670495 smallneuron-1.1.8/
--rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.8/.gitignore
--rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.8/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 20:23:17.670495 smallneuron-1.1.8/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.1.8/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.8/example.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-15 20:22:36.000000 smallneuron-1.1.8/pyproject.toml
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-15 20:23:17.670495 smallneuron-1.1.8/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:23:17.666495 smallneuron-1.1.8/src/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:23:17.670495 smallneuron-1.1.8/src/smallneuron/
--rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.8/src/smallneuron/__init__.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.8/src/smallneuron/build
--rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.8/src/smallneuron/gpio_h3.c
--rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.8/src/smallneuron/gpio_h3.h
--rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.8/src/smallneuron/gpio_h3.so
--rw-rw-r--   0 andres    (1000) andres    (1000)     1543 2024-05-15 20:22:36.000000 smallneuron-1.1.8/src/smallneuron/logger.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    14108 2024-05-15 20:22:36.000000 smallneuron-1.1.8/src/smallneuron/smallneuron.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.1.8/src/smallneuron/snapi.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.8/src/smallneuron/sndummy.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.8/src/smallneuron/sngpio.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.8/src/smallneuron/sninput.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.8/src/smallneuron/snmqtt.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3372 2024-05-15 20:22:36.000000 smallneuron-1.1.8/src/smallneuron/snserial.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.8/src/smallneuron/sntimer.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:23:17.670495 smallneuron-1.1.8/src/smallneuron.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 20:23:17.000000 smallneuron-1.1.8/src/smallneuron.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-15 20:23:17.000000 smallneuron-1.1.8/src/smallneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-15 20:23:17.000000 smallneuron-1.1.8/src/smallneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-15 20:23:17.000000 smallneuron-1.1.8/src/smallneuron.egg-info/top_level.txt
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:23:17.670495 smallneuron-1.1.8/src/smallneuron_pelainux.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.8/src/smallneuron_pelainux.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.8/src/smallneuron_pelainux.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.8/src/smallneuron_pelainux.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.8/src/smallneuron_pelainux.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:34:01.484450 smallneuron-1.1.9/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.9/.gitignore
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.9/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 20:34:01.484450 smallneuron-1.1.9/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.1.9/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.9/example.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-15 20:32:09.000000 smallneuron-1.1.9/pyproject.toml
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-15 20:34:01.484450 smallneuron-1.1.9/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:34:01.480450 smallneuron-1.1.9/src/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:34:01.480450 smallneuron-1.1.9/src/smallneuron/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron/__init__.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron/build
+-rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron/gpio_h3.c
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron/gpio_h3.h
+-rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron/gpio_h3.so
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1608 2024-05-15 20:33:23.000000 smallneuron-1.1.9/src/smallneuron/logger.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    14106 2024-05-15 20:33:23.000000 smallneuron-1.1.9/src/smallneuron/smallneuron.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.1.9/src/smallneuron/snapi.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.9/src/smallneuron/sndummy.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.9/src/smallneuron/sngpio.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.9/src/smallneuron/sninput.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.9/src/smallneuron/snmqtt.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3382 2024-05-15 20:33:23.000000 smallneuron-1.1.9/src/smallneuron/snserial.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.9/src/smallneuron/sntimer.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:34:01.484450 smallneuron-1.1.9/src/smallneuron.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 20:34:01.000000 smallneuron-1.1.9/src/smallneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-15 20:34:01.000000 smallneuron-1.1.9/src/smallneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-15 20:34:01.000000 smallneuron-1.1.9/src/smallneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-15 20:34:01.000000 smallneuron-1.1.9/src/smallneuron.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:34:01.484450 smallneuron-1.1.9/src/smallneuron_pelainux.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron_pelainux.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron_pelainux.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron_pelainux.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.9/src/smallneuron_pelainux.egg-info/top_level.txt
```

### Comparing `smallneuron-1.1.8/LICENSE` & `smallneuron-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/PKG-INFO` & `smallneuron-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.8
+Version: 1.1.9
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.1.8/README.md` & `smallneuron-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/example.py` & `smallneuron-1.1.9/example.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/pyproject.toml` & `smallneuron-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "smallneuron"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
   { name="Andres Artigas", email="andres@artigas.cl" },
 ]
 description = "Small Neuron Workflow"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smallneuron-1.1.8/src/smallneuron/gpio_h3.c` & `smallneuron-1.1.9/src/smallneuron/gpio_h3.c`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/src/smallneuron/gpio_h3.h` & `smallneuron-1.1.9/src/smallneuron/gpio_h3.h`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/src/smallneuron/gpio_h3.so` & `smallneuron-1.1.9/src/smallneuron/gpio_h3.so`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/src/smallneuron/logger.py` & `smallneuron-1.1.9/src/smallneuron/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import syslog
 from datetime import datetime
 from time import time
 import sys
 
 class Logger:
+    prev_log=time()
     logLevel=syslog.LOG_DEBUG
     def __init__(self, service_name):
         self.service_name = service_name
         self.prefix=""
 
     def error(self, *args):
         if syslog.LOG_ERR <= Logger.logLevel:
@@ -28,14 +29,19 @@
     def debug(self, *args):
         if syslog.LOG_DEBUG <= Logger.logLevel:
             self.__logger(syslog.LOG_DEBUG, *args)
 
     def set_level(level):
         Logger.logLevel=level
 
+    def perfMark(self,text):
+        t=time()
+        print(self.service_name, t, t-Logger.prev_time, text, file=sys.stderr)
+        Logger.prev_time=t
+        
     def __logger(self, severity, *args):
         try:
             syslog.openlog(self.service_name, syslog.LOG_CONS | syslog.LOG_PID | syslog.LOG_NDELAY, syslog.LOG_LOCAL1)
             msg = ""
             for a in args:
                 msg = msg + " " + str(a)
 
@@ -43,14 +49,9 @@
             syslog.closelog()
         except Exception as e:
             print("Syslog fail ", e)
 
     def ___current_full_date(self):
         return datetime.now().strftime("%d/%m/%Y %H:%M:%S")
     
-prev_time=time()
-def timeMark(text):
-    t=time()
-    print( t, t-prev_time, text, file=sys.stderr)
-    prev_time=t
```

### Comparing `smallneuron-1.1.8/src/smallneuron/smallneuron.py` & `smallneuron-1.1.9/src/smallneuron/smallneuron.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import sleep, time
 import threading
 import queue
 import re
 import os
 import json
-from .logger import Logger, timeMark
+from .logger import Logger
 import traceback
 from datetime import datetime
 import sys
 
 #
 # Para que funcione el tooltip debe set en formato svg, para generarlo usar:
 #
@@ -219,20 +219,20 @@
         self.putEvent("_start_")  # lanzamos evento de inicio
 
     def loop(self):
         try:
             self.printGraph()
             while True:
                 log.notice("[",self.count,"] State:", self.currentState)
-                timeMark("event end:")
+                log.perfMark("event end:")
                 eventTuple = self.events.get()
                 event  = eventTuple[0]  # text del evento
                 params = eventTuple[1]  # argumentos del evento
 
-                timeMark(f"[%d] start event %s"%(self.count,event))
+                log.perfMark(f"[%d] start event %s"%(self.count,event))
                 log.notice("[",self.count,"] Event:", event, params)
                 
 
                 # eliminamos el validUntil, para que no quede en un loop
                 validUntil=self.count
                 if type(params) == dict:
                     validUntil=params.pop("validUntil", self.count)
```

### Comparing `smallneuron-1.1.8/src/smallneuron/snapi.py` & `smallneuron-1.1.9/src/smallneuron/snapi.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/src/smallneuron/sndummy.py` & `smallneuron-1.1.9/src/smallneuron/sndummy.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/src/smallneuron/sngpio.py` & `smallneuron-1.1.9/src/smallneuron/sngpio.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/src/smallneuron/sninput.py` & `smallneuron-1.1.9/src/smallneuron/sninput.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/src/smallneuron/snmqtt.py` & `smallneuron-1.1.9/src/smallneuron/snmqtt.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/src/smallneuron/snserial.py` & `smallneuron-1.1.9/src/smallneuron/snserial.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 #
 import serial
 import time
 import re
 import threading
 import os.path
 import traceback
-from .logger import Logger, timeMark
+from .logger import Logger
 
 log=Logger("smallneuron.SnSerial")
 
 def eventWait(snserial):
     try:
         log.info("reader started")
         fails=0
         while True:
             try:
                 if not snserial.isOpen():
                     snserial.rotateOpen()
-                timeMark("eventWait read_until")
+                log.perfMark("eventWait read_until")
                 line = snserial.read_until(snserial.eol)
                 fails=0
                 for e in snserial.events:
                     if re.search(e[1], line) != None:
                         if snserial.eventManager == None:
                             log.error("Warning eventManager not defined")
                         else:
-                            timeMark("eventWait putEvent start")
+                            log.perfMark("eventWait putEvent start")
                             snserial.eventManager.putEvent(e[0], {"data": str(line)})
-                            timeMark("eventWait putEvent end")
+                            log.perfMark("eventWait putEvent end")
                         log.info("event ", e[0], line)
                         break
             except Exception as e:
-                timeMark("eventWait Exception")
+                log.perfMark("eventWait Exception")
                 fails=fails+1
                 if fails > 10:
                     raise("Falla multiples veces lectura serial "+str(fails))
                 log.warn("Reintentamos lectura "+str(e) )
                 time.sleep(1)
                 snserial.close()
                 
@@ -66,15 +66,15 @@
         self.events.append((event, pattern))
 
     def read_until(self, end_of_read_byte: bytes = b"\r"):
         line = b""
         c = b""
         while c != end_of_read_byte:
             c = self.read()
-            timeMark("read_until readChar")
+            log.perfMark("read_until readChar")
             line += c
         return line[:-1].decode("utf-8")
 
     def start(self):
         log.debug("SnSerial started")
         threading.Thread(target=lambda: eventWait(self)).start()
```

### Comparing `smallneuron-1.1.8/src/smallneuron/sntimer.py` & `smallneuron-1.1.9/src/smallneuron/sntimer.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/src/smallneuron.egg-info/PKG-INFO` & `smallneuron-1.1.9/src/smallneuron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.8
+Version: 1.1.9
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.1.8/src/smallneuron.egg-info/SOURCES.txt` & `smallneuron-1.1.9/src/smallneuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.8/src/smallneuron_pelainux.egg-info/PKG-INFO` & `smallneuron-1.1.9/src/smallneuron_pelainux.egg-info/PKG-INFO`

 * *Files identical despite different names*

