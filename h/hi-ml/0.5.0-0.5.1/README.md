# Comparing `tmp/hi-ml-0.5.0.tar.gz` & `tmp/hi-ml-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hi-ml-0.5.0.tar", last modified: Tue Mar 19 14:00:45 2024, max compression
+gzip compressed data, was "hi-ml-0.5.1.tar", last modified: Wed May 15 13:24:12 2024, max compression
```

## Comparing `hi-ml-0.5.0.tar` & `hi-ml-0.5.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:45.799172 hi-ml-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-19 14:00:28.000000 hi-ml-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 14:00:28.000000 hi-ml-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-19 14:00:45.799172 hi-ml-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-19 14:00:28.000000 hi-ml-0.5.0/package_description.md
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-19 14:00:28.000000 hi-ml-0.5.0/run_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 14:00:45.799172 hi-ml-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-03-19 14:00:28.000000 hi-ml-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:45.791172 hi-ml-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:45.791172 hi-ml-0.5.0/src/health_ml/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:45.795172 hi-ml-0.5.0/src/health_ml/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/configs/hello_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:45.795172 hi-ml-0.5.0/src/health_ml/data/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31962 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/deep_learning_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/eval_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15067 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/lightning_container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:45.795172 hi-ml-0.5.0/src/health_ml/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/model_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:45.795172 hi-ml-0.5.0/src/health_ml/networks/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:45.795172 hi-ml-0.5.0/src/health_ml/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/networks/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:45.795172 hi-ml-0.5.0/src/health_ml/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12693 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/networks/layers/attention_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:45.795172 hi-ml-0.5.0/src/health_ml/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/networks/nets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19548 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/runner_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/training_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:45.795172 hi-ml-0.5.0/src/health_ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/bag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/checkpoint_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    22287 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/checkpoint_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/data_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21038 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/fixed_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/lightning_loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21251 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/model_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/package_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    20982 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/regression_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26149 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/split_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-19 14:00:28.000000 hi-ml-0.5.0/src/health_ml/utils/type_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:00:45.799172 hi-ml-0.5.0/src/hi_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-19 14:00:45.000000 hi-ml-0.5.0/src/hi_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-19 14:00:45.000000 hi-ml-0.5.0/src/hi_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 14:00:45.000000 hi-ml-0.5.0/src/hi_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-19 14:00:45.000000 hi-ml-0.5.0/src/hi_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-19 14:00:45.000000 hi-ml-0.5.0/src/hi_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-19 14:00:45.000000 hi-ml-0.5.0/src/hi_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:12.631535 hi-ml-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-15 13:24:01.000000 hi-ml-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 13:24:01.000000 hi-ml-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-15 13:24:12.631535 hi-ml-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-15 13:24:01.000000 hi-ml-0.5.1/package_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 13:24:01.000000 hi-ml-0.5.1/run_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:24:12.631535 hi-ml-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-15 13:24:01.000000 hi-ml-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:12.623535 hi-ml-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:12.627535 hi-ml-0.5.1/src/health_ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:12.627535 hi-ml-0.5.1/src/health_ml/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/configs/hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:12.627535 hi-ml-0.5.1/src/health_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31962 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/deep_learning_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/eval_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15067 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/lightning_container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:12.627535 hi-ml-0.5.1/src/health_ml/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/model_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:12.627535 hi-ml-0.5.1/src/health_ml/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:12.627535 hi-ml-0.5.1/src/health_ml/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/networks/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:12.627535 hi-ml-0.5.1/src/health_ml/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12693 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/networks/layers/attention_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:12.627535 hi-ml-0.5.1/src/health_ml/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/networks/nets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19548 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/training_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:12.631535 hi-ml-0.5.1/src/health_ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/bag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/checkpoint_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22287 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/checkpoint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/data_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21038 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/fixed_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/lightning_loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21251 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/package_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20982 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/regression_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26149 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/split_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-15 13:24:01.000000 hi-ml-0.5.1/src/health_ml/utils/type_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:24:12.631535 hi-ml-0.5.1/src/hi_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-15 13:24:12.000000 hi-ml-0.5.1/src/hi_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-15 13:24:12.000000 hi-ml-0.5.1/src/hi_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:24:12.000000 hi-ml-0.5.1/src/hi_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 13:24:12.000000 hi-ml-0.5.1/src/hi_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-15 13:24:12.000000 hi-ml-0.5.1/src/hi_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 13:24:12.000000 hi-ml-0.5.1/src/hi_ml.egg-info/top_level.txt
```

### Comparing `hi-ml-0.5.0/LICENSE` & `hi-ml-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/PKG-INFO` & `hi-ml-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml
-Version: 0.5.0
+Version: 0.5.1
 Summary: Microsoft Health Futures package containing high level ML components
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Keywords: Health Futures,Health Intelligence,AzureML
 Platform: UNKNOWN
