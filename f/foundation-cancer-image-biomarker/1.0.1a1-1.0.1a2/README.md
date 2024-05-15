# Comparing `tmp/foundation_cancer_image_biomarker-1.0.1a1.tar.gz` & `tmp/foundation_cancer_image_biomarker-1.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation_cancer_image_biomarker-1.0.1a1.tar", max compression
+gzip compressed data, was "foundation_cancer_image_biomarker-1.0.1a2.tar", max compression
```

## Comparing `foundation_cancer_image_biomarker-1.0.1a1.tar` & `foundation_cancer_image_biomarker-1.0.1a2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1076 2024-05-04 05:11:49.211526 foundation_cancer_image_biomarker-1.0.1a1/LICENSE
--rw-r--r--   0        0        0     2340 2024-05-04 05:11:49.211526 foundation_cancer_image_biomarker-1.0.1a1/README.md
--rw-r--r--   0        0        0       24 2024-05-04 05:12:11.291516 foundation_cancer_image_biomarker-1.0.1a1/fmcib/__init__.py
--rw-r--r--   0        0        0       46 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/callbacks/__init__.py
--rw-r--r--   0        0        0     3355 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/callbacks/prediction_saver.py
--rw-r--r--   0        0        0     1069 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/callbacks/utils.py
--rw-r--r--   0        0        0     3193 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/datasets/__init__.py
--rw-r--r--   0        0        0     7460 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/datasets/ssl_radiomics_dataset.py
--rw-r--r--   0        0        0     2922 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/datasets/utils.py
--rw-r--r--   0        0        0     1221 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/__init__.py
--rw-r--r--   0        0        0     3912 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/autoencoder.py
--rw-r--r--   0        0        0     4881 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/load_model.py
--rw-r--r--   0        0        0    13087 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/models_genesis.py
--rw-r--r--   0        0        0       23 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/optimizers/__init__.py
--rw-r--r--   0        0        0     6826 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/optimizers/lars.py
--rw-r--r--   0        0        0     2532 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/preprocessing/__init__.py
--rw-r--r--   0        0        0     5641 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/preprocessing/seed_based_crop.py
--rw-r--r--   0        0        0     2308 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/run.py
--rw-r--r--   0        0        0        0 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/__init__.py
--rw-r--r--   0        0        0      226 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/__init__.py
--rw-r--r--   0        0        0     8551 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/neg_mining_info_nce_loss.py
--rw-r--r--   0        0        0     1110 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/nnclr_loss.py
--rw-r--r--   0        0        0      967 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/ntxent_loss.py
--rw-r--r--   0        0        0     4490 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/ntxent_mined_loss.py
--rw-r--r--   0        0        0     1872 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/swav_loss.py
--rw-r--r--   0        0        0      113 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/__init__.py
--rw-r--r--   0        0        0     1997 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/exneg_simclr.py
--rw-r--r--   0        0        0     2809 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/nnclr.py
--rw-r--r--   0        0        0     1922 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/simclr.py
--rw-r--r--   0        0        0     7822 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/swav.py
--rw-r--r--   0        0        0      166 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/__init__.py
--rw-r--r--   0        0        0     1373 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/duplicate.py
--rw-r--r--   0        0        0     1385 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/med3d.py
--rw-r--r--   0        0        0     1709 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/multicrop.py
--rw-r--r--   0        0        0     1532 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/random_resized_crop.py
--rw-r--r--   0        0        0       67 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/utils/__init__.py
--rw-r--r--   0        0        0      680 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/utils/download_utils.py
--rw-r--r--   0        0        0     9373 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/utils/idc_helper.py
--rw-r--r--   0        0        0       44 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/visualization/__init__.py
--rw-r--r--   0        0        0     3342 2024-05-04 05:11:49.991527 foundation_cancer_image_biomarker-1.0.1a1/fmcib/visualization/verify_io.py
--rw-r--r--   0        0        0     4570 2024-05-04 05:12:11.247516 foundation_cancer_image_biomarker-1.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     4244 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-1.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-14 16:58:06.391680 foundation_cancer_image_biomarker-1.0.1a2/LICENSE
+-rw-r--r--   0        0        0     2340 2024-05-14 16:58:06.391680 foundation_cancer_image_biomarker-1.0.1a2/README.md
+-rw-r--r--   0        0        0       24 2024-05-14 16:58:24.467692 foundation_cancer_image_biomarker-1.0.1a2/fmcib/__init__.py
+-rw-r--r--   0        0        0       46 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/callbacks/__init__.py
+-rw-r--r--   0        0        0     3355 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/callbacks/prediction_saver.py
+-rw-r--r--   0        0        0     1069 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/callbacks/utils.py
+-rw-r--r--   0        0        0     3193 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/datasets/__init__.py
+-rw-r--r--   0        0        0     7460 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/datasets/ssl_radiomics_dataset.py
+-rw-r--r--   0        0        0     2922 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/datasets/utils.py
+-rw-r--r--   0        0        0     1221 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/models/__init__.py
+-rw-r--r--   0        0        0     3912 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/models/autoencoder.py
+-rw-r--r--   0        0        0     4881 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/models/load_model.py
+-rw-r--r--   0        0        0    13087 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/models/models_genesis.py
+-rw-r--r--   0        0        0       23 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/optimizers/__init__.py
+-rw-r--r--   0        0        0     6826 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/optimizers/lars.py
+-rw-r--r--   0        0        0     2532 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/preprocessing/__init__.py
+-rw-r--r--   0        0        0     5641 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/preprocessing/seed_based_crop.py
+-rw-r--r--   0        0        0     2308 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/run.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/__init__.py
+-rw-r--r--   0        0        0      226 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/losses/__init__.py
+-rw-r--r--   0        0        0     8551 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/losses/neg_mining_info_nce_loss.py
+-rw-r--r--   0        0        0     1110 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/losses/nnclr_loss.py
+-rw-r--r--   0        0        0      967 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/losses/ntxent_loss.py
+-rw-r--r--   0        0        0     4490 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/losses/ntxent_mined_loss.py
+-rw-r--r--   0        0        0     1872 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/losses/swav_loss.py
+-rw-r--r--   0        0        0      113 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/modules/__init__.py
+-rw-r--r--   0        0        0     1997 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/modules/exneg_simclr.py
+-rw-r--r--   0        0        0     2809 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/modules/nnclr.py
+-rw-r--r--   0        0        0     1922 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/modules/simclr.py
+-rw-r--r--   0        0        0     7822 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/modules/swav.py
+-rw-r--r--   0        0        0      166 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/transforms/__init__.py
+-rw-r--r--   0        0        0     1373 2024-05-14 16:58:07.167687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/transforms/duplicate.py
+-rw-r--r--   0        0        0     1385 2024-05-14 16:58:07.171687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/transforms/med3d.py
+-rw-r--r--   0        0        0     1709 2024-05-14 16:58:07.171687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/transforms/multicrop.py
+-rw-r--r--   0        0        0     1532 2024-05-14 16:58:07.171687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/transforms/random_resized_crop.py
+-rw-r--r--   0        0        0       67 2024-05-14 16:58:07.171687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/utils/__init__.py
+-rw-r--r--   0        0        0      680 2024-05-14 16:58:07.171687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/utils/download_utils.py
+-rw-r--r--   0        0        0     9373 2024-05-14 16:58:07.171687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/utils/idc_helper.py
+-rw-r--r--   0        0        0       44 2024-05-14 16:58:07.171687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/visualization/__init__.py
+-rw-r--r--   0        0        0     3342 2024-05-14 16:58:07.171687 foundation_cancer_image_biomarker-1.0.1a2/fmcib/visualization/verify_io.py
+-rw-r--r--   0        0        0     4569 2024-05-14 16:58:24.423692 foundation_cancer_image_biomarker-1.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-1.0.1a2/PKG-INFO
```

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/LICENSE` & `foundation_cancer_image_biomarker-1.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/README.md` & `foundation_cancer_image_biomarker-1.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/callbacks/prediction_saver.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/callbacks/prediction_saver.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/callbacks/utils.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/datasets/__init__.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/datasets/ssl_radiomics_dataset.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/datasets/ssl_radiomics_dataset.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/datasets/utils.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/__init__.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/autoencoder.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/load_model.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/models/load_model.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/models/models_genesis.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/models/models_genesis.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/optimizers/lars.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/optimizers/lars.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/preprocessing/__init__.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/preprocessing/seed_based_crop.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/preprocessing/seed_based_crop.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/run.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/run.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/neg_mining_info_nce_loss.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/losses/neg_mining_info_nce_loss.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/nnclr_loss.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/losses/nnclr_loss.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/ntxent_loss.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/losses/ntxent_loss.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/ntxent_mined_loss.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/losses/ntxent_mined_loss.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/losses/swav_loss.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/losses/swav_loss.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/exneg_simclr.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/modules/exneg_simclr.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/nnclr.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/modules/nnclr.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/simclr.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/modules/simclr.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/ssl/modules/swav.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/ssl/modules/swav.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/duplicate.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/transforms/duplicate.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/med3d.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/transforms/med3d.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/multicrop.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/transforms/multicrop.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/transforms/random_resized_crop.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/transforms/random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/utils/download_utils.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/utils/idc_helper.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/utils/idc_helper.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/fmcib/visualization/verify_io.py` & `foundation_cancer_image_biomarker-1.0.1a2/fmcib/visualization/verify_io.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/pyproject.toml` & `foundation_cancer_image_biomarker-1.0.1a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "foundation-cancer-image-biomarker"
-version = "1.0.1a1"
+version = "1.0.1a2"
 description = "Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]"
 readme = "README.md"
 authors = ["Suraj Pai <bspai@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/AIM-Harvard/foundation-cancer-image-biomarker"
 homepage = "https://aim.hms.harvard.edu/foundation-cancer-image-biomarker"
 
@@ -23,20 +23,20 @@
 classifiers = [  #! Update me
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.12"
 project-lighter = {version = "0.0.2a19", allow-prereleases = true}
 wget = "^3.2"
 google-cloud-storage = "^2.9.0"
 thedicomsort = "^1.0.1"
 dcmrtstruct2nii = "^5"
 nibabel = "^5.1.0"
 matplotlib = "^3.7.1"
@@ -48,21 +48,21 @@
 scipy = "1.10.0"
 fonttools = "^4.44.0"
 pydantic = "1.10.13"
 lightly = "1.4.19"
 werkzeug = "^3.0.1"
 urllib3 = "^2.1.0"
 aiohttp = "^3.9.1"
-pip = "^23.3.2"
+pip = "^24.0"
 tornado = "^6.4"
 wandb = "^0.16.3"
 mpmath = "1.3.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.7.0"
+black = "^24.4.2"
 bandit = "^1.7.7"
 isort = {extras = ["colors"], version = "^5.10.1"}
 mypy = "^0.910"
 mypy-extensions = "^0.4.3"
 pre-commit = "^2.15.0"
 pydocstyle = "^6.1.1"
 pylint = "^2.11.1"
@@ -108,15 +108,15 @@
 profile = "black"
 multi_line_output = 3
 indent = 4
 color_output = true
 
 [tool.mypy]
 # https://mypy.readthedocs.io/en/latest/config_file.html#using-a-pyproject-toml-file
-python_version = 3.8
+python_version = 3.9
 pretty = true
 show_traceback = true
 color_output = true
 
 allow_redefinition = false
 check_untyped_defs = true
 disallow_any_generics = true
```

