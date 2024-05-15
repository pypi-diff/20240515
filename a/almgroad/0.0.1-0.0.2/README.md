# Comparing `tmp/almgroad-0.0.1-py3-none-any.whl.zip` & `tmp/almgroad-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 2545 bytes, number of entries: 6
--rw-rw----  2.0 unx       33 b- defN 24-May-14 19:19 almgroad/__init__.py
+Zip file size: 2823 bytes, number of entries: 7
+-rw-rw----  2.0 unx       55 b- defN 24-May-15 03:30 almgroad/__init__.py
+-rw-rw----  2.0 unx      128 b- defN 24-May-15 03:17 almgroad/chat.py
 -rw-rw----  2.0 unx      937 b- defN 24-May-14 19:17 almgroad/infoinsta.py
--rw-rw----  2.0 unx     1410 b- defN 24-May-14 19:20 almgroad-0.0.1.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 24-May-14 19:20 almgroad-0.0.1.dist-info/WHEEL
--rw-rw----  2.0 unx        9 b- defN 24-May-14 19:20 almgroad-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      453 b- defN 24-May-14 19:20 almgroad-0.0.1.dist-info/RECORD
-6 files, 2934 bytes uncompressed, 1721 bytes compressed:  41.3%
+-rw-rw----  2.0 unx     1410 b- defN 24-May-15 03:32 almgroad-0.0.2.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 24-May-15 03:32 almgroad-0.0.2.dist-info/WHEEL
+-rw-rw----  2.0 unx        9 b- defN 24-May-15 03:32 almgroad-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      525 b- defN 24-May-15 03:32 almgroad-0.0.2.dist-info/RECORD
+7 files, 3156 bytes uncompressed, 1891 bytes compressed:  40.1%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: almgroad/__init__.py
 Comment: 
 
+Filename: almgroad/chat.py
+Comment: 
+
 Filename: almgroad/infoinsta.py
 Comment: 
 
-Filename: almgroad-0.0.1.dist-info/METADATA
+Filename: almgroad-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: almgroad-0.0.1.dist-info/WHEEL
+Filename: almgroad-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: almgroad-0.0.1.dist-info/top_level.txt
+Filename: almgroad-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: almgroad-0.0.1.dist-info/RECORD
+Filename: almgroad-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## almgroad/__init__.py

```diff
@@ -1 +1,2 @@
-from .infoinsta import Info_Insta
+from .infoinsta import Info_Insta
+from .chat import GPT
```

## Comparing `almgroad-0.0.1.dist-info/METADATA` & `almgroad-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almgroad
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Ibrahim Mohammed
 Author-email: ibrahom0780@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

