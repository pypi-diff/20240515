# Comparing `tmp/almgroad-0.0.5-py3-none-any.whl.zip` & `tmp/almgroad-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 2825 bytes, number of entries: 7
--rw-rw----  2.0 unx       55 b- defN 24-May-15 03:30 almgroad/__init__.py
+Zip file size: 22931 bytes, number of entries: 8
+-rw-rw----  2.0 unx       76 b- defN 24-May-15 08:45 almgroad/__init__.py
 -rw-rw----  2.0 unx      128 b- defN 24-May-15 03:17 almgroad/chat.py
 -rw-rw----  2.0 unx     1071 b- defN 24-May-15 04:51 almgroad/infoinsta.py
--rw-rw----  2.0 unx     1434 b- defN 24-May-15 04:52 almgroad-0.0.5.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 24-May-15 04:52 almgroad-0.0.5.dist-info/WHEEL
--rw-rw----  2.0 unx        9 b- defN 24-May-15 04:52 almgroad-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      526 b- defN 24-May-15 04:52 almgroad-0.0.5.dist-info/RECORD
-7 files, 3315 bytes uncompressed, 1893 bytes compressed:  42.9%
+-rw-rw----  2.0 unx    84842 b- defN 24-May-15 08:45 almgroad/ktkt.py
+-rw-rw----  2.0 unx     1434 b- defN 24-May-15 08:46 almgroad-0.0.6.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 24-May-15 08:46 almgroad-0.0.6.dist-info/WHEEL
+-rw-rw----  2.0 unx        9 b- defN 24-May-15 08:46 almgroad-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      600 b- defN 24-May-15 08:46 almgroad-0.0.6.dist-info/RECORD
+8 files, 88252 bytes uncompressed, 21891 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -3,20 +3,23 @@
 
 Filename: almgroad/chat.py
 Comment: 
 
 Filename: almgroad/infoinsta.py
 Comment: 
 
-Filename: almgroad-0.0.5.dist-info/METADATA
+Filename: almgroad/ktkt.py
 Comment: 
 
-Filename: almgroad-0.0.5.dist-info/WHEEL
+Filename: almgroad-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: almgroad-0.0.5.dist-info/top_level.txt
+Filename: almgroad-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: almgroad-0.0.5.dist-info/RECORD
+Filename: almgroad-0.0.6.dist-info/top_level.txt
+Comment: 
+
+Filename: almgroad-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## almgroad/__init__.py

```diff
@@ -1,2 +1,3 @@
 from .infoinsta import Info_Insta
-from .chat import GPT
+from .chat import GPT
+from .ktkt import kt
```

## Comparing `almgroad-0.0.5.dist-info/METADATA` & `almgroad-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almgroad
-Version: 0.0.5
+Version: 0.0.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Ibrahim Mohammed
 Author-email: ibrahom0780@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `almgroad-0.0.5.dist-info/RECORD` & `almgroad-0.0.6.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
-almgroad/__init__.py,sha256=zoMF5LnI35a-tr86tp-UCgfcgFqVNHl_aXZB9Eh_UF8,55
+almgroad/__init__.py,sha256=om0PblUp2nD_rrZMxJoaoGqXS9urpx0Lj74WnSMq8KY,76
 almgroad/chat.py,sha256=hUyCJzd5TaS-x1Y92c9Q5hCFMVnpKKg-nSvysy_KN30,128
 almgroad/infoinsta.py,sha256=DzqhmwPWbeBrSXoSZp9DsZQiVC6Nlx8PnZn9wM8sNrM,1071
-almgroad-0.0.5.dist-info/METADATA,sha256=xABvYRO04uOUCOPw9vC5Q46WWDnnacpgNY0e4bB-C3E,1434
-almgroad-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-almgroad-0.0.5.dist-info/top_level.txt,sha256=Sp5hguX1HExRTUrSZFyTESQ8fyBMsW2XsjXu84UhJ-w,9
-almgroad-0.0.5.dist-info/RECORD,,
+almgroad/ktkt.py,sha256=I8OIFV7YRzewNBcxn-ap_32KEbe5oCuq_ghCRwdMLbM,84842
+almgroad-0.0.6.dist-info/METADATA,sha256=MshKH6UcQrgMwKf_RKSS8DJVHYguWCANHSQiGz6IZbY,1434
+almgroad-0.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+almgroad-0.0.6.dist-info/top_level.txt,sha256=Sp5hguX1HExRTUrSZFyTESQ8fyBMsW2XsjXu84UhJ-w,9
+almgroad-0.0.6.dist-info/RECORD,,
```

