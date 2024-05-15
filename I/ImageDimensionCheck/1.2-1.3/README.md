# Comparing `tmp/ImageDimensionCheck-1.2-py3-none-any.whl.zip` & `tmp/ImageDimensionCheck-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2813 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     2417 b- defN 24-May-15 08:08 ImageDimensionCheck/__init__.py
--rw-rw-rw-  2.0 fat      681 b- defN 24-May-15 08:10 ImageDimensionCheck-1.2.dist-info/License.txt
--rw-rw-rw-  2.0 fat      383 b- defN 24-May-15 08:10 ImageDimensionCheck-1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 08:10 ImageDimensionCheck-1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 24-May-15 08:10 ImageDimensionCheck-1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      526 b- defN 24-May-15 08:10 ImageDimensionCheck-1.2.dist-info/RECORD
-6 files, 4119 bytes uncompressed, 1847 bytes compressed:  55.2%
+Zip file size: 2831 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     2450 b- defN 24-May-15 08:13 ImageDimensionCheck/__init__.py
+-rw-rw-rw-  2.0 fat      681 b- defN 24-May-15 08:13 ImageDimensionCheck-1.3.dist-info/License.txt
+-rw-rw-rw-  2.0 fat      383 b- defN 24-May-15 08:13 ImageDimensionCheck-1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 08:13 ImageDimensionCheck-1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 24-May-15 08:13 ImageDimensionCheck-1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      526 b- defN 24-May-15 08:13 ImageDimensionCheck-1.3.dist-info/RECORD
+6 files, 4152 bytes uncompressed, 1865 bytes compressed:  55.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: ImageDimensionCheck/__init__.py
 Comment: 
 
-Filename: ImageDimensionCheck-1.2.dist-info/License.txt
+Filename: ImageDimensionCheck-1.3.dist-info/License.txt
 Comment: 
 
-Filename: ImageDimensionCheck-1.2.dist-info/METADATA
+Filename: ImageDimensionCheck-1.3.dist-info/METADATA
 Comment: 
 
-Filename: ImageDimensionCheck-1.2.dist-info/WHEEL
+Filename: ImageDimensionCheck-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: ImageDimensionCheck-1.2.dist-info/top_level.txt
+Filename: ImageDimensionCheck-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ImageDimensionCheck-1.2.dist-info/RECORD
+Filename: ImageDimensionCheck-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ImageDimensionCheck/__init__.py

```diff
@@ -1,10 +1,11 @@
 import glob
 import cv2
 import os
+from collections import Counter
 def CheckImageDimension(path,extension=['jpg','png']):
     path = path + "//"
     for ext in extension:
         pattern = path + '*.' + f'{ext}'
         files = glob.glob(pattern)
         print(f'The number of {ext} files:', files)
```

## Comparing `ImageDimensionCheck-1.2.dist-info/License.txt` & `ImageDimensionCheck-1.3.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `ImageDimensionCheck-1.2.dist-info/RECORD` & `ImageDimensionCheck-1.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-ImageDimensionCheck/__init__.py,sha256=_2A08uZy1I4W_vBdmars_sIPMA7ZR9RZpEASMrE0OAo,2417
-ImageDimensionCheck-1.2.dist-info/License.txt,sha256=-yhss5DjkbDGu0qex5cIplTDrDByvpTAJSinwMkY9hI,681
-ImageDimensionCheck-1.2.dist-info/METADATA,sha256=dhLMtwSFD9iDtqpq29i8_Z1VkWWiTVzXPiDAavHObHA,383
-ImageDimensionCheck-1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ImageDimensionCheck-1.2.dist-info/top_level.txt,sha256=eUT3M4j7r7bBczs3WljnWZYYAIWao9mq8MOidch_pg0,20
-ImageDimensionCheck-1.2.dist-info/RECORD,,
+ImageDimensionCheck/__init__.py,sha256=apcwA37hqXjizDH1a_2g7agEBi72dHq-ppc8eWFxUcE,2450
+ImageDimensionCheck-1.3.dist-info/License.txt,sha256=-yhss5DjkbDGu0qex5cIplTDrDByvpTAJSinwMkY9hI,681
+ImageDimensionCheck-1.3.dist-info/METADATA,sha256=BThJZX9zGdATVkrjUsLS01cNc_5kMNqBeC8pINdhjYA,383
+ImageDimensionCheck-1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ImageDimensionCheck-1.3.dist-info/top_level.txt,sha256=eUT3M4j7r7bBczs3WljnWZYYAIWao9mq8MOidch_pg0,20
+ImageDimensionCheck-1.3.dist-info/RECORD,,
```

