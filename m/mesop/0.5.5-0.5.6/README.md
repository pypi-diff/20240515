# Comparing `tmp/mesop-0.5.5-py3-none-any.whl.zip` & `tmp/mesop-0.5.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 4866711 bytes, number of entries: 262
+Zip file size: 4866571 bytes, number of entries: 262
 -rw-r--r--  2.0 unx     5582 b- defN 20-Jan-01 00:00 mesop/__init__.py
 -rw-r--r--  2.0 unx     1506 b- defN 20-Jan-01 00:00 mesop/example_index.py
 -rw-r--r--  2.0 unx       99 b- defN 20-Jan-01 00:00 mesop/version.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Jan-01 00:00 mesop/bin/__init__.py
 -rw-r--r--  2.0 unx     7639 b- defN 20-Jan-01 00:00 mesop/bin/bin.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Jan-01 00:00 mesop/cli/__init__.py
 -rw-r--r--  2.0 unx     3100 b- defN 20-Jan-01 00:00 mesop/cli/execute_module.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Jan-01 00:00 mesop/colab/__init__.py
--rw-r--r--  2.0 unx     1814 b- defN 20-Jan-01 00:00 mesop/colab/colab_run.py
+-rw-r--r--  2.0 unx     1607 b- defN 20-Jan-01 00:00 mesop/colab/colab_run.py
 -rw-r--r--  2.0 unx      783 b- defN 20-Jan-01 00:00 mesop/colab/colab_run_test.py
 -rw-r--r--  2.0 unx      464 b- defN 20-Jan-01 00:00 mesop/colab/colab_show.py
 -rw-r--r--  2.0 unx      140 b- defN 20-Jan-01 00:00 mesop/colab/colab_utils.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Jan-01 00:00 mesop/commands/__init__.py
 -rw-r--r--  2.0 unx      104 b- defN 20-Jan-01 00:00 mesop/commands/navigate.py
 -rw-r--r--  2.0 unx      804 b- defN 20-Jan-01 00:00 mesop/component_helpers/__init__.py
 -rw-r--r--  2.0 unx    12992 b- defN 20-Jan-01 00:00 mesop/component_helpers/diff_component_test.py
@@ -251,14 +251,14 @@
 -rwxr-xr-x  2.0 unx   369019 b- defN 20-Jan-01 00:00 mesop/web/src/app/prod/web_package/moment/min/moment-with-locales.min.js
 -rwxr-xr-x  2.0 unx   127877 b- defN 20-Jan-01 00:00 mesop/web/src/app/prod/web_package/rxjs/bundles/rxjs.umd.min.js
 -rwxr-xr-x  2.0 unx   166253 b- defN 20-Jan-01 00:00 mesop/web/src/app/prod/web_package/zone.js/dist/zone.js
 -rw-r--r--  2.0 unx        0 b- defN 20-Jan-01 00:00 rules_python/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Jan-01 00:00 rules_python/python/__init__.py
 -rw-r--r--  2.0 unx      628 b- defN 20-Jan-01 00:00 rules_python/python/runfiles/__init__.py
 -rw-r--r--  2.0 unx    14668 b- defN 20-Jan-01 00:00 rules_python/python/runfiles/runfiles.py
--rw-r--r--  2.0 unx    11358 b- defN 20-Jan-01 00:00 mesop-0.5.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1064 b- defN 20-Jan-01 00:00 mesop-0.5.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-Jan-01 00:00 mesop-0.5.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 20-Jan-01 00:00 mesop-0.5.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 20-Jan-01 00:00 mesop-0.5.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    23904 b- defN 20-Jan-01 00:00 mesop-0.5.5.dist-info/RECORD
-262 files, 23975688 bytes uncompressed, 4828283 bytes compressed:  79.9%
+-rw-r--r--  2.0 unx    11358 b- defN 20-Jan-01 00:00 mesop-0.5.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1064 b- defN 20-Jan-01 00:00 mesop-0.5.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 20-Jan-01 00:00 mesop-0.5.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 20-Jan-01 00:00 mesop-0.5.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 20-Jan-01 00:00 mesop-0.5.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    23904 b- defN 20-Jan-01 00:00 mesop-0.5.6.dist-info/RECORD
+262 files, 23975481 bytes uncompressed, 4828143 bytes compressed:  79.9%
```

## zipnote {}

```diff
@@ -762,26 +762,26 @@
 
 Filename: rules_python/python/runfiles/__init__.py
 Comment: 
 
 Filename: rules_python/python/runfiles/runfiles.py
 Comment: 
 