### Comparing `foundation_cancer_image_biomarker-1.0.1a1/PKG-INFO` & `foundation_cancer_image_biomarker-1.0.1a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: foundation-cancer-image-biomarker
-Version: 1.0.1a1
+Version: 1.0.1a2
 Summary: Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]
 Home-page: https://aim.hms.harvard.edu/foundation-cancer-image-biomarker
 License: MIT
 Author: Suraj Pai
 Author-email: bspai@bwh.harvard.edu
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
 Requires-Dist: dcmrtstruct2nii (>=5,<6)
 Requires-Dist: fonttools (>=4.44.0,<5.0.0)
 Requires-Dist: google-cloud-storage (>=2.9.0,<3.0.0)
 Requires-Dist: itk (>=5.3.0,<6.0.0)
 Requires-Dist: lightly (==1.4.19)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mpmath (==1.3.0)
 Requires-Dist: nibabel (>=5.1.0,<6.0.0)
-Requires-Dist: pip (>=23.3.2,<24.0.0)
+Requires-Dist: pip (>=24.0,<25.0)
 Requires-Dist: platipy (==0.4.1)
 Requires-Dist: project-lighter (==0.0.2a19)
 Requires-Dist: pydantic (==1.10.13)
 Requires-Dist: pydicom (>=2.4.0,<3.0.0)
 Requires-Dist: pydicom-seg (>=0.4.1,<0.5.0)
 Requires-Dist: pynrrd (>=1.0.0,<2.0.0)
 Requires-Dist: scipy (==1.10.0)
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1 Name: foundation-cancer-image-biomarker Version: 1.0.1a1
+Metadata-Version: 2.1 Name: foundation-cancer-image-biomarker Version: 1.0.1a2
 Summary: Official repo for Foundation Models for Quantitative Biomarker
 Discovery in Cancer Imaging [INSERT DOI] Home-page: https://
 aim.hms.harvard.edu/foundation-cancer-image-biomarker License: MIT Author:
