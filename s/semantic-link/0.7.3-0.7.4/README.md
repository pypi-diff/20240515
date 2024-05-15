# Comparing `tmp/semantic_link-0.7.3-py3-none-any.whl.zip` & `tmp/semantic_link-0.7.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
 Zip file size: 8236 bytes, number of entries: 5
--rw-rw-r--  2.0 unx    12690 b- defN 24-May-14 10:11 semantic_link-0.7.3.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     5068 b- defN 24-May-14 10:11 semantic_link-0.7.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-14 10:11 semantic_link-0.7.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 24-May-14 10:11 semantic_link-0.7.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      420 b- defN 24-May-14 10:11 semantic_link-0.7.3.dist-info/RECORD
+-rw-rw-r--  2.0 unx    12690 b- defN 24-May-15 07:56 semantic_link-0.7.4.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     5068 b- defN 24-May-15 07:56 semantic_link-0.7.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-15 07:56 semantic_link-0.7.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 24-May-15 07:56 semantic_link-0.7.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      420 b- defN 24-May-15 07:56 semantic_link-0.7.4.dist-info/RECORD
 5 files, 18271 bytes uncompressed, 7448 bytes compressed:  59.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: semantic_link-0.7.3.dist-info/LICENSE.txt
+Filename: semantic_link-0.7.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: semantic_link-0.7.3.dist-info/METADATA
+Filename: semantic_link-0.7.4.dist-info/METADATA
 Comment: 
 
-Filename: semantic_link-0.7.3.dist-info/WHEEL
+Filename: semantic_link-0.7.4.dist-info/WHEEL
 Comment: 
 
-Filename: semantic_link-0.7.3.dist-info/top_level.txt
+Filename: semantic_link-0.7.4.dist-info/top_level.txt
 Comment: 
 
-Filename: semantic_link-0.7.3.dist-info/RECORD
+Filename: semantic_link-0.7.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `semantic_link-0.7.3.dist-info/LICENSE.txt` & `semantic_link-0.7.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `semantic_link-0.7.3.dist-info/METADATA` & `semantic_link-0.7.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: semantic-link
-Version: 0.7.3
+Version: 0.7.4
 Summary: Semantic link for Microsoft Fabric
 Home-page: https://learn.microsoft.com/en-us/fabric/data-science/semantic-link-overview
 Author: Microsoft
 Author-email: semanticdatascience@service.microsoft.com
 License: proprietary and confidential
 Platform: Microsoft Fabric
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: ../LICENSE.txt
-Requires-Dist: semantic-link-sempy ==0.7.3
-Requires-Dist: semantic-link-functions-geopandas ==0.7.3
-Requires-Dist: semantic-link-functions-holidays ==0.7.3
-Requires-Dist: semantic-link-functions-meteostat ==0.7.3
-Requires-Dist: semantic-link-functions-phonenumbers ==0.7.3
-Requires-Dist: semantic-link-functions-validators ==0.7.3
+Requires-Dist: semantic-link-sempy ==0.7.4
+Requires-Dist: semantic-link-functions-geopandas ==0.7.4
+Requires-Dist: semantic-link-functions-holidays ==0.7.4
+Requires-Dist: semantic-link-functions-meteostat ==0.7.4
+Requires-Dist: semantic-link-functions-phonenumbers ==0.7.4
+Requires-Dist: semantic-link-functions-validators ==0.7.4
 
 Semantic link is a feature that allows you to establish a connection between [Power BI datasets](https://learn.microsoft.com/en-us/power-bi/connect-data/service-datasets-understand) and [Synapse Data Science in Microsoft Fabric](https://learn.microsoft.com/en-us/fabric/data-science/data-science-overview).  
 
 The primary goals of semantic link are to facilitate data connectivity, enable the propagation of semantic information, and seamlessly integrate with established tools used by data scientists, such as notebooks.  
 
 Semantic link helps you to preserve domain knowledge about data semantics in a standardized way that can speed up data analysis and reduce errors.
```

