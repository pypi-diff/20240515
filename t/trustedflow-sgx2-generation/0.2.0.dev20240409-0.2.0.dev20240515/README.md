# Comparing `tmp/trustedflow_sgx2_generation-0.2.0.dev20240409-cp310-cp310-manylinux2014_x86_64.whl.zip` & `tmp/trustedflow_sgx2_generation-0.2.0.dev20240515-cp310-cp310-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,10 @@
-Zip file size: 3578609 bytes, number of entries: 9
--rw-r--r--  2.0 unx      581 b- defN 24-Apr-09 02:57 trustedflow/attestation/generation/__init__.py
--rwxr-xr-x  2.0 unx  5904320 b- defN 24-Apr-09 02:59 trustedflow/attestation/generation/generator.so
--rw-r--r--  2.0 unx      581 b- defN 24-Apr-09 02:57 trustedflow/attestation/verification/__init__.py
--rwxr-xr-x  2.0 unx  5934176 b- defN 24-Apr-09 02:59 trustedflow/attestation/verification/verifier.so
--rw-r--r--  2.0 unx    11356 b- defN 24-Apr-09 02:59 trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/LICENSE
--rw-r--r--  2.0 unx      642 b- defN 24-Apr-09 02:59 trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/METADATA
--rw-r--r--  2.0 unx      113 b- defN 24-Apr-09 02:59 trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 24-Apr-09 02:59 trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      968 b- defN 24-Apr-09 02:59 trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/RECORD
-9 files, 11852782 bytes uncompressed, 3576887 bytes compressed:  69.8%
+Zip file size: 3578081 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx  5904320 b- defN 24-May-15 14:00 trustedflow/attestation/generation/sgx2/generator.so
+-rw-r--r--  2.0 unx      581 b- defN 24-May-15 13:57 trustedflow/attestation/verification/__init__.py
+-rwxr-xr-x  2.0 unx  5934176 b- defN 24-May-15 13:59 trustedflow/attestation/verification/verifier.so
+-rw-r--r--  2.0 unx    11356 b- defN 24-May-15 14:00 trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/LICENSE
+-rw-r--r--  2.0 unx      642 b- defN 24-May-15 14:00 trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 24-May-15 14:00 trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 24-May-15 14:00 trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      871 b- defN 24-May-15 14:00 trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/RECORD
+8 files, 11852109 bytes uncompressed, 3576517 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,28 +1,25 @@
-Filename: trustedflow/attestation/generation/__init__.py
-Comment: 
-
-Filename: trustedflow/attestation/generation/generator.so
+Filename: trustedflow/attestation/generation/sgx2/generator.so
 Comment: 
 
 Filename: trustedflow/attestation/verification/__init__.py
 Comment: 
 
 Filename: trustedflow/attestation/verification/verifier.so
 Comment: 
 
-Filename: trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/LICENSE
+Filename: trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/LICENSE
 Comment: 
 
-Filename: trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/METADATA
+Filename: trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/METADATA
 Comment: 
 
-Filename: trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/WHEEL
+Filename: trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/WHEEL
 Comment: 
 
-Filename: trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/top_level.txt
+Filename: trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/top_level.txt
 Comment: 
 
-Filename: trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/RECORD
+Filename: trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `trustedflow/attestation/generation/generator.so` & `trustedflow/attestation/generation/sgx2/generator.so`

 * *Files identical despite different names*

## Comparing `trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/LICENSE` & `trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/METADATA` & `trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustedflow-sgx2-generation
-Version: 0.2.0.dev20240409
+Version: 0.2.0.dev20240515
 Summary: An attestation report generation library for sgx2
 Home-page: https://github.com/secretflow/trustedflow
 Author: secretflow
 Author-email: secretflow-contact@service.alipay.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/RECORD` & `trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-trustedflow/attestation/generation/__init__.py,sha256=olnX_kXTVg1I_hqG5gqS21-jAh4LE4JomsyQTtvBnCU,581
-trustedflow/attestation/generation/generator.so,sha256=b5wFjI8s0Qfp9aynuOav6esGaGA-vYzfIHrJQS_yruo,5904320
+trustedflow/attestation/generation/sgx2/generator.so,sha256=b5wFjI8s0Qfp9aynuOav6esGaGA-vYzfIHrJQS_yruo,5904320
 trustedflow/attestation/verification/__init__.py,sha256=olnX_kXTVg1I_hqG5gqS21-jAh4LE4JomsyQTtvBnCU,581
 trustedflow/attestation/verification/verifier.so,sha256=FULocYDItBC-5eoQdzlvwnLyM_pDFoR0GPr3PZ8HasY,5934176
-trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
-trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/METADATA,sha256=81-pFa9kQsHaysvPGjQ-N0v-wQ6Wd2yJRimyrBdk4As,642
-trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/WHEEL,sha256=3ji-nK5jramZCcxZ-bRSaxTH_DCMHUueruCckNMQuxg,113
-trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/top_level.txt,sha256=WrzyYsQZnTtydHYt7avRZW_3Btrw99LwyEYH3j6QrEk,45
-trustedflow_sgx2_generation-0.2.0.dev20240409.dist-info/RECORD,,
+trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
+trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/METADATA,sha256=msv8Zzn0jZh_bYHdshZGAx4IzsxZubxpXC_-ygF3bKM,642
+trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/WHEEL,sha256=XcXIRX2bPo-EGCFnthMC441x8LAB1n06gaqRMpx0fSU,113
+trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/top_level.txt,sha256=LljZmJeXkWFUBBd8Z3Q8fijgDYXrKa7Bc_lRQ7_zUTs,50
+trustedflow_sgx2_generation-0.2.0.dev20240515.dist-info/RECORD,,
```

