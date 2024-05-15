# Comparing `tmp/smallneuron-1.2.0.tar.gz` & `tmp/smallneuron-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallneuron-1.2.0.tar", last modified: Wed May 15 20:51:46 2024, max compression
+gzip compressed data, was "smallneuron-1.2.1.tar", last modified: Wed May 15 21:12:06 2024, max compression
```

## Comparing `smallneuron-1.2.0.tar` & `smallneuron-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:51:46.263034 smallneuron-1.2.0/
--rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.2.0/.gitignore
--rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.2.0/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 20:51:46.263034 smallneuron-1.2.0/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.2.0/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.2.0/example.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-15 20:51:06.000000 smallneuron-1.2.0/pyproject.toml
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-15 20:51:46.263034 smallneuron-1.2.0/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:51:46.259034 smallneuron-1.2.0/src/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:51:46.263034 smallneuron-1.2.0/src/smallneuron/
--rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron/__init__.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron/build
--rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron/gpio_h3.c
--rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron/gpio_h3.h
--rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron/gpio_h3.so
--rw-rw-r--   0 andres    (1000) andres    (1000)     1733 2024-05-15 20:50:25.000000 smallneuron-1.2.0/src/smallneuron/logger.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    14106 2024-05-15 20:33:23.000000 smallneuron-1.2.0/src/smallneuron/smallneuron.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.2.0/src/smallneuron/snapi.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.2.0/src/smallneuron/sndummy.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.2.0/src/smallneuron/sngpio.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.2.0/src/smallneuron/sninput.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.2.0/src/smallneuron/snmqtt.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3334 2024-05-15 20:50:25.000000 smallneuron-1.2.0/src/smallneuron/snserial.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.2.0/src/smallneuron/sntimer.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:51:46.263034 smallneuron-1.2.0/src/smallneuron.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 20:51:46.000000 smallneuron-1.2.0/src/smallneuron.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-15 20:51:46.000000 smallneuron-1.2.0/src/smallneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-15 20:51:46.000000 smallneuron-1.2.0/src/smallneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-15 20:51:46.000000 smallneuron-1.2.0/src/smallneuron.egg-info/top_level.txt
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 20:51:46.263034 smallneuron-1.2.0/src/smallneuron_pelainux.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron_pelainux.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron_pelainux.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron_pelainux.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.2.0/src/smallneuron_pelainux.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:12:06.882379 smallneuron-1.2.1/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.2.1/.gitignore
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.2.1/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 21:12:06.882379 smallneuron-1.2.1/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.2.1/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.2.1/example.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-15 21:10:56.000000 smallneuron-1.2.1/pyproject.toml
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-15 21:12:06.882379 smallneuron-1.2.1/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:12:06.878379 smallneuron-1.2.1/src/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:12:06.882379 smallneuron-1.2.1/src/smallneuron/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron/__init__.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron/build
+-rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron/gpio_h3.c
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron/gpio_h3.h
+-rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron/gpio_h3.so
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1733 2024-05-15 20:50:25.000000 smallneuron-1.2.1/src/smallneuron/logger.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    14444 2024-05-15 21:10:56.000000 smallneuron-1.2.1/src/smallneuron/smallneuron.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.2.1/src/smallneuron/snapi.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.2.1/src/smallneuron/sndummy.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.2.1/src/smallneuron/sngpio.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.2.1/src/smallneuron/sninput.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.2.1/src/smallneuron/snmqtt.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3334 2024-05-15 20:50:25.000000 smallneuron-1.2.1/src/smallneuron/snserial.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.2.1/src/smallneuron/sntimer.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:12:06.882379 smallneuron-1.2.1/src/smallneuron.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-15 21:12:06.000000 smallneuron-1.2.1/src/smallneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-15 21:12:06.000000 smallneuron-1.2.1/src/smallneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-15 21:12:06.000000 smallneuron-1.2.1/src/smallneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-15 21:12:06.000000 smallneuron-1.2.1/src/smallneuron.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-15 21:12:06.882379 smallneuron-1.2.1/src/smallneuron_pelainux.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron_pelainux.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron_pelainux.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron_pelainux.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.2.1/src/smallneuron_pelainux.egg-info/top_level.txt
```

### Comparing `smallneuron-1.2.0/LICENSE` & `smallneuron-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/PKG-INFO` & `smallneuron-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.2.0
+Version: 1.2.1
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.2.0/README.md` & `smallneuron-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/example.py` & `smallneuron-1.2.1/example.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/pyproject.toml` & `smallneuron-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "smallneuron"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Andres Artigas", email="andres@artigas.cl" },
 ]
 description = "Small Neuron Workflow"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smallneuron-1.2.0/src/smallneuron/gpio_h3.c` & `smallneuron-1.2.1/src/smallneuron/gpio_h3.c`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/src/smallneuron/gpio_h3.h` & `smallneuron-1.2.1/src/smallneuron/gpio_h3.h`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/src/smallneuron/gpio_h3.so` & `smallneuron-1.2.1/src/smallneuron/gpio_h3.so`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/src/smallneuron/logger.py` & `smallneuron-1.2.1/src/smallneuron/logger.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/src/smallneuron/smallneuron.py` & `smallneuron-1.2.1/src/smallneuron/smallneuron.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,34 +237,40 @@
                 if type(params) == dict:
                     validUntil=params.pop("validUntil", self.count)
 
                 if validUntil < self.count:
                     log.warn("[",self.count,"] ", event, " is caduced ", validUntil, "<", self.count)
 
                 elif event in self.net:
+                    log.perfMark(f"     event in net")
                     if not self.currentState in self.net[event]:
                         log.warn("[",self.count,"] ", event, " not valid for state ", self.currentState, "discarted!")
                     else:
+                        log.perfMark(f"     get node")
                         node: Node = self.net[event][self.currentState][0]
                         log.info("[",self.count,"] entqer ", node.state, params, self.currentState)
                         
                         # indicamos al nodo actual que salimos
+                        log.perfMark(f"     leave old node")
                         self.currentNode.leave(event,params,node.state)
                         
                         # Entramos al nodo nuevo
+                        log.perfMark(f"     enter node")
                         node.enter(event, params, self.currentState)
                         self.currentNode=node
                         self.prevState = self.currentState
                         self.currentState = node.state
                         self.currentArgs = params
                         self.count = self.count + 1  # increment event count
+                        log.perfMark(f"     print graph")
                         self.printGraph(event)
                 elif event in self.cmds:
                     log.info("[", self.count, "] Manager new  cmd ", event)
                     node: Node = self.cmds[event][0]
+                    log.perfMark(f"     enter cmd")
                     node.enter(event, params, self.currentState)
                     self.printGraph(event)
                 else:
                     log.warn("[",self.count,"] ", event, " not exist")
         except Exception as e:
             log.error(e)
             log.error(traceback.format_exc())
```