-Filename: mesop-0.5.5.dist-info/LICENSE
+Filename: mesop-0.5.6.dist-info/LICENSE
 Comment: 
 
-Filename: mesop-0.5.5.dist-info/METADATA
+Filename: mesop-0.5.6.dist-info/METADATA
 Comment: 
 
-Filename: mesop-0.5.5.dist-info/WHEEL
+Filename: mesop-0.5.6.dist-info/WHEEL
 Comment: 
 
-Filename: mesop-0.5.5.dist-info/entry_points.txt
+Filename: mesop-0.5.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: mesop-0.5.5.dist-info/top_level.txt
+Filename: mesop-0.5.6.dist-info/top_level.txt
 Comment: 
 
-Filename: mesop-0.5.5.dist-info/RECORD
+Filename: mesop-0.5.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mesop/version.py

```diff
@@ -1,6 +1,6 @@
 """Contains the version string."""
 
-VERSION = "0.5.5"
+VERSION = "0.5.6"
 
 if __name__ == "__main__":
   print(VERSION)
```

## mesop/colab/colab_run.py

```diff
@@ -1,8 +1,7 @@
-import sys
 import threading
 
 from absl import flags
 
 from mesop.colab import colab_utils
 from mesop.runtime import enable_debug_mode
 from mesop.server.constants import EDITOR_PACKAGE_PATH, PROD_PACKAGE_PATH
@@ -16,31 +15,24 @@
   When running in Colab environment, this will launch the web server.
 
   Otherwise, this is a no-op.
   """
   if not colab_utils.is_running_in_colab():
     print("Not running Colab: `colab_run` is a no-op")
     return
-  # Parse the flags before creating the app otherwise you will
+  # Ensures the flags are marked as parsed before creating the app otherwise you will
   # get UnparsedFlagAccessError.
   #
-  # This currently parses a list without any flags because typically Mesop
-  # will be run with gunicorn as a WSGI app and there may be unexpected
-  # flags such as "--bind".
+  # Depending on the Colab environment, the flags may or may not be parsed.
   #
-  # Example:
-  # $ gunicorn --bind :8080 main:me
-  #
-  # We will ignore all CLI flags, but we could provide a way to override
+  # Note: this ignore all Mesop CLI flags, but we could provide a way to override
   # Mesop defined flags in the future (e.g. enable_component_tree_diffs)
   # if necessary.
-  #
-  # Note: absl-py requires the first arg (program name), and will raise an error
-  # if we pass an empty list.
-  flags.FLAGS(sys.argv[:1])
+  if not flags.FLAGS.is_parsed():
+    flags.FLAGS.mark_as_parsed()
   flask_app = configure_flask_app(prod_mode=prod_mode)
   if not prod_mode:
     enable_debug_mode()
 
   configure_static_file_serving(
     flask_app,
     static_file_runfiles_base=PROD_PACKAGE_PATH
```

