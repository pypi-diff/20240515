# Comparing `tmp/ImageDimensionCheck-1.0-py3-none-any.whl.zip` & `tmp/ImageDimensionCheck-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2616 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     1401 b- defN 24-May-15 05:51 ImageDimensionCheck/__init__.py
--rw-rw-rw-  2.0 fat      681 b- defN 24-May-15 07:06 ImageDimensionCheck-1.0.dist-info/License.txt
--rw-rw-rw-  2.0 fat      383 b- defN 24-May-15 07:06 ImageDimensionCheck-1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 07:06 ImageDimensionCheck-1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 24-May-15 07:06 ImageDimensionCheck-1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      526 b- defN 24-May-15 07:06 ImageDimensionCheck-1.0.dist-info/RECORD
-6 files, 3103 bytes uncompressed, 1650 bytes compressed:  46.8%
+Zip file size: 2725 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     1860 b- defN 24-May-15 07:33 ImageDimensionCheck/__init__.py
+-rw-rw-rw-  2.0 fat      681 b- defN 24-May-15 07:34 ImageDimensionCheck-1.1.dist-info/License.txt
+-rw-rw-rw-  2.0 fat      383 b- defN 24-May-15 07:34 ImageDimensionCheck-1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 07:34 ImageDimensionCheck-1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 24-May-15 07:34 ImageDimensionCheck-1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      526 b- defN 24-May-15 07:34 ImageDimensionCheck-1.1.dist-info/RECORD
+6 files, 3562 bytes uncompressed, 1759 bytes compressed:  50.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: ImageDimensionCheck/__init__.py
 Comment: 
 
-Filename: ImageDimensionCheck-1.0.dist-info/License.txt
+Filename: ImageDimensionCheck-1.1.dist-info/License.txt
 Comment: 
 
-Filename: ImageDimensionCheck-1.0.dist-info/METADATA
+Filename: ImageDimensionCheck-1.1.dist-info/METADATA
 Comment: 
 
-Filename: ImageDimensionCheck-1.0.dist-info/WHEEL
+Filename: ImageDimensionCheck-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: ImageDimensionCheck-1.0.dist-info/top_level.txt
+Filename: ImageDimensionCheck-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ImageDimensionCheck-1.0.dist-info/RECORD
+Filename: ImageDimensionCheck-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ImageDimensionCheck/__init__.py

```diff
@@ -41,8 +41,27 @@
             break
 
     if flag==1:
         print('Different dimensions detected')
         return False
     else:
         print('All images have same dimensions')
-        return True
+        return True
+    
+
+
+def unique_extension(path):
+    path = path + "/"
+    image_files = os.listdir(path)
+    number_of_images = len(image_files)
+    if not image_files:
+        print("No images found in the specified directory.")
+        return
+
+    extension_list = []
+    for img in image_files:
+         ext = img.split('.')[1]
+         extension_list.append(ext)
+
+    unique_ext = Counter(extension_list)
+    print(unique_ext)
+    return unique_ext
```

## Comparing `ImageDimensionCheck-1.0.dist-info/License.txt` & `ImageDimensionCheck-1.1.dist-info/License.txt`

 * *Files identical despite different names*