### Comparing `smallneuron-1.2.0/src/smallneuron/snapi.py` & `smallneuron-1.2.1/src/smallneuron/snapi.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/src/smallneuron/sndummy.py` & `smallneuron-1.2.1/src/smallneuron/sndummy.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/src/smallneuron/sngpio.py` & `smallneuron-1.2.1/src/smallneuron/sngpio.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/src/smallneuron/sninput.py` & `smallneuron-1.2.1/src/smallneuron/sninput.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/src/smallneuron/snmqtt.py` & `smallneuron-1.2.1/src/smallneuron/snmqtt.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/src/smallneuron/snserial.py` & `smallneuron-1.2.1/src/smallneuron/snserial.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/src/smallneuron/sntimer.py` & `smallneuron-1.2.1/src/smallneuron/sntimer.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/src/smallneuron.egg-info/PKG-INFO` & `smallneuron-1.2.1/src/smallneuron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.2.0
+Version: 1.2.1
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.2.0/src/smallneuron.egg-info/SOURCES.txt` & `smallneuron-1.2.1/src/smallneuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smallneuron-1.2.0/src/smallneuron_pelainux.egg-info/PKG-INFO` & `smallneuron-1.2.1/src/smallneuron_pelainux.egg-info/PKG-INFO`

 * *Files identical despite different names*

