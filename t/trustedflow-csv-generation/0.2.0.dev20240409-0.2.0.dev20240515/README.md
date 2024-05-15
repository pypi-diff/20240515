# Comparing `tmp/trustedflow_csv_generation-0.2.0.dev20240409-cp310-cp310-manylinux2014_x86_64.whl.zip` & `tmp/trustedflow_csv_generation-0.2.0.dev20240515-cp310-cp310-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 3875568 bytes, number of entries: 9
--rw-r--r--  2.0 unx      581 b- defN 24-Apr-09 02:57 trustedflow/attestation/generation/__init__.py
--rwxr-xr-x  2.0 unx  6806536 b- defN 24-Apr-09 03:00 trustedflow/attestation/generation/generator.so
--rw-r--r--  2.0 unx      581 b- defN 24-Apr-09 02:57 trustedflow/attestation/verification/__init__.py
--rwxr-xr-x  2.0 unx  5934176 b- defN 24-Apr-09 02:59 trustedflow/attestation/verification/verifier.so
--rw-r--r--  2.0 unx    11356 b- defN 24-Apr-09 03:00 trustedflow_csv_generation-0.2.0.dev20240409.dist-info/LICENSE
--rw-r--r--  2.0 unx      639 b- defN 24-Apr-09 03:00 trustedflow_csv_generation-0.2.0.dev20240409.dist-info/METADATA
--rw-r--r--  2.0 unx      113 b- defN 24-Apr-09 03:00 trustedflow_csv_generation-0.2.0.dev20240409.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 24-Apr-09 03:00 trustedflow_csv_generation-0.2.0.dev20240409.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      963 b- defN 24-Apr-09 03:00 trustedflow_csv_generation-0.2.0.dev20240409.dist-info/RECORD
-9 files, 12754990 bytes uncompressed, 3873856 bytes compressed:  69.6%
+Zip file size: 7438610 bytes, number of entries: 10
+-rwxr-xr-x  2.0 unx  6806536 b- defN 24-May-15 14:00 trustedflow/attestation/generation/csv/generator.so
+-rwxr-xr-x  2.0 unx  5904320 b- defN 24-May-15 14:00 trustedflow/attestation/generation/sgx2/generator.so
+-rwxr-xr-x  2.0 unx  5913952 b- defN 24-May-15 14:00 trustedflow/attestation/generation/tdx/generator.so
+-rw-r--r--  2.0 unx      581 b- defN 24-May-15 13:57 trustedflow/attestation/verification/__init__.py
+-rwxr-xr-x  2.0 unx  5934176 b- defN 24-May-15 13:59 trustedflow/attestation/verification/verifier.so
+-rw-r--r--  2.0 unx    11356 b- defN 24-May-15 14:00 trustedflow_csv_generation-0.2.0.dev20240515.dist-info/LICENSE
+-rw-r--r--  2.0 unx      639 b- defN 24-May-15 14:00 trustedflow_csv_generation-0.2.0.dev20240515.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 24-May-15 14:00 trustedflow_csv_generation-0.2.0.dev20240515.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-15 14:00 trustedflow_csv_generation-0.2.0.dev20240515.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1088 b- defN 24-May-15 14:00 trustedflow_csv_generation-0.2.0.dev20240515.dist-info/RECORD
+10 files, 24572810 bytes uncompressed, 7436700 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
-Filename: trustedflow/attestation/generation/__init__.py
+Filename: trustedflow/attestation/generation/csv/generator.so
 Comment: 
 
-Filename: trustedflow/attestation/generation/generator.so
+Filename: trustedflow/attestation/generation/sgx2/generator.so
+Comment: 
+
+Filename: trustedflow/attestation/generation/tdx/generator.so
 Comment: 
 
 Filename: trustedflow/attestation/verification/__init__.py
 Comment: 
 
 Filename: trustedflow/attestation/verification/verifier.so
 Comment: 
 
-Filename: trustedflow_csv_generation-0.2.0.dev20240409.dist-info/LICENSE
+Filename: trustedflow_csv_generation-0.2.0.dev20240515.dist-info/LICENSE
 Comment: 
 
-Filename: trustedflow_csv_generation-0.2.0.dev20240409.dist-info/METADATA
+Filename: trustedflow_csv_generation-0.2.0.dev20240515.dist-info/METADATA
 Comment: 
 
