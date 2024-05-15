# Comparing `tmp/smallneuron-1.1.5.tar.gz` & `tmp/smallneuron-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallneuron-1.1.5.tar", last modified: Tue May 14 21:06:57 2024, max compression
+gzip compressed data, was "smallneuron-1.1.6.tar", last modified: Wed May 15 19:49:59 2024, max compression
```

## Comparing `smallneuron-1.1.5.tar` & `smallneuron-1.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 21:06:57.718116 smallneuron-1.1.5/
--rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.5/.gitignore
--rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.5/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-14 21:06:57.718116 smallneuron-1.1.5/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.1.5/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.5/example.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-14 21:06:00.000000 smallneuron-1.1.5/pyproject.toml
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-14 21:06:57.718116 smallneuron-1.1.5/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 21:06:57.714116 smallneuron-1.1.5/src/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 21:06:57.718116 smallneuron-1.1.5/src/smallneuron/
--rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron/__init__.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron/build
--rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron/gpio_h3.c
--rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron/gpio_h3.h
--rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron/gpio_h3.so
--rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.1.5/src/smallneuron/logger.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    13970 2024-05-13 15:29:30.000000 smallneuron-1.1.5/src/smallneuron/smallneuron.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.1.5/src/smallneuron/snapi.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.5/src/smallneuron/sndummy.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.5/src/smallneuron/sngpio.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.5/src/smallneuron/sninput.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.5/src/smallneuron/snmqtt.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3093 2024-05-14 21:05:38.000000 smallneuron-1.1.5/src/smallneuron/snserial.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.5/src/smallneuron/sntimer.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 21:06:57.718116 smallneuron-1.1.5/src/smallneuron.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-14 21:06:57.000000 smallneuron-1.1.5/src/smallneuron.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-14 21:06:57.000000 smallneuron-1.1.5/src/smallneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-14 21:06:57.000000 smallneuron-1.1.5/src/smallneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-14 21:06:57.000000 smallneuron-1.1.5/src/smallneuron.egg-info/top_level.txt
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 21:06:57.718116 smallneuron-1.1.5/src/smallneuron_pelainux.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron_pelainux.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron_pelainux.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron_pelainux.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron_pelainux.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:49:59.643151 smallneuron-1.1.6/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.6/.gitignore
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.6/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 19:49:59.643151 smallneuron-1.1.6/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.1.6/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.6/example.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-15 19:49:23.000000 smallneuron-1.1.6/pyproject.toml
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-15 19:49:59.643151 smallneuron-1.1.6/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:49:59.639150 smallneuron-1.1.6/src/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:49:59.643151 smallneuron-1.1.6/src/smallneuron/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron/__init__.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron/build
+-rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron/gpio_h3.c
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron/gpio_h3.h
+-rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron/gpio_h3.so
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.1.6/src/smallneuron/logger.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    14214 2024-05-15 19:49:08.000000 smallneuron-1.1.6/src/smallneuron/smallneuron.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.1.6/src/smallneuron/snapi.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.6/src/smallneuron/sndummy.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.6/src/smallneuron/sngpio.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.6/src/smallneuron/sninput.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.6/src/smallneuron/snmqtt.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3093 2024-05-14 21:05:38.000000 smallneuron-1.1.6/src/smallneuron/snserial.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.6/src/smallneuron/sntimer.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:49:59.643151 smallneuron-1.1.6/src/smallneuron.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 19:49:59.000000 smallneuron-1.1.6/src/smallneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-15 19:49:59.000000 smallneuron-1.1.6/src/smallneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-15 19:49:59.000000 smallneuron-1.1.6/src/smallneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-15 19:49:59.000000 smallneuron-1.1.6/src/smallneuron.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:49:59.643151 smallneuron-1.1.6/src/smallneuron_pelainux.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron_pelainux.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron_pelainux.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron_pelainux.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron_pelainux.egg-info/top_level.txt
```

### Comparing `smallneuron-1.1.5/LICENSE` & `smallneuron-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/PKG-INFO` & `smallneuron-1.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.5
+Version: 1.1.6
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.1.5/README.md` & `smallneuron-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/example.py` & `smallneuron-1.1.6/example.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/pyproject.toml` & `smallneuron-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "smallneuron"
-version = "1.1.5"
+version = "1.1.6"
 authors = [
   { name="Andres Artigas", email="andres@artigas.cl" },
 ]
 description = "Small Neuron Workflow"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smallneuron-1.1.5/src/smallneuron/gpio_h3.c` & `smallneuron-1.1.6/src/smallneuron/gpio_h3.c`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/src/smallneuron/gpio_h3.h` & `smallneuron-1.1.6/src/smallneuron/gpio_h3.h`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/src/smallneuron/gpio_h3.so` & `smallneuron-1.1.6/src/smallneuron/gpio_h3.so`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/src/smallneuron/logger.py` & `smallneuron-1.1.6/src/smallneuron/logger.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/src/smallneuron/smallneuron.py` & `smallneuron-1.1.6/src/smallneuron/smallneuron.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from time import sleep
+from time import sleep, time
 import threading
 import queue
 import re
 import os
 import json
 from .logger import Logger
 import traceback
@@ -68,14 +68,15 @@
         self.currentState = None
         self.currentArgs = None
         self.currentNode =None
         self.prevState = None
         self.count = 0 # state count
         self.graph_n = 0
         self.events = queue.SimpleQueue()
+        self.prev_time=time()
         self.net = (
             {}
         )  # estructura es { "evento1": { "estado Origen1" : (nodoDestino1, "event_desc1" ), "estadoOrigen2": (nodoDestino2, "event_desc2") }, "evento2"...
         self.cmds = (
             {}
         )  # estructura es { "evento1": (nodoDestino1, "event_desc1" ), "evento2": (nodoDestino2, "event_desc2")...
         self.graphDir=graphDir_and_prefix
@@ -90,16 +91,20 @@
         self.events.put((event, params, {})) # TODO: parece el el tercer argumento no se usa nunca
 
     def watchEvent(self,event, event_args={}, event_pattern=None, 
                 bridge=None, bridge_args={}, mode="loop",period=1):
                 watcher=SnWatcher(self,event,event_args, event_pattern)
                 watcher.run(bridge,bridge_args,mode,period)
                 return watcher
-
-
+    
+    def timeMark(self, text):
+        t=time()
+        print(text, t-self.prev_time, t)
+        self.prev_time=t
+ 
     def linkEdge(self, event, nodeFrom: Node, nodeTo: Node, desc=""):
         if event in self.cmds:
             print("Error event already in cmds ", event)
             raise "Error event already in cmds"
         elif event in self.net:
             if nodeFrom.state in self.net[event]:
                 print("Error edge already included ", event, nodeFrom, nodeTo)
@@ -219,15 +224,17 @@
         self.putEvent("_start_")  # lanzamos evento de inicio
 
     def loop(self):
         try:
             self.printGraph()
             while True:
                 log.notice("[",self.count,"] State:", self.currentState)
+                self.timeMark("event end:")
                 eventTuple = self.events.get()
+                self.timeMark("event start:")
                 event  = eventTuple[0]  # text del evento
                 params = eventTuple[1]  # argumentos del evento
 
                 log.notice("[",self.count,"] Event:", event, params)
                 
 
                 # eliminamos el validUntil, para que no quede en un loop
```