-Suraj Pai Author-email: bspai@bwh.harvard.edu Requires-Python: >=3.8,<3.12
+Suraj Pai Author-email: bspai@bwh.harvard.edu Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Requires-Dist: aiohttp
-(>=3.9.1,<4.0.0) Requires-Dist: dcmrtstruct2nii (>=5,<6) Requires-Dist:
-fonttools (>=4.44.0,<5.0.0) Requires-Dist: google-cloud-storage
+:: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aiohttp (>=3.9.1,<4.0.0) Requires-Dist: dcmrtstruct2nii (>=5,<6)
+Requires-Dist: fonttools (>=4.44.0,<5.0.0) Requires-Dist: google-cloud-storage
 (>=2.9.0,<3.0.0) Requires-Dist: itk (>=5.3.0,<6.0.0) Requires-Dist: lightly
 (==1.4.19) Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist: mpmath
 (==1.3.0) Requires-Dist: nibabel (>=5.1.0,<6.0.0) Requires-Dist: pip
-(>=23.3.2,<24.0.0) Requires-Dist: platipy (==0.4.1) Requires-Dist: project-
-lighter (==0.0.2a19) Requires-Dist: pydantic (==1.10.13) Requires-Dist: pydicom
+(>=24.0,<25.0) Requires-Dist: platipy (==0.4.1) Requires-Dist: project-lighter
+(==0.0.2a19) Requires-Dist: pydantic (==1.10.13) Requires-Dist: pydicom
 (>=2.4.0,<3.0.0) Requires-Dist: pydicom-seg (>=0.4.1,<0.5.0) Requires-Dist:
 pynrrd (>=1.0.0,<2.0.0) Requires-Dist: scipy (==1.10.0) Requires-Dist:
 thedicomsort (>=1.0.1,<2.0.0) Requires-Dist: tornado (>=6.4,<7.0) Requires-
 Dist: urllib3 (>=2.1.0,<3.0.0) Requires-Dist: wandb (>=0.16.3,<0.17.0)
 Requires-Dist: werkzeug (>=3.0.1,<4.0.0) Requires-Dist: wget (>=3.2,<4.0)
 Project-URL: Repository, https://github.com/AIM-Harvard/foundation-cancer-
 image-biomarker Description-Content-Type: text/markdown
```

