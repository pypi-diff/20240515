# Comparing `tmp/ns1-python-0.9.18.tar.gz` & `tmp/ns1-python-0.9.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ns1-python-0.9.18.tar", last modified: Wed Feb 28 19:30:50 2018, max compression
+gzip compressed data, was "dist/ns1-python-0.9.19.tar", last modified: Thu Mar 14 16:41:17 2019, max compression
```

## Comparing `ns1-python-0.9.18.tar` & `ns1-python-0.9.19.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 jvcelak    (501) staff       (20)        0 2018-02-28 19:30:50.000000 ns1-python-0.9.18/
--rw-r--r--   0 jvcelak    (501) staff       (20)     3258 2018-02-28 19:30:50.000000 ns1-python-0.9.18/PKG-INFO
-drwxr-xr-x   0 jvcelak    (501) staff       (20)        0 2018-02-28 19:30:50.000000 ns1-python-0.9.18/ns1/
--rw-r--r--   0 jvcelak    (501) staff       (20)     6959 2016-11-04 18:29:55.000000 ns1-python-0.9.18/ns1/config.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     6006 2016-11-04 18:29:55.000000 ns1-python-0.9.18/ns1/records.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     5995 2018-02-28 19:29:55.000000 ns1-python-0.9.18/ns1/__init__.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     9011 2018-01-24 21:52:06.000000 ns1-python-0.9.18/ns1/zones.py
-drwxr-xr-x   0 jvcelak    (501) staff       (20)        0 2018-02-28 19:30:50.000000 ns1-python-0.9.18/ns1/rest/
-drwxr-xr-x   0 jvcelak    (501) staff       (20)        0 2018-02-28 19:30:50.000000 ns1-python-0.9.18/ns1/rest/transport/
--rw-r--r--   0 jvcelak    (501) staff       (20)      275 2016-11-04 18:29:55.000000 ns1-python-0.9.18/ns1/rest/transport/__init__.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     3770 2018-02-28 19:25:53.000000 ns1-python-0.9.18/ns1/rest/transport/basic.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     6442 2018-01-24 22:38:11.000000 ns1-python-0.9.18/ns1/rest/transport/twisted.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     2842 2018-01-24 21:52:06.000000 ns1-python-0.9.18/ns1/rest/transport/requests.py
--rw-r--r--   0 jvcelak    (501) staff       (20)      852 2018-01-24 21:52:06.000000 ns1-python-0.9.18/ns1/rest/transport/base.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     2911 2017-12-20 10:45:38.000000 ns1-python-0.9.18/ns1/rest/monitoring.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     6185 2017-06-13 19:17:55.000000 ns1-python-0.9.18/ns1/rest/records.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     2424 2016-11-04 18:29:55.000000 ns1-python-0.9.18/ns1/rest/resource.py
--rw-r--r--   0 jvcelak    (501) staff       (20)        0 2016-11-04 18:29:55.000000 ns1-python-0.9.18/ns1/rest/__init__.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     2843 2018-01-24 21:52:06.000000 ns1-python-0.9.18/ns1/rest/zones.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     1739 2017-10-02 10:42:12.000000 ns1-python-0.9.18/ns1/rest/stats.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     1736 2017-10-02 10:42:12.000000 ns1-python-0.9.18/ns1/rest/errors.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     4093 2016-11-04 18:29:55.000000 ns1-python-0.9.18/ns1/rest/data.py
--rw-r--r--   0 jvcelak    (501) staff       (20)      463 2016-11-04 18:29:55.000000 ns1-python-0.9.18/ns1/rest/account.py
--rw-r--r--   0 jvcelak    (501) staff       (20)     1461 2018-01-24 21:52:20.000000 ns1-python-0.9.18/setup.py
--rw-r--r--   0 jvcelak    (501) staff       (20)       92 2018-02-28 19:30:50.000000 ns1-python-0.9.18/setup.cfg
--rw-r--r--   0 jvcelak    (501) staff       (20)     1851 2018-01-25 10:57:02.000000 ns1-python-0.9.18/README.rst
-drwxr-xr-x   0 jvcelak    (501) staff       (20)        0 2018-02-28 19:30:50.000000 ns1-python-0.9.18/ns1_python.egg-info/
--rw-r--r--   0 jvcelak    (501) staff       (20)     3258 2018-02-28 19:30:50.000000 ns1-python-0.9.18/ns1_python.egg-info/PKG-INFO
--rw-r--r--   0 jvcelak    (501) staff       (20)      547 2018-02-28 19:30:50.000000 ns1-python-0.9.18/ns1_python.egg-info/SOURCES.txt
--rw-r--r--   0 jvcelak    (501) staff       (20)        4 2018-02-28 19:30:50.000000 ns1-python-0.9.18/ns1_python.egg-info/top_level.txt
--rw-r--r--   0 jvcelak    (501) staff       (20)        1 2018-02-28 19:30:50.000000 ns1-python-0.9.18/ns1_python.egg-info/dependency_links.txt
+drwxr-xr-x   0 mburtless   (502) staff       (20)        0 2019-03-14 16:41:17.000000 ns1-python-0.9.19/
+-rw-r--r--   0 mburtless   (502) staff       (20)     3224 2019-03-14 16:41:17.000000 ns1-python-0.9.19/PKG-INFO
+-rw-r--r--   0 mburtless   (502) staff       (20)     1851 2019-02-21 19:36:45.000000 ns1-python-0.9.19/README.rst
+drwxr-xr-x   0 mburtless   (502) staff       (20)        0 2019-03-14 16:41:17.000000 ns1-python-0.9.19/ns1/
+-rw-r--r--   0 mburtless   (502) staff       (20)     6565 2019-03-14 15:50:26.000000 ns1-python-0.9.19/ns1/__init__.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     6959 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/config.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     2813 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/monitoring.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     6006 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/records.py
+drwxr-xr-x   0 mburtless   (502) staff       (20)        0 2019-03-14 16:41:17.000000 ns1-python-0.9.19/ns1/rest/
+-rw-r--r--   0 mburtless   (502) staff       (20)        0 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/__init__.py
+-rw-r--r--   0 mburtless   (502) staff       (20)      463 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/account.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     4093 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/data.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     1736 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/errors.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     3175 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/monitoring.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     6185 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/records.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     2424 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/resource.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     1739 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/stats.py
+drwxr-xr-x   0 mburtless   (502) staff       (20)        0 2019-03-14 16:41:17.000000 ns1-python-0.9.19/ns1/rest/transport/
+-rw-r--r--   0 mburtless   (502) staff       (20)      275 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/transport/__init__.py
+-rw-r--r--   0 mburtless   (502) staff       (20)      852 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/transport/base.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     3735 2019-03-13 14:48:47.000000 ns1-python-0.9.19/ns1/rest/transport/basic.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     2842 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/transport/requests.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     6442 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/transport/twisted.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     2843 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/rest/zones.py
+-rw-r--r--   0 mburtless   (502) staff       (20)     9011 2019-02-21 19:36:45.000000 ns1-python-0.9.19/ns1/zones.py
+drwxr-xr-x   0 mburtless   (502) staff       (20)        0 2019-03-14 16:41:17.000000 ns1-python-0.9.19/ns1_python.egg-info/
+-rw-r--r--   0 mburtless   (502) staff       (20)     3224 2019-03-14 16:41:16.000000 ns1-python-0.9.19/ns1_python.egg-info/PKG-INFO
+-rw-r--r--   0 mburtless   (502) staff       (20)      565 2019-03-14 16:41:17.000000 ns1-python-0.9.19/ns1_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mburtless   (502) staff       (20)        1 2019-03-14 16:41:16.000000 ns1-python-0.9.19/ns1_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mburtless   (502) staff       (20)        4 2019-03-14 16:41:16.000000 ns1-python-0.9.19/ns1_python.egg-info/top_level.txt
+-rw-r--r--   0 mburtless   (502) staff       (20)       92 2019-03-14 16:41:17.000000 ns1-python-0.9.19/setup.cfg
+-rw-r--r--   0 mburtless   (502) staff       (20)     1461 2019-02-21 19:36:45.000000 ns1-python-0.9.19/setup.py
```

### Comparing `ns1-python-0.9.18/PKG-INFO` & `ns1-python-0.9.19/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: ns1-python
-Version: 0.9.18
+Version: 0.9.19
 Summary: Python SDK for the NS1 DNS platform
 Home-page: https://github.com/ns1/ns1-python
 Author: NS1 Developers
 Author-email: devteam@ns1.com
 License: MIT
