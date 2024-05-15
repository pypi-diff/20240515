# Comparing `tmp/ezyli_utils-2.0.6.tar.gz` & `tmp/ezyli_utils-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyli_utils-2.0.6.tar", last modified: Sat Mar  9 13:51:06 2024, max compression
+gzip compressed data, was "ezyli_utils-2.0.7.tar", last modified: Wed May 15 13:06:31 2024, max compression
```

## Comparing `ezyli_utils-2.0.6.tar` & `ezyli_utils-2.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ezytako   (1000) ezytako   (1000)        0 2024-03-09 13:51:06.142018 ezyli_utils-2.0.6/
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)       55 2024-03-09 13:51:06.142018 ezyli_utils-2.0.6/PKG-INFO
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)     6095 2024-03-09 13:50:47.000000 ezyli_utils-2.0.6/README.md
-drwxrwxr-x   0 ezytako   (1000) ezytako   (1000)        0 2024-03-09 13:51:06.142018 ezyli_utils-2.0.6/ezyli_utils/
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)      105 2024-02-28 02:20:37.000000 ezyli_utils-2.0.6/ezyli_utils/__init__.py
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)    11192 2024-03-01 12:17:40.000000 ezyli_utils-2.0.6/ezyli_utils/amqp_manager.py
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)     8883 2024-03-09 13:50:01.000000 ezyli_utils-2.0.6/ezyli_utils/schemas.py
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)      234 2024-02-28 02:20:05.000000 ezyli_utils-2.0.6/ezyli_utils/utils.py
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)      263 2024-02-10 09:16:34.000000 ezyli_utils-2.0.6/ezyli_utils/validator.py
-drwxrwxr-x   0 ezytako   (1000) ezytako   (1000)        0 2024-03-09 13:51:06.142018 ezyli_utils-2.0.6/ezyli_utils.egg-info/
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)       55 2024-03-09 13:51:06.000000 ezyli_utils-2.0.6/ezyli_utils.egg-info/PKG-INFO
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)      313 2024-03-09 13:51:06.000000 ezyli_utils-2.0.6/ezyli_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)        1 2024-03-09 13:51:06.000000 ezyli_utils-2.0.6/ezyli_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)       31 2024-03-09 13:51:06.000000 ezyli_utils-2.0.6/ezyli_utils.egg-info/requires.txt
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)       12 2024-03-09 13:51:06.000000 ezyli_utils-2.0.6/ezyli_utils.egg-info/top_level.txt
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)       38 2024-03-09 13:51:06.142018 ezyli_utils-2.0.6/setup.cfg
--rw-rw-r--   0 ezytako   (1000) ezytako   (1000)      210 2024-03-09 13:51:01.000000 ezyli_utils-2.0.6/setup.py
+drwxrwxr-x   0 ezytako   (1000) ezytako   (1000)        0 2024-05-15 13:06:31.288415 ezyli_utils-2.0.7/
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)       55 2024-05-15 13:06:31.288415 ezyli_utils-2.0.7/PKG-INFO
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)     6095 2024-05-15 13:04:45.000000 ezyli_utils-2.0.7/README.md
+drwxrwxr-x   0 ezytako   (1000) ezytako   (1000)        0 2024-05-15 13:06:31.288415 ezyli_utils-2.0.7/ezyli_utils/
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)      105 2024-02-28 02:20:37.000000 ezyli_utils-2.0.7/ezyli_utils/__init__.py
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)    11192 2024-03-01 12:17:40.000000 ezyli_utils-2.0.7/ezyli_utils/amqp_manager.py
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)     9033 2024-05-15 13:03:53.000000 ezyli_utils-2.0.7/ezyli_utils/schemas.py
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)      234 2024-02-28 02:20:05.000000 ezyli_utils-2.0.7/ezyli_utils/utils.py
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)      263 2024-02-10 09:16:34.000000 ezyli_utils-2.0.7/ezyli_utils/validator.py
+drwxrwxr-x   0 ezytako   (1000) ezytako   (1000)        0 2024-05-15 13:06:31.288415 ezyli_utils-2.0.7/ezyli_utils.egg-info/
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)       55 2024-05-15 13:06:31.000000 ezyli_utils-2.0.7/ezyli_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)      313 2024-05-15 13:06:31.000000 ezyli_utils-2.0.7/ezyli_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)        1 2024-05-15 13:06:31.000000 ezyli_utils-2.0.7/ezyli_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)       31 2024-05-15 13:06:31.000000 ezyli_utils-2.0.7/ezyli_utils.egg-info/requires.txt
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)       12 2024-05-15 13:06:31.000000 ezyli_utils-2.0.7/ezyli_utils.egg-info/top_level.txt
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)       38 2024-05-15 13:06:31.288415 ezyli_utils-2.0.7/setup.cfg
+-rw-rw-r--   0 ezytako   (1000) ezytako   (1000)      210 2024-05-15 13:04:37.000000 ezyli_utils-2.0.7/setup.py
```

### Comparing `ezyli_utils-2.0.6/README.md` & `ezyli_utils-2.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 ### Push a specific version
 ```bash
 twine upload dist/my_package-0.1.tar.gz
 ```
 Example
 ```bash
-twine upload dist/ezyli_utils-2.0.6.tar.gz
+twine upload dist/ezyli_utils-2.0.7.tar.gz
 ```
 
 5. After uploading, your package should be available on PyPI and can be installed with pip:
 
 ```bash
 pip install your-package-name
 ```
```

### Comparing `ezyli_utils-2.0.6/ezyli_utils/amqp_manager.py` & `ezyli_utils-2.0.7/ezyli_utils/amqp_manager.py`

 * *Files identical despite different names*

### Comparing `ezyli_utils-2.0.6/ezyli_utils/schemas.py` & `ezyli_utils-2.0.7/ezyli_utils/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
                                 "type": "array",
                                 "items": {"type": "number"},
                                 "minItems": 2,
                                 "maxItems": 2,
                             },
                         },
                         "lat_first": {"type": "boolean"},
+                        "precision": {"type": "integer", "enum": [0, 1]}, 
                     },
                     "required": ["origin", "destination", "waypoints"],
                 },
                 "receiver": {
                     "type": "object",
                     "properties": {"queue_name": {"type": "string"}},
                     "required": ["queue_name"],
@@ -168,14 +169,15 @@
                         "mode": {"type": "string"},
                         "matrix_types": {
                             "type": "array",
                             "items": {"type": "string", "enum": ["TIME", "DISTANCE"]},
                             "minItems": 1,
                         },
                         "lat_first": {"type": "boolean"},
+                        "precision": {"type": "integer", "enum": [0, 1]}, 
                     },
                     "required": ["coord_params", "mode", "matrix_types"],
                 },
                 "receiver": {
                     "type": "object",
                     "properties": {"queue_name": {"type": "string"}},
                     "required": ["queue_name"],
```

