# Comparing `tmp/samgis-1.4.1.tar.gz` & `tmp/samgis-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samgis-1.4.1.tar", max compression
+gzip compressed data, was "samgis-1.5.1.tar", max compression
```

## Comparing `samgis-1.4.1.tar` & `samgis-1.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1083 2023-12-26 17:08:59.536811 samgis-1.4.1/LICENSE.txt
--rw-r--r--   0        0        0     4483 2024-04-21 20:31:14.348763 samgis-1.4.1/README.md
--rw-r--r--   0        0        0     1697 2024-04-21 21:36:44.338368 samgis-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      871 2024-03-14 22:19:15.162025 samgis-1.4.1/samgis/__init__.py
--rw-r--r--   0        0        0      259 2024-04-21 20:09:08.722043 samgis-1.4.1/samgis/__version__.py
--rw-r--r--   0        0        0       37 2023-12-28 22:28:53.465242 samgis-1.4.1/samgis/io/__init__.py
--rw-r--r--   0        0        0     4268 2024-04-21 20:09:08.722874 samgis-1.4.1/samgis/io/coordinates_pixel_conversion.py
--rw-r--r--   0        0        0     3594 2024-04-21 20:09:08.723676 samgis-1.4.1/samgis/io/geo_helpers.py
--rw-r--r--   0        0        0    10924 2024-04-14 19:45:50.292575 samgis-1.4.1/samgis/io/raster_helpers.py
--rw-r--r--   0        0        0     9333 2024-04-21 20:09:08.724534 samgis-1.4.1/samgis/io/tms2geotiff.py
--rw-r--r--   0        0        0     8359 2024-04-21 20:09:08.725416 samgis-1.4.1/samgis/io/wrappers_helpers.py
--rw-r--r--   0        0        0       57 2023-12-28 22:28:53.468814 samgis-1.4.1/samgis/prediction_api/__init__.py
--rw-r--r--   0        0        0     3862 2024-04-21 20:09:08.726222 samgis-1.4.1/samgis/prediction_api/predictors.py
--rw-r--r--   0        0        0       32 2023-12-28 22:28:53.470549 samgis-1.4.1/samgis/utilities/__init__.py
--rw-r--r--   0        0        0     2016 2024-01-31 21:48:25.987034 samgis-1.4.1/samgis/utilities/constants.py
--rw-r--r--   0        0        0     2468 2024-04-21 20:09:08.726938 samgis-1.4.1/samgis/utilities/type_hints.py
--rw-r--r--   0        0        0     5795 1970-01-01 00:00:00.000000 samgis-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-12-26 17:08:59.536811 samgis-1.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     7188 2024-05-15 19:06:56.572501 samgis-1.5.1/README.md
+-rw-r--r--   0        0        0     1655 2024-05-15 18:48:58.872273 samgis-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      923 2024-04-29 14:10:04.501931 samgis-1.5.1/samgis/__init__.py
+-rw-r--r--   0        0        0      259 2024-05-15 18:51:05.745730 samgis-1.5.1/samgis/__version__.py
+-rw-r--r--   0        0        0       37 2023-12-28 22:28:53.465242 samgis-1.5.1/samgis/io/__init__.py
+-rw-r--r--   0        0        0     4268 2024-04-21 20:09:08.722874 samgis-1.5.1/samgis/io/coordinates_pixel_conversion.py
+-rw-r--r--   0        0        0     3594 2024-04-21 20:09:08.723676 samgis-1.5.1/samgis/io/geo_helpers.py
+-rw-r--r--   0        0        0    12256 2024-04-29 14:10:04.502760 samgis-1.5.1/samgis/io/raster_helpers.py
+-rw-r--r--   0        0        0     9333 2024-04-21 20:09:08.724534 samgis-1.5.1/samgis/io/tms2geotiff.py
+-rw-r--r--   0        0        0     8359 2024-04-21 20:09:08.725416 samgis-1.5.1/samgis/io/wrappers_helpers.py
+-rw-r--r--   0        0        0       57 2023-12-28 22:28:53.468814 samgis-1.5.1/samgis/prediction_api/__init__.py
+-rw-r--r--   0        0        0     4787 2024-05-15 18:48:58.877405 samgis-1.5.1/samgis/prediction_api/predictors.py
+-rw-r--r--   0        0        0       32 2023-12-28 22:28:53.470549 samgis-1.5.1/samgis/utilities/__init__.py
+-rw-r--r--   0        0        0     2078 2024-05-15 18:48:58.881969 samgis-1.5.1/samgis/utilities/constants.py
+-rw-r--r--   0        0        0     2468 2024-04-21 20:09:08.726938 samgis-1.5.1/samgis/utilities/type_hints.py
+-rw-r--r--   0        0        0     8402 1970-01-01 00:00:00.000000 samgis-1.5.1/PKG-INFO
```

### Comparing `samgis-1.4.1/LICENSE.txt` & `samgis-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `samgis-1.4.1/pyproject.toml` & `samgis-1.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 [tool.poetry]
 name = "samgis"
-version = "1.4.1"
+version = "1.5.1"
 description = "A backend for machine learning instance segmentation on geospatial data even without dedicated graphics cards."
 authors = ["alessandro trinca tornidor <alessandro@trinca.tornidor.com>"]
 license = "MIT license"
 readme = "README.md"
 
 [metadata]
 name = "samgis"
-version = "1.4.1"
+version = "1.5.1"
 
 [tool.poetry.urls]
 Source = "https://github.com/trincadev/samgis-be"
 Demo = "https://huggingface.co/spaces/aletrn/samgis"
 
 [tool.poetry.dependencies]
 bson = "^0.5.10"
 contextily = "^1.5.2"
 geopandas = "^0.14.3"
 loguru = "^0.7.2"
 numpy = [
     {version = "1.25.2", python = "~3.10"},
     {version = "^1.26", python = "~3.11"}
 ]
-onnxruntime = "1.16.3"
-opencv-python-headless = "^4.8.1.78"
 pillow = "^10.2.0"
 python = ">=3.10, <3.12"
 python-dotenv = "^1.0.1"
 rasterio = "^1.3.9"
 requests = "^2.31.0"
-samgis-core = "~1.2.0"
+samgis-core = "~2.0.0"
 
 [tool.poetry.group.aws_lambda]
 optional = true
 
 [tool.poetry.group.aws_lambda.dependencies]
 aws-lambda-powertools = "^2.30.2"
 awslambdaric = "^2.0.10"
@@ -61,14 +59,15 @@
 sphinx-autodoc-defaultargs = "^0.1.2"
 
 [tool.poetry.group.fastapi]
 optional = true
 
 [tool.poetry.group.fastapi.dependencies]
 fastapi = "^0.110.0"
+jinja2 = "^3.1.3"
 loguru = "^0.7.2"
 pydantic = "^2.6.3"
 uvicorn = "^0.28.0" 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `samgis-1.4.1/samgis/__init__.py` & `samgis-1.5.1/samgis/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # not used here but contextily_tile is imported in samgis.io.tms2geotiff
 from contextily import tile as contextily_tile
 from pathlib import Path
 from samgis.utilities.constants import SERVICE_NAME
 
 PROJECT_ROOT_FOLDER = Path(globals().get("__file__", "./_")).absolute().parent.parent