-Description-Content-Type: UNKNOWN
 Description: ==============
         NS1 Python SDK
         ==============
         
         :Info: A Python SDK for accessing NS1, the Data Driven DNS platform.
         
         .. image:: https://travis-ci.org/ns1/ns1-python.svg?branch=master
```

### Comparing `ns1-python-0.9.18/ns1/config.py` & `ns1-python-0.9.19/ns1/config.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/ns1/records.py` & `ns1-python-0.9.19/ns1/records.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/ns1/__init__.py` & `ns1-python-0.9.19/ns1/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2014 NSONE, Inc.
 #
 # License under The MIT License (MIT). See LICENSE in project root.
 #
 
 from .config import Config
 
-version = "0.9.18"
+version = "0.9.19"
 
 
 class NS1:
 
     def __init__(self, apiKey=None, config=None, configFile=None, keyID=None):
         """
         Create a new top level NS1 API object
@@ -178,7 +178,24 @@
             if len(parts) <= 2:
                 zone = '.'.join(parts)
             else:
                 zone = '.'.join(parts[1:])
         z = ns1.zones.Zone(self.config, zone)
         return z.loadRecord(domain, type, callback=callback, errback=errback,
                             **kwargs)
+
+    def loadMonitors(self, callback=None, errback=None, **kwargs):
+        """
+        Load all monitors
+        """
+        import ns1.monitoring
+        monitors_list = self.monitors().list(callback, errback)
+
+        return [ns1.monitoring.Monitor(self.config, m) for m in monitors_list]
+
+    def createMonitor(self, callback=None, errback=None, **kwargs):
+        """
+        Create a monitor
+        """
+        import ns1.monitoring
+        monitor = ns1.monitoring.Monitor(self.config)
+        return monitor.create(callback=callback, errback=errback, **kwargs)
```

### Comparing `ns1-python-0.9.18/ns1/zones.py` & `ns1-python-0.9.19/ns1/zones.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/ns1/rest/transport/basic.py` & `ns1-python-0.9.19/ns1/rest/transport/basic.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,14 +44,16 @@
             if not self._verify:
                 context.check_hostname = False
                 context.verify_mode = ssl.CERT_NONE
             opener = build_opener(HTTPSHandler(context=context))
         else:
             opener = build_opener(HTTPSHandler)
 
+        if sys.version_info.major >= 3 and isinstance(data, str):
+            data = data.encode('utf-8')
         request = Request(url, headers=headers, data=data)
         request.get_method = lambda: method
 
         def handleProblem(code, resp, msg):
             if errback:
                 errback((resp, msg))
                 return
@@ -78,19 +80,15 @@
         # always pass the body to the handleProblem function
         try:
             resp = opener.open(request, timeout=self._timeout)
             body = resp.read()
         except HTTPError as e:
             resp = e
             body = resp.read()
-        except Exception as e:
-            body = '"Service Unavailable"'
-            resp = HTTPError(url, 503, body, headers, None)
-        finally:
-            if resp.code != 200:
+            if not 200 <= resp.code < 300:
                 handleProblem(resp.code, resp, body)
 
         # TODO make sure json is valid
         try:
             jsonOut = json.loads(body)
         except ValueError:
             if errback:
```

### Comparing `ns1-python-0.9.18/ns1/rest/transport/twisted.py` & `ns1-python-0.9.19/ns1/rest/transport/twisted.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/ns1/rest/transport/requests.py` & `ns1-python-0.9.19/ns1/rest/transport/requests.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/ns1/rest/transport/base.py` & `ns1-python-0.9.19/ns1/rest/transport/base.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/ns1/rest/monitoring.py` & `ns1-python-0.9.19/ns1/rest/monitoring.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,30 +5,36 @@
 #
 from . import resource
 
 
 class Monitors(resource.BaseResource):
 
     ROOT = 'monitoring/jobs'
-    PASSTHRU_FIELDS = ['name', 'config']
+    PASSTHRU_FIELDS = [
+      'name', 'config', 'region_scope', 'regions', 'job_type', 
+      'policy', 'notes', 'rules', 'notify_delay', 'notify_list'
+    ]
+    INT_FIELDS = ['frequency']
+    BOOL_FIELDS = ['active', 'rapid_recheck', 'notify_regional']
 
     def list(self, callback=None, errback=None):
         return self._make_request('GET', '%s' % (self.ROOT),
                                   callback=callback,
                                   errback=errback)
 
     def update(self, jobid, body, callback=None, errback=None, **kwargs):
         self._buildStdBody(body, kwargs)
         return self._make_request('POST',
                                   '%s/%s' % (self.ROOT, jobid),
                                   body=body,
                                   callback=callback,
                                   errback=errback)
 
-    def create(self, body, callback=None, errback=None):
+    def create(self, body, callback=None, errback=None, **kwargs):
+        self._buildStdBody(body, kwargs)
         return self._make_request('PUT', '%s' % (self.ROOT), body=body,
                                   callback=callback,
                                   errback=errback)
 
     def retrieve(self, jobid, callback=None, errback=None):
         return self._make_request('GET', '%s/%s' % (self.ROOT, jobid),
                                   callback=callback,
```

### Comparing `ns1-python-0.9.18/ns1/rest/records.py` & `ns1-python-0.9.19/ns1/rest/records.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/ns1/rest/resource.py` & `ns1-python-0.9.19/ns1/rest/resource.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/ns1/rest/zones.py` & `ns1-python-0.9.19/ns1/rest/zones.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/ns1/rest/stats.py` & `ns1-python-0.9.19/ns1/rest/stats.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/ns1/rest/errors.py` & `ns1-python-0.9.19/ns1/rest/errors.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/ns1/rest/data.py` & `ns1-python-0.9.19/ns1/rest/data.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/setup.py` & `ns1-python-0.9.19/setup.py`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/README.rst` & `ns1-python-0.9.19/README.rst`

 * *Files identical despite different names*

### Comparing `ns1-python-0.9.18/ns1_python.egg-info/PKG-INFO` & `ns1-python-0.9.19/ns1_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: ns1-python
-Version: 0.9.18
+Version: 0.9.19
 Summary: Python SDK for the NS1 DNS platform
 Home-page: https://github.com/ns1/ns1-python
 Author: NS1 Developers
 Author-email: devteam@ns1.com
 License: MIT
-Description-Content-Type: UNKNOWN
 Description: ==============
         NS1 Python SDK
         ==============
         
         :Info: A Python SDK for accessing NS1, the Data Driven DNS platform.
         
         .. image:: https://travis-ci.org/ns1/ns1-python.svg?branch=master
```

### Comparing `ns1-python-0.9.18/ns1_python.egg-info/SOURCES.txt` & `ns1-python-0.9.19/ns1_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.rst
 setup.cfg
 setup.py
 ns1/__init__.py
 ns1/config.py
+ns1/monitoring.py
 ns1/records.py
 ns1/zones.py
 ns1/rest/__init__.py
 ns1/rest/account.py
 ns1/rest/data.py
 ns1/rest/errors.py
 ns1/rest/monitoring.py
```