### Comparing `smallneuron-1.1.5/src/smallneuron/snapi.py` & `smallneuron-1.1.6/src/smallneuron/snapi.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/src/smallneuron/sndummy.py` & `smallneuron-1.1.6/src/smallneuron/sndummy.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/src/smallneuron/sngpio.py` & `smallneuron-1.1.6/src/smallneuron/sngpio.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/src/smallneuron/sninput.py` & `smallneuron-1.1.6/src/smallneuron/sninput.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/src/smallneuron/snmqtt.py` & `smallneuron-1.1.6/src/smallneuron/snmqtt.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/src/smallneuron/snserial.py` & `smallneuron-1.1.6/src/smallneuron/snserial.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/src/smallneuron/sntimer.py` & `smallneuron-1.1.6/src/smallneuron/sntimer.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/src/smallneuron.egg-info/PKG-INFO` & `smallneuron-1.1.6/src/smallneuron.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.5
+Version: 1.1.6
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.1.5/src/smallneuron.egg-info/SOURCES.txt` & `smallneuron-1.1.6/src/smallneuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.5/src/smallneuron_pelainux.egg-info/PKG-INFO` & `smallneuron-1.1.6/src/smallneuron_pelainux.egg-info/PKG-INFO`

 * *Files identical despite different names*

