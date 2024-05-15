# Comparing `tmp/smallneuron-1.1.6.tar.gz` & `tmp/smallneuron-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallneuron-1.1.6.tar", last modified: Wed May 15 19:49:59 2024, max compression
+gzip compressed data, was "smallneuron-1.1.7.tar", last modified: Wed May 15 19:57:41 2024, max compression
```

## Comparing `smallneuron-1.1.6.tar` & `smallneuron-1.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:49:59.643151 smallneuron-1.1.6/
--rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.6/.gitignore
--rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.6/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 19:49:59.643151 smallneuron-1.1.6/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.1.6/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.6/example.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-15 19:49:23.000000 smallneuron-1.1.6/pyproject.toml
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-15 19:49:59.643151 smallneuron-1.1.6/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:49:59.639150 smallneuron-1.1.6/src/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:49:59.643151 smallneuron-1.1.6/src/smallneuron/
--rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron/__init__.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron/build
--rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron/gpio_h3.c
--rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron/gpio_h3.h
--rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron/gpio_h3.so
--rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.1.6/src/smallneuron/logger.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    14214 2024-05-15 19:49:08.000000 smallneuron-1.1.6/src/smallneuron/smallneuron.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.1.6/src/smallneuron/snapi.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.6/src/smallneuron/sndummy.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.6/src/smallneuron/sngpio.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.6/src/smallneuron/sninput.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.6/src/smallneuron/snmqtt.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3093 2024-05-14 21:05:38.000000 smallneuron-1.1.6/src/smallneuron/snserial.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.6/src/smallneuron/sntimer.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:49:59.643151 smallneuron-1.1.6/src/smallneuron.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 19:49:59.000000 smallneuron-1.1.6/src/smallneuron.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-15 19:49:59.000000 smallneuron-1.1.6/src/smallneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-15 19:49:59.000000 smallneuron-1.1.6/src/smallneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-15 19:49:59.000000 smallneuron-1.1.6/src/smallneuron.egg-info/top_level.txt
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:49:59.643151 smallneuron-1.1.6/src/smallneuron_pelainux.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron_pelainux.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron_pelainux.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron_pelainux.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.6/src/smallneuron_pelainux.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:57:41.256169 smallneuron-1.1.7/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.7/.gitignore
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.7/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 19:57:41.256169 smallneuron-1.1.7/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.1.7/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.7/example.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-15 19:57:12.000000 smallneuron-1.1.7/pyproject.toml
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-15 19:57:41.256169 smallneuron-1.1.7/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:57:41.252169 smallneuron-1.1.7/src/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:57:41.256169 smallneuron-1.1.7/src/smallneuron/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.7/src/smallneuron/__init__.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.7/src/smallneuron/build
+-rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.7/src/smallneuron/gpio_h3.c
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.7/src/smallneuron/gpio_h3.h
+-rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.7/src/smallneuron/gpio_h3.so
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.1.7/src/smallneuron/logger.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    14243 2024-05-15 19:56:30.000000 smallneuron-1.1.7/src/smallneuron/smallneuron.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.1.7/src/smallneuron/snapi.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.7/src/smallneuron/sndummy.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.7/src/smallneuron/sngpio.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.7/src/smallneuron/sninput.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.7/src/smallneuron/snmqtt.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3093 2024-05-14 21:05:38.000000 smallneuron-1.1.7/src/smallneuron/snserial.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.7/src/smallneuron/sntimer.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:57:41.256169 smallneuron-1.1.7/src/smallneuron.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 19:57:41.000000 smallneuron-1.1.7/src/smallneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-15 19:57:41.000000 smallneuron-1.1.7/src/smallneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-15 19:57:41.000000 smallneuron-1.1.7/src/smallneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-15 19:57:41.000000 smallneuron-1.1.7/src/smallneuron.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 19:57:41.256169 smallneuron-1.1.7/src/smallneuron_pelainux.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.7/src/smallneuron_pelainux.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.7/src/smallneuron_pelainux.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.7/src/smallneuron_pelainux.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.7/src/smallneuron_pelainux.egg-info/top_level.txt
```

### Comparing `smallneuron-1.1.6/LICENSE` & `smallneuron-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/PKG-INFO` & `smallneuron-1.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.6
+Version: 1.1.7
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.1.6/README.md` & `smallneuron-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/example.py` & `smallneuron-1.1.7/example.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/pyproject.toml` & `smallneuron-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "smallneuron"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
   { name="Andres Artigas", email="andres@artigas.cl" },
 ]
 description = "Small Neuron Workflow"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smallneuron-1.1.6/src/smallneuron/gpio_h3.c` & `smallneuron-1.1.7/src/smallneuron/gpio_h3.c`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/src/smallneuron/gpio_h3.h` & `smallneuron-1.1.7/src/smallneuron/gpio_h3.h`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/src/smallneuron/gpio_h3.so` & `smallneuron-1.1.7/src/smallneuron/gpio_h3.so`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/src/smallneuron/logger.py` & `smallneuron-1.1.7/src/smallneuron/logger.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/src/smallneuron/smallneuron.py` & `smallneuron-1.1.7/src/smallneuron/smallneuron.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import queue
 import re
 import os
 import json
 from .logger import Logger
 import traceback
 from datetime import datetime
+import sys
 
 #
 # Para que funcione el tooltip debe set en formato svg, para generarlo usar:
 #
 #    dot -Tsvg -osmallneuron.svg smallneuron.dot
 #
 # Despues visualizar smallneuron.svg con chrome
@@ -94,15 +95,15 @@
                 bridge=None, bridge_args={}, mode="loop",period=1):
                 watcher=SnWatcher(self,event,event_args, event_pattern)
                 watcher.run(bridge,bridge_args,mode,period)
                 return watcher
     
     def timeMark(self, text):
         t=time()
-        print(text, t-self.prev_time, t)
+        print( text, t-self.prev_time, t, file=sys.stderr)
         self.prev_time=t
  
     def linkEdge(self, event, nodeFrom: Node, nodeTo: Node, desc=""):
         if event in self.cmds:
             print("Error event already in cmds ", event)
             raise "Error event already in cmds"
         elif event in self.net:
```

### Comparing `smallneuron-1.1.6/src/smallneuron/snapi.py` & `smallneuron-1.1.7/src/smallneuron/snapi.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/src/smallneuron/sndummy.py` & `smallneuron-1.1.7/src/smallneuron/sndummy.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/src/smallneuron/sngpio.py` & `smallneuron-1.1.7/src/smallneuron/sngpio.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/src/smallneuron/sninput.py` & `smallneuron-1.1.7/src/smallneuron/sninput.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/src/smallneuron/snmqtt.py` & `smallneuron-1.1.7/src/smallneuron/snmqtt.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/src/smallneuron/snserial.py` & `smallneuron-1.1.7/src/smallneuron/snserial.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/src/smallneuron/sntimer.py` & `smallneuron-1.1.7/src/smallneuron/sntimer.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/src/smallneuron.egg-info/PKG-INFO` & `smallneuron-1.1.7/src/smallneuron.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.6
+Version: 1.1.7
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.1.6/src/smallneuron.egg-info/SOURCES.txt` & `smallneuron-1.1.7/src/smallneuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.6/src/smallneuron_pelainux.egg-info/PKG-INFO` & `smallneuron-1.1.7/src/smallneuron_pelainux.egg-info/PKG-INFO`

 * *Files identical despite different names*