## Comparing `mesop-0.5.5.dist-info/LICENSE` & `mesop-0.5.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mesop-0.5.5.dist-info/METADATA` & `mesop-0.5.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mesop
-Version: 0.5.5
+Version: 0.5.6
 Summary: Build UIs in Python
 Home-page: https://github.com/google/mesop
 Author: Google Inc.
 License: Apache 2.0
 Keywords: mesop
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `mesop-0.5.5.dist-info/RECORD` & `mesop-0.5.6.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 mesop/__init__.py,sha256=g0bMXnMqLWSeHq942mFNirAbG_iMdWAvIFy73jSWtLw,5582
 mesop/example_index.py,sha256=vmQPyMpI0o6Lx9f2cDDzgZYtN2H66DT3BdRXrgBxJOs,1506
-mesop/version.py,sha256=I1HwAajxdc50kmz-jM5ONqKyaQ9x0NWzrwiypfML5So,99
+mesop/version.py,sha256=nC2o7lCunyKch4o3uNQT5hg1JfW0JhgWH0mCNvA5o9g,99
 mesop/bin/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mesop/bin/bin.py,sha256=nBM_1hbC3KmLXOQXdy2bBRSpDsF7oh8_n1AIZ66XeuE,7639
 mesop/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mesop/cli/execute_module.py,sha256=Nv12fUPlz5fD4pAc25J9EcFByE-jIhwwZIS7CT40T_w,3100
 mesop/colab/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mesop/colab/colab_run.py,sha256=JM4NxCXWV0zjh1G2OpblB1v6n6ftepP10pKj1XEzgGg,1814
+mesop/colab/colab_run.py,sha256=0MOX2l-Z5Bq-HrNBAl6znOEpGPJrk8h5fM0JNCCv4aM,1607
 mesop/colab/colab_run_test.py,sha256=c0HlERooyJuPWzvhI_YchD7Wzs23J9I7y4A9uHmFHQI,783
 mesop/colab/colab_show.py,sha256=AOsaV30G8Fy_WMkaTWr6GLDjefCvJHVZSdX7PLBP8B0,464
 mesop/colab/colab_utils.py,sha256=vWY3bJGVD5jr29YCH-sK5TxdNSQvHS5DxySiYqUOlO0,140
 mesop/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mesop/commands/navigate.py,sha256=J4QypIWe-CgmrsPuGx36B8_VzLV5__PUuqSkD25RcWo,104
 mesop/component_helpers/__init__.py,sha256=JYdSjQWL3z1TxTX7HKA6P9UPSMsLwcQXAQqDNJj2O24,804
 mesop/component_helpers/diff_component_test.py,sha256=R4n2ogt6dchC1K6z08BD5DbDvKBVivWvITQXTbuSh7U,12992
@@ -250,13 +250,13 @@
 mesop/web/src/app/prod/web_package/moment/min/moment-with-locales.min.js,sha256=QwcluVRoJ33LzMJ-COPYcydsAIJzcxCwsa0zA5JRGEc,369019
 mesop/web/src/app/prod/web_package/rxjs/bundles/rxjs.umd.min.js,sha256=mbzINdjdIRwkAi7royyVyxUPILvHbZ3_ae5pyxNAR8c,127877
 mesop/web/src/app/prod/web_package/zone.js/dist/zone.js,sha256=j9ym_cb4MrX6OfB-E53nmWo_-ZLy6pbFaoJu1QjwywI,166253
 rules_python/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rules_python/python/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rules_python/python/runfiles/__init__.py,sha256=LhomQ0Zu2cbUBSsQ_vJ3LXbeUUqYWIW4VfOSOv8e3nw,628
 rules_python/python/runfiles/runfiles.py,sha256=ykO_KMECFjRNhBSaRz4ldv4rmC7hPzz36wR8OTtGEwA,14668
-mesop-0.5.5.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-mesop-0.5.5.dist-info/METADATA,sha256=Gj7Uildtq0MLHb1ghdqnNVT-xml7T_mK6kobQ2vscQc,1064
-mesop-0.5.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-mesop-0.5.5.dist-info/entry_points.txt,sha256=b6e1SBw6Wc7IbwKAJc5Xr1-N1lNhNJwusoQ7ur-ZwoY,49
-mesop-0.5.5.dist-info/top_level.txt,sha256=Hq66Iuz4szLul1gShAeh8mDesAKjNxiG6Ge4mUom9Rw,19
-mesop-0.5.5.dist-info/RECORD,,
+mesop-0.5.6.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+mesop-0.5.6.dist-info/METADATA,sha256=v_RzDMfGm3DuR2GOufZV1nTZd3GKDEojxvvbI1q2q4s,1064
+mesop-0.5.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+mesop-0.5.6.dist-info/entry_points.txt,sha256=b6e1SBw6Wc7IbwKAJc5Xr1-N1lNhNJwusoQ7ur-ZwoY,49
+mesop-0.5.6.dist-info/top_level.txt,sha256=Hq66Iuz4szLul1gShAeh8mDesAKjNxiG6Ge4mUom9Rw,19
+mesop-0.5.6.dist-info/RECORD,,
```

