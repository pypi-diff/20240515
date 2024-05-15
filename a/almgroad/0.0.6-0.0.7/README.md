# Comparing `tmp/almgroad-0.0.6-py3-none-any.whl.zip` & `tmp/almgroad-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 22931 bytes, number of entries: 8
--rw-rw----  2.0 unx       76 b- defN 24-May-15 08:45 almgroad/__init__.py
+Zip file size: 23581 bytes, number of entries: 9
+-rw-rw----  2.0 unx      105 b- defN 24-May-15 17:41 almgroad/__init__.py
 -rw-rw----  2.0 unx      128 b- defN 24-May-15 03:17 almgroad/chat.py
 -rw-rw----  2.0 unx     1071 b- defN 24-May-15 04:51 almgroad/infoinsta.py
 -rw-rw----  2.0 unx    84842 b- defN 24-May-15 08:45 almgroad/ktkt.py
--rw-rw----  2.0 unx     1434 b- defN 24-May-15 08:46 almgroad-0.0.6.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 24-May-15 08:46 almgroad-0.0.6.dist-info/WHEEL
--rw-rw----  2.0 unx        9 b- defN 24-May-15 08:46 almgroad-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      600 b- defN 24-May-15 08:46 almgroad-0.0.6.dist-info/RECORD
-8 files, 88252 bytes uncompressed, 21891 bytes compressed:  75.2%
+-rw-rw----  2.0 unx      829 b- defN 24-May-15 17:40 almgroad/tik_tok.py
+-rw-rw----  2.0 unx     1434 b- defN 24-May-15 17:42 almgroad-0.0.7.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 24-May-15 17:42 almgroad-0.0.7.dist-info/WHEEL
+-rw-rw----  2.0 unx        9 b- defN 24-May-15 17:42 almgroad-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      676 b- defN 24-May-15 17:42 almgroad-0.0.7.dist-info/RECORD
+9 files, 89186 bytes uncompressed, 22427 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -6,20 +6,23 @@
 
 Filename: almgroad/infoinsta.py
 Comment: 
 
 Filename: almgroad/ktkt.py
 Comment: 
 
-Filename: almgroad-0.0.6.dist-info/METADATA
+Filename: almgroad/tik_tok.py
 Comment: 
 
-Filename: almgroad-0.0.6.dist-info/WHEEL
+Filename: almgroad-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: almgroad-0.0.6.dist-info/top_level.txt
+Filename: almgroad-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: almgroad-0.0.6.dist-info/RECORD
+Filename: almgroad-0.0.7.dist-info/top_level.txt
+Comment: 
+
+Filename: almgroad-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## almgroad/__init__.py

```diff
@@ -1,3 +1,4 @@
 from .infoinsta import Info_Insta
 from .chat import GPT
-from .ktkt import kt
+from .ktkt import kt
+from .tik_tok import Tik_Tok
```

## Comparing `almgroad-0.0.6.dist-info/METADATA` & `almgroad-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almgroad
-Version: 0.0.6
+Version: 0.0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Ibrahim Mohammed
 Author-email: ibrahom0780@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

