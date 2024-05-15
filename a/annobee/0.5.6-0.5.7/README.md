# Comparing `tmp/annobee-0.5.6-py3-none-any.whl.zip` & `tmp/annobee-0.5.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12870 bytes, number of entries: 12
--rw-rw-r--  2.0 unx      229 b- defN 24-May-15 10:22 annobee/__init__.py
--rw-rw-r--  2.0 unx     5420 b- defN 24-May-15 11:01 annobee/cli.py
+Zip file size: 12876 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx       30 b- defN 24-May-15 11:15 annobee/__init__.py
+-rw-rw-r--  2.0 unx     6243 b- defN 24-May-15 11:16 annobee/cli.py
 -rw-rw-r--  2.0 unx      975 b- defN 24-May-14 15:26 annobee/config.py
 -rw-rw-r--  2.0 unx    29294 b- defN 24-May-14 16:06 annobee/criterias.py
 -rw-rw-r--  2.0 unx     8227 b- defN 24-May-14 16:07 annobee/utils.py
 -rw-rw-r--  2.0 unx     2033 b- defN 24-May-14 15:29 annobee/variant.py
--rw-rw-r--  2.0 unx     1074 b- defN 24-May-15 11:02 annobee-0.5.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx      642 b- defN 24-May-15 11:02 annobee-0.5.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-15 11:02 annobee-0.5.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       46 b- defN 24-May-15 11:02 annobee-0.5.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 24-May-15 11:02 annobee-0.5.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      924 b- defN 24-May-15 11:02 annobee-0.5.6.dist-info/RECORD
-12 files, 48964 bytes uncompressed, 11330 bytes compressed:  76.9%
+-rw-rw-r--  2.0 unx     1074 b- defN 24-May-15 11:17 annobee-0.5.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      642 b- defN 24-May-15 11:17 annobee-0.5.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-15 11:17 annobee-0.5.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       46 b- defN 24-May-15 11:17 annobee-0.5.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 24-May-15 11:17 annobee-0.5.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      923 b- defN 24-May-15 11:17 annobee-0.5.7.dist-info/RECORD
+12 files, 49587 bytes uncompressed, 11336 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: annobee/utils.py
 Comment: 
 
 Filename: annobee/variant.py
 Comment: 
 
-Filename: annobee-0.5.6.dist-info/LICENSE
+Filename: annobee-0.5.7.dist-info/LICENSE
 Comment: 
 
-Filename: annobee-0.5.6.dist-info/METADATA
+Filename: annobee-0.5.7.dist-info/METADATA
 Comment: 
 
-Filename: annobee-0.5.6.dist-info/WHEEL
+Filename: annobee-0.5.7.dist-info/WHEEL
 Comment: 
 
-Filename: annobee-0.5.6.dist-info/entry_points.txt
+Filename: annobee-0.5.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: annobee-0.5.6.dist-info/top_level.txt
+Filename: annobee-0.5.7.dist-info/top_level.txt
 Comment: 
 
-Filename: annobee-0.5.6.dist-info/RECORD
+Filename: annobee-0.5.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## annobee/__init__.py

```diff
@@ -1 +1 @@
-from .cli import get_ba1, get_bp3, get_bp4, get_bp6, get_bs1, get_bs2, get_pm1, get_pm2, get_pm4, get_pm5, get_pp2, get_pp3, get_pp5, get_ps1, get_ps4, get_pvs1, get_va_pathogenicity, get_criteria, main, get_bp7, get_bp1, get_all
+from .cli import Annobee, main
```

## annobee/cli.py

