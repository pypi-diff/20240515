# Comparing `tmp/trustedflow_tdx_generation-0.2.0.dev20240409-cp310-cp310-manylinux2014_x86_64.whl.zip` & `tmp/trustedflow_tdx_generation-0.2.0.dev20240515-cp310-cp310-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3585271 bytes, number of entries: 9
--rw-r--r--  2.0 unx      581 b- defN 24-Apr-09 02:57 trustedflow/attestation/generation/__init__.py
--rwxr-xr-x  2.0 unx  5913952 b- defN 24-Apr-09 02:59 trustedflow/attestation/generation/generator.so
--rw-r--r--  2.0 unx      581 b- defN 24-Apr-09 02:57 trustedflow/attestation/verification/__init__.py
--rwxr-xr-x  2.0 unx  5934176 b- defN 24-Apr-09 02:59 trustedflow/attestation/verification/verifier.so
--rw-r--r--  2.0 unx    11356 b- defN 24-Apr-09 02:59 trustedflow_tdx_generation-0.2.0.dev20240409.dist-info/LICENSE
--rw-r--r--  2.0 unx      639 b- defN 24-Apr-09 02:59 trustedflow_tdx_generation-0.2.0.dev20240409.dist-info/METADATA
--rw-r--r--  2.0 unx      113 b- defN 24-Apr-09 02:59 trustedflow_tdx_generation-0.2.0.dev20240409.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 24-Apr-09 02:59 trustedflow_tdx_generation-0.2.0.dev20240409.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      963 b- defN 24-Apr-09 02:59 trustedflow_tdx_generation-0.2.0.dev20240409.dist-info/RECORD
-9 files, 11862406 bytes uncompressed, 3583559 bytes compressed:  69.8%
+Zip file size: 5363188 bytes, number of entries: 9
+-rwxr-xr-x  2.0 unx  5904320 b- defN 24-May-15 14:00 trustedflow/attestation/generation/sgx2/generator.so
+-rwxr-xr-x  2.0 unx  5913952 b- defN 24-May-15 14:00 trustedflow/attestation/generation/tdx/generator.so
+-rw-r--r--  2.0 unx      581 b- defN 24-May-15 13:57 trustedflow/attestation/verification/__init__.py
+-rwxr-xr-x  2.0 unx  5934176 b- defN 24-May-15 13:59 trustedflow/attestation/verification/verifier.so
+-rw-r--r--  2.0 unx    11356 b- defN 24-May-15 14:00 trustedflow_tdx_generation-0.2.0.dev20240515.dist-info/LICENSE
+-rw-r--r--  2.0 unx      639 b- defN 24-May-15 14:00 trustedflow_tdx_generation-0.2.0.dev20240515.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 24-May-15 14:00 trustedflow_tdx_generation-0.2.0.dev20240515.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-15 14:00 trustedflow_tdx_generation-0.2.0.dev20240515.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      977 b- defN 24-May-15 14:00 trustedflow_tdx_generation-0.2.0.dev20240515.dist-info/RECORD
+9 files, 17766163 bytes uncompressed, 5361456 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: trustedflow/attestation/generation/__init__.py
+Filename: trustedflow/attestation/generation/sgx2/generator.so
 Comment: 
 
-Filename: trustedflow/attestation/generation/generator.so
+Filename: trustedflow/attestation/generation/tdx/generator.so
 Comment: 
 
 Filename: trustedflow/attestation/verification/__init__.py
 Comment: 
 
 Filename: trustedflow/attestation/verification/verifier.so
 Comment: 
 
-Filename: trustedflow_tdx_generation-0.2.0.dev20240409.dist-info/LICENSE
+Filename: trustedflow_tdx_generation-0.2.0.dev20240515.dist-info/LICENSE
 Comment: 
 
-Filename: trustedflow_tdx_generation-0.2.0.dev20240409.dist-info/METADATA
+Filename: trustedflow_tdx_generation-0.2.0.dev20240515.dist-info/METADATA
 Comment: 
 
-Filename: trustedflow_tdx_generation-0.2.0.dev20240409.dist-info/WHEEL
+Filename: trustedflow_tdx_generation-0.2.0.dev20240515.dist-info/WHEEL
 Comment: 
 
-Filename: trustedflow_tdx_generation-0.2.0.dev20240409.dist-info/top_level.txt
+Filename: trustedflow_tdx_generation-0.2.0.dev20240515.dist-info/top_level.txt
 Comment: 
 
-Filename: trustedflow_tdx_generation-0.2.0.dev20240409.dist-info/RECORD
+Filename: trustedflow_tdx_generation-0.2.0.dev20240515.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `trustedflow/attestation/generation/generator.so` & `trustedflow/attestation/generation/tdx/generator.so`

 * *Files identical despite different names*

## Comparing `trustedflow_tdx_generation-0.2.0.dev20240409.dist-info/LICENSE` & `trustedflow_tdx_generation-0.2.0.dev20240515.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `trustedflow_tdx_generation-0.2.0.dev20240409.dist-info/METADATA` & `trustedflow_tdx_generation-0.2.0.dev20240515.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustedflow-tdx-generation
-Version: 0.2.0.dev20240409
+Version: 0.2.0.dev20240515
 Summary: An attestation report generation library for tdx
 Home-page: https://github.com/secretflow/trustedflow
 Author: secretflow
 Author-email: secretflow-contact@service.alipay.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