+WORKDIR = os.getenv("WORKDIR", PROJECT_ROOT_FOLDER)
 MODEL_FOLDER = Path(PROJECT_ROOT_FOLDER / "machine_learning_models")
 
 IS_AWS_LAMBDA = bool(os.getenv("IS_AWS_LAMBDA", ""))
 
 if IS_AWS_LAMBDA:
     try:
         from aws_lambda_powertools import Logger
```

### Comparing `samgis-1.4.1/samgis/io/coordinates_pixel_conversion.py` & `samgis-1.5.1/samgis/io/coordinates_pixel_conversion.py`

 * *Files identical despite different names*

### Comparing `samgis-1.4.1/samgis/io/geo_helpers.py` & `samgis-1.5.1/samgis/io/geo_helpers.py`

 * *Files identical despite different names*

### Comparing `samgis-1.4.1/samgis/io/raster_helpers.py` & `samgis-1.5.1/samgis/io/raster_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """helpers for computer vision duties"""
 import numpy as np
 from numpy import ndarray, bitwise_not
+from rasterio import open as rasterio_open
 
 from samgis import app_logger
 from samgis.utilities.type_hints import XYZTerrainProvidersNames
+from samgis.utilities.constants import OUTPUT_CRS_STRING
 
 
 def get_nextzen_terrain_rgb_formula(red: ndarray, green: ndarray, blue: ndarray) -> ndarray:
     """
     Compute a 32-bits 2d digital elevation model from a nextzen 'terrarium' (terrain-rgb) raster.
     'Terrarium' format PNG tiles contain raw elevation data in meters, in Mercator projection (EPSG:3857).
     All values are positive with a 32,768 offset, split into the red, green, and blue channels,
@@ -288,7 +290,41 @@
     arr[np.isnan(arr)] = 0
     check4 = np.array_equal(arr, np.zeros((arr_size, arr_size)))
     arr_check5 = np.ones((arr_size, arr_size)) * val
     arr_check5_tmp[np.isnan(arr_check5_tmp)] = val
     check5 = np.array_equal(arr_check5_tmp, arr_check5)
     app_logger.debug(f"array checks:{check1}, {check2}, {check3}, {check4}, {check5}.")
     return check1 or check2 or check3 or check4 or check5
+
+
+def write_raster_png(arr, transform, prefix: str, suffix: str, folder_output_path="/tmp"):
+    from pathlib import Path
+    from rasterio.plot import reshape_as_raster
+
+    output_filename = Path(folder_output_path) / f"{prefix}_{suffix}.png"
+
+    with rasterio_open(
+            output_filename, 'w', driver='PNG',
+            height=arr.shape[0],
+            width=arr.shape[1],
+            count=3,
+            dtype=str(arr.dtype),
+            crs=OUTPUT_CRS_STRING,
+            transform=transform) as dst:
+        dst.write(reshape_as_raster(arr))
+    app_logger.info(f"written:{output_filename} as PNG, use {OUTPUT_CRS_STRING} as CRS.")
+
+
+def write_raster_tiff(arr, transform, prefix: str, suffix: str, folder_output_path="/tmp"):
+    from pathlib import Path
+    output_filename = Path(folder_output_path) / f"{prefix}_{suffix}.tiff"
+
+    with rasterio_open(
+            output_filename, 'w', driver='GTiff',
+            height=arr.shape[0],
+            width=arr.shape[1],
+            count=1,
+            dtype=str(arr.dtype),
+            crs=OUTPUT_CRS_STRING,
+            transform=transform) as dst:
+        dst.write(arr, 1)
+    app_logger.info(f"written:{output_filename} as TIFF, use {OUTPUT_CRS_STRING} as CRS.")
```

### Comparing `samgis-1.4.1/samgis/io/tms2geotiff.py` & `samgis-1.5.1/samgis/io/tms2geotiff.py`

 * *Files identical despite different names*

### Comparing `samgis-1.4.1/samgis/io/wrappers_helpers.py` & `samgis-1.5.1/samgis/io/wrappers_helpers.py`

 * *Files identical despite different names*

### Comparing `samgis-1.4.1/samgis/utilities/constants.py` & `samgis-1.5.1/samgis/utilities/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """Project constants"""
+import os
+
+
 INPUT_CRS_STRING = "EPSG:4326"
 OUTPUT_CRS_STRING = "EPSG:3857"
 DRIVER_RASTERIO_GTIFF = "GTiff"
 ROOT = "/tmp"
 CUSTOM_RESPONSE_MESSAGES = {
     200: "ok",
     400: "Bad Request",
@@ -34,7 +37,8 @@
 COMPLETE_URL_TILES_MAPBOX = f"https://{DOMAIN_URL_TILES_MAPBOX}/{RELATIVE_URL_TILES_MAPBOX}"
 # https://s3.amazonaws.com/elevation-tiles-prod/terrarium/13/1308/3167.png
 DOMAIN_URL_TILES_NEXTZEN = "s3.amazonaws.com"
 RELATIVE_URL_TILES_NEXTZEN = "elevation-tiles-prod/terrarium/{z}/{x}/{y}.png"  # "terrarium/{z}/{x}/{y}.png"
 COMPLETE_URL_TILES_NEXTZEN = f"https://{DOMAIN_URL_TILES_NEXTZEN}/{RELATIVE_URL_TILES_NEXTZEN}"
 CHANNEL_EXAGGERATIONS_LIST = [2.5, 1.1, 2.0]
 SLOPE_CELLSIZE = 61
+MODEL_NAME = os.getenv("MODEL_NAME", "mobile_sam")
```

### Comparing `samgis-1.4.1/samgis/utilities/type_hints.py` & `samgis-1.5.1/samgis/utilities/type_hints.py`

 * *Files identical despite different names*

