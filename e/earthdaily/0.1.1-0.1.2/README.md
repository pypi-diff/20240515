# Comparing `tmp/earthdaily-0.1.1.tar.gz` & `tmp/earthdaily-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthdaily-0.1.1.tar", last modified: Mon May 13 14:06:33 2024, max compression
+gzip compressed data, was "earthdaily-0.1.2.tar", last modified: Wed May 15 16:11:08 2024, max compression
```

## Comparing `earthdaily-0.1.1.tar` & `earthdaily-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-13 14:06:33.000000 earthdaily-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-13 14:06:33.509983 earthdaily-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-13 14:06:33.000000 earthdaily-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.505983 earthdaily-0.1.1/earthdaily/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.505983 earthdaily-0.1.1/earthdaily/accessor/
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/accessor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.505983 earthdaily-0.1.1/earthdaily/accessor/whittaker/
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/accessor/whittaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/accessor/whittaker/_pywapor_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.505983 earthdaily-0.1.1/earthdaily/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/earthdaily/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/datasets/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/datasets/data/pivot.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/datasets/data/pivot_corumba.geojson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/earthdaily/earthdatastore/
--rw-r--r--   0 runner    (1001) docker     (127)    37428 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/_scales_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/
--rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/_zonal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/custom_reducers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/geometry_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/harmonizer/
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/earthdaily/earthdatastore/mask/
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/mask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.505983 earthdaily-0.1.1/earthdaily.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:06:33.509983 earthdaily-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-13 14:06:33.000000 earthdaily-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.526383 earthdaily-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-15 16:11:07.000000 earthdaily-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-15 16:11:08.526383 earthdaily-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-15 16:11:07.000000 earthdaily-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily/accessor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/accessor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily/accessor/whittaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/accessor/whittaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/accessor/whittaker/_pywapor_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/datasets/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/datasets/data/pivot.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/datasets/data/pivot_corumba.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily/earthdatastore/
+-rw-r--r--   0 runner    (1001) docker     (127)    37428 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/_scales_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.526383 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/_zonal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.526383 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/custom_reducers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/geometry_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.526383 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/harmonizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.526383 earthdaily-0.1.2/earthdaily/earthdatastore/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-15 16:11:07.000000 earthdaily-0.1.2/earthdaily/earthdatastore/mask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:11:08.522382 earthdaily-0.1.2/earthdaily.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-15 16:11:08.000000 earthdaily-0.1.2/earthdaily.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-15 16:11:08.000000 earthdaily-0.1.2/earthdaily.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:11:08.000000 earthdaily-0.1.2/earthdaily.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:11:08.000000 earthdaily-0.1.2/earthdaily.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 16:11:08.000000 earthdaily-0.1.2/earthdaily.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 16:11:08.000000 earthdaily-0.1.2/earthdaily.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:11:08.526383 earthdaily-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-15 16:11:07.000000 earthdaily-0.1.2/setup.py
```

### Comparing `earthdaily-0.1.1/LICENSE` & `earthdaily-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/PKG-INFO` & `earthdaily-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthdaily
-Version: 0.1.1
+Version: 0.1.2
 Summary: earthdaily: easy authentication, search and retrieval of Earth Data Store collections data
 Home-page: UNKNOWN
 Author: EarthDaily Agro
 License: MIT
 Keywords: Earth Data Store,earthdaily,earthdailyagro,stac
 Platform: UNKNOWN
 Requires-Python: >=3.10
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_hrji1bbk_/tmpo04r2cyu_TarContainer/0/2", line 25, column 36: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthdaily Version: 0.1.1 Summary: earthdaily: easy
+Metadata-Version: 2.1 Name: earthdaily Version: 0.1.2 Summary: earthdaily: easy
 authentication, search and retrieval of Earth Data Store collections data Home-
 page: UNKNOWN Author: EarthDaily Agro License: MIT Keywords: Earth Data
 Store,earthdaily,earthdailyagro,stac Platform: UNKNOWN Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 
 ************ EEaarrtthhDDaaiillyy PPyytthhoonn CClliieenntt ************
 Your gateway to the Earth Data Store STAC Catalog.
