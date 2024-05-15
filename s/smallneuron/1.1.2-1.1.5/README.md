# Comparing `tmp/smallneuron-1.1.2.tar.gz` & `tmp/smallneuron-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallneuron-1.1.2.tar", last modified: Tue May 14 20:54:50 2024, max compression
+gzip compressed data, was "smallneuron-1.1.5.tar", last modified: Tue May 14 21:06:57 2024, max compression
```

## Comparing `smallneuron-1.1.2.tar` & `smallneuron-1.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 20:54:50.790821 smallneuron-1.1.2/
--rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.2/.gitignore
--rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.2/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-14 20:54:50.790821 smallneuron-1.1.2/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.1.2/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.2/example.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-14 20:53:12.000000 smallneuron-1.1.2/pyproject.toml
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-14 20:54:50.790821 smallneuron-1.1.2/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 20:54:50.782821 smallneuron-1.1.2/src/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 20:54:50.786821 smallneuron-1.1.2/src/smallneuron/
--rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron/__init__.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron/build
--rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron/gpio_h3.c
--rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron/gpio_h3.h
--rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron/gpio_h3.so
--rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.1.2/src/smallneuron/logger.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    13970 2024-05-13 15:29:30.000000 smallneuron-1.1.2/src/smallneuron/smallneuron.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.1.2/src/smallneuron/snapi.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.2/src/smallneuron/sndummy.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.2/src/smallneuron/sngpio.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.2/src/smallneuron/sninput.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.2/src/smallneuron/snmqtt.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3094 2024-05-14 20:50:23.000000 smallneuron-1.1.2/src/smallneuron/snserial.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.2/src/smallneuron/sntimer.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 20:54:50.786821 smallneuron-1.1.2/src/smallneuron.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-14 20:54:50.000000 smallneuron-1.1.2/src/smallneuron.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-14 20:54:50.000000 smallneuron-1.1.2/src/smallneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-14 20:54:50.000000 smallneuron-1.1.2/src/smallneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-14 20:54:50.000000 smallneuron-1.1.2/src/smallneuron.egg-info/top_level.txt
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 20:54:50.786821 smallneuron-1.1.2/src/smallneuron_pelainux.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron_pelainux.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron_pelainux.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron_pelainux.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron_pelainux.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 21:06:57.718116 smallneuron-1.1.5/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.5/.gitignore
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.5/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-14 21:06:57.718116 smallneuron-1.1.5/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.1.5/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.5/example.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-14 21:06:00.000000 smallneuron-1.1.5/pyproject.toml
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-14 21:06:57.718116 smallneuron-1.1.5/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 21:06:57.714116 smallneuron-1.1.5/src/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 21:06:57.718116 smallneuron-1.1.5/src/smallneuron/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron/__init__.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron/build
+-rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron/gpio_h3.c
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron/gpio_h3.h
+-rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron/gpio_h3.so
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.1.5/src/smallneuron/logger.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    13970 2024-05-13 15:29:30.000000 smallneuron-1.1.5/src/smallneuron/smallneuron.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.1.5/src/smallneuron/snapi.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.5/src/smallneuron/sndummy.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.5/src/smallneuron/sngpio.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.5/src/smallneuron/sninput.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.5/src/smallneuron/snmqtt.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3093 2024-05-14 21:05:38.000000 smallneuron-1.1.5/src/smallneuron/snserial.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.5/src/smallneuron/sntimer.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 21:06:57.718116 smallneuron-1.1.5/src/smallneuron.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-14 21:06:57.000000 smallneuron-1.1.5/src/smallneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-14 21:06:57.000000 smallneuron-1.1.5/src/smallneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-14 21:06:57.000000 smallneuron-1.1.5/src/smallneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-14 21:06:57.000000 smallneuron-1.1.5/src/smallneuron.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 21:06:57.718116 smallneuron-1.1.5/src/smallneuron_pelainux.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron_pelainux.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron_pelainux.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron_pelainux.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.5/src/smallneuron_pelainux.egg-info/top_level.txt
```

### Comparing `smallneuron-1.1.2/LICENSE` & `smallneuron-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/PKG-INFO` & `smallneuron-1.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.2
+Version: 1.1.5
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.1.2/README.md` & `smallneuron-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/example.py` & `smallneuron-1.1.5/example.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/pyproject.toml` & `smallneuron-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "smallneuron"
-version = "1.1.2"
+version = "1.1.5"
 authors = [
   { name="Andres Artigas", email="andres@artigas.cl" },
 ]
 description = "Small Neuron Workflow"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smallneuron-1.1.2/src/smallneuron/gpio_h3.c` & `smallneuron-1.1.5/src/smallneuron/gpio_h3.c`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/src/smallneuron/gpio_h3.h` & `smallneuron-1.1.5/src/smallneuron/gpio_h3.h`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/src/smallneuron/gpio_h3.so` & `smallneuron-1.1.5/src/smallneuron/gpio_h3.so`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/src/smallneuron/logger.py` & `smallneuron-1.1.5/src/smallneuron/logger.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/src/smallneuron/smallneuron.py` & `smallneuron-1.1.5/src/smallneuron/smallneuron.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/src/smallneuron/snapi.py` & `smallneuron-1.1.5/src/smallneuron/snapi.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/src/smallneuron/sndummy.py` & `smallneuron-1.1.5/src/smallneuron/sndummy.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/src/smallneuron/sngpio.py` & `smallneuron-1.1.5/src/smallneuron/sngpio.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/src/smallneuron/sninput.py` & `smallneuron-1.1.5/src/smallneuron/sninput.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/src/smallneuron/snmqtt.py` & `smallneuron-1.1.5/src/smallneuron/snmqtt.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/src/smallneuron/snserial.py` & `smallneuron-1.1.5/src/smallneuron/snserial.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                             snserial.eventManager.putEvent(e[0], {"data": str(line)})
                         log.info("event ", e[0], line)
                         break
             except Exception as e:
                 fails=fails+1
                 if fails > 10:
                     raise("Falla multiples veces lectura serial "+str(fails))
-                log.error("Reintentamos lectura "+str(e) )
+                log.warn("Reintentamos lectura "+str(e) )
                 time.sleep(1)
                 snserial.close()
                 
     except Exception as e:
         log.error(e)
         log.error(traceback.format_exc())
         snserial.eventManager.putEvent("panic", str(e))
```

### Comparing `smallneuron-1.1.2/src/smallneuron/sntimer.py` & `smallneuron-1.1.5/src/smallneuron/sntimer.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/src/smallneuron.egg-info/PKG-INFO` & `smallneuron-1.1.5/src/smallneuron.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.2
+Version: 1.1.5
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.1.2/src/smallneuron.egg-info/SOURCES.txt` & `smallneuron-1.1.5/src/smallneuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.2/src/smallneuron_pelainux.egg-info/PKG-INFO` & `smallneuron-1.1.5/src/smallneuron_pelainux.egg-info/PKG-INFO`

 * *Files identical despite different names*

