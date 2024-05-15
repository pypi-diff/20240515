# Comparing `tmp/rubberduckie-2024.5.1-py3-none-any.whl.zip` & `tmp/rubberduckie-2024.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 8726 bytes, number of entries: 17
+Zip file size: 8725 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      415 b- defN 24-May-15 08:34 rubberduckie/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 09:48 rubberduckie/cdsw/__init__.py
--rw-r--r--  2.0 unx     6384 b- defN 24-May-15 07:46 rubberduckie/cdsw/hadoop.py
+-rw-r--r--  2.0 unx     6384 b- defN 24-May-15 12:49 rubberduckie/cdsw/hadoop.py
 -rw-r--r--  2.0 unx     3414 b- defN 24-May-15 08:33 rubberduckie/cdsw/import_fix.py
 -rw-r--r--  2.0 unx      745 b- defN 24-May-15 08:33 rubberduckie/cdsw/misc.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 05:14 rubberduckie/da/__init__.py
 -rw-r--r--  2.0 unx     2441 b- defN 24-May-15 07:47 rubberduckie/da/pilot.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 11:00 rubberduckie/dl/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 04:32 rubberduckie/ml/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 04:32 rubberduckie/plot/__init__.py
 -rw-r--r--  2.0 unx     1849 b- defN 24-May-15 07:46 rubberduckie/plot/evaluation.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 04:32 rubberduckie/xai/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-15 12:18 rubberduckie-2024.5.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      929 b- defN 24-May-15 12:18 rubberduckie-2024.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-15 12:18 rubberduckie-2024.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-May-15 12:18 rubberduckie-2024.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1419 b- defN 24-May-15 12:18 rubberduckie-2024.5.1.dist-info/RECORD
-17 files, 17701 bytes uncompressed, 6348 bytes compressed:  64.1%
+-rw-r--r--  2.0 unx        0 b- defN 24-May-15 12:50 rubberduckie-2024.5.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      929 b- defN 24-May-15 12:50 rubberduckie-2024.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-15 12:50 rubberduckie-2024.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-15 12:50 rubberduckie-2024.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1419 b- defN 24-May-15 12:50 rubberduckie-2024.5.2.dist-info/RECORD
+17 files, 17701 bytes uncompressed, 6347 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: rubberduckie/plot/evaluation.py
 Comment: 
 
 Filename: rubberduckie/xai/__init__.py
 Comment: 
 
-Filename: rubberduckie-2024.5.1.dist-info/LICENSE.txt
+Filename: rubberduckie-2024.5.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: rubberduckie-2024.5.1.dist-info/METADATA
+Filename: rubberduckie-2024.5.2.dist-info/METADATA
 Comment: 
 
-Filename: rubberduckie-2024.5.1.dist-info/WHEEL
+Filename: rubberduckie-2024.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: rubberduckie-2024.5.1.dist-info/top_level.txt
+Filename: rubberduckie-2024.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: rubberduckie-2024.5.1.dist-info/RECORD
+Filename: rubberduckie-2024.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rubberduckie-2024.5.1.dist-info/METADATA` & `rubberduckie-2024.5.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubberduckie
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: By Data Scientists and For Data Scientists
 Author-email: Colin & Team <colin.syd.au@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: scikit-learn
```

## Comparing `rubberduckie-2024.5.1.dist-info/RECORD` & `rubberduckie-2024.5.2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 rubberduckie/da/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rubberduckie/da/pilot.py,sha256=q7vnGn8kwY4hme0LPMMNdb62Eirb5AB-LdTeWrjzhIU,2441
 rubberduckie/dl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rubberduckie/ml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rubberduckie/plot/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rubberduckie/plot/evaluation.py,sha256=DrjoYTpfuKokaS6dRMHAxKMAZYuqDD0hACYk53Gwwuc,1849
 rubberduckie/xai/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rubberduckie-2024.5.1.dist-info/LICENSE.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rubberduckie-2024.5.1.dist-info/METADATA,sha256=xwUqSzlOc_qiPdd2J9G_dQ3LWjhyzYJQwJDLEjBs13s,929
-rubberduckie-2024.5.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-rubberduckie-2024.5.1.dist-info/top_level.txt,sha256=10EHDBDRla6FQ9v_RwhUA08sGKU1P499ZlDoj2XQXqc,13
-rubberduckie-2024.5.1.dist-info/RECORD,,
+rubberduckie-2024.5.2.dist-info/LICENSE.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+rubberduckie-2024.5.2.dist-info/METADATA,sha256=ECMYBpgW-iSGWotUcUbyPTowzrmoag5TvzX47BG8WJM,929
+rubberduckie-2024.5.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+rubberduckie-2024.5.2.dist-info/top_level.txt,sha256=10EHDBDRla6FQ9v_RwhUA08sGKU1P499ZlDoj2XQXqc,13
+rubberduckie-2024.5.2.dist-info/RECORD,,
```

