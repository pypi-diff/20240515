# Comparing `tmp/semantic_link_functions_geopandas-0.7.3-py3-none-any.whl.zip` & `tmp/semantic_link_functions_geopandas-0.7.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3953 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       97 b- defN 24-May-14 10:08 sempy_functions_geopandas/__init__.py
--rw-rw-r--  2.0 unx     1383 b- defN 24-May-14 10:08 sempy_functions_geopandas/_geopandas.py
--rw-rw-r--  2.0 unx     1141 b- defN 24-May-14 10:11 semantic_link_functions_geopandas-0.7.3.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     1855 b- defN 24-May-14 10:11 semantic_link_functions_geopandas-0.7.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-14 10:11 semantic_link_functions_geopandas-0.7.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       26 b- defN 24-May-14 10:11 semantic_link_functions_geopandas-0.7.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      708 b- defN 24-May-14 10:11 semantic_link_functions_geopandas-0.7.3.dist-info/RECORD
-7 files, 5302 bytes uncompressed, 2661 bytes compressed:  49.8%
+Zip file size: 3954 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       97 b- defN 24-May-15 07:53 sempy_functions_geopandas/__init__.py
+-rw-rw-r--  2.0 unx     1383 b- defN 24-May-15 07:53 sempy_functions_geopandas/_geopandas.py
+-rw-rw-r--  2.0 unx     1141 b- defN 24-May-15 07:56 semantic_link_functions_geopandas-0.7.4.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     1855 b- defN 24-May-15 07:56 semantic_link_functions_geopandas-0.7.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-15 07:56 semantic_link_functions_geopandas-0.7.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       26 b- defN 24-May-15 07:56 semantic_link_functions_geopandas-0.7.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      708 b- defN 24-May-15 07:56 semantic_link_functions_geopandas-0.7.4.dist-info/RECORD
+7 files, 5302 bytes uncompressed, 2662 bytes compressed:  49.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sempy_functions_geopandas/__init__.py
 Comment: 
 
 Filename: sempy_functions_geopandas/_geopandas.py
 Comment: 
 
-Filename: semantic_link_functions_geopandas-0.7.3.dist-info/LICENSE.txt
+Filename: semantic_link_functions_geopandas-0.7.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: semantic_link_functions_geopandas-0.7.3.dist-info/METADATA
+Filename: semantic_link_functions_geopandas-0.7.4.dist-info/METADATA
 Comment: 
 
-Filename: semantic_link_functions_geopandas-0.7.3.dist-info/WHEEL
+Filename: semantic_link_functions_geopandas-0.7.4.dist-info/WHEEL
 Comment: 
 
-Filename: semantic_link_functions_geopandas-0.7.3.dist-info/top_level.txt
+Filename: semantic_link_functions_geopandas-0.7.4.dist-info/top_level.txt
 Comment: 
 
-Filename: semantic_link_functions_geopandas-0.7.3.dist-info/RECORD
+Filename: semantic_link_functions_geopandas-0.7.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `semantic_link_functions_geopandas-0.7.3.dist-info/LICENSE.txt` & `semantic_link_functions_geopandas-0.7.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `semantic_link_functions_geopandas-0.7.3.dist-info/METADATA` & `semantic_link_functions_geopandas-0.7.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-link-functions-geopandas
-Version: 0.7.3
+Version: 0.7.4
 Summary: Semantic link functions for Geopandas. Enables conversion of a FabricDataFrame to a GeoDataFrame.
 Home-page: https://github.com/microsoft/semantic-link-functions
 Author: Microsoft
 Author-email: semanticdatascience@service.microsoft.com
 License: MIT License
 Platform: Microsoft Fabric
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: ../LICENSE.txt
 Requires-Dist: geopandas
 Requires-Dist: folium
 Requires-Dist: mapclassify
-Requires-Dist: semantic-link-sempy ==0.7.3
+Requires-Dist: semantic-link-sempy ==0.7.4
 
 FabricDataFrames dynamically expose semantic functions based on logic defined by each function. For example, the is_holiday function shows up in the autocomplete suggestions when you're working on a FabricDataFrame containing both a datetime column and a country column.
 
 Each semantic function uses information about the data types, metadata (such as Power BI data categories), and the data in a FabricDataFrame or FabricSeries to determine its relevance to the particular data on which you're working.
 
 Semantic functions are automatically discovered when annotated with the @semantic_function decorator. You can think of semantic functions as being similar to C# extension methods applied to the popular DataFrame concept.
```

## Comparing `semantic_link_functions_geopandas-0.7.3.dist-info/RECORD` & `semantic_link_functions_geopandas-0.7.4.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 sempy_functions_geopandas/__init__.py,sha256=CItuT_RwqSfL3BmEgTuh5ddGRAfOsxvQ84FzHfuFvkE,97
 sempy_functions_geopandas/_geopandas.py,sha256=xMDAizH0MeX93dF3zOaIOrOv55hL0kPfyzVqxNUMq-s,1383
-semantic_link_functions_geopandas-0.7.3.dist-info/LICENSE.txt,sha256=ws_MuBL-SCEBqPBFl9_FqZkaaydIJmxHrJG2parhU4M,1141
-semantic_link_functions_geopandas-0.7.3.dist-info/METADATA,sha256=w9BAj3H8O4NsGQSy2zTiznjPe_AzLLq8NAtjysJ7dfQ,1855
-semantic_link_functions_geopandas-0.7.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-semantic_link_functions_geopandas-0.7.3.dist-info/top_level.txt,sha256=Scr21O7qL4sTmEHRS1VyvOFK3rw_cICZ02X4RfprL4w,26
-semantic_link_functions_geopandas-0.7.3.dist-info/RECORD,,
+semantic_link_functions_geopandas-0.7.4.dist-info/LICENSE.txt,sha256=ws_MuBL-SCEBqPBFl9_FqZkaaydIJmxHrJG2parhU4M,1141
+semantic_link_functions_geopandas-0.7.4.dist-info/METADATA,sha256=LFM9Iwo2JjDXD3WJGvCikqnvAPk3JfeTDFaBcyhmDtI,1855
+semantic_link_functions_geopandas-0.7.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+semantic_link_functions_geopandas-0.7.4.dist-info/top_level.txt,sha256=Scr21O7qL4sTmEHRS1VyvOFK3rw_cICZ02X4RfprL4w,26
+semantic_link_functions_geopandas-0.7.4.dist-info/RECORD,,
```

