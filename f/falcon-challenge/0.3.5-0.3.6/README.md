# Comparing `tmp/falcon_challenge-0.3.5.tar.gz` & `tmp/falcon_challenge-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_challenge-0.3.5.tar", last modified: Sun May 12 15:59:09 2024, max compression
+gzip compressed data, was "falcon_challenge-0.3.6.tar", last modified: Wed May 15 19:06:22 2024, max compression
```

## Comparing `falcon_challenge-0.3.5.tar` & `falcon_challenge-0.3.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:09.299744 falcon_challenge-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-12 15:59:09.299744 falcon_challenge-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:09.295744 falcon_challenge-0.3.5/decoder_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/decoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/ndt2_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/random_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13812 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/sklearn_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:09.295744 falcon_challenge-0.3.5/falcon_challenge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/falcon_challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/falcon_challenge/challenge_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/falcon_challenge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/falcon_challenge/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    28393 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/falcon_challenge/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/falcon_challenge/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:09.299744 falcon_challenge-0.3.5/falcon_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-12 15:59:09.000000 falcon_challenge-0.3.5/falcon_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-12 15:59:09.000000 falcon_challenge-0.3.5/falcon_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 15:59:09.000000 falcon_challenge-0.3.5/falcon_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-12 15:59:09.000000 falcon_challenge-0.3.5/falcon_challenge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-12 15:59:09.000000 falcon_challenge-0.3.5/falcon_challenge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:09.299744 falcon_challenge-0.3.5/preproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/assemble_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/h2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/m1_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/m1_reachgrasp_preprocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/m2_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/m2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/merge_answers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/nwb_create_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/wrapper_convert_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/zip_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 15:59:09.299744 falcon_challenge-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:22.154477 falcon_challenge-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-15 19:06:22.154477 falcon_challenge-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:22.150477 falcon_challenge-0.3.6/decoder_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/decoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/ndt2_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/random_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13812 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/decoder_demos/sklearn_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:22.154477 falcon_challenge-0.3.6/falcon_challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/falcon_challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/falcon_challenge/challenge_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/falcon_challenge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/falcon_challenge/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28367 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/falcon_challenge/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/falcon_challenge/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:22.154477 falcon_challenge-0.3.6/falcon_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-15 19:06:22.000000 falcon_challenge-0.3.6/falcon_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-15 19:06:22.000000 falcon_challenge-0.3.6/falcon_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:06:22.000000 falcon_challenge-0.3.6/falcon_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 19:06:22.000000 falcon_challenge-0.3.6/falcon_challenge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 19:06:22.000000 falcon_challenge-0.3.6/falcon_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:22.154477 falcon_challenge-0.3.6/preproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/assemble_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/h2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/m1_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/m1_reachgrasp_preprocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/m2_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/m2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/merge_answers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/nwb_create_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/wrapper_convert_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/preproc/zip_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:06:22.154477 falcon_challenge-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-15 19:06:14.000000 falcon_challenge-0.3.6/setup.py
```

### Comparing `falcon_challenge-0.3.5/LICENSE` & `falcon_challenge-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/PKG-INFO` & `falcon_challenge-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.3.5
+Version: 0.3.6
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.3.5/README.md` & `falcon_challenge-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/decoder_demos/decoding_utils.py` & `falcon_challenge-0.3.6/decoder_demos/decoding_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/decoder_demos/filtering.py` & `falcon_challenge-0.3.6/decoder_demos/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/decoder_demos/ndt2_sample.py` & `falcon_challenge-0.3.6/decoder_demos/ndt2_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/decoder_demos/random_decoder.py` & `falcon_challenge-0.3.6/decoder_demos/random_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/decoder_demos/rnn_decoder.py` & `falcon_challenge-0.3.6/decoder_demos/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/decoder_demos/sklearn_decoder.py` & `falcon_challenge-0.3.6/decoder_demos/sklearn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/decoder_demos/sklearn_sample.py` & `falcon_challenge-0.3.6/decoder_demos/sklearn_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/falcon_challenge/config.py` & `falcon_challenge-0.3.6/falcon_challenge/config.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/falcon_challenge/dataloaders.py` & `falcon_challenge-0.3.6/falcon_challenge/dataloaders.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/falcon_challenge/evaluator.py` & `falcon_challenge-0.3.6/falcon_challenge/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             'S11_set_2', 
             'S12_set_1',
             'S12_set_2',
         ],
     },
     'm1': {
         'held_in': ['20120924', '20120926', '20120927', '20120928'],
-        'held_out': ['20121004', '20121017', '20121022', '20121024'],
+        'held_out': ['20121004', '20121017', '20121024'],
     },
     'h2': {
         'held_in': [
             '2022.05.18', 
             '2022.05.23', 
             '2022.05.25', 
             '2022.06.01', 
@@ -113,15 +113,15 @@
     FalconTask.m1: ['L_20120924', 'L_20120926', 'L_20120927', 'L_20120928'],
     FalconTask.m2: ['20201019', '20201020', '20201027', '20201028'],
     FalconTask.h2: DATASET_HELDINOUT_MAP['h2']['held_in'],
 }
 
 HELD_OUT_KEYS = {
     FalconTask.h1: ['S6_', 'S7_', 'S8_', 'S9_', 'S10_', 'S11_', 'S12_'],
-    FalconTask.m1: ['L_20121004', 'L_20121017', 'L_20121022', 'L_20121024'],
+    FalconTask.m1: ['L_20121004', 'L_20121017', 'L_20121024'],
     FalconTask.m2: ['20201030', '20201118', '20201119', '20201124'],
     FalconTask.h2: DATASET_HELDINOUT_MAP['h2']['held_out'],
 }
 
 RECOMMENDED_BATCH_SIZES = {
     FalconTask.h1: 8,
     FalconTask.m1: 4,
```

### Comparing `falcon_challenge-0.3.5/falcon_challenge/interface.py` & `falcon_challenge-0.3.6/falcon_challenge/interface.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/falcon_challenge.egg-info/PKG-INFO` & `falcon_challenge-0.3.6/falcon_challenge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.3.5
+Version: 0.3.6
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.3.5/falcon_challenge.egg-info/SOURCES.txt` & `falcon_challenge-0.3.6/falcon_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/preproc/assemble_data.py` & `falcon_challenge-0.3.6/preproc/assemble_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/preproc/filtering.py` & `falcon_challenge-0.3.6/preproc/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/preproc/h2_preproc.py` & `falcon_challenge-0.3.6/preproc/h2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/preproc/m1_fewshot_trial_counts.py` & `falcon_challenge-0.3.6/preproc/m1_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/preproc/m1_reachgrasp_preprocv2.py` & `falcon_challenge-0.3.6/preproc/m1_reachgrasp_preprocv2.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/preproc/m2_fewshot_trial_counts.py` & `falcon_challenge-0.3.6/preproc/m2_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/preproc/m2_preproc.py` & `falcon_challenge-0.3.6/preproc/m2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/preproc/merge_answers.py` & `falcon_challenge-0.3.6/preproc/merge_answers.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/preproc/nwb_create_utils.py` & `falcon_challenge-0.3.6/preproc/nwb_create_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/preproc/wrapper_convert_batch.py` & `falcon_challenge-0.3.6/preproc/wrapper_convert_batch.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/preproc/zip_data.py` & `falcon_challenge-0.3.6/preproc/zip_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.5/setup.py` & `falcon_challenge-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falcon_challenge',
-    version='0.3.5',
+    version='0.3.6',
 
     url='https://github.com/snel-repo/stability-benchmark',
     author='Joel Ye',
     author_email='joelye9@gmail.com',
 
     packages=find_packages(exclude=['data_demos', 'data']),
     install_requires=[
```

