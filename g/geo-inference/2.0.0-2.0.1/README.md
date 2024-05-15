# Comparing `tmp/geo_inference-2.0.0.tar.gz` & `tmp/geo_inference-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_inference-2.0.0.tar", last modified: Wed Apr 17 02:21:41 2024, max compression
+gzip compressed data, was "geo_inference-2.0.1.tar", last modified: Wed Apr 17 02:53:15 2024, max compression
```

## Comparing `geo_inference-2.0.0.tar` & `geo_inference-2.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-04-17 02:21:41.508881 geo_inference-2.0.0/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     1072 2023-08-23 18:27:00.000000 geo_inference-2.0.0/LICENSE
--rw-r--r--   0 valhassa (17081319) geousers  (1100)       50 2023-11-28 18:37:26.000000 geo_inference-2.0.0/MANIFEST.in
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     6231 2024-04-17 02:21:41.508881 geo_inference-2.0.0/PKG-INFO
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     3514 2024-04-16 19:23:22.000000 geo_inference-2.0.0/README.md
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-04-17 02:21:41.508881 geo_inference-2.0.0/geo_inference/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      156 2024-04-17 02:20:58.000000 geo_inference-2.0.0/geo_inference/__init__.py
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-04-17 02:21:41.508881 geo_inference-2.0.0/geo_inference/config/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)        0 2023-11-28 18:37:26.000000 geo_inference-2.0.0/geo_inference/config/__init__.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      767 2023-11-28 18:37:26.000000 geo_inference-2.0.0/geo_inference/config/log_config.yaml
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      637 2024-03-12 16:11:07.000000 geo_inference-2.0.0/geo_inference/config/logging_config.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      457 2024-03-12 16:11:07.000000 geo_inference-2.0.0/geo_inference/config/sample.yaml
--rw-r--r--   0 valhassa (17081319) geousers  (1100)    16062 2024-04-12 23:47:20.000000 geo_inference-2.0.0/geo_inference/geo_blocks.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     5612 2024-04-16 18:13:37.000000 geo_inference-2.0.0/geo_inference/geo_inference.py
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-04-17 02:21:41.508881 geo_inference-2.0.0/geo_inference/utils/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)        0 2023-11-28 18:37:26.000000 geo_inference-2.0.0/geo_inference/utils/__init__.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     3424 2024-04-06 04:23:36.000000 geo_inference-2.0.0/geo_inference/utils/geo.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)    22881 2024-04-06 15:55:07.000000 geo_inference-2.0.0/geo_inference/utils/geo_transforms.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     9775 2024-04-11 03:07:16.000000 geo_inference-2.0.0/geo_inference/utils/helpers.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)    11870 2024-04-10 16:49:51.000000 geo_inference-2.0.0/geo_inference/utils/polygon.py
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-04-17 02:21:41.508881 geo_inference-2.0.0/geo_inference.egg-info/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     6231 2024-04-17 02:21:41.000000 geo_inference-2.0.0/geo_inference.egg-info/PKG-INFO
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      707 2024-04-17 02:21:41.000000 geo_inference-2.0.0/geo_inference.egg-info/SOURCES.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)        1 2024-04-17 02:21:41.000000 geo_inference-2.0.0/geo_inference.egg-info/dependency_links.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)       67 2024-04-17 02:21:41.000000 geo_inference-2.0.0/geo_inference.egg-info/entry_points.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      264 2024-04-17 02:21:41.000000 geo_inference-2.0.0/geo_inference.egg-info/requires.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)       14 2024-04-17 02:21:41.000000 geo_inference-2.0.0/geo_inference.egg-info/top_level.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     1845 2024-04-17 02:20:58.000000 geo_inference-2.0.0/pyproject.toml
--rw-r--r--   0 valhassa (17081319) geousers  (1100)       38 2024-04-17 02:21:41.508881 geo_inference-2.0.0/setup.cfg
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-04-17 02:21:41.508881 geo_inference-2.0.0/tests/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     6201 2024-04-10 18:14:44.000000 geo_inference-2.0.0/tests/test_geo_blocks.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     1842 2024-04-11 03:12:23.000000 geo_inference-2.0.0/tests/test_geo_inference.py
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-04-17 02:53:15.810466 geo_inference-2.0.1/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     1072 2023-08-23 18:27:00.000000 geo_inference-2.0.1/LICENSE
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)       50 2023-11-28 18:37:26.000000 geo_inference-2.0.1/MANIFEST.in
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     6209 2024-04-17 02:53:15.810466 geo_inference-2.0.1/PKG-INFO
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     3505 2024-04-17 02:45:20.000000 geo_inference-2.0.1/README.md
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-04-17 02:53:15.810466 geo_inference-2.0.1/geo_inference/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      156 2024-04-17 02:52:53.000000 geo_inference-2.0.1/geo_inference/__init__.py
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-04-17 02:53:15.810466 geo_inference-2.0.1/geo_inference/config/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)        0 2023-11-28 18:37:26.000000 geo_inference-2.0.1/geo_inference/config/__init__.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      767 2023-11-28 18:37:26.000000 geo_inference-2.0.1/geo_inference/config/log_config.yaml
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      637 2024-03-12 16:11:07.000000 geo_inference-2.0.1/geo_inference/config/logging_config.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      457 2024-03-12 16:11:07.000000 geo_inference-2.0.1/geo_inference/config/sample.yaml
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)    16062 2024-04-12 23:47:20.000000 geo_inference-2.0.1/geo_inference/geo_blocks.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     5612 2024-04-16 18:13:37.000000 geo_inference-2.0.1/geo_inference/geo_inference.py
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-04-17 02:53:15.810466 geo_inference-2.0.1/geo_inference/utils/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)        0 2023-11-28 18:37:26.000000 geo_inference-2.0.1/geo_inference/utils/__init__.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     3424 2024-04-06 04:23:36.000000 geo_inference-2.0.1/geo_inference/utils/geo.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)    22881 2024-04-06 15:55:07.000000 geo_inference-2.0.1/geo_inference/utils/geo_transforms.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     9775 2024-04-11 03:07:16.000000 geo_inference-2.0.1/geo_inference/utils/helpers.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)    11870 2024-04-10 16:49:51.000000 geo_inference-2.0.1/geo_inference/utils/polygon.py
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-04-17 02:53:15.810466 geo_inference-2.0.1/geo_inference.egg-info/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     6209 2024-04-17 02:53:15.000000 geo_inference-2.0.1/geo_inference.egg-info/PKG-INFO
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      707 2024-04-17 02:53:15.000000 geo_inference-2.0.1/geo_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)        1 2024-04-17 02:53:15.000000 geo_inference-2.0.1/geo_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)       67 2024-04-17 02:53:15.000000 geo_inference-2.0.1/geo_inference.egg-info/entry_points.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      264 2024-04-17 02:53:15.000000 geo_inference-2.0.1/geo_inference.egg-info/requires.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)       14 2024-04-17 02:53:15.000000 geo_inference-2.0.1/geo_inference.egg-info/top_level.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     1832 2024-04-17 02:52:53.000000 geo_inference-2.0.1/pyproject.toml
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)       38 2024-04-17 02:53:15.810466 geo_inference-2.0.1/setup.cfg
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-04-17 02:53:15.810466 geo_inference-2.0.1/tests/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     6201 2024-04-10 18:14:44.000000 geo_inference-2.0.1/tests/test_geo_blocks.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     1842 2024-04-11 03:12:23.000000 geo_inference-2.0.1/tests/test_geo_inference.py
```

### Comparing `geo_inference-2.0.0/LICENSE` & `geo_inference-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.0/PKG-INFO` & `geo_inference-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: geo-inference
-Version: 2.0.0
-Summary: Extract features from high-resolution geospatial imagery using foundation models
+Version: 2.0.1
+Summary: Extract features from geospatial imagery using deep learning models
 Author-email: Victor Alhassan <victor.alhassan@nrcan-rncan.gc.ca>
 License: MIT License
         
         Copyright (c) 2023 Victor Alhassan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -61,15 +61,15 @@
 
 # Geo Inference
 
 geo-inference is a Python package designed for feature extraction from geospatial imagery using compatible deep learning models. It provides a convenient way to extract features from large TIFF images and save the output mask as a TIFF file. It also supports converting the output mask to vector format (*file_name.geojson*), YOLO format (*file_name.csv*), and COCO format (*file_name.json*). This package is particularly useful for applications in remote sensing, environmental monitoring, and urban planning.
 
 ## Installation
 
