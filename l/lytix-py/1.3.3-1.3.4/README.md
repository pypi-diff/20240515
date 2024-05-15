# Comparing `tmp/lytix_py-1.3.3.tar.gz` & `tmp/lytix_py-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytix_py-1.3.3.tar", last modified: Mon May 13 18:47:34 2024, max compression
+gzip compressed data, was "lytix_py-1.3.4.tar", last modified: Wed May 15 17:31:35 2024, max compression
```

## Comparing `lytix_py-1.3.3.tar` & `lytix_py-1.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:47:34.836047 lytix_py-1.3.3/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.3.3/LICENSE.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-13 18:47:34.835833 lytix_py-1.3.3/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.3.3/README.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-13 18:47:17.000000 lytix_py-1.3.3/pyproject.toml
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-13 18:47:34.836103 lytix_py-1.3.3/setup.cfg
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:47:34.833182 lytix_py-1.3.3/src/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:47:34.834401 lytix_py-1.3.3/src/lytix_py/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:47:34.835081 lytix_py-1.3.3/src/lytix_py/LLLogger/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      886 2024-05-06 00:20:17.000000 lytix_py-1.3.3/src/lytix_py/LLLogger/LLLogger.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:47:34.835190 lytix_py-1.3.3/src/lytix_py/MetricCollector/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     2794 2024-05-13 18:46:14.000000 lytix_py-1.3.3/src/lytix_py/MetricCollector/MetricCollector.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      133 2024-05-13 18:41:07.000000 lytix_py-1.3.3/src/lytix_py/__init__.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      658 2024-05-13 18:47:25.000000 lytix_py-1.3.3/src/lytix_py/envVars.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:47:34.835603 lytix_py-1.3.3/src/lytix_py.egg-info/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-13 18:47:34.000000 lytix_py-1.3.3/src/lytix_py.egg-info/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      345 2024-05-13 18:47:34.000000 lytix_py-1.3.3/src/lytix_py.egg-info/SOURCES.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-13 18:47:34.000000 lytix_py-1.3.3/src/lytix_py.egg-info/dependency_links.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-13 18:47:34.000000 lytix_py-1.3.3/src/lytix_py.egg-info/requires.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-13 18:47:34.000000 lytix_py-1.3.3/src/lytix_py.egg-info/top_level.txt
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-15 17:31:35.025112 lytix_py-1.3.4/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.3.4/LICENSE.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-15 17:31:35.024877 lytix_py-1.3.4/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.3.4/README.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-15 17:31:09.000000 lytix_py-1.3.4/pyproject.toml
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-15 17:31:35.025156 lytix_py-1.3.4/setup.cfg
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-15 17:31:35.022989 lytix_py-1.3.4/src/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-15 17:31:35.023706 lytix_py-1.3.4/src/lytix_py/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-15 17:31:35.024376 lytix_py-1.3.4/src/lytix_py/LLLogger/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      886 2024-05-06 00:20:17.000000 lytix_py-1.3.4/src/lytix_py/LLLogger/LLLogger.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-15 17:31:35.024505 lytix_py-1.3.4/src/lytix_py/MetricCollector/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     2815 2024-05-15 17:30:42.000000 lytix_py-1.3.4/src/lytix_py/MetricCollector/MetricCollector.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      133 2024-05-13 18:41:07.000000 lytix_py-1.3.4/src/lytix_py/__init__.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      658 2024-05-13 18:47:25.000000 lytix_py-1.3.4/src/lytix_py/envVars.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-15 17:31:35.024679 lytix_py-1.3.4/src/lytix_py.egg-info/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-15 17:31:35.000000 lytix_py-1.3.4/src/lytix_py.egg-info/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      345 2024-05-15 17:31:35.000000 lytix_py-1.3.4/src/lytix_py.egg-info/SOURCES.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-15 17:31:35.000000 lytix_py-1.3.4/src/lytix_py.egg-info/dependency_links.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-15 17:31:35.000000 lytix_py-1.3.4/src/lytix_py.egg-info/requires.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-15 17:31:35.000000 lytix_py-1.3.4/src/lytix_py.egg-info/top_level.txt
```

### Comparing `lytix_py-1.3.3/LICENSE.md` & `lytix_py-1.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.3/PKG-INFO` & `lytix_py-1.3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.3.3
+Version: 1.3.4
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lytix_py-1.3.3/pyproject.toml` & `lytix_py-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lytix-py"
-version = "1.3.3"
+version = "1.3.4"
 authors = [
   { name="Lytix", email="support@lytix.com" },
 ]
 description = "Official Lytix Client Packages"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lytix_py-1.3.3/src/lytix_py/LLLogger/LLLogger.py` & `lytix_py-1.3.4/src/lytix_py/LLLogger/LLLogger.py`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.3/src/lytix_py/MetricCollector/MetricCollector.py` & `lytix_py-1.3.4/src/lytix_py/MetricCollector/MetricCollector.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,25 +62,25 @@
             "metricMetadata": metricMetadata
         }
         self._sendPostRequest("modelIO", body)
 
     """
     Capture a model io event while also capturing the time to respond
     """
-    def captureModelTrace(self, modelName: str, userInput: str, callback, metricMetadata: dict = None):
+    def captureModelTrace(self, modelName: str, userInput: str, callback, metricMetadata: dict = {}):
         if LytixCreds.LX_API_KEY is None: 
             return callback()
 
         startTime = time.time()
         modelOutput = callback()
         try:
             responseTime = int((time.time() - startTime) * 1000)  # Convert to milliseconds
             # Capture modelIO event along with the response time
             self.captureModelIO(modelName, userInput, modelOutput, metricMetadata)
-            self.increment("model.responseTime", responseTime, {"modelName": modelName})
+            self.increment("model.responseTime", responseTime, {"modelName": modelName}.update(metricMetadata))
         except Exception as err:
             self.logger.error(f"Failed to capture model trace: {err}", err, modelName, userInput)
             raise err
         finally:
             return modelOutput
 
 MetricCollector = _MetricCollector()
```

### Comparing `lytix_py-1.3.3/src/lytix_py/envVars.py` & `lytix_py-1.3.4/src/lytix_py/envVars.py`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.3/src/lytix_py.egg-info/PKG-INFO` & `lytix_py-1.3.4/src/lytix_py.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.3.3
+Version: 1.3.4
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