```

### Comparing `earthdaily-0.1.1/README.md` & `earthdaily-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/accessor/__init__.py` & `earthdaily-0.1.2/earthdaily/accessor/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/accessor/whittaker/__init__.py` & `earthdaily-0.1.2/earthdaily/accessor/whittaker/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/accessor/whittaker/_pywapor_core.py` & `earthdaily-0.1.2/earthdaily/accessor/whittaker/_pywapor_core.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/datasets/__init__.py` & `earthdaily-0.1.2/earthdaily/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/datasets/data/pivot.geojson` & `earthdaily-0.1.2/earthdaily/datasets/data/pivot.geojson`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/datasets/data/pivot_corumba.geojson` & `earthdaily-0.1.2/earthdaily/datasets/data/pivot_corumba.geojson`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/earthdatastore/__init__.py` & `earthdaily-0.1.2/earthdaily/earthdatastore/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/earthdatastore/_scales_collections.py` & `earthdaily-0.1.2/earthdaily/earthdatastore/_scales_collections.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/__init__.py` & `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/_zonal.py` & `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/_zonal.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py` & `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py` & `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json` & `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/custom_reducers.py` & `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/custom_reducers.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,13 +26,13 @@
             list(dim for dim in data_array_grouped.dims if dim != "time"),
         )
         return result
 
     @staticmethod
     def register_custom_reducers():
         # register custom methods fo DataArrayGroupBy
-        xr.core.groupby.DataArrayGroupBy.mode = CustomReducers.mode
-        xr.core.groupby.DatasetGroupBy.mode = CustomReducers.mode
+        groupby.DataArrayGroupBy.mode = CustomReducers.mode
+        groupby.DatasetGroupBy.mode = CustomReducers.mode
         np.mode = CustomReducers._np_mode
 
 
 CustomReducers.register_custom_reducers()
```

### Comparing `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/geometry_manager.py` & `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/geometry_manager.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py` & `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/preprocessing.py` & `earthdaily-0.1.2/earthdaily/earthdatastore/cube_utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/earthdaily/earthdatastore/mask/__init__.py` & `earthdaily-0.1.2/earthdaily/earthdatastore/mask/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 class Mask:
     def __init__(self, dataset: xr.Dataset, intersects=None, bbox=None):
         self._obj = dataset
         if bbox and intersects is None:
             intersects = _bbox_to_intersects(bbox)
         if isinstance(intersects, gpd.GeoDataFrame):
-            intersects = intersects.to_crs(self._obj.rio.crs).head(1)
+            intersects = intersects.to_crs(self._obj.rio.crs)
         self.intersects = intersects
 
     def ag_cloud_mask(
         self,
         acm_datacube,
         add_mask_var=False,
         mask_statistics=False,
```

### Comparing `earthdaily-0.1.1/earthdaily.egg-info/PKG-INFO` & `earthdaily-0.1.2/earthdaily.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthdaily
-Version: 0.1.1
+Version: 0.1.2
 Summary: earthdaily: easy authentication, search and retrieval of Earth Data Store collections data
 Home-page: UNKNOWN
 Author: EarthDaily Agro
 License: MIT
 Keywords: Earth Data Store,earthdaily,earthdailyagro,stac
 Platform: UNKNOWN
 Requires-Python: >=3.10
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_hrji1bbk_/tmpo04r2cyu_TarContainer/0/35", line 25, column 36: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthdaily Version: 0.1.1 Summary: earthdaily: easy
+Metadata-Version: 2.1 Name: earthdaily Version: 0.1.2 Summary: earthdaily: easy
 authentication, search and retrieval of Earth Data Store collections data Home-
 page: UNKNOWN Author: EarthDaily Agro License: MIT Keywords: Earth Data
 Store,earthdaily,earthdailyagro,stac Platform: UNKNOWN Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 
 ************ EEaarrtthhDDaaiillyy PPyytthhoonn CClliieenntt ************
 Your gateway to the Earth Data Store STAC Catalog.
```

### Comparing `earthdaily-0.1.1/earthdaily.egg-info/SOURCES.txt` & `earthdaily-0.1.2/earthdaily.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.1/setup.py` & `earthdaily-0.1.2/setup.py`

 * *Files identical despite different names*