-Geo-inference requires Python 3.11 or later. To install the package, use:
+Geo-inference requires Python 3.11. To install the package, use:
 
 ```
 pip install geo-inference
 ```
 
 ## Usage
```

### Comparing `geo_inference-2.0.0/README.md` & `geo_inference-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Geo Inference
 
 geo-inference is a Python package designed for feature extraction from geospatial imagery using compatible deep learning models. It provides a convenient way to extract features from large TIFF images and save the output mask as a TIFF file. It also supports converting the output mask to vector format (*file_name.geojson*), YOLO format (*file_name.csv*), and COCO format (*file_name.json*). This package is particularly useful for applications in remote sensing, environmental monitoring, and urban planning.
 
 ## Installation
 
-Geo-inference requires Python 3.11 or later. To install the package, use:
+Geo-inference requires Python 3.11. To install the package, use:
 
 ```
 pip install geo-inference
 ```
 
 ## Usage
```

### Comparing `geo_inference-2.0.0/geo_inference/config/log_config.yaml` & `geo_inference-2.0.1/geo_inference/config/log_config.yaml`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.0/geo_inference/config/logging_config.py` & `geo_inference-2.0.1/geo_inference/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.0/geo_inference/geo_blocks.py` & `geo_inference-2.0.1/geo_inference/geo_blocks.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.0/geo_inference/geo_inference.py` & `geo_inference-2.0.1/geo_inference/geo_inference.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.0/geo_inference/utils/geo.py` & `geo_inference-2.0.1/geo_inference/utils/geo.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.0/geo_inference/utils/geo_transforms.py` & `geo_inference-2.0.1/geo_inference/utils/geo_transforms.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.0/geo_inference/utils/helpers.py` & `geo_inference-2.0.1/geo_inference/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.0/geo_inference/utils/polygon.py` & `geo_inference-2.0.1/geo_inference/utils/polygon.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.0/geo_inference.egg-info/PKG-INFO` & `geo_inference-2.0.1/geo_inference.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: geo-inference
-Version: 2.0.0
-Summary: Extract features from high-resolution geospatial imagery using foundation models
+Version: 2.0.1
+Summary: Extract features from geospatial imagery using deep learning models
 Author-email: Victor Alhassan <victor.alhassan@nrcan-rncan.gc.ca>
 License: MIT License
         
         Copyright (c) 2023 Victor Alhassan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -61,15 +61,15 @@
 
 # Geo Inference
 
 geo-inference is a Python package designed for feature extraction from geospatial imagery using compatible deep learning models. It provides a convenient way to extract features from large TIFF images and save the output mask as a TIFF file. It also supports converting the output mask to vector format (*file_name.geojson*), YOLO format (*file_name.csv*), and COCO format (*file_name.json*). This package is particularly useful for applications in remote sensing, environmental monitoring, and urban planning.
 
 ## Installation
 
-Geo-inference requires Python 3.11 or later. To install the package, use:
+Geo-inference requires Python 3.11. To install the package, use:
 
 ```
 pip install geo-inference
 ```
 
 ## Usage
```

### Comparing `geo_inference-2.0.0/geo_inference.egg-info/SOURCES.txt` & `geo_inference-2.0.1/geo_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.0/pyproject.toml` & `geo_inference-2.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geo-inference"
-version = "2.0.0"
-description = "Extract features from high-resolution geospatial imagery using foundation models"
+version = "2.0.1"
+description = "Extract features from geospatial imagery using deep learning models"
 readme = "README.md"
 authors = [{ name = "Victor Alhassan", email = "victor.alhassan@nrcan-rncan.gc.ca" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
@@ -47,15 +47,15 @@
 [project.scripts]
 geo_inference = "geo_inference.geo_inference:main"
 
 [tool.setuptools.packages.find]
 include = ["geo_inference*"]
 
 [tool.bumpver]
-current_version = "2.0.0"
+current_version = "2.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `geo_inference-2.0.0/tests/test_geo_blocks.py` & `geo_inference-2.0.1/tests/test_geo_blocks.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.0/tests/test_geo_inference.py` & `geo_inference-2.0.1/tests/test_geo_inference.py`

 * *Files identical despite different names*

