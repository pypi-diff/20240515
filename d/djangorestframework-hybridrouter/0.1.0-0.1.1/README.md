# Comparing `tmp/djangorestframework_hybridrouter-0.1.0.tar.gz` & `tmp/djangorestframework_hybridrouter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework_hybridrouter-0.1.0.tar", last modified: Wed May 15 20:22:06 2024, max compression
+gzip compressed data, was "djangorestframework_hybridrouter-0.1.1.tar", last modified: Wed May 15 20:45:29 2024, max compression
```

## Comparing `djangorestframework_hybridrouter-0.1.0.tar` & `djangorestframework_hybridrouter-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:22:06.298983 djangorestframework_hybridrouter-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 20:21:59.000000 djangorestframework_hybridrouter-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 20:22:06.298983 djangorestframework_hybridrouter-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-15 20:21:59.000000 djangorestframework_hybridrouter-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:22:06.298983 djangorestframework_hybridrouter-0.1.0/djangorestframework_hybridrouter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 20:22:06.000000 djangorestframework_hybridrouter-0.1.0/djangorestframework_hybridrouter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-15 20:22:06.000000 djangorestframework_hybridrouter-0.1.0/djangorestframework_hybridrouter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:22:06.000000 djangorestframework_hybridrouter-0.1.0/djangorestframework_hybridrouter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 20:22:06.000000 djangorestframework_hybridrouter-0.1.0/djangorestframework_hybridrouter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 20:22:06.000000 djangorestframework_hybridrouter-0.1.0/djangorestframework_hybridrouter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:22:06.298983 djangorestframework_hybridrouter-0.1.0/hybridrouter/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:21:59.000000 djangorestframework_hybridrouter-0.1.0/hybridrouter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-15 20:21:59.000000 djangorestframework_hybridrouter-0.1.0/hybridrouter/hybridrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:22:06.298983 djangorestframework_hybridrouter-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-15 20:21:59.000000 djangorestframework_hybridrouter-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:45:29.517597 djangorestframework_hybridrouter-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 20:45:25.000000 djangorestframework_hybridrouter-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 20:45:29.517597 djangorestframework_hybridrouter-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-15 20:45:25.000000 djangorestframework_hybridrouter-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:45:29.513597 djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-15 20:45:29.000000 djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-15 20:45:29.000000 djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:45:29.000000 djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 20:45:29.000000 djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 20:45:29.000000 djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:45:29.513597 djangorestframework_hybridrouter-0.1.1/hybridrouter/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:45:25.000000 djangorestframework_hybridrouter-0.1.1/hybridrouter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-15 20:45:25.000000 djangorestframework_hybridrouter-0.1.1/hybridrouter/hybridrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:45:29.517597 djangorestframework_hybridrouter-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-15 20:45:25.000000 djangorestframework_hybridrouter-0.1.1/setup.py
```

### Comparing `djangorestframework_hybridrouter-0.1.0/LICENSE` & `djangorestframework_hybridrouter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework_hybridrouter-0.1.0/PKG-INFO` & `djangorestframework_hybridrouter-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-hybridrouter
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to regsiter viewsets and views in the same router
 Home-page: https://github.com/enzofrnt/djangorestframework-hybridrouter
 Author: Made by enzo_frnt from a 
 Keywords: Django,Django REST Framework,viewsets,views,router,view,viewset
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django
```

### Comparing `djangorestframework_hybridrouter-0.1.0/djangorestframework_hybridrouter.egg-info/PKG-INFO` & `djangorestframework_hybridrouter-0.1.1/djangorestframework_hybridrouter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-hybridrouter
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to regsiter viewsets and views in the same router
 Home-page: https://github.com/enzofrnt/djangorestframework-hybridrouter
 Author: Made by enzo_frnt from a 
 Keywords: Django,Django REST Framework,viewsets,views,router,view,viewset
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django
```

### Comparing `djangorestframework_hybridrouter-0.1.0/hybridrouter/hybridrouter.py` & `djangorestframework_hybridrouter-0.1.1/hybridrouter/hybridrouter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from django.urls import re_path, reverse
+from django.urls import re_path
+from rest_framework.reverse import reverse
 from rest_framework.routers import DefaultRouter
 from rest_framework.views import APIView
 from rest_framework.response import Response
 from urllib.parse import urlsplit, urlunsplit
 
 class HybridRouter(DefaultRouter):    
     def __init__(self, *args, **kwargs):
```

### Comparing `djangorestframework_hybridrouter-0.1.0/setup.py` & `djangorestframework_hybridrouter-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='djangorestframework-hybridrouter',
-    version='0.1.0',
+    version='0.1.1',
     packages=[
         'hybridrouter',
     ],
     install_requires=[
         'Django',
         'djangorestframework',
     ],
```

