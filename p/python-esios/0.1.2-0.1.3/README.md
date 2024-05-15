# Comparing `tmp/python_esios-0.1.2.tar.gz` & `tmp/python_esios-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_esios-0.1.2.tar", last modified: Wed May 15 06:30:20 2024, max compression
+gzip compressed data, was "python_esios-0.1.3.tar", last modified: Wed May 15 06:42:23 2024, max compression
```

## Comparing `python_esios-0.1.2.tar` & `python_esios-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:20.144859 python_esios-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:07.000000 python_esios-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 06:30:20.144859 python_esios-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-15 06:30:07.000000 python_esios-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:20.140859 python_esios-0.1.2/esios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:07.000000 python_esios-0.1.2/esios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-15 06:30:07.000000 python_esios-0.1.2/esios/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:20.140859 python_esios-0.1.2/esios/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 06:30:07.000000 python_esios-0.1.2/esios/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:20.140859 python_esios-0.1.2/esios/endpoints/indicators/
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-15 06:30:07.000000 python_esios-0.1.2/esios/endpoints/indicators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:30:20.144859 python_esios-0.1.2/python_esios.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 06:30:20.000000 python_esios-0.1.2/python_esios.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 06:30:20.000000 python_esios-0.1.2/python_esios.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:30:20.000000 python_esios-0.1.2/python_esios.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 06:30:20.000000 python_esios-0.1.2/python_esios.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 06:30:20.000000 python_esios-0.1.2/python_esios.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:30:20.144859 python_esios-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 06:30:07.000000 python_esios-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:23.082380 python_esios-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:14.000000 python_esios-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 06:42:23.082380 python_esios-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-15 06:42:14.000000 python_esios-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:23.078380 python_esios-0.1.3/esios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:14.000000 python_esios-0.1.3/esios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-15 06:42:14.000000 python_esios-0.1.3/esios/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:23.078380 python_esios-0.1.3/esios/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 06:42:14.000000 python_esios-0.1.3/esios/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:23.078380 python_esios-0.1.3/esios/endpoints/indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-15 06:42:15.000000 python_esios-0.1.3/esios/endpoints/indicators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:23.082380 python_esios-0.1.3/python_esios.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 06:42:23.000000 python_esios-0.1.3/python_esios.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 06:42:23.000000 python_esios-0.1.3/python_esios.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:42:23.000000 python_esios-0.1.3/python_esios.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 06:42:23.000000 python_esios-0.1.3/python_esios.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 06:42:23.000000 python_esios-0.1.3/python_esios.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:42:23.082380 python_esios-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 06:42:15.000000 python_esios-0.1.3/setup.py
```

### Comparing `python_esios-0.1.2/PKG-INFO` & `python_esios-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esios
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python wrapper for the ESIOS API
 Home-page: https://github.com/datons/python-esios
 Author: Jesús López
 Author-email: jesus.lopez@datons.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_esios-0.1.2/esios/api_client.py` & `python_esios-0.1.3/esios/api_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import requests
 import os
 
 class APIClient:
     base_url = 'https://api.esios.ree.es'
-    headers = {
-        'Accept': "application/json; application/vnd.esios-api-v1+json",
-        'Content-Type': "application/json",
-        'Host': 'api.esios.ree.es',
-    }
 
     def __init__(self, api_key=None):
-        if api_key is None:
-            api_key = os.getenv('ESIOS_API_KEY')  # Try to get the API key from environment variable
-            if api_key is None:
-                raise ValueError("API key must be provided either through constructor or as an environment variable 'ESIOS_API_KEY'")
-        self.api_key = api_key
-        self.headers['x-api-key'] = self.api_key
+        self.api_key = api_key if api_key else os.getenv('ESIOS_API_KEY')
+        if not self.api_key:
+            raise ValueError("API key must be provided directly or set in the 'ESIOS_API_KEY' environment variable")
+        self.headers = {
+            'Accept': "application/json; application/vnd.esios-api-v1+json",
+            'Content-Type': "application/json",
+            'Host': 'api.esios.ree.es',
+            'x-api-key': self.api_key
+        }
 
     def _api_call(self, method, endpoint, params=None, data=None):
         url = self.base_url + endpoint
         response = requests.request(method, url, headers=self.headers, params=params, json=data)
         response.raise_for_status()
         return response
```

### Comparing `python_esios-0.1.2/esios/endpoints/indicators/__init__.py` & `python_esios-0.1.3/esios/endpoints/indicators/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 from esios.api_client import APIClient
 import html
 
 class Indicators(APIClient):
-    def __init__(self, api_key):
+    def __init__(self, api_key=None):
         super().__init__(api_key)
     
     def list(self, df=False):
         """
         Fetches a list of indicators.
 
         Parameters
```

### Comparing `python_esios-0.1.2/python_esios.egg-info/PKG-INFO` & `python_esios-0.1.3/python_esios.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esios
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python wrapper for the ESIOS API
 Home-page: https://github.com/datons/python-esios
 Author: Jesús López
 Author-email: jesus.lopez@datons.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_esios-0.1.2/setup.py` & `python_esios-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 setup(
     name='python-esios',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'requests',
         'pandas',
     ],
     author="Jesús López",
     author_email="jesus.lopez@datons.ai",
```