```

### Comparing `hi-ml-0.5.0/package_description.md` & `hi-ml-0.5.1/package_description.md`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/setup.py` & `hi-ml-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/configs/hello_world.py` & `hi-ml-0.5.1/src/health_ml/configs/hello_world.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/deep_learning_config.py` & `hi-ml-0.5.1/src/health_ml/deep_learning_config.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/eval_runner.py` & `hi-ml-0.5.1/src/health_ml/eval_runner.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/experiment_config.py` & `hi-ml-0.5.1/src/health_ml/experiment_config.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/lightning_container.py` & `hi-ml-0.5.1/src/health_ml/lightning_container.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/model_trainer.py` & `hi-ml-0.5.1/src/health_ml/model_trainer.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/networks/layers/attention_layers.py` & `hi-ml-0.5.1/src/health_ml/networks/layers/attention_layers.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/runner.py` & `hi-ml-0.5.1/src/health_ml/runner.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/runner_base.py` & `hi-ml-0.5.1/src/health_ml/runner_base.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/training_runner.py` & `hi-ml-0.5.1/src/health_ml/training_runner.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/__init__.py` & `hi-ml-0.5.1/src/health_ml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/bag_utils.py` & `hi-ml-0.5.1/src/health_ml/utils/bag_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/box_utils.py` & `hi-ml-0.5.1/src/health_ml/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/checkpoint_handler.py` & `hi-ml-0.5.1/src/health_ml/utils/checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/checkpoint_utils.py` & `hi-ml-0.5.1/src/health_ml/utils/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/common_utils.py` & `hi-ml-0.5.1/src/health_ml/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/config_loader.py` & `hi-ml-0.5.1/src/health_ml/utils/config_loader.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/data_augmentations.py` & `hi-ml-0.5.1/src/health_ml/utils/data_augmentations.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/diagnostics.py` & `hi-ml-0.5.1/src/health_ml/utils/diagnostics.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/fixed_paths.py` & `hi-ml-0.5.1/src/health_ml/utils/fixed_paths.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/lightning_loggers.py` & `hi-ml-0.5.1/src/health_ml/utils/lightning_loggers.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/logging.py` & `hi-ml-0.5.1/src/health_ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/lr_scheduler.py` & `hi-ml-0.5.1/src/health_ml/utils/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/model_util.py` & `hi-ml-0.5.1/src/health_ml/utils/model_util.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/package_setup.py` & `hi-ml-0.5.1/src/health_ml/utils/package_setup.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/regression_test_utils.py` & `hi-ml-0.5.1/src/health_ml/utils/regression_test_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/reports.py` & `hi-ml-0.5.1/src/health_ml/utils/reports.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/serialization.py` & `hi-ml-0.5.1/src/health_ml/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/split_dataset.py` & `hi-ml-0.5.1/src/health_ml/utils/split_dataset.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/health_ml/utils/type_annotations.py` & `hi-ml-0.5.1/src/health_ml/utils/type_annotations.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.5.0/src/hi_ml.egg-info/PKG-INFO` & `hi-ml-0.5.1/src/hi_ml.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml
-Version: 0.5.0
+Version: 0.5.1
 Summary: Microsoft Health Futures package containing high level ML components
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Keywords: Health Futures,Health Intelligence,AzureML
 Platform: UNKNOWN
```

### Comparing `hi-ml-0.5.0/src/hi_ml.egg-info/SOURCES.txt` & `hi-ml-0.5.1/src/hi_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