-Filename: trustedflow_csv_generation-0.2.0.dev20240409.dist-info/WHEEL
+Filename: trustedflow_csv_generation-0.2.0.dev20240515.dist-info/WHEEL
 Comment: 
 
-Filename: trustedflow_csv_generation-0.2.0.dev20240409.dist-info/top_level.txt
+Filename: trustedflow_csv_generation-0.2.0.dev20240515.dist-info/top_level.txt
 Comment: 
 
-Filename: trustedflow_csv_generation-0.2.0.dev20240409.dist-info/RECORD
+Filename: trustedflow_csv_generation-0.2.0.dev20240515.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `trustedflow/attestation/generation/generator.so` & `trustedflow/attestation/generation/csv/generator.so`

 * *Files identical despite different names*

## Comparing `trustedflow_csv_generation-0.2.0.dev20240409.dist-info/LICENSE` & `trustedflow_csv_generation-0.2.0.dev20240515.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `trustedflow_csv_generation-0.2.0.dev20240409.dist-info/METADATA` & `trustedflow_csv_generation-0.2.0.dev20240515.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustedflow-csv-generation
-Version: 0.2.0.dev20240409
+Version: 0.2.0.dev20240515
 Summary: An attestation report generation library for csv
 Home-page: https://github.com/secretflow/trustedflow
 Author: secretflow
 Author-email: secretflow-contact@service.alipay.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `trustedflow_csv_generation-0.2.0.dev20240409.dist-info/RECORD` & `trustedflow_csv_generation-0.2.0.dev20240515.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-trustedflow/attestation/generation/__init__.py,sha256=olnX_kXTVg1I_hqG5gqS21-jAh4LE4JomsyQTtvBnCU,581
-trustedflow/attestation/generation/generator.so,sha256=MEPP_nfoEYg8vsxn8gC5iEkCY1j90sy7699j-8nsPK4,6806536
+trustedflow/attestation/generation/csv/generator.so,sha256=MEPP_nfoEYg8vsxn8gC5iEkCY1j90sy7699j-8nsPK4,6806536
+trustedflow/attestation/generation/sgx2/generator.so,sha256=b5wFjI8s0Qfp9aynuOav6esGaGA-vYzfIHrJQS_yruo,5904320
+trustedflow/attestation/generation/tdx/generator.so,sha256=15WlMPpJF91vh9GSxFibnxjDlGvsx7b15GmEWSeejUc,5913952
 trustedflow/attestation/verification/__init__.py,sha256=olnX_kXTVg1I_hqG5gqS21-jAh4LE4JomsyQTtvBnCU,581
 trustedflow/attestation/verification/verifier.so,sha256=FULocYDItBC-5eoQdzlvwnLyM_pDFoR0GPr3PZ8HasY,5934176
-trustedflow_csv_generation-0.2.0.dev20240409.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
-trustedflow_csv_generation-0.2.0.dev20240409.dist-info/METADATA,sha256=YfPUduFYPOcPmSR_h-Okj7dA8X5vhvLTwP7cKe-DnGc,639
-trustedflow_csv_generation-0.2.0.dev20240409.dist-info/WHEEL,sha256=3ji-nK5jramZCcxZ-bRSaxTH_DCMHUueruCckNMQuxg,113
-trustedflow_csv_generation-0.2.0.dev20240409.dist-info/top_level.txt,sha256=WrzyYsQZnTtydHYt7avRZW_3Btrw99LwyEYH3j6QrEk,45
-trustedflow_csv_generation-0.2.0.dev20240409.dist-info/RECORD,,
+trustedflow_csv_generation-0.2.0.dev20240515.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
+trustedflow_csv_generation-0.2.0.dev20240515.dist-info/METADATA,sha256=vC1M3Huhm_QCkfqj7ba8zz7El2vJ4Olu237WDwLazUs,639
+trustedflow_csv_generation-0.2.0.dev20240515.dist-info/WHEEL,sha256=XcXIRX2bPo-EGCFnthMC441x8LAB1n06gaqRMpx0fSU,113
+trustedflow_csv_generation-0.2.0.dev20240515.dist-info/top_level.txt,sha256=XRmHKla_R6TESrZldg1PGu6m8m3n11gwi8cp0DTQ_as,49
+trustedflow_csv_generation-0.2.0.dev20240515.dist-info/RECORD,,
```

