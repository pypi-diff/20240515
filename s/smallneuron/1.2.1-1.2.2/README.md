# Comparing `tmp/smallneuron-1.2.1.tar.gz` & `tmp/smallneuron-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallneuron-1.2.1.tar", last modified: Wed May 15 21:12:06 2024, max compression
+gzip compressed data, was "smallneuron-1.2.2.tar", last modified: Wed May 15 21:28:54 2024, max compression
```

## Comparing `smallneuron-1.2.1.tar` & `smallneuron-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:12:06.882379 smallneuron-1.2.1/
--rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.2.1/.gitignore
--rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.2.1/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 21:12:06.882379 smallneuron-1.2.1/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.2.1/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.2.1/example.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-15 21:10:56.000000 smallneuron-1.2.1/pyproject.toml
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-15 21:12:06.882379 smallneuron-1.2.1/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:12:06.878379 smallneuron-1.2.1/src/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:12:06.882379 smallneuron-1.2.1/src/smallneuron/
--rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron/__init__.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron/build
--rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron/gpio_h3.c
--rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron/gpio_h3.h
--rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron/gpio_h3.so
--rw-rw-r--   0 andres    (1000) andres    (1000)     1733 2024-05-15 20:50:25.000000 smallneuron-1.2.1/src/smallneuron/logger.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    14444 2024-05-15 21:10:56.000000 smallneuron-1.2.1/src/smallneuron/smallneuron.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.2.1/src/smallneuron/snapi.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.2.1/src/smallneuron/sndummy.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.2.1/src/smallneuron/sngpio.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.2.1/src/smallneuron/sninput.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.2.1/src/smallneuron/snmqtt.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3334 2024-05-15 20:50:25.000000 smallneuron-1.2.1/src/smallneuron/snserial.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.2.1/src/smallneuron/sntimer.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:12:06.882379 smallneuron-1.2.1/src/smallneuron.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 21:12:06.000000 smallneuron-1.2.1/src/smallneuron.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-15 21:12:06.000000 smallneuron-1.2.1/src/smallneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-15 21:12:06.000000 smallneuron-1.2.1/src/smallneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-15 21:12:06.000000 smallneuron-1.2.1/src/smallneuron.egg-info/top_level.txt
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:12:06.882379 smallneuron-1.2.1/src/smallneuron_pelainux.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron_pelainux.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron_pelainux.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron_pelainux.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron_pelainux.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:28:54.972277 smallneuron-1.2.2/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.2.2/.gitignore
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.2.2/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 21:28:54.972277 smallneuron-1.2.2/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.2.2/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.2.2/example.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-15 21:28:29.000000 smallneuron-1.2.2/pyproject.toml
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-15 21:28:54.972277 smallneuron-1.2.2/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:28:54.968277 smallneuron-1.2.2/src/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:28:54.968277 smallneuron-1.2.2/src/smallneuron/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.2.2/src/smallneuron/__init__.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.2.2/src/smallneuron/build
+-rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.2.2/src/smallneuron/gpio_h3.c
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.2.2/src/smallneuron/gpio_h3.h
+-rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.2.2/src/smallneuron/gpio_h3.so
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1733 2024-05-15 20:50:25.000000 smallneuron-1.2.2/src/smallneuron/logger.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    14351 2024-05-15 21:26:53.000000 smallneuron-1.2.2/src/smallneuron/smallneuron.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.2.2/src/smallneuron/snapi.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.2.2/src/smallneuron/sndummy.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.2.2/src/smallneuron/sngpio.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.2.2/src/smallneuron/sninput.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.2.2/src/smallneuron/snmqtt.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3334 2024-05-15 20:50:25.000000 smallneuron-1.2.2/src/smallneuron/snserial.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.2.2/src/smallneuron/sntimer.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:28:54.972277 smallneuron-1.2.2/src/smallneuron.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 21:28:54.000000 smallneuron-1.2.2/src/smallneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-15 21:28:54.000000 smallneuron-1.2.2/src/smallneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-15 21:28:54.000000 smallneuron-1.2.2/src/smallneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-15 21:28:54.000000 smallneuron-1.2.2/src/smallneuron.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:28:54.972277 smallneuron-1.2.2/src/smallneuron_pelainux.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.2.2/src/smallneuron_pelainux.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.2.2/src/smallneuron_pelainux.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.2.2/src/smallneuron_pelainux.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.2.2/src/smallneuron_pelainux.egg-info/top_level.txt
```

### Comparing `smallneuron-1.2.1/LICENSE` & `smallneuron-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/PKG-INFO` & `smallneuron-1.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.2.1
+Version: 1.2.2
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.2.1/README.md` & `smallneuron-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/example.py` & `smallneuron-1.2.2/example.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/pyproject.toml` & `smallneuron-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "smallneuron"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Andres Artigas", email="andres@artigas.cl" },
 ]
 description = "Small Neuron Workflow"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smallneuron-1.2.1/src/smallneuron/gpio_h3.c` & `smallneuron-1.2.2/src/smallneuron/gpio_h3.c`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/src/smallneuron/gpio_h3.h` & `smallneuron-1.2.2/src/smallneuron/gpio_h3.h`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/src/smallneuron/gpio_h3.so` & `smallneuron-1.2.2/src/smallneuron/gpio_h3.so`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/src/smallneuron/logger.py` & `smallneuron-1.2.2/src/smallneuron/logger.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/src/smallneuron/smallneuron.py` & `smallneuron-1.2.2/src/smallneuron/smallneuron.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,18 @@
         self.style = style
         self._cmd=False
         if state in Node.nodelist:
             raise "Estado ya existe como Nodo" + state
         Node.nodelist[state] = self
 
     def enter(self, event, args, stateFrom):
-        pass #  print("Node: Enter:", self.state, "event trigger:", event, "from", stateFrom)
+        log.perfMark("     In Node.enter()")
 
     def leave(self, event, args, stateTo):
-        pass # print("Node: Leave:", self.state, "event trigger:", event, "to", stateTo)
+        log.perfMark("     In Node.leave()")
 
     def __eq__(self, other):
         return self.state == other.state
 
 
 class LambdaNode(Node):
     def __init__(self, state, lambdaEnter, desc="", style=""):
```

### Comparing `smallneuron-1.2.1/src/smallneuron/snapi.py` & `smallneuron-1.2.2/src/smallneuron/snapi.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/src/smallneuron/sndummy.py` & `smallneuron-1.2.2/src/smallneuron/sndummy.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/src/smallneuron/sngpio.py` & `smallneuron-1.2.2/src/smallneuron/sngpio.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/src/smallneuron/sninput.py` & `smallneuron-1.2.2/src/smallneuron/sninput.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/src/smallneuron/snmqtt.py` & `smallneuron-1.2.2/src/smallneuron/snmqtt.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/src/smallneuron/snserial.py` & `smallneuron-1.2.2/src/smallneuron/snserial.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/src/smallneuron/sntimer.py` & `smallneuron-1.2.2/src/smallneuron/sntimer.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/src/smallneuron.egg-info/PKG-INFO` & `smallneuron-1.2.2/src/smallneuron.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.2.1
+Version: 1.2.2
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.2.1/src/smallneuron.egg-info/SOURCES.txt` & `smallneuron-1.2.2/src/smallneuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.1/src/smallneuron_pelainux.egg-info/PKG-INFO` & `smallneuron-1.2.2/src/smallneuron_pelainux.egg-info/PKG-INFO`

 * *Files identical despite different names*

