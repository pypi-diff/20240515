# Comparing `tmp/smartcitizen_connector-1.0.4.tar.gz` & `tmp/smartcitizen_connector-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartcitizen_connector-1.0.4.tar", last modified: Thu May  2 14:44:04 2024, max compression
+gzip compressed data, was "smartcitizen_connector-1.0.5.tar", last modified: Wed May 15 10:17:39 2024, max compression
```

## Comparing `smartcitizen_connector-1.0.4.tar` & `smartcitizen_connector-1.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.194266 smartcitizen_connector-1.0.4/smartcitizen_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/_config/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/_config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/device/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24439 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/device/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/measurement/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/measurement/measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/models/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/search/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/search/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/sensor/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-02 14:44:04.000000 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-02 14:44:04.000000 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:44:04.000000 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:44:04.000000 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 14:44:04.000000 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 14:44:04.000000 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.852537 smartcitizen_connector-1.0.5/smartcitizen_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/_config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/device/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24676 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/device/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/measurement/measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/search/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/sensor/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-15 10:17:35.000000 smartcitizen_connector-1.0.5/smartcitizen_connector/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:17:39.856537 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-15 10:17:39.000000 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-15 10:17:39.000000 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:17:39.000000 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:17:39.000000 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 10:17:39.000000 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 10:17:39.000000 smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/top_level.txt
```

### Comparing `smartcitizen_connector-1.0.4/LICENSE` & `smartcitizen_connector-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.4/PKG-INFO` & `smartcitizen_connector-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcitizen-connector
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python connector to download information collected in SmartCitizen API
 Home-page: https://github.com/fablabbcn/smartcitizen-connector
 Author: oscgonfer
 License: GNU General Public License v3
 Project-URL: Documentation, https://docs.smartcitizen.me/
 Project-URL: Source Code, https://github.com/fablabbcn/smartcitizen-connector
 Keywords: sensors,Smart Citizen
```

### Comparing `smartcitizen_connector-1.0.4/README.md` & `smartcitizen_connector-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.4/setup.py` & `smartcitizen_connector-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 PROJECT_URLS = {
     "Documentation": "https://docs.smartcitizen.me/",
     "Source Code": "https://github.com/fablabbcn/smartcitizen-connector",
 }
 
 setup(
     name="smartcitizen-connector",
-    version="1.0.4",
+    version="1.0.5",
     description="Python connector to download information collected in SmartCitizen API",
     author="oscgonfer",
     license="GNU General Public License v3",
     keywords=['sensors', 'Smart Citizen'],
     long_description = open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/fablabbcn/smartcitizen-connector",
```

### Comparing `smartcitizen_connector-1.0.4/smartcitizen_connector/_config/config.py` & `smartcitizen_connector-1.0.5/smartcitizen_connector/_config/config.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.4/smartcitizen_connector/device/device.py` & `smartcitizen_connector-1.0.5/smartcitizen_connector/device/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,16 +229,20 @@
         clean_na: Optional[str] = None,
         resample: Optional[bool] = False,
         rename: Optional[bool] = True)->DataFrame:
 
         if 'SC_ADMIN_BEARER' in environ:
             logger.info('Admin Bearer found, using it')
             headers = {'Authorization':'Bearer ' + environ['SC_ADMIN_BEARER']}
+        elif 'SC_BEARER' in environ:
+            logger.info('Bearer found in environment, using it.')
+            # TODO make this explicit
+            headers = {'Authorization':'Bearer ' + environ['SC_BEARER']}
         else:
-            logger.warning('Admin Bearer not found')
+            logger.warning('No Bearer not found, you might get throttled!')
             headers = None
 
         logger.info(f'Make sure we are up to date')
         self.__load__()
         logger.info(f'Requesting data from SC API')
         logger.info(f'Device ID: {self.id}')
         rollup = convert_freq_to_rollup(frequency)
```

### Comparing `smartcitizen_connector-1.0.4/smartcitizen_connector/measurement/measurement.py` & `smartcitizen_connector-1.0.5/smartcitizen_connector/measurement/measurement.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.4/smartcitizen_connector/models/models.py` & `smartcitizen_connector-1.0.5/smartcitizen_connector/models/models.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.4/smartcitizen_connector/search/search.py` & `smartcitizen_connector-1.0.5/smartcitizen_connector/search/search.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,17 +19,21 @@
     Returns
     -------
         A list of kit IDs that comply with the requirements, or the full df, depending on full.
     """
     if 'SC_ADMIN_BEARER' in environ:
         logger.info('Admin Bearer found, using it')
         headers = {'Authorization':'Bearer ' + environ['SC_ADMIN_BEARER']}
+    elif 'SC_BEARER' in environ:
+        logger.info('Bearer found in environment, using it.')
+        # TODO make this explicit
+        headers = {'Authorization':'Bearer ' + environ['SC_BEARER']}
     else:
+        logger.warning('No Bearer not found, you might get throttled!')
         headers = None
-        logger.info('Admin Bearer not found')
 
     # Value check
     if value is None: logger.error(f'Value needs a value, {value} supplied'); return None
 
     url = config.API_SEARCH_URL  + f'{value}'
 
     df = DataFrame()
@@ -79,17 +83,21 @@
     -------
         DataFrame with devices
     """
 
     if 'SC_ADMIN_BEARER' in environ:
         logger.info('Admin Bearer found, using it')
         headers = {'Authorization':'Bearer ' + environ['SC_ADMIN_BEARER']}
+    elif 'SC_BEARER' in environ:
+        logger.info('Bearer found in environment, using it.')
+        # TODO make this explicit
+        headers = {'Authorization':'Bearer ' + environ['SC_BEARER']}
     else:
+        logger.warning('No Bearer not found, you might get throttled!')
         headers = None
-        logger.info('Admin Bearer not found')
 
     url = f'{config.API_URL}{endpoint}/?'
     url_queries = 0
     for search_item in search_items:
         # Value check
         key = search_item['key']
         value = search_item['value']
```

### Comparing `smartcitizen_connector-1.0.4/smartcitizen_connector/sensor/sensor.py` & `smartcitizen_connector-1.0.5/smartcitizen_connector/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.4/smartcitizen_connector/tools/tools.py` & `smartcitizen_connector-1.0.5/smartcitizen_connector/tools/tools.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/PKG-INFO` & `smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcitizen-connector
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python connector to download information collected in SmartCitizen API
 Home-page: https://github.com/fablabbcn/smartcitizen-connector
 Author: oscgonfer
 License: GNU General Public License v3
 Project-URL: Documentation, https://docs.smartcitizen.me/
 Project-URL: Source Code, https://github.com/fablabbcn/smartcitizen-connector
 Keywords: sensors,Smart Citizen
```

### Comparing `smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/SOURCES.txt` & `smartcitizen_connector-1.0.5/smartcitizen_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