```diff
@@ -1,101 +1,106 @@
 import argparse
 import requests
 import json
 
-API_URL = 'http://localhost:5000/api/interpret'
-
-def get_criteria(endpoint, variant, genome_build='hg38'):
-    response = requests.post(endpoint, json={
-        'variant': variant,
-        'genome_build': genome_build,
-        'adjustments': {}
-    })
-    response_data = response.json()
-    return response_data.get('INFO', {})
-
-def get_ps1(info):
-    return info.get('PS')[0]
-
-def get_pm5(info):
-    return info.get('PM')[4]
-
-def get_bp7(info):
-    return info.get('BP')[6]
-
-def get_pvs1(info):
-    return info.get('PVS1')
-
-def get_bp1(info):
-    return info.get('BP')[0]
-
-def get_pp2(info):
-    return info.get('PP')[1]
-
-def get_ps4(info):
-    return info.get('PS')[3]
-
-def get_bs1(info):
-    return info.get('BS')[0]
-
-def get_bs2(info):
-    return info.get('BS')[1]
-
-def get_pm2(info):
-    return info.get('PM')[1]
-
-def get_pm1(info):
-    return info.get('PM')[0]
-
-def get_pp5(info):
-    return info.get('PP')[4]
-
-def get_bp6(info):
-    return info.get('BP')[5]
-
-def get_ba1(info):
-    return info.get('BA1')
-
-def get_pp3(info):
-    return info.get('PP')[2]
-
-def get_bp4(info):
-    return info.get('BP')[3]
-
-def get_pm4(info):
-    return info.get('PM')[3]
-
-def get_bp3(info):
-    return info.get('BP')[2]
-
-def get_va_pathogenicity(info):
-    return info.get('VA_PATHOGENICITY')
-
-def get_all(info):
-    return {
-        'PS1': get_ps1(info),
-        'PM5': get_pm5(info),
-        'BP7': get_bp7(info),
-        'PVS1': get_pvs1(info),
-        'BP1': get_bp1(info),
-        'PP2': get_pp2(info),
-        'PS4': get_ps4(info),
-        'BS1': get_bs1(info),
-        'BS2': get_bs2(info),
-        'PM2': get_pm2(info),
-        'PM1': get_pm1(info),
-        'PP5': get_pp5(info),
-        'BP6': get_bp6(info),
-        'BA1': get_ba1(info),
-        'PP3': get_pp3(info),
-        'BP4': get_bp4(info),
-        'PM4': get_pm4(info),
-        'BP3': get_bp3(info),
-        'VA_PATHOGENICITY': get_va_pathogenicity(info)
-    }
+class Annobee:
+    def __init__(self, endpoint='http://localhost:5000/api/interpret'):
+        self.endpoint = endpoint
+
+    def set_endpoint(self, endpoint):
+        self.endpoint = endpoint
+
+    def get_criteria(self, variant, genome_build='hg38'):
+        response = requests.post(self.endpoint, json={
+            'variant': variant,
+            'genome_build': genome_build,
+            'adjustments': {}
+        })
+        response_data = response.json()
+        return response_data.get('INFO', {})
+
+    def get_ps1(self, info):
+        return info.get('PS')[0]
+
+    def get_pm5(self, info):
+        return info.get('PM')[4]
+
+    def get_bp7(self, info):
+        return info.get('BP')[6]
+
+    def get_pvs1(self, info):
+        return info.get('PVS1')
+
+    def get_bp1(self, info):
+        return info.get('BP')[0]
+
+    def get_pp2(self, info):
+        return info.get('PP')[1]
+
+    def get_ps4(self, info):
+        return info.get('PS')[3]
+
+    def get_bs1(self, info):
+        return info.get('BS')[0]
+
+    def get_bs2(self, info):
+        return info.get('BS')[1]
+
+    def get_pm2(self, info):
+        return info.get('PM')[1]
+
+    def get_pm1(self, info):
+        return info.get('PM')[0]
+
+    def get_pp5(self, info):
+        return info.get('PP')[4]
+
+    def get_bp6(self, info):
+        return info.get('BP')[5]
+
+    def get_ba1(self, info):
+        return info.get('BA1')
+
+    def get_pp3(self, info):
+        return info.get('PP')[2]
+
+    def get_bp4(self, info):
+        return info.get('BP')[3]
+
+    def get_pm4(self, info):
+        return info.get('PM')[3]
+
+    def get_bp3(self, info):
+        return info.get('BP')[2]
+
+    def get_va_pathogenicity(self, info):
+        return info.get('VA_PATHOGENICITY')
+
+    def get_all(self, info):
+        return {
+            'PS1': self.get_ps1(info),
+            'PM5': self.get_pm5(info),
+            'BP7': self.get_bp7(info),
+            'PVS1': self.get_pvs1(info),
+            'BP1': self.get_bp1(info),
+            'PP2': self.get_pp2(info),
+            'PS4': self.get_ps4(info),
+            'BS1': self.get_bs1(info),
+            'BS2': self.get_bs2(info),
+            'PM2': self.get_pm2(info),
+            'PM1': self.get_pm1(info),
+            'PP5': self.get_pp5(info),
+            'BP6': self.get_bp6(info),
+            'BA1': self.get_ba1(info),
+            'PP3': self.get_pp3(info),
+            'BP4': self.get_bp4(info),
+            'PM4': self.get_pm4(info),
+            'BP3': self.get_bp3(info),
+            'VA_PATHOGENICITY': self.get_va_pathogenicity(info)
+        }
 
 def main():
     parser = argparse.ArgumentParser(description='Annovar SDK CLI')
     parser.add_argument('variant', type=str, help='Variant in the format chr-pos-ref-alt Example: 1-12345-A-G')
     parser.add_argument('-endpoint', type=str, default='http://localhost:5000/api/interpret', help='API endpoint to use')
     parser.add_argument('-ps1', action='store_true', help='Evaluate PS1 criteria')
     parser.add_argument('-pm5', action='store_true', help='Evaluate PM5 criteria')
@@ -115,54 +120,55 @@
     parser.add_argument('-bp4', action='store_true', help='Evaluate BP4 criteria')
     parser.add_argument('-pm4', action='store_true', help='Evaluate PM4 criteria')
     parser.add_argument('-bp3', action='store_true', help='Evaluate BP3 criteria')
     parser.add_argument('-all', action='store_true', help='Evaluate all criteria')
 
     args = parser.parse_args()
 
-    variant_info = get_criteria(args.endpoint, args.variant)
+    annobee = Annobee(endpoint=args.endpoint)
+    variant_info = annobee.get_criteria(args.variant)
 
     results = {}
     if args.all:
-        results = get_all(variant_info)
+        results = annobee.get_all(variant_info)
     else:
         if args.ps1:
-            results['PS1'] = get_ps1(variant_info)
+            results['PS1'] = annobee.get_ps1(variant_info)
         if args.pm5:
-            results['PM5'] = get_pm5(variant_info)
+            results['PM5'] = annobee.get_pm5(variant_info)
         if args.bp7:
-            results['BP7'] = get_bp7(variant_info)
+            results['BP7'] = annobee.get_bp7(variant_info)
         if args.pvs1:
-            results['PVS1'] = get_pvs1(variant_info)
+            results['PVS1'] = annobee.get_pvs1(variant_info)
         if args.bp1:
-            results['BP1'] = get_bp1(variant_info)
+            results['BP1'] = annobee.get_bp1(variant_info)
         if args.pp2:
-            results['PP2'] = get_pp2(variant_info)
+            results['PP2'] = annobee.get_pp2(variant_info)
         if args.ps4:
-            results['PS4'] = get_ps4(variant_info)
+            results['PS4'] = annobee.get_ps4(variant_info)
         if args.bs1:
-            results['BS1'] = get_bs1(variant_info)
+            results['BS1'] = annobee.get_bs1(variant_info)
         if args.bs2:
-            results['BS2'] = get_bs2(variant_info)
+            results['BS2'] = annobee.get_bs2(variant_info)
         if args.pm2:
-            results['PM2'] = get_pm2(variant_info)
+            results['PM2'] = annobee.get_pm2(variant_info)
         if args.pm1:
-            results['PM1'] = get_pm1(variant_info)
+            results['PM1'] = annobee.get_pm1(variant_info)
         if args.pp5:
-            results['PP5'] = get_pp5(variant_info)
+            results['PP5'] = annobee.get_pp5(variant_info)
         if args.bp6:
-            results['BP6'] = get_bp6(variant_info)
+            results['BP6'] = annobee.get_bp6(variant_info)
         if args.ba1:
-            results['BA1'] = get_ba1(variant_info)
+            results['BA1'] = annobee.get_ba1(variant_info)
         if args.pp3:
-            results['PP3'] = get_pp3(variant_info)
+            results['PP3'] = annobee.get_pp3(variant_info)
         if args.bp4:
-            results['BP4'] = get_bp4(variant_info)
+            results['BP4'] = annobee.get_bp4(variant_info)
         if args.pm4:
-            results['PM4'] = get_pm4(variant_info)
+            results['PM4'] = annobee.get_pm4(variant_info)
         if args.bp3:
-            results['BP3'] = get_bp3(variant_info)
+            results['BP3'] = annobee.get_bp3(variant_info)
     
     print(json.dumps(results, indent=4))
 
 if __name__ == '__main__':
     main()
```

