# Comparing `tmp/ASCA-1.2-py3-none-any.whl.zip` & `tmp/ASCA-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7590 bytes, number of entries: 7
+Zip file size: 7593 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat    15440 b- defN 24-May-15 16:31 ASCA/ASCA.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-15 15:49 ASCA/__init__.py
--rw-rw-rw-  2.0 fat     1326 b- defN 24-May-15 16:56 ASCA-1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4139 b- defN 24-May-15 16:56 ASCA-1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 16:56 ASCA-1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-May-15 16:56 ASCA-1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      500 b- defN 24-May-15 16:56 ASCA-1.2.dist-info/RECORD
-7 files, 21502 bytes uncompressed, 6712 bytes compressed:  68.8%
+-rw-rw-rw-  2.0 fat     1326 b- defN 24-May-15 16:59 ASCA-1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4144 b- defN 24-May-15 16:59 ASCA-1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-15 16:59 ASCA-1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-May-15 16:59 ASCA-1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      500 b- defN 24-May-15 16:59 ASCA-1.3.dist-info/RECORD
+7 files, 21507 bytes uncompressed, 6715 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: ASCA/ASCA.py
 Comment: 
 
 Filename: ASCA/__init__.py
 Comment: 
 
-Filename: ASCA-1.2.dist-info/LICENSE
+Filename: ASCA-1.3.dist-info/LICENSE
 Comment: 
 
-Filename: ASCA-1.2.dist-info/METADATA
+Filename: ASCA-1.3.dist-info/METADATA
 Comment: 
 
-Filename: ASCA-1.2.dist-info/WHEEL
+Filename: ASCA-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: ASCA-1.2.dist-info/top_level.txt
+Filename: ASCA-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ASCA-1.2.dist-info/RECORD
+Filename: ASCA-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ASCA-1.2.dist-info/LICENSE` & `ASCA-1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ASCA-1.2.dist-info/METADATA` & `ASCA-1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASCA
-Version: 1.2
+Version: 1.3
 Summary: ASCA: ANOVA-simultaneous component analysis
 Author: Sin Yong Teng
 Author-email: tsyet12@gmail.com
 License: BSD 2-Clause
 Keywords: Design of Experiments,Chemometrics,Artificial Intelligence
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: matplotlib
-Requires-Dist: sklearn
+Requires-Dist: scikit-learn
 Requires-Dist: numpy
 
 # ASCA: ANOVA-Simultaneous Component Analysis in Python
 
 
 <!-- TABLE OF CONTENTS -->
 ## Table of Contents
```

