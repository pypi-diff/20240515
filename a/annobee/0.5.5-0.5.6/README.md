# Comparing `tmp/annobee-0.5.5-py3-none-any.whl.zip` & `tmp/annobee-0.5.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12871 bytes, number of entries: 12
+Zip file size: 12870 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx      229 b- defN 24-May-15 10:22 annobee/__init__.py
--rw-rw-r--  2.0 unx     5420 b- defN 24-May-15 10:54 annobee/cli.py
+-rw-rw-r--  2.0 unx     5420 b- defN 24-May-15 11:01 annobee/cli.py
 -rw-rw-r--  2.0 unx      975 b- defN 24-May-14 15:26 annobee/config.py
 -rw-rw-r--  2.0 unx    29294 b- defN 24-May-14 16:06 annobee/criterias.py
 -rw-rw-r--  2.0 unx     8227 b- defN 24-May-14 16:07 annobee/utils.py
 -rw-rw-r--  2.0 unx     2033 b- defN 24-May-14 15:29 annobee/variant.py
--rw-rw-r--  2.0 unx     1074 b- defN 24-May-15 10:54 annobee-0.5.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx      642 b- defN 24-May-15 10:54 annobee-0.5.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-15 10:54 annobee-0.5.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       46 b- defN 24-May-15 10:54 annobee-0.5.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 24-May-15 10:54 annobee-0.5.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      924 b- defN 24-May-15 10:54 annobee-0.5.5.dist-info/RECORD
-12 files, 48964 bytes uncompressed, 11331 bytes compressed:  76.9%
+-rw-rw-r--  2.0 unx     1074 b- defN 24-May-15 11:02 annobee-0.5.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      642 b- defN 24-May-15 11:02 annobee-0.5.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-15 11:02 annobee-0.5.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       46 b- defN 24-May-15 11:02 annobee-0.5.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 24-May-15 11:02 annobee-0.5.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      924 b- defN 24-May-15 11:02 annobee-0.5.6.dist-info/RECORD
+12 files, 48964 bytes uncompressed, 11330 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: annobee/utils.py
 Comment: 
 
 Filename: annobee/variant.py
 Comment: 
 
-Filename: annobee-0.5.5.dist-info/LICENSE
+Filename: annobee-0.5.6.dist-info/LICENSE
 Comment: 
 
-Filename: annobee-0.5.5.dist-info/METADATA
+Filename: annobee-0.5.6.dist-info/METADATA
 Comment: 
 
-Filename: annobee-0.5.5.dist-info/WHEEL
+Filename: annobee-0.5.6.dist-info/WHEEL
 Comment: 
 
-Filename: annobee-0.5.5.dist-info/entry_points.txt
+Filename: annobee-0.5.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: annobee-0.5.5.dist-info/top_level.txt
+Filename: annobee-0.5.6.dist-info/top_level.txt
 Comment: 
 
-Filename: annobee-0.5.5.dist-info/RECORD
+Filename: annobee-0.5.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `annobee-0.5.5.dist-info/LICENSE` & `annobee-0.5.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `annobee-0.5.5.dist-info/METADATA` & `annobee-0.5.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annobee
-Version: 0.5.5
+Version: 0.5.6
 Summary: Annovar SDK for variant interpretation
 Home-page: https://github.com/variantAnnotation/annobee-sdk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `annobee-0.5.5.dist-info/RECORD` & `annobee-0.5.6.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 annobee/__init__.py,sha256=Dp0Z2T4rou1Fc9SIKcB1H036-Tz-_Em_MDYDz9NLqRU,229
 annobee/cli.py,sha256=sXMzV962t5ahj8EZnQuC9YLxtsbOh48jqcDVMowtNF4,5420
 annobee/config.py,sha256=ajneMjOXJ-hCmoFgrfRcGC2AwVjlzkxqpPDJVZDemjM,975
 annobee/criterias.py,sha256=mwcFzVwA0qqwKEpVZlOT20uuZJrGstE3umc4b3AUy7I,29294
 annobee/utils.py,sha256=zuVMCTy-u6A_ctUPwZpGnZLABAgSqA3A212LOj6rMQE,8227
 annobee/variant.py,sha256=iBtznyO8q4Jg_KT_GJCxNksKwcKiTx0KWbHBSe9zqc0,2033
-annobee-0.5.5.dist-info/LICENSE,sha256=sx_oGsaZeCcwck7YgyvgmMG8wqXPNPtqOOdzIwPg1Go,1074
-annobee-0.5.5.dist-info/METADATA,sha256=XHTeNxYhoSUZZcuf3A_-FPw9gIY-Ohlh2oUxs1rjueQ,642
-annobee-0.5.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-annobee-0.5.5.dist-info/entry_points.txt,sha256=YXR-e-gk3DdcMB1yPysdW7HwePCpE3q02I0vA1cPsgU,46
-annobee-0.5.5.dist-info/top_level.txt,sha256=T_SHMlCCeg7RpkVafZhLv3cj9ICW5cRnHFXhSQrcvgA,8
-annobee-0.5.5.dist-info/RECORD,,
+annobee-0.5.6.dist-info/LICENSE,sha256=sx_oGsaZeCcwck7YgyvgmMG8wqXPNPtqOOdzIwPg1Go,1074
+annobee-0.5.6.dist-info/METADATA,sha256=14O31NC5nnA5f2Kw15a38ibh04E8tciSZcsWfZEAljQ,642
+annobee-0.5.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+annobee-0.5.6.dist-info/entry_points.txt,sha256=YXR-e-gk3DdcMB1yPysdW7HwePCpE3q02I0vA1cPsgU,46
+annobee-0.5.6.dist-info/top_level.txt,sha256=T_SHMlCCeg7RpkVafZhLv3cj9ICW5cRnHFXhSQrcvgA,8
+annobee-0.5.6.dist-info/RECORD,,
```