## Comparing `annobee-0.5.6.dist-info/LICENSE` & `annobee-0.5.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `annobee-0.5.6.dist-info/METADATA` & `annobee-0.5.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annobee
-Version: 0.5.6
+Version: 0.5.7
 Summary: Annovar SDK for variant interpretation
 Home-page: https://github.com/variantAnnotation/annobee-sdk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `annobee-0.5.6.dist-info/RECORD` & `annobee-0.5.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-annobee/__init__.py,sha256=Dp0Z2T4rou1Fc9SIKcB1H036-Tz-_Em_MDYDz9NLqRU,229
-annobee/cli.py,sha256=sXMzV962t5ahj8EZnQuC9YLxtsbOh48jqcDVMowtNF4,5420
+annobee/__init__.py,sha256=WDJsRUTfio3pdrNusEOKK_j5EjaWOYtCLsLhipmNHK8,30
+annobee/cli.py,sha256=ZSR6mCfi4fS7nSQPsAhOPPc8AxQk1KLSiLy3jIGzTGE,6243
 annobee/config.py,sha256=ajneMjOXJ-hCmoFgrfRcGC2AwVjlzkxqpPDJVZDemjM,975
 annobee/criterias.py,sha256=mwcFzVwA0qqwKEpVZlOT20uuZJrGstE3umc4b3AUy7I,29294
 annobee/utils.py,sha256=zuVMCTy-u6A_ctUPwZpGnZLABAgSqA3A212LOj6rMQE,8227
 annobee/variant.py,sha256=iBtznyO8q4Jg_KT_GJCxNksKwcKiTx0KWbHBSe9zqc0,2033
