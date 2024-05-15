# Comparing `tmp/samgis_core-1.2.2.tar.gz` & `tmp/samgis_core-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samgis_core-1.2.2.tar", max compression
+gzip compressed data, was "samgis_core-2.0.0.tar", max compression
```

## Comparing `samgis_core-1.2.2.tar` & `samgis_core-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      262 2024-01-27 16:18:49.002975 samgis_core-1.2.2/README.md
--rw-r--r--   0        0        0      754 2024-05-14 22:22:17.767167 samgis_core-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      351 2024-05-14 22:31:35.821860 samgis_core-1.2.2/samgis_core/__init__.py
--rw-r--r--   0        0        0       94 2024-04-21 19:58:55.709199 samgis_core-1.2.2/samgis_core/__version__.py
--rw-r--r--   0        0        0       57 2024-01-26 19:56:25.000000 samgis_core-1.2.2/samgis_core/prediction_api/__init__.py
--rw-r--r--   0        0        0     7437 2024-05-14 22:22:17.767952 samgis_core-1.2.2/samgis_core/prediction_api/sam_onnx2.py
--rw-r--r--   0        0        0     5539 2024-05-14 22:22:17.768708 samgis_core-1.2.2/samgis_core/prediction_api/sam_onnx_inference.py
--rw-r--r--   0        0        0       32 2024-01-26 19:56:25.000000 samgis_core-1.2.2/samgis_core/utilities/__init__.py
--rw-r--r--   0        0        0      227 2024-05-14 22:57:43.817191 samgis_core-1.2.2/samgis_core/utilities/constants.py
--rw-r--r--   0        0        0      650 2024-04-21 19:58:55.718527 samgis_core-1.2.2/samgis_core/utilities/fastapi_logger.py
--rw-r--r--   0        0        0      263 2024-05-14 22:22:17.770297 samgis_core-1.2.2/samgis_core/utilities/plot_images.py
--rw-r--r--   0        0        0     2689 2024-04-21 19:58:55.721439 samgis_core-1.2.2/samgis_core/utilities/serialize.py
--rw-r--r--   0        0        0     1068 2024-05-14 22:22:17.771157 samgis_core-1.2.2/samgis_core/utilities/type_hints.py
--rw-r--r--   0        0        0     3286 2024-05-14 22:22:17.772035 samgis_core-1.2.2/samgis_core/utilities/utilities.py
--rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 samgis_core-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      262 2024-01-27 16:18:49.002975 samgis_core-2.0.0/README.md
+-rw-r--r--   0        0        0      754 2024-05-15 14:42:14.325883 samgis_core-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      351 2024-05-14 22:31:35.821860 samgis_core-2.0.0/samgis_core/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-21 19:58:55.709199 samgis_core-2.0.0/samgis_core/__version__.py
+-rw-r--r--   0        0        0       57 2024-01-26 19:56:25.000000 samgis_core-2.0.0/samgis_core/prediction_api/__init__.py
+-rw-r--r--   0        0        0     7437 2024-05-15 13:19:45.263381 samgis_core-2.0.0/samgis_core/prediction_api/sam_onnx2.py
+-rw-r--r--   0        0        0     5539 2024-05-14 22:22:17.768708 samgis_core-2.0.0/samgis_core/prediction_api/sam_onnx_inference.py
+-rw-r--r--   0        0        0       32 2024-01-26 19:56:25.000000 samgis_core-2.0.0/samgis_core/utilities/__init__.py
+-rw-r--r--   0        0        0      227 2024-05-14 22:57:43.817191 samgis_core-2.0.0/samgis_core/utilities/constants.py
+-rw-r--r--   0        0        0      650 2024-04-21 19:58:55.718527 samgis_core-2.0.0/samgis_core/utilities/fastapi_logger.py
+-rw-r--r--   0        0        0      263 2024-05-14 22:22:17.770297 samgis_core-2.0.0/samgis_core/utilities/plot_images.py
+-rw-r--r--   0        0        0     2689 2024-04-21 19:58:55.721439 samgis_core-2.0.0/samgis_core/utilities/serialize.py
+-rw-r--r--   0        0        0     1068 2024-05-14 22:22:17.771157 samgis_core-2.0.0/samgis_core/utilities/type_hints.py
+-rw-r--r--   0        0        0     3286 2024-05-14 22:22:17.772035 samgis_core-2.0.0/samgis_core/utilities/utilities.py
+-rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 samgis_core-2.0.0/PKG-INFO
```

### Comparing `samgis_core-1.2.2/pyproject.toml` & `samgis_core-2.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "samgis_core"
-version = "1.2.2"
+version = "2.0.0"
 description = "SamGIS CORE"
 authors = ["alessandro trinca tornidor <alessandro@trinca.tornidor.com>"]
 license = "MIT license"
 readme = "README.md"
 
 [metadata]
 name = "samgis_core"
-version = "1.2.2"
+version = "2.0.0"
 
 [tool.poetry.urls]
 Source = "https://gitlab.com/aletrn/samgis_core"
 
 [tool.poetry.dependencies]
 numpy = [
     {version = "1.25.2", python = "~3.10"},
```

### Comparing `samgis_core-1.2.2/samgis_core/prediction_api/sam_onnx2.py` & `samgis_core-2.0.0/samgis_core/prediction_api/sam_onnx2.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.2.2/samgis_core/prediction_api/sam_onnx_inference.py` & `samgis_core-2.0.0/samgis_core/prediction_api/sam_onnx_inference.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.2.2/samgis_core/utilities/fastapi_logger.py` & `samgis_core-2.0.0/samgis_core/utilities/fastapi_logger.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.2.2/samgis_core/utilities/serialize.py` & `samgis_core-2.0.0/samgis_core/utilities/serialize.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.2.2/samgis_core/utilities/type_hints.py` & `samgis_core-2.0.0/samgis_core/utilities/type_hints.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.2.2/samgis_core/utilities/utilities.py` & `samgis_core-2.0.0/samgis_core/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.2.2/PKG-INFO` & `samgis_core-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samgis_core
-Version: 1.2.2
+Version: 2.0.0
 Summary: SamGIS CORE
 License: MIT
 Author: alessandro trinca tornidor
 Author-email: alessandro@trinca.tornidor.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