-annobee-0.5.6.dist-info/LICENSE,sha256=sx_oGsaZeCcwck7YgyvgmMG8wqXPNPtqOOdzIwPg1Go,1074
-annobee-0.5.6.dist-info/METADATA,sha256=14O31NC5nnA5f2Kw15a38ibh04E8tciSZcsWfZEAljQ,642
-annobee-0.5.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-annobee-0.5.6.dist-info/entry_points.txt,sha256=YXR-e-gk3DdcMB1yPysdW7HwePCpE3q02I0vA1cPsgU,46
-annobee-0.5.6.dist-info/top_level.txt,sha256=T_SHMlCCeg7RpkVafZhLv3cj9ICW5cRnHFXhSQrcvgA,8
-annobee-0.5.6.dist-info/RECORD,,
+annobee-0.5.7.dist-info/LICENSE,sha256=sx_oGsaZeCcwck7YgyvgmMG8wqXPNPtqOOdzIwPg1Go,1074
+annobee-0.5.7.dist-info/METADATA,sha256=bI7UaLwId5-rtmNqMzwrhqajmIR40uwk5e57p-mGLTc,642
+annobee-0.5.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+annobee-0.5.7.dist-info/entry_points.txt,sha256=YXR-e-gk3DdcMB1yPysdW7HwePCpE3q02I0vA1cPsgU,46
+annobee-0.5.7.dist-info/top_level.txt,sha256=T_SHMlCCeg7RpkVafZhLv3cj9ICW5cRnHFXhSQrcvgA,8
+annobee-0.5.7.dist-info/RECORD,,
```

