# Comparing `tmp/dcnum-0.17.2.tar.gz` & `tmp/dcnum-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.17.2.tar", last modified: Fri Mar 22 09:38:54 2024, max compression
+gzip compressed data, was "dcnum-0.18.0.tar", last modified: Wed May 15 14:44:20 2024, max compression
```

## Comparing `dcnum-0.17.2.tar` & `dcnum-0.18.0.tar`

### file list

```diff
@@ -1,118 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.526260 dcnum-0.17.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.510260 dcnum-0.17.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.510260 dcnum-0.17.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-22 09:38:49.000000 dcnum-0.17.2/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-22 09:38:49.000000 dcnum-0.17.2/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-03-22 09:38:49.000000 dcnum-0.17.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-22 09:38:49.000000 dcnum-0.17.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-03-22 09:38:49.000000 dcnum-0.17.2/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-22 09:38:49.000000 dcnum-0.17.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-22 09:38:54.526260 dcnum-0.17.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-22 09:38:49.000000 dcnum-0.17.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.510260 dcnum-0.17.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-03-22 09:38:49.000000 dcnum-0.17.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.510260 dcnum-0.17.2/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-22 09:38:49.000000 dcnum-0.17.2/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-22 09:38:49.000000 dcnum-0.17.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-22 09:38:49.000000 dcnum-0.17.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-22 09:38:49.000000 dcnum-0.17.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 09:38:54.526260 dcnum-0.17.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.510260 dcnum-0.17.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.514260 dcnum-0.17.2/src/dcnum/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-22 09:38:54.000000 dcnum-0.17.2/src/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.514260 dcnum-0.17.2/src/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.514260 dcnum-0.17.2/src/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_background/bg_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12834 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.514260 dcnum-0.17.2/src/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.514260 dcnum-0.17.2/src/dcnum/feat/feat_moments/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.514260 dcnum-0.17.2/src/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15005 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.518260 dcnum-0.17.2/src/dcnum/logic/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27022 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/logic/ctrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/logic/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/logic/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.518260 dcnum-0.17.2/src/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/meta/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.518260 dcnum-0.17.2/src/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    18202 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.518260 dcnum-0.17.2/src/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/segm/segmenter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.518260 dcnum-0.17.2/src/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    10535 2024-03-22 09:38:49.000000 dcnum-0.17.2/src/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.526260 dcnum-0.17.2/src/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-22 09:38:54.000000 dcnum-0.17.2/src/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-22 09:38:54.000000 dcnum-0.17.2/src/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 09:38:54.000000 dcnum-0.17.2/src/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-22 09:38:54.000000 dcnum-0.17.2/src/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-22 09:38:54.000000 dcnum-0.17.2/src/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.526260 dcnum-0.17.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:38:54.526260 dcnum-0.17.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
--rw-r--r--   0 runner    (1001) docker     (127)   650653 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/data/fmt-hdf5_shapein_empty.zip
--rw-r--r--   0 runner    (1001) docker     (127)   275920 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_feat_background_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_feat_background_bg_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_feat_background_bg_sparsemed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_feat_event_extractor_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_feat_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_feat_moments_based_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_logic_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_logic_join.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_logic_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    20851 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_logic_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_meta_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_meta_ppid_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_meta_ppid_bg.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_meta_ppid_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_meta_ppid_feat.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_meta_ppid_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_meta_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_read_basin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_segm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_write_queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-03-22 09:38:49.000000 dcnum-0.17.2/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.486162 dcnum-0.18.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.470162 dcnum-0.18.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.470162 dcnum-0.18.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-15 14:44:16.000000 dcnum-0.18.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-15 14:44:16.000000 dcnum-0.18.0/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-15 14:44:16.000000 dcnum-0.18.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 14:44:16.000000 dcnum-0.18.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-05-15 14:44:16.000000 dcnum-0.18.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-15 14:44:16.000000 dcnum-0.18.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-15 14:44:20.486162 dcnum-0.18.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-15 14:44:16.000000 dcnum-0.18.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.470162 dcnum-0.18.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-15 14:44:16.000000 dcnum-0.18.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-15 14:44:16.000000 dcnum-0.18.0/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-15 14:44:16.000000 dcnum-0.18.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 14:44:16.000000 dcnum-0.18.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-15 14:44:16.000000 dcnum-0.18.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:44:20.486162 dcnum-0.18.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.470162 dcnum-0.18.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/src/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-15 14:44:20.000000 dcnum-0.18.0/src/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/src/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/src/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_background/bg_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13064 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20705 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/src/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/src/dcnum/feat/feat_contour/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_contour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_contour/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_contour/moments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_contour/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/src/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.478162 dcnum-0.18.0/src/dcnum/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27998 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/logic/ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/logic/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/logic/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.478162 dcnum-0.18.0/src/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/meta/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.478162 dcnum-0.18.0/src/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/read/hdf5_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/read/mapped.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.478162 dcnum-0.18.0/src/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12220 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/segm/segmenter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.478162 dcnum-0.18.0/src/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.486162 dcnum-0.18.0/src/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-15 14:44:20.000000 dcnum-0.18.0/src/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-15 14:44:20.000000 dcnum-0.18.0/src/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:44:20.000000 dcnum-0.18.0/src/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 14:44:20.000000 dcnum-0.18.0/src/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 14:44:20.000000 dcnum-0.18.0/src/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.486162 dcnum-0.18.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.486162 dcnum-0.18.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   650653 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   284743 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/data/fmt-hdf5_shapein_empty.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   275920 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_background_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_background_bg_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_background_bg_sparsemed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_event_extractor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_moments_based_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_logic_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_logic_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_logic_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24892 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_logic_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_ppid_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_ppid_bg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_ppid_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_ppid_feat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_ppid_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_read_basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_read_hdf5_index_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_segm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_segm_no_mask_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_write_queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_write_writer.py
```

### Comparing `dcnum-0.17.2/.github/workflows/check.yml` & `dcnum-0.18.0/.github/workflows/check.yml`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     - name: Install dependencies
       run: |
         # prerequisites
         python -m pip install --upgrade pip wheel
         python -m pip install coverage flake8 pytest
     - name: Install dcnum
       run: |
+        # https://github.com/luispedro/mahotas/issues/144
+        pip install mahotas==1.4.13
         pip install -e .
     - name: List installed packages
       run: |
         pip freeze
     - name: Lint with flake8
       run: |
         flake8 --exclude _version.py .
```

### Comparing `dcnum-0.17.2/.github/workflows/deploy_pypi.yml` & `dcnum-0.18.0/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/.gitignore` & `dcnum-0.18.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/CHANGELOG` & `dcnum-0.18.0/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,50 @@
+0.18.0
+ - BREAKING CHANGE: mask postprocessing did a morphological opening instead
+   of a morphological closing, failing to remove spurious noise
+ - BREAKING CHANGE: perform first fill_holes and then closing_disk in mask
+   postprocessing
+ - feat: allow to specify ranges when creating an HDF5Data instance to
+   enable e.g. processing only a portion of an input file
+ - feat: volume computation via contour revolve algorithm
+ - feat: background offset (flickering) correction via the
+   "offset_correction" keyword for the "sparsemed" background computer
+   and "bg_off" everywhere else
+ - enh: allow creating HDF5Writer from h5py.File
+ - fix: mask postprocessing did a morphological opening instead
+   of a morphological closing, failing to remove spurious noise
+ - fix: remove mask ppid part for segmenters that do not use it
+ - fix: mask postprocessing with "fill_holes" using `cv2.floodFill`
+   sometimes segmented the entire frame if the upper left pixel was not
+   set to background
+ - enh: perform first fill_holes and then closing_disk in mask
+   postprocessing
+ - enh: pop read-cache items before adding a new one
+ - enh: allow to request the raw contour from `moments_based_features`
+ - ref: increment DCNUM_PPID_GENERATION to 8
+ - ref: added new super class `BaseImageChunkCache`
+ - ref: use HDF5Writer in Background class
+ - ref: minor cleanup
+ - ref: rename submodule `feat_moments` to `feat_contour`
+ - ref: remove unused `name` property from `Background` class
 0.17.2
  - fix: make sure unsupported features are not propagated in
    `concatenated_hdf5_data` (#27)
 0.17.1
  - ref: remove "bg_med" and "index_online" from protected scalar features,
    because "bg_med" may change due to a different background computation
    method and "index_online" enumerates events from online segmentation
 0.17.0
  - feat: allow to register topical search paths
  - ref: remove deprecated `get_ppid_from_kwargs` methods
  - ref: remove deprecated `preselect` and `ptp_median` keyword
    arguments from `QueueEventExtractor`
  - ref: remove deprecated "key" from `get_class_method_info` info dict
- - ref: issue UserWarning instead of DeprecationWarning when
+ - ref: issue UserWarning instead of DeprecationWarning when checking
+   segmenter keyword arguments
  - ref: remove pixel size check for HDF5 data
  - ref: remove unused `_get_model_file` from GPUSegmenter
 0.16.8
  - fix: correctly set number of workers for CPUSegmenter
  - enh: update list of environment variables that should be set to
    disable multithreading in subprocesses
 0.16.7
```

### Comparing `dcnum-0.17.2/LICENSE` & `dcnum-0.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/PKG-INFO` & `dcnum-0.18.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.17.2
+Version: 0.18.0
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Maximilian Schlögel, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.17.2/README.rst` & `dcnum-0.18.0/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/docs/conf.py` & `dcnum-0.18.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/docs/extensions/github_changelog.py` & `dcnum-0.18.0/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/pyproject.toml` & `dcnum-0.18.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/src/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.18.0/src/dcnum/feat/event_extractor_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/src/dcnum/feat/feat_background/base.py` & `dcnum-0.18.0/src/dcnum/feat/feat_background/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import abc
 import functools
 import inspect
 import multiprocessing as mp
 import pathlib
-import uuid
 
 import h5py
-import numpy as np
 
 from ...meta import ppid
 from ...read import HDF5Data
-from ...write import create_with_basins, set_default_filter_kwargs
+from ...write import HDF5Writer, create_with_basins, set_default_filter_kwargs
 
 
 # All subprocesses should use 'spawn' to avoid issues with threads
 # and 'fork' on POSIX systems.
 mp_spawn = mp.get_context('spawn')
 
 
@@ -89,49 +87,39 @@
             #       because HDF5Data properly resolves basins and the image
             #       feature might be in a basin.
             self.hdin = HDF5Data(self.h5in)
             self.input_data = self.hdin.image.h5ds
         else:
             self.input_data = input_data
 
-        #: unique identifier
-        self.name = str(uuid.uuid4())
         #: shape of event images
         self.image_shape = self.input_data[0].shape
         #: total number of events
         self.image_count = len(self.input_data)
 
         if self.h5out is None:
             if not output_path.exists():
                 # If the output path does not exist, then we create
                 # an output file with basins (for user convenience).
                 create_with_basins(path_out=output_path,
                                    basin_paths=self.paths_ref)
             # "a", because output file already exists
             self.h5out = h5py.File(output_path, "a", libver="latest")
 
-        # Initialize background data
-        ds_kwargs = set_default_filter_kwargs(compression=compress)
-        h5bg = self.h5out.require_dataset(
-            "events/image_bg",
-            shape=self.input_data.shape,
-            dtype=np.uint8,
-            chunks=(min(100, self.image_count),
-                    self.image_shape[0],
-                    self.image_shape[1]),
-            **ds_kwargs,
+        # Initialize writer
+        self.writer = HDF5Writer(
+            obj=self.h5out,
+            ds_kwds=set_default_filter_kwargs(compression=compress),
         )
-        h5bg.attrs.create('CLASS', np.string_('IMAGE'))
-        h5bg.attrs.create('IMAGE_VERSION', np.string_('1.2'))
-        h5bg.attrs.create('IMAGE_SUBCLASS', np.string_('IMAGE_GRAYSCALE'))
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, tb):
+        self.writer.close()
         # Close h5in and h5out
         if self.hdin is not None:  # we have an input file
             self.hdin.close()  # this closes self.h5in
         if self.h5in is not self.h5out and self.h5out is not None:
             self.h5out.close()
 
     @abc.abstractmethod
@@ -196,20 +184,28 @@
         """Return progress of background computation, float in [0,1]"""
         if self.image_count == 0:
             return 0.
         else:
             return self.image_proc.value / self.image_count
 
     def process(self):
+        # Delete any old background data
+        for key in ["image_bg", "bg_off"]:
+            if key in self.h5out["events"]:
+                del self.h5out["events"][key]
+        # Perform the actual background computation
         self.process_approach()
         bg_ppid = self.get_ppid()
-        # Store pipeline information in the image_bg feature
-        self.h5out["events/image_bg"].attrs["dcnum ppid background"] = bg_ppid
-        self.h5out["events/image_bg"].attrs["dcnum ppid generation"] = \
-            ppid.DCNUM_PPID_GENERATION
+        # Store pipeline information in the image_bg/bg_off feature
+        for key in ["image_bg", "bg_off"]:
+            if key in self.h5out["events"]:
+                self.h5out[f"events/{key}"].attrs["dcnum ppid background"] = \
+                    bg_ppid
+                self.h5out[F"events/{key}"].attrs["dcnum ppid generation"] = \
+                    ppid.DCNUM_PPID_GENERATION
 
     @abc.abstractmethod
     def process_approach(self):
         """The actual background computation approach"""
 
 
 @functools.cache
```

### Comparing `dcnum-0.17.2/src/dcnum/feat/feat_background/bg_copy.py` & `dcnum-0.18.0/src/dcnum/feat/feat_background/bg_copy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import h5py
 
 from .base import Background
 
 
 class BackgroundCopy(Background):
-
     @staticmethod
     def check_user_kwargs():
         pass
 
-    def process_approach(self):
+    def process(self):
         """Perform median computation on entire input data"""
         if self.h5in != self.h5out:
             hin = self.hdin.image_bg.h5ds
-            if "image_bg" in self.h5out["events"]:
-                del self.h5out["events/image_bg"]
             h5py.h5o.copy(src_loc=hin.parent.id,
                           src_name=b"image_bg",
                           dst_loc=self.h5out["events"].id,
                           dst_name=b"image_bg",
                           )
 
         # set progress to 100%
         self.image_proc.value = self.image_count
+
+    def process_approach(self):
+        # We do the copying in `process`, because we do not want to modify
+        # any metadata or delete datasets as is done in the base class.
+        # But we still have to implement this method, because it is an
+        # abstractmethod in the base class.
+        pass
```

### Comparing `dcnum-0.17.2/src/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.18.0/src/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,19 +168,26 @@
             ii += 1
 
     def process_approach(self):
         """Perform median computation on entire input data"""
         num_steps = int(np.ceil(self.image_count / self.batch_size))
         for ii in range(num_steps):
             self.process_next_batch()
-        # Set the remaining kernel_size median values to the last one
-        last_image = self.h5out["events/image_bg"][-self.kernel_size-1]
-        for ii in range(self.kernel_size):
-            self.h5out["events/image_bg"][self.image_count-ii-1] = last_image
-        self.image_proc.value = self.image_count
+
+        # Set the remaining median bg images to the last one.
+        num_remaining = (self.input_data.shape[0]
+                         - self.h5out["events/image_bg"].shape[0])
+        if num_remaining:
+            last_image = self.h5out["events/image_bg"][-1]
+            last_chunk = np.repeat(
+                last_image[np.newaxis],
+                num_remaining,
+                axis=0)
+            self.writer.store_feature_chunk("image_bg", last_chunk)
+            self.image_proc.value += num_remaining
 
     def process_next_batch(self):
         """Process one batch of input data"""
         cur_slice_in, cur_slice_out, output_size = \
             self.get_slices_for_batch(self.current_batch)
 
         if output_size:
@@ -204,17 +211,19 @@
                 if self.worker_counter.value == num_jobs:
                     break
 
             # Write output data to HDF5 file
             # TODO:
             #  Do this in a different thread so workers can keep going
             #  and use a lock somewhere in case the disk is too slow.
-            self.h5out["events/image_bg"][cur_slice_out] = \
+            self.writer.store_feature_chunk(
+                "image_bg",
                 self.shared_output[:output_size].reshape(output_size,
-                                                         *self.image_shape)
+                                                         *self.image_shape),
+            )
 
         self.current_batch += 1
         self.image_proc.value += self.batch_size
 
 
 class WorkerRollMed(mp_spawn.Process):
     def __init__(self, job_queue, counter, shared_input, shared_output,
```

### Comparing `dcnum-0.17.2/src/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.18.0/src/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class BackgroundSparseMed(Background):
     def __init__(self, input_data, output_path, kernel_size=200,
                  split_time=1., thresh_cleansing=0, frac_cleansing=.8,
+                 offset_correction=True,
                  compress=True, num_cpus=None):
         """Sparse median background correction with cleansing
 
         In contrast to the rolling median background correction,
         this algorithm only computes the background image every
         `split_time` seconds, but with a larger window (default kernel size is
         200 frames instead of 100 frames).
@@ -53,14 +54,29 @@
             operation when excluding background images from the series.
             Larger values mean more background images are excluded.
             Set to zero to enforce a fixed fraction via `frac_cleansing`.
         frac_cleansing: float
             Fraction between 0 and 1 indicating how many background images
             must still be present after cleansing (in case the cleansing
             factor is too large). Set to 1 to disable cleansing altogether.
+        offset_correction: bool
+            The sparse median background correction produces one median
+            image for multiple input frames (BTW this also leads to very
+            efficient data storage with HDF5 data compression filters). In
+            case the input frames are subject to frame-by-frame brightness
+            variations (e.g. flickering of the illumination source), it
+            is useful to have an offset value per frame that can then be
+            used in a later step to perform a more accurate background
+            correction. This offset is computed here by taking a 20px wide
+            slice from each frame (where the channel wall is located)
+            and computing the median therein relative to the computed
+            background image. The data are written to the "bg_off" feature
+            in the output file alongside "image_bg". To obtain the
+            corrected background image, add "image_bg" and "bg_off".
+            Set this to False if you don't need the "bg_off" feature.
         compress: bool
             Whether to compress background data. Set this to False
             for faster processing.
         num_cpus: int
             Number of CPUs to use for median computation. Defaults to
             `multiprocessing.cpu_count()`.
         """
@@ -68,15 +84,17 @@
             input_data=input_data,
             output_path=output_path,
             compress=compress,
             num_cpus=num_cpus,
             kernel_size=kernel_size,
             split_time=split_time,
             thresh_cleansing=thresh_cleansing,
-            frac_cleansing=frac_cleansing)
+            frac_cleansing=frac_cleansing,
+            offset_correction=offset_correction,
+        )
 
         if kernel_size > len(self.input_data):
             logger.warning(
                 f"The kernel size {kernel_size} is too large for input data"
                 f"size {len(self.input_data)}. Setting it to input data size!")
             kernel_size = len(self.input_data)
 
@@ -84,14 +102,16 @@
         self.kernel_size = kernel_size
         #: time between background images in the background series
         self.split_time = split_time
         #: cleansing threshold factor
         self.thresh_cleansing = thresh_cleansing
         #: keep at least this many background images from the series
         self.frac_cleansing = frac_cleansing
+        #: offset/flickering correction
+        self.offset_correction = offset_correction
 
         # time axis
         self.time = None
         if self.h5in is not None:
             hd = HDF5Data(self.h5in)
             if "time" in hd:
                 # use actual time from dataset
@@ -171,19 +191,21 @@
         super(BackgroundSparseMed, self).__exit__(type, value, tb)
 
     @staticmethod
     def check_user_kwargs(*,
                           kernel_size: int = 200,
                           split_time: float = 1.,
                           thresh_cleansing: float = 0,
-                          frac_cleansing: float = .8):
+                          frac_cleansing: float = .8,
+                          offset_correction: bool = True,
+                          ):
         """Initialize user-defined properties of this class
 
         This method primarily exists so that the CLI knows which
-        keyword arguements can be passed to this class.
+        keyword arguments can be passed to this class.
 
         Parameters
         ----------
         kernel_size: int
             Kernel size for median computation. This is the number of
             events that are used to compute the median for each pixel.
         split_time: float
@@ -193,14 +215,29 @@
             operation when excluding background images from the series.
             Larger values mean more background images are excluded.
             Set to 0 (default) to enforce a fixed fraction `frac_cleansing`.
         frac_cleansing: float
             Fraction between 0 and 1 indicating how many background images
             must still be present after cleansing (in case the cleansing
             factor is too large). Set to 1 to disable cleansing altogether.
+        offset_correction: bool
+            The sparse median background correction produces one median
+            image for multiple input frames (BTW this also leads to very
+            efficient data storage with HDF5 data compression filters). In
+            case the input frames are subject to frame-by-frame brightness
+            variations (e.g. flickering of the illumination source), it
+            is useful to have an offset value per frame that can then be
+            used in a later step to perform a more accurate background
+            correction. This offset is computed here by taking a 20px wide
+            slice from each frame (where the channel wall is located)
+            and computing the median therein relative to the computed
+            background image. The data are written to the "bg_off" feature
+            in the output file alongside "image_bg". To obtain the
+            corrected background image, add "image_bg" and "bg_off".
+            Set this to False if you don't need the "bg_off" feature.
         """
         assert kernel_size > 0
         assert split_time > 0
         assert thresh_cleansing >= 0, "Cleansing threshold must be >=0"
         assert frac_cleansing > 0, "Cleansing fraction must be >0"
         assert frac_cleansing <= 1, "Cleansing fraction must be <=1"
 
@@ -296,16 +333,27 @@
 
         # Write background data
         pos = 0
         step = 1000
         while pos < self.image_count:
             stop = min(pos + step, self.image_count)
             cur_slice = slice(pos, stop)
-            self.h5out["events/image_bg"][cur_slice] = \
-                bg_images[bg_idx[cur_slice]]
+            cur_bg_data = bg_images[bg_idx[cur_slice]]
+            self.writer.store_feature_chunk("image_bg", cur_bg_data)
+            if self.offset_correction:
+                # Record background offset correction "bg_off". We take a
+                # slice of 20px from the top of the image (there are normally
+                # no events here, only the channel walls are visible).
+                sh, sw = self.input_data.shape[1:]
+                roi_full = (slice(None), slice(0, 20), slice(0, sw))
+                roi_cur = (cur_slice, slice(0, 20), slice(0, sw))
+                val_bg = np.mean(cur_bg_data[roi_full], axis=(1, 2))
+                val_dat = np.mean(self.input_data[roi_cur], axis=(1, 2))
+                # background image = image_bg + bg_off
+                self.writer.store_feature_chunk("bg_off", val_dat - val_bg)
             pos += step
 
     def process_second(self,
                        ii: int,
                        second: float | int):
         idx_start = np.argmin(np.abs(second - self.time))
         idx_stop = idx_start + self.kernel_size
```

### Comparing `dcnum-0.17.2/src/dcnum/feat/feat_moments/mt_legacy.py` & `dcnum-0.18.0/src/dcnum/feat/feat_contour/moments.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 import cv2
 import numpy as np
 
 
-from .ct_opencv import contour_single_opencv
+from .contour import contour_single_opencv
 
 
-def moments_based_features(mask, pixel_size):
+def moments_based_features(
+        mask: np.ndarray,
+        pixel_size: float,
+        ret_contour: bool = False,
+        ):
+    """Compute moment-based features for a mask image
+
+    Parameters
+    ----------
+    mask: np.ndarray
+        3D stack of 2D boolean mask images to analyze
+    pixel_size: float
+        pixel size of the mask image in µm
+    ret_contour: bool
+        whether to also return the raw contour
+    """
     assert pixel_size is not None and pixel_size != 0
+    raw_contours = []
 
     size = mask.shape[0]
 
     empty = np.full(size, np.nan, dtype=np.float64)
 
     # features from raw contour
     feat_area_msd = np.copy(empty)
@@ -38,25 +54,30 @@
     # used to figure out which events need to be removed due
     # to invalid computed features, often due to invalid contours.
     valid = np.full(size, False)
 
     for ii in range(size):
         # raw contour
         cont_raw = contour_single_opencv(mask[ii])
-        if len(cont_raw.shape) < 2:
-            continue
-        if cv2.contourArea(cont_raw) == 0:
+        # only continue if the contour is valid
+        not_valid = len(cont_raw.shape) < 2 or cv2.contourArea(cont_raw) == 0
+
+        if ret_contour:
+            raw_contours.append(None if not_valid else cont_raw)
+
+        if not_valid:
             continue
 
         mu_raw = cv2.moments(cont_raw)
         arc_raw = np.float64(cv2.arcLength(cont_raw, True))
         area_raw = np.float64(mu_raw["m00"])
 
         # convex hull
         cont_cvx = np.squeeze(cv2.convexHull(cont_raw))
+
         mu_cvx = cv2.moments(cont_cvx)
         arc_cvx = np.float64(cv2.arcLength(cont_cvx, True))
 
         if mu_cvx["m00"] == 0 or mu_raw["m00"] == 0:
             # contour size too small
             continue
 
@@ -106,15 +127,15 @@
                 feat_inert_ratio_prnc[ii] = np.sqrt(i_ratio)
 
             feat_eccentr_prnc[ii] = np.sqrt((i_1 - i_2) / i_1)
 
         # specify validity
         valid[ii] = True
 
-    return {
+    data = {
         "area_msd": feat_area_msd,
         "area_ratio": feat_area_ratio,
         "area_um": feat_area_um,
         "area_um_raw": feat_area_um_raw,
         "aspect": feat_aspect,
         "deform": feat_deform,
         "deform_raw": feat_deform_raw,
@@ -127,7 +148,10 @@
         "pos_x": feat_pos_x,
         "pos_y": feat_pos_y,
         "size_x": feat_size_x,
         "size_y": feat_size_y,
         "tilt": feat_tilt,
         "valid": valid,
     }
+    if ret_contour:
+        data["contour"] = raw_contours
+    return data
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dcnum-0.17.2/src/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.18.0/src/dcnum/feat/feat_texture/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/src/dcnum/feat/gate.py` & `dcnum-0.18.0/src/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/src/dcnum/feat/queue_event_extractor.py` & `dcnum-0.18.0/src/dcnum/feat/queue_event_extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import numpy as np
 
 from ..meta.ppid import kwargs_to_ppid, ppid_to_kwargs
 from ..read import HDF5Data
 
 from .feat_brightness import brightness_features
-from .feat_moments import moments_based_features
+from .feat_contour import moments_based_features, volume_from_contours
 from .feat_texture import haralick_texture_features
 from .gate import Gate
 
 
 # All subprocesses should use 'spawn' to avoid issues with threads
 # and 'fork' on POSIX systems.
 mp_spawn = mp.get_context("spawn")
@@ -174,33 +174,54 @@
         args["worker_monitor"] = mp_spawn.RawArray("L", num_extractors)
         args["log_level"] = log_level
         return args
 
     def get_events_from_masks(self, masks, data_index, *,
                               brightness: bool = True,
                               haralick: bool = True,
+                              volume: bool = True,
                               ):
         """Get events dictionary, performing event-based gating"""
         events = {"mask": masks}
         image = self.data.image[data_index][np.newaxis]
         image_bg = self.data.image_bg[data_index][np.newaxis]
         image_corr = self.data.image_corr[data_index][np.newaxis]
+        if "bg_off" in self.data:
+            bg_off = self.data["bg_off"][data_index]
+        else:
+            bg_off = None
 
         events.update(
             moments_based_features(
                 masks,
-                pixel_size=self.data.pixel_size))
+                pixel_size=self.data.pixel_size,
+                ret_contour=volume,
+                ))
+
         if brightness:
             events.update(brightness_features(
-                mask=masks, image=image, image_bg=image_bg,
+                mask=masks,
+                image=image,
+                image_bg=image_bg,
+                bg_off=bg_off,
                 image_corr=image_corr
             ))
         if haralick:
             events.update(haralick_texture_features(
-                mask=masks, image=image, image_corr=image_corr
+                mask=masks,
+                image=image,
+                image_corr=image_corr,
+            ))
+
+        if volume:
+            events.update(volume_from_contours(
+                contour=events.pop("contour"),  # remove contour from events!
+                pos_x=events["pos_x"],
+                pos_y=events["pos_y"],
+                pixel_size=self.data.pixel_size,
             ))
 
         # gating on feature arrays
         if self.gate.box_gates:
             valid = self.gate.gate_events(events)
             gated_events = {}
             for key in events:
```

### Comparing `dcnum-0.17.2/src/dcnum/logic/ctrl.py` & `dcnum-0.18.0/src/dcnum/logic/ctrl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import collections
 import datetime
+import hashlib
 import json
 import logging
 from logging.handlers import QueueListener
 import multiprocessing as mp
+import numbers
 import os
 import pathlib
 import platform
 import socket
 import threading
 import time
 import traceback
 import uuid
 
 import h5py
+import numpy as np
 
 from ..feat.feat_background.base import get_available_background_methods
 from ..feat.queue_event_extractor import QueueEventExtractor
 from ..feat import gate
 from ..feat import EventExtractorManagerThread
 from ..segm import SegmenterManagerThread, get_available_segmenters
 from ..meta import ppid
@@ -378,14 +381,32 @@
             hw.h5.attrs["pipeline:dcnum data"] = self.ppdict["dat_id"]
             hw.h5.attrs["pipeline:dcnum background"] = self.ppdict["bg_id"]
             hw.h5.attrs["pipeline:dcnum segmenter"] = self.ppdict["seg_id"]
             hw.h5.attrs["pipeline:dcnum feature"] = self.ppdict["feat_id"]
             hw.h5.attrs["pipeline:dcnum gate"] = self.ppdict["gate_id"]
             hw.h5.attrs["pipeline:dcnum hash"] = self.pphash
             hw.h5.attrs["pipeline:dcnum yield"] = self.event_count
+            # index mapping information
+            im = self.job.kwargs["data_kwargs"].get("index_mapping", None)
+            if im is None:
+                dim = "0"
+            elif isinstance(im, numbers.Number):
+                dim = f"{im}"
+            elif isinstance(im, slice):
+                dim = (f"{im.start if im.start is not None else 'n'}"
+                       + f"-{im.stop if im.stop is not None else 'n'}"
+                       + f"-{im.step if im.step is not None else 'n'}"
+                       )
+            elif isinstance(im, (list, np.ndarray)):
+                idhash = hashlib.md5(
+                    np.array(im, dtype=np.uint32).tobytes()).hexdigest()
+                dim = f"h-{idhash[:8]}"
+            else:
+                dim = "unknown"
+            hw.h5.attrs["pipeline:dcnum mapping"] = dim
             # regular metadata
             hw.h5.attrs["experiment:event count"] = self.event_count
             hw.h5.attrs["imaging:pixel size"] = self.draw.pixel_size
             # Add job information to resulting .rtdc file
             hw.store_log(f"dcnum-job-{time_string}",
                          json.dumps({
                              "dcnum version": version_tuple,
@@ -499,15 +520,15 @@
 
         if self.job["debug"]:
             num_slots = 1
             num_extractors = 1
             num_segmenters = 1
         elif seg_cls.hardware_processor == "cpu":  # CPU segmenter
             # We could in principle set the number of slots to one and
-            # jave both number of extractors and number of segmenters set
+            # have both number of extractors and number of segmenters set
             # to the total number of CPUs. However, we would need more RAM
             # (for caching the image data) and we also have more overhead.
             # Having two slots shared between all workers is more efficient.
             num_slots = 2
             # Split segmentation and feature extraction workers evenly.
             num_extractors = self.job["num_procs"] // 2
             num_segmenters = self.job["num_procs"] - num_extractors
@@ -518,18 +539,19 @@
         num_extractors = max(1, num_extractors)
         num_segmenters = max(1, num_segmenters)
         self.job.kwargs["segmenter_kwargs"]["num_workers"] = num_segmenters
 
         slot_chunks = mp_spawn.Array("i", num_slots)
         slot_states = mp_spawn.Array("u", num_slots)
 
-        # Initialize thread
+        # Initialize segmenter manager thread
         thr_segm = SegmenterManagerThread(
             segmenter=seg_cls(**self.job["segmenter_kwargs"]),
             image_data=imdat,
+            bg_off=self.dtin["bg_off"] if "bg_off" in self.dtin else None,
             slot_states=slot_states,
             slot_chunks=slot_chunks,
             debug=self.job["debug"],
         )
         thr_segm.start()
 
         # Start feature extractor thread
```

### Comparing `dcnum-0.17.2/src/dcnum/logic/job.py` & `dcnum-0.18.0/src/dcnum/logic/job.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/src/dcnum/meta/paths.py` & `dcnum-0.18.0/src/dcnum/meta/paths.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/src/dcnum/meta/ppid.py` & `dcnum-0.18.0/src/dcnum/meta/ppid.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pathlib
 from typing import Dict, List, Protocol
 import warnings
 
 
 #: Increment this string if there are breaking changes that make
 #: previous pipelines unreproducible.
-DCNUM_PPID_GENERATION = "7"
+DCNUM_PPID_GENERATION = "8"
 
 
 class ClassWithPPIDCapabilities(Protocol):
     def get_ppid(self) -> str:
         """full pipeline identifier for the class (instance method)"""
         pass
```

### Comparing `dcnum-0.17.2/src/dcnum/read/cache.py` & `dcnum-0.18.0/src/dcnum/read/cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,154 +1,154 @@
+import abc
 import collections
 import functools
 import hashlib
 import pathlib
+from typing import Tuple
 import warnings
 
 import h5py
 import numpy as np
 
 
 class EmptyDatasetWarning(UserWarning):
     """Used for files that contain no actual data"""
     pass
 
 
-class HDF5ImageCache:
+class BaseImageChunkCache(abc.ABC):
     def __init__(self,
-                 h5ds: h5py.Dataset,
+                 shape: Tuple[int],
                  chunk_size: int = 1000,
                  cache_size: int = 2,
-                 boolean: bool = False):
-        """An HDF5 image cache
-
-        Deformability cytometry data files commonly contain image stacks
-        that are chunked in various ways. Loading just a single image
-        can be time-consuming, because an entire HDF5 chunk has to be
-        loaded, decompressed and from that one image extracted. The
-        `HDF5ImageCache` class caches the chunks from the HDF5 files
-        into memory, making single-image-access very fast.
-        """
-        self.shape = h5ds.shape
+                 ):
+        self.shape = shape
+        chunk_size = min(shape[0], chunk_size)
         self._len = self.shape[0]
-        if self._len == 0:
-            warnings.warn(f"Input image '{h5ds.name}' in "
-                          f"file {h5ds.file.filename} has zero length",
-                          EmptyDatasetWarning)
-        # TODO:
-        # - adjust chunking to multiples of the chunks in the dataset
-        #   (which might slightly speed up things)
-        chunk_size = min(h5ds.shape[0], chunk_size)
-        self.h5ds = h5ds
-        self.chunk_size = chunk_size
-        self.boolean = boolean
-        self.cache_size = cache_size
         #: This is a FILO cache for the chunks
         self.cache = collections.OrderedDict()
         self.image_shape = self.shape[1:]
         self.chunk_shape = (chunk_size,) + self.shape[1:]
+        self.chunk_size = chunk_size
+        self.cache_size = cache_size
         self.num_chunks = int(np.ceil(self._len / (self.chunk_size or 1)))
 
+    def __getitem__(self, index):
+        chunk_index, sub_index = self._get_chunk_index_for_index(index)
+        return self.get_chunk(chunk_index)[sub_index]
+
+    def __len__(self):
+        return self._len
+
+    @abc.abstractmethod
+    def _get_chunk_data(self, chunk_slice):
+        """Implemented in subclass to obtain actual data"""
+
     def _get_chunk_index_for_index(self, index):
         if index < 0:
             index = self._len + index
         elif index >= self._len:
             raise IndexError(
                 f"Index {index} out of bounds for HDF5ImageCache "
                 f"of size {self._len}")
         chunk_index = index // self.chunk_size
         sub_index = index % self.chunk_size
         return chunk_index, sub_index
 
-    def __getitem__(self, index):
-        chunk_index, sub_index = self._get_chunk_index_for_index(index)
-        return self.get_chunk(chunk_index)[sub_index]
-
-    def __len__(self):
-        return self._len
-
     def get_chunk(self, chunk_index):
         """Return one chunk of images"""
         if chunk_index not in self.cache:
-            fslice = slice(self.chunk_size * chunk_index,
-                           self.chunk_size * (chunk_index + 1)
-                           )
-            data = self.h5ds[fslice]
-            if self.boolean:
-                data = np.array(data, dtype=bool)
-            self.cache[chunk_index] = data
-            if len(self.cache) > self.cache_size:
+            if len(self.cache) >= self.cache_size:
                 # Remove the first item
                 self.cache.popitem(last=False)
+            data = self._get_chunk_data(self.get_chunk_slice(chunk_index))
+            self.cache[chunk_index] = data
         return self.cache[chunk_index]
 
     def get_chunk_size(self, chunk_index):
         """Return the number of images in this chunk"""
         if chunk_index < self.num_chunks - 1:
             return self.chunk_size
         else:
             chunk_size = self._len - chunk_index*self.chunk_size
             if chunk_size < 0:
                 raise IndexError(f"{self} only has {self.num_chunks} chunks!")
             return chunk_size
 
+    def get_chunk_slice(self, chunk_index):
+        """Return the slice corresponding to the chunk index"""
+        ch_slice = slice(self.chunk_size * chunk_index,
+                         self.chunk_size * (chunk_index + 1)
+                         )
+        return ch_slice
+
     def iter_chunks(self):
-        size = self.h5ds.shape[0]
         index = 0
         chunk = 0
         while True:
             yield chunk
             chunk += 1
             index += self.chunk_size
-            if index >= size:
+            if index >= self._len:
                 break
 
 
-class ImageCorrCache:
+class HDF5ImageCache(BaseImageChunkCache):
     def __init__(self,
-                 image: HDF5ImageCache,
-                 image_bg: HDF5ImageCache):
-        self.image = image
-        self.image_bg = image_bg
-        self.chunk_size = image.chunk_size
-        self.num_chunks = image.num_chunks
-        self.h5ds = image.h5ds
-        self.shape = image.shape
-        self.chunk_shape = image.chunk_shape
-        #: This is a FILO cache for the corrected image chunks
-        self.cache = collections.OrderedDict()
-        self.cache_size = image.cache_size
+                 h5ds: h5py.Dataset,
+                 chunk_size: int = 1000,
+                 cache_size: int = 2,
+                 boolean: bool = False):
+        """An HDF5 image cache
 
-    def _get_chunk_index_for_index(self, index):
-        if index < 0:
-            index = len(self.h5ds) + index
-        chunk_index = index // self.chunk_size
-        sub_index = index % self.chunk_size
-        return chunk_index, sub_index
+        Deformability cytometry data files commonly contain image stacks
+        that are chunked in various ways. Loading just a single image
+        can be time-consuming, because an entire HDF5 chunk has to be
+        loaded, decompressed and from that one image extracted. The
+        `HDF5ImageCache` class caches the chunks from the HDF5 files
+        into memory, making single-image-access very fast.
+        """
+        super(HDF5ImageCache, self).__init__(
+            shape=h5ds.shape,
+            chunk_size=chunk_size,
+            cache_size=cache_size)
+        # TODO:
+        # - adjust chunking to multiples of the chunks in the dataset
+        #   (which might slightly speed up things)
+        self.h5ds = h5ds
+        self.boolean = boolean
 
-    def __getitem__(self, index):
-        chunk_index, sub_index = self._get_chunk_index_for_index(index)
-        return self.get_chunk(chunk_index)[sub_index]
+        if self._len == 0:
+            warnings.warn(f"Input image '{h5ds.name}' in "
+                          f"file {h5ds.file.filename} has zero length",
+                          EmptyDatasetWarning)
 
-    def __len__(self):
-        return len(self.image)
+    def _get_chunk_data(self, chunk_slice):
+        data = self.h5ds[chunk_slice]
+        if self.boolean:
+            data = np.array(data, dtype=bool)
+        return data
 
-    def get_chunk(self, chunk_index):
-        if chunk_index not in self.cache:
-            data = np.array(
-                self.image.get_chunk(chunk_index), dtype=np.int16) \
-                - self.image_bg.get_chunk(chunk_index)
-            self.cache[chunk_index] = data
-            if len(self.cache) > self.cache_size:
-                # Remove the first item
-                self.cache.popitem(last=False)
-        return self.cache[chunk_index]
 
-    def iter_chunks(self):
-        return self.image.iter_chunks()
+class ImageCorrCache(BaseImageChunkCache):
+    def __init__(self,
+                 image: HDF5ImageCache,
+                 image_bg: HDF5ImageCache):
+        super(ImageCorrCache, self).__init__(
+            shape=image.shape,
+            chunk_size=image.chunk_size,
+            cache_size=image.cache_size)
+        self.image = image
+        self.image_bg = image_bg
+
+    def _get_chunk_data(self, chunk_slice):
+        data = np.array(
+            self.image._get_chunk_data(chunk_slice), dtype=np.int16) \
+           - self.image_bg._get_chunk_data(chunk_slice)
+        return data
 
 
 @functools.cache
 def md5sum(path, blocksize=65536, count=0):
     """Compute (partial) MD5 sum of a file
 
     Parameters
```

### Comparing `dcnum-0.17.2/src/dcnum/read/hdf5_data.py` & `dcnum-0.18.0/src/dcnum/read/hdf5_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,94 +9,138 @@
 import warnings
 
 import h5py
 import numpy as np
 
 from .cache import HDF5ImageCache, ImageCorrCache, md5sum
 from .const import PROTECTED_FEATURES
+from .mapped import get_mapped_object, get_mapping_indices
 
 
 class HDF5Data:
     """HDF5 (.rtdc) input file data instance"""
     def __init__(self,
                  path: pathlib.Path | h5py.File | BinaryIO,
                  pixel_size: float = None,
                  md5_5m: str = None,
                  meta: Dict = None,
                  basins: List[Dict[List[str] | str]] = None,
                  logs: Dict[List[str]] = None,
                  tables: Dict[np.ndarray] = None,
                  image_cache_size: int = 2,
+                 index_mapping: int | slice | List | np.ndarray = None,
                  ):
+        """
+
+        Parameters
+        ----------
+        path:
+            path to data file
+        pixel_size:
+            pixel size in µm
+        md5_5m:
+            MD5 sum of the first 5 MiB; computed if not provided
+        meta:
+            metadata dictionary; extracted from HDF5 attributes
+            if not provided
+        basins:
+            list of basin dictionaries; extracted from HDF5 attributes
+            if not provided
+        logs:
+            dictionary of logs; extracted from HDF5 attributes
+            if not provided
+        tables:
+            dictionary of tables; extracted from HDF5 attributes
+            if not provided
+        image_cache_size:
+            size of the image cache to use when accessing image data
+        index_mapping:
+            select only a subset of input events, transparently reducing the
+            size of the dataset, possible data types are
+            - int `N`: use the first `N` events
+            - slice: use the events defined by a slice
+            - list: list of integers specifying the event indices to use
+            Numpy indexing rules apply. E.g. to only process the first
+            100 events, set this to `100` or `slice(0, 100)`.
+        """
         # Init is in __setstate__ so we can pickle this class
         # and use it for multiprocessing.
         if isinstance(path, h5py.File):
             self.h5 = path
             path = path.filename
+
         self.__setstate__({"path": path,
                            "pixel_size": pixel_size,
                            "md5_5m": md5_5m,
                            "meta": meta,
                            "basins": basins,
                            "logs": logs,
                            "tables": tables,
                            "image_cache_size": image_cache_size,
+                           "index_mapping": index_mapping,
                            })
 
     def __contains__(self, item):
         return item in self.keys()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     def __getitem__(self, feat):
         if feat in ["image", "image_bg", "mask"]:
-            data = self.get_image_cache(feat)
+            data = self.get_image_cache(feat)  # already index-mapped
             if data is None:
                 raise KeyError(f"Feature '{feat}' not found in {self}!")
             else:
                 return data
         elif feat in self._cache_scalar:  # check for scalar cached
             return self._cache_scalar[feat]
         elif (feat in self.h5["events"]
               and len(self.h5["events"][feat].shape) == 1):  # cache scalar
-            self._cache_scalar[feat] = self.h5["events"][feat][:]
+            if self.index_mapping is None:
+                idx_map = slice(None)  # no mapping indices, just slice
+            else:
+                idx_map = get_mapping_indices(self.index_mapping)
+            self._cache_scalar[feat] = self.h5["events"][feat][idx_map]
             return self._cache_scalar[feat]
         else:
             if feat in self.h5["events"]:
                 # Not cached (possibly slow)
                 warnings.warn(f"Feature {feat} not cached (possibly slow)")
-                return self.h5["events"][feat]
+                return get_mapped_object(
+                    obj=self.h5["events"][feat],
+                    index_mapping=self.index_mapping)
             else:
                 # Check the basins
                 for idx in range(len(self.basins)):
                     bn, bn_features = self.get_basin_data(idx)
                     if bn_features and feat in bn_features:
-                        return bn[feat]
+                        return bn[feat]  # already index-mapped
         # If we got here, then the feature data does not exist.
         raise KeyError(f"Feature '{feat}' not found in {self}!")
 
     def __getstate__(self):
         return {"path": self.path,
                 "pixel_size": self.pixel_size,
                 "md5_5m": self.md5_5m,
                 "meta": self.meta,
                 "logs": self.logs,
                 "tables": self.tables,
                 "basins": self.basins,
-                "image_cache_size": self.image.cache_size
+                "image_cache_size": self.image.cache_size,
+                "index_mapping": self.index_mapping,
                 }
 
     def __setstate__(self, state):
         # Make sure these properties exist (we rely on __init__, because
         # we want this class to be pickable and __init__ is not called by
-        # `pickle.load`.
+        # `pickle.load`).
         # Cached properties
         self._feats = None
         self._keys = None
         self._len = None
         self.image_cache_size = state["image_cache_size"]
         # Image cache
         if not hasattr(self, "_image_cache"):
@@ -112,15 +156,15 @@
 
         self.path = state["path"]
 
         self.md5_5m = state["md5_5m"]
         if self.md5_5m is None:
             if isinstance(self.path, pathlib.Path):
                 # 5MB md5sum of input file
-                self.md5_5m = md5sum(self.path, count=80)
+                self.md5_5m = md5sum(self.path, blocksize=65536, count=80)
             else:
                 self.md5_5m = str(uuid.uuid4()).replace("-", "")
         self.meta = state["meta"]
         self.logs = state["logs"]
         self.tables = state["tables"]
         self.basins = state["basins"]
         if (self.meta is None
@@ -161,20 +205,25 @@
                     self.basins.append(bn_dict)
 
         if state["pixel_size"] is not None:
             self.pixel_size = state["pixel_size"]
 
         self.image_cache_size = state["image_cache_size"]
 
+        self.index_mapping = state["index_mapping"]
+
         if self.h5 is None:
             self.h5 = h5py.File(self.path, libver="latest")
 
     def __len__(self):
         if self._len is None:
-            self._len = self.h5.attrs["experiment:event count"]
+            if self.index_mapping is not None:
+                self._len = get_mapping_indices(self.index_mapping).size
+            else:
+                self._len = self.h5.attrs["experiment:event count"]
         return self._len
 
     @property
     def image(self):
         return self.get_image_cache("image")
 
     @property
@@ -251,28 +300,34 @@
         return "hdf"
 
     @classmethod
     def get_ppid_from_ppkw(cls, kwargs):
         # Data does not really fit into the PPID scheme we use for the rest
         # of the pipeline. This implementation here is custom.
         code = cls.get_ppid_code()
-        kwid = f"p={kwargs['pixel_size']:.8f}".rstrip("0")
+        ppid_ps = f"{kwargs['pixel_size']:.8f}".rstrip("0")
+        kwid = "^".join([f"p={ppid_ps}"])
         return ":".join([code, kwid])
 
     @staticmethod
     def get_ppkw_from_ppid(dat_ppid):
         # Data does not fit in the PPID scheme we use, but we still
         # would like to pass pixel_size to __init__ if we need it.
-        code, pp_dat_kwargs = dat_ppid.split(":")
+        code, kwargs_str = dat_ppid.split(":")
         if code != HDF5Data.get_ppid_code():
             raise ValueError(f"Could not find data method '{code}'!")
-        p, val = pp_dat_kwargs.split("=")
-        if p != "p":
-            raise ValueError(f"Invalid parameter '{p}'!")
-        return {"pixel_size": float(val)}
+        kwitems = kwargs_str.split("^")
+        kwargs = {}
+        for item in kwitems:
+            var, val = item.split("=")
+            if var == "p":
+                kwargs["pixel_size"] = float(val)
+            else:
+                raise ValueError(f"Invalid parameter '{var}'!")
+        return kwargs
 
     def get_basin_data(self, index):
         """Return HDF5Data info for a basin index in `self.basins`
 
         Returns
         -------
         data: HDF5Data
@@ -294,15 +349,15 @@
                         path = prel
                         break
             else:
                 path = None
             if path is None:
                 self._basin_data[index] = (None, None)
             else:
-                h5dat = HDF5Data(path)
+                h5dat = HDF5Data(path, index_mapping=self.index_mapping)
                 features = bn_dict.get("features")
                 if features is None:
                     # Only get the features from the actual HDF5 file.
                     # If this file has basins as well, the basin metadata
                     # should have been copied over to the parent file. This
                     # makes things a little cleaner, because basins are not
                     # nested, but all basins are available in the top file.
@@ -332,15 +387,16 @@
                             ds = bndat.h5[f"events/{feat}"]
                             break
                 else:
                     ds = None
 
             if ds is not None:
                 image = HDF5ImageCache(
-                    h5ds=ds,
+                    h5ds=get_mapped_object(obj=ds,
+                                           index_mapping=self.index_mapping),
                     cache_size=self.image_cache_size,
                     boolean=feat == "mask")
             else:
                 image = None
             self._image_cache[feat] = image
 
         return self._image_cache[feat]
@@ -382,14 +438,15 @@
         List of features to take from the input files.
 
     Notes
     -----
     - If one of the input files does not contain a feature from the first
       input `paths`, then a `ValueError` is raised. Use the `features`
       argument to specify which features you need instead.
+    - Basins are not considered.
     """
     h5kwargs = {"mode": "w", "libver": "latest"}
     if isinstance(path_out, (pathlib.Path, str)):
         h5kwargs["name"] = path_out
     elif path_out is True:
         tf = tempfile.NamedTemporaryFile(prefix="dcnum_vc_",
                                          suffix=".hdf5",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dcnum-0.17.2/src/dcnum/segm/segm_thresh.py` & `dcnum-0.18.0/src/dcnum/segm/segm_thresh.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,34 +12,34 @@
 
     def __init__(self, thresh=-6, *args, **kwargs):
         """Simple image thresholding segmentation
 
         Parameters
         ----------
         thresh: int
-            grayscale threhold value for creating the mask image;
+            grayscale threshold value for creating the mask image;
             For a background-corrected image, pixels with values below
             this value are considered to be part of the mask.
         """
         super(SegmentThresh, self).__init__(thresh=thresh, *args, **kwargs)
 
     @staticmethod
     def segment_approach(image, *,
                          thresh: float = -6):
-        """Mask retrieval as it is done in Shape-In
+        """Mask retrieval using basic thresholding
 
         Parameters
         ----------
         image: 2d ndarray
             Background-corrected frame image
         thresh: float
             Threshold value for creation of binary mask; a negative value
             means that pixels darker than the background define the threshold
             level.
 
         Returns
         -------
         mask: 2d boolean ndarray
-            Mask image for the give index
+            Mask image for the given index
         """
         assert thresh < 0, "threshold values above zero not supported!"
         return image < thresh
```

### Comparing `dcnum-0.17.2/src/dcnum/segm/segmenter.py` & `dcnum-0.18.0/src/dcnum/segm/segmenter.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,18 +64,16 @@
                 f"is disabled for segmenter {self.__class__}")
 
     @staticmethod
     @functools.cache
     def get_border(shape):
         """Cached boolean image with outer pixels set to True"""
         border = np.zeros(shape, dtype=bool)
-        border[0, :] = True
-        border[-1, :] = True
-        border[:, 0] = True
-        border[:, -1] = True
+        border[[0, -1], :] = True
+        border[:, [0, -1]] = True
         return border
 
     @staticmethod
     @functools.cache
     def get_disk(radius):
         """Cached `skimage.morphology.disk(radius)`"""
         return morphology.disk(radius)
@@ -117,46 +115,63 @@
         """Return the pipeline ID from given keyword arguments
 
         See Also
         --------
         get_ppid: Same method for class instances
         """
         kwargs = copy.deepcopy(kwargs)
-        if kwargs_mask is None and kwargs.get("kwargs_mask", None) is None:
-            raise KeyError("`kwargs_mask` must be either specified as "
-                           "keyword argument to this method or as a key "
-                           "in `kwargs`!")
-        if kwargs_mask is None:
-            # see check above (kwargs_mask may also be {})
-            kwargs_mask = kwargs.pop("kwargs_mask")
-        # Start with the default mask kwargs defined for this subclass
-        kwargs_mask_used = copy.deepcopy(cls.mask_default_kwargs)
-        kwargs_mask_used.update(kwargs_mask)
-        code = cls.get_ppid_code()
-        csegm = kwargs_to_ppid(cls, "segment_approach", kwargs)
-        cmask = kwargs_to_ppid(cls, "process_mask", kwargs_mask_used)
-        return ":".join([code, csegm, cmask])
+        if cls.mask_postprocessing:
+            if kwargs_mask is None and kwargs.get("kwargs_mask", None) is None:
+                raise KeyError("`kwargs_mask` must be either specified as "
+                               "keyword argument to this method or as a key "
+                               "in `kwargs`!")
+            if kwargs_mask is None:
+                # see check above (kwargs_mask may also be {})
+                kwargs_mask = kwargs.pop("kwargs_mask")
+            # Start with the default mask kwargs defined for this subclass
+            kwargs_mask_used = copy.deepcopy(cls.mask_default_kwargs)
+            kwargs_mask_used.update(kwargs_mask)
+        elif kwargs_mask:
+            raise ValueError(f"The segmenter '{cls.__name__}' does not "
+                             f"support mask postprocessing, but 'kwargs_mask' "
+                             f"was provided: {kwargs_mask}")
+
+        ppid_parts = [
+            cls.get_ppid_code(),
+            kwargs_to_ppid(cls, "segment_approach", kwargs),
+            ]
+
+        if cls.mask_postprocessing:
+            ppid_parts.append(
+                kwargs_to_ppid(cls, "process_mask", kwargs_mask_used))
+
+        return ":".join(ppid_parts)
 
     @staticmethod
     def get_ppkw_from_ppid(segm_ppid):
         """Return keyword arguments for this pipeline identifier"""
-        code, pp_kwargs, pp_kwargs_mask = segm_ppid.split(":")
+        ppid_parts = segm_ppid.split(":")
+        code = ppid_parts[0]
+        pp_kwargs = ppid_parts[1]
+
         for cls_code in get_available_segmenters():
             if cls_code == code:
                 cls = get_available_segmenters()[cls_code]
                 break
         else:
             raise ValueError(
                 f"Could not find segmenter '{code}'!")
         kwargs = ppid_to_kwargs(cls=cls,
                                 method="segment_approach",
                                 ppid=pp_kwargs)
-        kwargs["kwargs_mask"] = ppid_to_kwargs(cls=cls,
-                                               method="process_mask",
-                                               ppid=pp_kwargs_mask)
+        if cls.mask_postprocessing:
+            pp_kwargs_mask = ppid_parts[2]
+            kwargs["kwargs_mask"] = ppid_to_kwargs(cls=cls,
+                                                   method="process_mask",
+                                                   ppid=pp_kwargs_mask)
         return kwargs
 
     @staticmethod
     def process_mask(labels, *,
                      clear_border: bool = True,
                      fill_holes: bool = True,
                      closing_disk: int = 5):
@@ -192,55 +207,71 @@
                 indices = sorted(np.unique(labels[border]))
                 for li in indices:
                     if li == 0:
                         # ignore background values
                         continue
                     labels[labels == li] = 0
 
-        # scikit-image is too slow for us here. So we use OpenCV.
-        # https://github.com/scikit-image/scikit-image/issues/1190
-
-        if closing_disk:
-            #
-            # from skimage import morphology
-            # morphology.binary_closing(
-            #    mask,
-            #    footprint=morphology.disk(closing_disk),
-            #    out=mask)
-            #
-            element = Segmenter.get_disk(closing_disk)
-            labels_uint8 = np.array(labels, dtype=np.uint8)
-            labels_dilated = cv2.dilate(labels_uint8, element)
-            labels_eroded = cv2.erode(labels_dilated, element)
-            labels, _ = ndi.label(
-                input=labels_eroded > 0,
-                structure=ndi.generate_binary_structure(2, 2))
-
         if fill_holes:
             # Floodfill only works with uint8 (too small) or int32
             if labels.dtype != np.int32:
                 labels = np.array(labels, dtype=np.int32)
             #
             # from scipy import ndimage
             # mask_old = ndimage.binary_fill_holes(mask)
             #
             # Floodfill algorithm fills the background image and
             # the resulting inversion is the image with holes filled.
             # This will destroy labels (adding 2,147,483,647 to background)
+            # Since floodfill will use the upper left corner of the image as
+            # a seed, we have to make sure it is set to background. We set
+            # a line of pixels in the upper channel wall to zero to be sure.
+            labels[0, :] = 0
+            # ...and a 4x4 pixel region in the top left corner.
+            labels[1, :2] = 0
             cv2.floodFill(labels, None, (0, 0), 2147483647)
             mask = labels != 2147483647
             labels, _ = ndi.label(
                 input=mask,
                 structure=ndi.generate_binary_structure(2, 2))
 
+        if closing_disk:
+            # scikit-image is too slow for us here. So we use OpenCV.
+            # https://github.com/scikit-image/scikit-image/issues/1190
+            #
+            # from skimage import morphology
+            # morphology.binary_closing(
+            #    mask,
+            #    footprint=morphology.disk(closing_disk),
+            #    out=mask)
+            #
+            element = Segmenter.get_disk(closing_disk)
+            # Note: erode/dilate not implemented for int32
+            labels_uint8 = np.array(labels, dtype=np.uint8)
+            # Historically, we would like to do a closing (dilation followed
+            # by erosion) on the image data where lower brightness values
+            # meant "we have an event". However, since we are now working
+            # with labels instead of image data (0 is background and labels
+            # are enumerated with integers), high "brightness" values are
+            # actually the event. Thus, we have to perform an opening
+            # (erosion followed by dilation) of the label image.
+            labels_eroded = cv2.erode(labels_uint8, element)
+            labels_dilated = cv2.dilate(labels_eroded, element)
+            labels, _ = ndi.label(
+                input=labels_dilated > 0,
+                structure=ndi.generate_binary_structure(2, 2))
+
         return labels
 
-    def segment_chunk(self, image_data, chunk):
+    def segment_chunk(self, image_data, chunk, bg_off=None):
         """Return the integer labels for one `image_data` chunk"""
         data = image_data.get_chunk(chunk)
+        if bg_off is not None:
+            bg_off_chunk = bg_off[image_data.get_chunk_slice(chunk)]
+            data = data - bg_off_chunk.reshape(-1, 1, 1)
         return self.segment_batch(data)
 
     def segment_frame(self, image):
         """Return the integer label image for `index`"""
         segm_wrap = self.segment_frame_wrapper()
         # obtain mask or label
         mol = segm_wrap(image)
```

### Comparing `dcnum-0.17.2/src/dcnum/segm/segmenter_cpu.py` & `dcnum-0.18.0/src/dcnum/segm/segmenter_cpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,19 +92,19 @@
         Parameters
         ----------
         image_shape: tuple of int
             Shape of one single image in the array
         batch_size: int
             Number of images in the array
         dtype:
-            ctype, e.g. `np.ctypeslib.ctypes.c_uint8`
-            or `np.ctypeslib.ctypes.c_bool`
+            numpy dtype
         """
         sx, sy = image_shape
-        sa_raw = mp_spawn.RawArray(dtype, int(sx * sy * batch_size))
+        ctype = np.ctypeslib.as_ctypes_type(dtype)
+        sa_raw = mp_spawn.RawArray(ctype, int(sx * sy * batch_size))
         # Convert the RawArray to something we can write to fast
         # (similar to memory view, but without having to cast) using
         # np.ctypeslib.as_array. See discussion in
         # https://stackoverflow.com/questions/37705974
         sa_np = np.ctypeslib.as_array(sa_raw).reshape(batch_size, sx, sy)
         return sa_raw, sa_np
 
@@ -168,22 +168,22 @@
             self.mp_batch_index.value = -1
             self.mp_shutdown.value = 0
 
         if self._mp_image_np is None:
             self.mp_image_raw, self._mp_image_np = self._create_shared_array(
                 image_shape=self.image_shape,
                 batch_size=batch_size,
-                dtype=np.ctypeslib.ctypes.c_int32,
+                dtype=image_data.dtype,
             )
 
         if self._mp_labels_np is None:
             self.mp_labels_raw, self._mp_labels_np = self._create_shared_array(
                 image_shape=self.image_shape,
                 batch_size=batch_size,
-                dtype=np.ctypeslib.ctypes.c_uint16,
+                dtype=np.uint16,
             )
 
         # populate image data
         self._mp_image_np[:] = image_data[start:stop]
 
         # Create the workers
         if self.debug:
```

### Comparing `dcnum-0.17.2/src/dcnum/segm/segmenter_gpu.py` & `dcnum-0.18.0/src/dcnum/segm/segmenter_gpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/src/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.18.0/src/dcnum/segm/segmenter_manager_thread.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 class SegmenterManagerThread(threading.Thread):
     def __init__(self,
                  segmenter: Segmenter,
                  image_data: HDF5ImageCache | ImageCorrCache,
                  slot_states: mp.Array,
                  slot_chunks: mp.Array,
+                 bg_off: np.ndarray = None,
                  debug: bool = False,
                  *args, **kwargs):
         """Manage the segmentation of image data
 
         Parameters
         ----------
         segmenter:
@@ -34,14 +35,18 @@
             segmentation for a free slot. A free slot means a value of "s"
             (for "task is with segmenter"). After the segmenter has done
             its job for a slot, the slot value will be set to "e" (for
             "task is with feature extractor").
         slot_chunks:
             For each slot in `slot_states`, this shared array defines
             on which chunk in `image_data` the segmentation took place.
+        bg_off:
+            1d array containing additional background image offset values
+            that are added to each background image before subtraction
+            from the input image
         debug:
             Whether to run in debugging mode (more verbose messages and
             CPU-based segmentation is done in one single thread instead
             of in multiple subprocesses).
 
         Notes
         -----
@@ -61,14 +66,16 @@
         super(SegmenterManagerThread, self).__init__(
               name="SegmenterManager", *args, **kwargs)
         self.logger = logging.getLogger("dcnum.segm.SegmenterManagerThread")
         #: Segmenter instance
         self.segmenter = segmenter
         #: Image data which is being segmented
         self.image_data = image_data
+        #: Additional, optional background offset
+        self.bg_off = bg_off
         #: Slot states
         self.slot_states = slot_states
         #: Current slot chunk index for the slot states
         self.slot_chunks = slot_chunks
         #: List containing the segmented labels of each slot
         self.labels_list = [None] * len(self.slot_states)
         #: Time counter for segmentation
@@ -85,15 +92,15 @@
             # Wait for a free slot to perform segmentation (compute labels)
             while True:
                 # - "e" there is data from the segmenter (the extractor
                 #   can take it and process it)
                 # - "s" the extractor processed the data and is waiting
                 #   for the segmenter
                 if self.slot_states[cur_slot] != "e":
-                    # It's the segmenters turn. Note that we use '!= "e"',
+                    # It's the segmenter's turn. Note that we use '!= "e"',
                     # because the initial value is "\x00".
                     break
                 else:
                     # Try another slot.
                     empty_slots += 1
                     cur_slot = (cur_slot + 1) % num_slots
                 if empty_slots >= num_slots:
@@ -102,15 +109,17 @@
                     time.sleep(.01)
 
             t1 = time.monotonic()
 
             # We have a free slot to compute the segmentation
             labels = self.segmenter.segment_chunk(
                 image_data=self.image_data,
-                chunk=chunk)
+                chunk=chunk,
+                bg_off=self.bg_off,
+            )
 
             # TODO: make this more memory efficient (pre-shared mp.Arrays?)
             # Store labels in a list accessible by the main thread
             self.labels_list[cur_slot] = np.copy(labels)
             # Remember the chunk index for this slot
             self.slot_chunks[cur_slot] = chunk
             # This must be done last: Let the extractor know that this
```

### Comparing `dcnum-0.17.2/src/dcnum/write/deque_writer_thread.py` & `dcnum-0.18.0/src/dcnum/write/deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/src/dcnum/write/queue_collector_thread.py` & `dcnum-0.18.0/src/dcnum/write/queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/src/dcnum/write/writer.py` & `dcnum-0.18.0/src/dcnum/write/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import hashlib
 import json
 import pathlib
-from typing import List
+from typing import Dict, List
 import warnings
 
 import h5py
 import hdf5plugin
 import numpy as np
 
 from .._version import version
@@ -13,29 +13,61 @@
 
 class CreatingFileWithoutBasinWarning(UserWarning):
     """Issued when creating a basin-based dataset without basins"""
     pass
 
 
 class HDF5Writer:
-    def __init__(self, path, mode="a", ds_kwds=None):
-        """Write deformability cytometry HDF5 data"""
-        self.h5 = h5py.File(path, mode=mode, libver="latest")
+    def __init__(self,
+                 # TODO: make this a mandatory argument when `path` is
+                 #       properly removed
+                 obj: h5py.File | pathlib.Path | str = None,
+                 mode: str = "a",
+                 ds_kwds: Dict = None,
+                 path: pathlib.Path | str = None,
+                 ):
+        """Write deformability cytometry HDF5 data
+
+        Parameters
+        ----------
+        obj: h5py.File | pathlib.Path | str
+            object to instantiate the writer from; If this is already
+            a :class:`h5py.File` object, then it is used, otherwise the
+            argument is passed to :class:`h5py.File`
+        mode: str
+            opening mode when using :class:`h5py.File`
+        ds_kwds: Dict
+            keyword arguments with which to initialize new Datasets
+            (e.g. compression)
+        """
+        if path is not None:
+            obj = path
+            warnings.warn("The `path` keyword argument is deprecated, use "
+                          "`obj` instead",
+                          DeprecationWarning)
+        if isinstance(obj, h5py.File):
+            self.h5 = obj
+            self.h5_owned = False
+        else:
+            self.h5 = h5py.File(obj, mode=mode, libver="latest")
+            self.h5_owned = True
         self.events = self.h5.require_group("events")
         ds_kwds = set_default_filter_kwargs(ds_kwds)
         self.ds_kwds = ds_kwds
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     def close(self):
-        self.h5.close()
+        self.h5.flush()
+        if self.h5_owned:
+            self.h5.close()
 
     @staticmethod
     def get_best_nd_chunks(item_shape, feat_dtype=np.float64):
         """Return best chunks for HDF5 datasets
 
         Chunking has performance implications. It’s recommended to keep the
         total size of dataset chunks between 10 KiB and 1 MiB. This number
```

### Comparing `dcnum-0.17.2/src/dcnum.egg-info/PKG-INFO` & `dcnum-0.18.0/src/dcnum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.17.2
+Version: 0.18.0
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Maximilian Schlögel, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.17.2/src/dcnum.egg-info/SOURCES.txt` & `dcnum-0.18.0/src/dcnum.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -25,31 +25,33 @@
 src/dcnum/feat/feat_background/base.py
 src/dcnum/feat/feat_background/bg_copy.py
 src/dcnum/feat/feat_background/bg_roll_median.py
 src/dcnum/feat/feat_background/bg_sparse_median.py
 src/dcnum/feat/feat_brightness/__init__.py
 src/dcnum/feat/feat_brightness/bright_all.py
 src/dcnum/feat/feat_brightness/common.py
-src/dcnum/feat/feat_moments/__init__.py
-src/dcnum/feat/feat_moments/ct_opencv.py
-src/dcnum/feat/feat_moments/mt_legacy.py
+src/dcnum/feat/feat_contour/__init__.py
+src/dcnum/feat/feat_contour/contour.py
+src/dcnum/feat/feat_contour/moments.py
+src/dcnum/feat/feat_contour/volume.py
 src/dcnum/feat/feat_texture/__init__.py
 src/dcnum/feat/feat_texture/common.py
 src/dcnum/feat/feat_texture/tex_all.py
 src/dcnum/logic/__init__.py
 src/dcnum/logic/ctrl.py
 src/dcnum/logic/job.py
 src/dcnum/logic/json_encoder.py
 src/dcnum/meta/__init__.py
 src/dcnum/meta/paths.py
 src/dcnum/meta/ppid.py
 src/dcnum/read/__init__.py
 src/dcnum/read/cache.py
 src/dcnum/read/const.py
 src/dcnum/read/hdf5_data.py
+src/dcnum/read/mapped.py
 src/dcnum/segm/__init__.py
 src/dcnum/segm/segm_thresh.py
 src/dcnum/segm/segmenter.py
 src/dcnum/segm/segmenter_cpu.py
 src/dcnum/segm/segmenter_gpu.py
 src/dcnum/segm/segmenter_manager_thread.py
 src/dcnum/write/__init__.py
@@ -65,14 +67,15 @@
 tests/test_feat_background_bg_sparsemed.py
 tests/test_feat_brightness.py
 tests/test_feat_event_extractor_manager.py
 tests/test_feat_gate.py
 tests/test_feat_haralick.py
 tests/test_feat_moments_based.py
 tests/test_feat_moments_based_extended.py
+tests/test_feat_volume.py
 tests/test_init.py
 tests/test_logic_job.py
 tests/test_logic_join.py
 tests/test_logic_json.py
 tests/test_logic_pipeline.py
 tests/test_meta_paths.py
 tests/test_meta_ppid_base.py
@@ -80,17 +83,20 @@
 tests/test_meta_ppid_data.py
 tests/test_meta_ppid_feat.py
 tests/test_meta_ppid_gate.py
 tests/test_meta_ppid_segm.py
 tests/test_read_basin.py
 tests/test_read_concat_hdf5.py
 tests/test_read_hdf5.py
+tests/test_read_hdf5_index_mapping.py
 tests/test_segm_base.py
+tests/test_segm_no_mask_proc.py
 tests/test_segm_thresh.py
 tests/test_write_deque_writer_thread.py
 tests/test_write_queue_collector_thread.py
 tests/test_write_writer.py
 tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
 tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+tests/data/fmt-hdf5_cytoshot_full-features_2024.zip
 tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
 tests/data/fmt-hdf5_shapein_empty.zip
 tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
```

### Comparing `dcnum-0.17.2/tests/conftest.py` & `dcnum-0.18.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip` & `dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/data/fmt-hdf5_shapein_empty.zip` & `dcnum-0.18.0/tests/data/fmt-hdf5_shapein_empty.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip` & `dcnum-0.18.0/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/helper_methods.py` & `dcnum-0.18.0/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_feat_background_base.py` & `dcnum-0.18.0/tests/test_feat_background_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_feat_background_bg_copy.py` & `dcnum-0.18.0/tests/test_feat_background_bg_copy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.18.0/tests/test_feat_background_bg_roll_median.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         mic.process_next_batch()
         assert mic.get_progress() == 90 / event_count
 
         assert mic.current_batch == 1
 
     with h5py.File(output_path) as h5:
         ds = h5["events/image_bg"]
-        assert ds.shape == (event_count, 5, 7)
+        assert ds.shape == (90, 5, 7)
         assert np.all(ds[90:] == 0), "not processed"
         assert np.all(ds[:90, 0, 0] == 0)
         assert np.all(ds[:90, 0, 1] == 1)
         assert np.all(ds[:90, 0, 2] == 2)
         assert np.all(ds[:90, 1, 0] == 7)
```

### Comparing `dcnum-0.17.2/tests/test_feat_background_bg_sparsemed.py` & `dcnum-0.18.0/tests/test_feat_background_bg_sparsemed.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         assert np.allclose(bic.step_times,
                            np.arange(0, duration, split_time))
         # process the data
         bic.process()
         # even though the actual kernel size is smaller (which is properly
         # logged, the pipeline identifier should have a kernel size of 200.
         # This is good, because it helps to check for reproducibility.
-        assert bic.get_ppid() == "sparsemed:k=200^s=0.01^t=0^f=0.8"
+        assert bic.get_ppid() == "sparsemed:k=200^s=0.01^t=0^f=0.8^o=1"
 
     assert output_path.exists()
 
 
 @pytest.mark.filterwarnings(
     "ignore::dcnum.write.writer.CreatingFileWithoutBasinWarning")
 def test_median_sparsemend_worker(tmp_path):
```

### Comparing `dcnum-0.17.2/tests/test_feat_brightness.py` & `dcnum-0.18.0/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_feat_event_extractor_manager.py` & `dcnum-0.18.0/tests/test_feat_event_extractor_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,17 @@
     assert "image" in hd
     log_queue = mp_spawn.Queue()
 
     slot_chunks = mp_spawn.Array("i", 1)
     slot_states = mp_spawn.Array("u", 1)
 
     thr_segm = SegmenterManagerThread(
-        segmenter=SegmentThresh(),
+        segmenter=SegmentThresh(
+            kwargs_mask={"closing_disk": 0},  # otherwise no event in 1st image
+        ),
         image_data=hd.image_corr,
         slot_states=slot_states,
         slot_chunks=slot_chunks,
         debug=True,
     )
     thr_segm.start()
```

### Comparing `dcnum-0.17.2/tests/test_feat_gate.py` & `dcnum-0.18.0/tests/test_feat_gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_feat_haralick.py` & `dcnum-0.18.0/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_feat_moments_based.py` & `dcnum-0.18.0/tests/test_feat_moments_based.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 import h5py
 import numpy as np
 import scipy.ndimage as ndi
 
-from dcnum.feat import feat_moments
+from dcnum.feat import feat_contour
 
 from helper_methods import retrieve_data
 
 data_path = pathlib.Path(__file__).parent / "data"
 
 
 def test_inert_ratio_prnc():
@@ -24,15 +24,15 @@
     mask[np.array(np.round(x1 + offset), dtype=int),
          np.array(np.round(y1 + offset), dtype=int)] = True
     mask = ndi.binary_fill_holes(mask)
 
     # sanity check that fill_holes worked
     assert np.sum(mask) > 22000
 
-    data = feat_moments.moments_based_features(
+    data = feat_contour.moments_based_features(
         mask=mask[np.newaxis],
         pixel_size=0.2645
     )
 
     raw = data["inert_ratio_raw"][0]
     assert np.allclose(raw, 1.125606191144217)
 
@@ -55,15 +55,15 @@
 
                 # sanity checks (nothing at boundary)
                 assert not np.any(maskij[0, :])
                 assert not np.any(maskij[-1, :])
                 assert not np.any(maskij[:, 0])
                 assert not np.any(maskij[:, -1])
 
-                dataij = feat_moments.moments_based_features(
+                dataij = feat_contour.moments_based_features(
                     mask=maskij[np.newaxis],
                     pixel_size=0.2645
                 )
 
                 prnc = dataij["inert_ratio_prnc"][0]
                 tilt = dataij["tilt"][0]
 
@@ -95,15 +95,15 @@
 
     mask[c[:, 1] + 10, c[:, 0] + 12] = True
     mask = ndi.binary_fill_holes(mask)
 
     # sanity check that fill_holes worked
     assert np.sum(mask) == 12
 
-    data = feat_moments.moments_based_features(
+    data = feat_contour.moments_based_features(
         mask=mask[np.newaxis],
         pixel_size=0.2645
     )
 
     raw = data["inert_ratio_raw"][0]
     prnc = data["inert_ratio_prnc"][0]
     tilt = data["tilt"][0]
@@ -131,15 +131,15 @@
 
     mask[c[:, 1] + 10, c[:, 0] + 12] = True
     mask = ndi.binary_fill_holes(mask)
 
     # sanity check that fill_holes worked
     assert np.sum(mask) == 18
 
-    data = feat_moments.moments_based_features(
+    data = feat_contour.moments_based_features(
         mask=mask[np.newaxis],
         pixel_size=0.2645
     )
 
     raw = data["inert_ratio_raw"][0]
     prnc = data["inert_ratio_prnc"][0]
     tilt = data["tilt"][0]
@@ -167,15 +167,15 @@
         "inert_ratio_cvx",
         "inert_ratio_raw",
         "inert_ratio_prnc",
     ]
 
     # Make data available
     with h5py.File(path) as h5:
-        data = feat_moments.moments_based_features(
+        data = feat_contour.moments_based_features(
             mask=h5["events/mask"][:],
             pixel_size=0.2645
         )
         for feat in feats:
             if feat.count("inert"):
                 rtol = 2e-5
                 atol = 1e-8
@@ -196,15 +196,15 @@
         [0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0],
     ], dtype=bool)[np.newaxis]
-    data = feat_moments.moments_based_features(
+    data = feat_contour.moments_based_features(
                 mask=masks,
                 pixel_size=0.2645
             )
     assert data["deform"].shape == (1,)
     assert np.isnan(data["deform"][0])
     assert np.isnan(data["area_um"][0])
 
@@ -214,15 +214,15 @@
         [0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0],
     ], dtype=bool)[np.newaxis]
-    data = feat_moments.moments_based_features(
+    data = feat_contour.moments_based_features(
                 mask=masks,
                 pixel_size=0.2645
             )
     assert data["deform"].shape == (1,)
     assert np.isnan(data["deform"][0])
     assert np.isnan(data["area_um"][0])
 
@@ -232,15 +232,15 @@
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
     ], dtype=bool)[np.newaxis]
-    data = feat_moments.moments_based_features(
+    data = feat_contour.moments_based_features(
                 mask=masks,
                 pixel_size=0.2645
             )
     assert data["deform"].shape == (1,)
     assert np.isnan(data["deform"][0])
     assert np.isnan(data["area_um"][0])
 
@@ -252,15 +252,15 @@
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 0, 0, 0, 0],
     ], dtype=bool)[np.newaxis]
-    data = feat_moments.moments_based_features(
+    data = feat_contour.moments_based_features(
                 mask=masks,
                 pixel_size=0.2645
             )
     assert data["deform"].shape == (1,)
     assert np.isnan(data["deform"][0])
     assert np.isnan(data["area_um"][0])
 
@@ -270,15 +270,15 @@
         [0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0],
         [0, 0, 1, 1, 0, 0],
         [0, 0, 1, 1, 0, 0],
         [0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0],
     ], dtype=bool)[np.newaxis]
-    data = feat_moments.moments_based_features(
+    data = feat_contour.moments_based_features(
                 mask=masks,
                 pixel_size=0.2645
             )
     assert data["deform"].shape == (1,)
     # This is the deformation of a square (compared to circle)
     assert np.allclose(data["deform"][0], 0.11377307454724206)
     # Without moments-based computation, this would be 4*pxsize=0.066125
@@ -300,15 +300,15 @@
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
         [0, 0, 1, 0, 0, 0],
     ], dtype=bool)
     mixed_masks = np.append(mask_valid[None, ...],
                             mask_invalid[None, ...], axis=0)
-    data = feat_moments.moments_based_features(
+    data = feat_contour.moments_based_features(
                 mask=mixed_masks,
                 pixel_size=0.2645)
     assert data["deform"].shape == (2,)
     assert np.all(data["valid"][:] == np.array([True, False]))
     assert not np.isnan(data["deform"][0])
     assert np.isnan(data["deform"][1])
 
@@ -336,15 +336,15 @@
         assert np.sum(mask) > 8000
         # sanity checks (nothing at boundary)
         assert not np.any(mask[0, :])
         assert not np.any(mask[-1, :])
         assert not np.any(mask[:, 0])
         assert not np.any(mask[:, -1])
 
-        data = feat_moments.moments_based_features(
+        data = feat_contour.moments_based_features(
             mask=mask[np.newaxis],
             pixel_size=0.2645
         )
         tilt = data["tilt"][0]
 
         th = np.mod(theta, np.pi)
         if th > np.pi/2:
```

### Comparing `dcnum-0.17.2/tests/test_logic_job.py` & `dcnum-0.18.0/tests/test_logic_job.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_logic_join.py` & `dcnum-0.18.0/tests/test_logic_join.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_logic_pipeline.py` & `dcnum-0.18.0/tests/test_logic_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,68 +36,98 @@
 
     # perform the initial pipeline
     with logic.DCNumJobRunner(job=job) as runner:
         runner.run()
 
     with h5py.File(path2) as h5:
         assert h5.attrs["pipeline:dcnum background"] \
-               == "sparsemed:k=150^s=1^t=0^f=0.8"
+               == "sparsemed:k=150^s=1^t=0^f=0.8^o=1"
 
     # now when we do everything again, not a things should be done
     job2 = logic.DCNumPipelineJob(path_in=path2,
                                   path_out=path2.with_name("final_out.rtdc"),
                                   background_kwargs={"kernel_size": 250},
                                   debug=True)
     with logic.DCNumJobRunner(job=job2) as runner2:
         runner2.run()
 
     with h5py.File(job2["path_out"]) as h5:
         assert "deform" in h5["events"]
         assert "image" in h5["events"]
         assert "image_bg" in h5["events"]
-        assert len(h5["events/deform"]) == 395
+        assert len(h5["events/deform"]) == 285
         assert h5.attrs["pipeline:dcnum background"] \
-               == "sparsemed:k=250^s=1^t=0^f=0.8"
+               == "sparsemed:k=250^s=1^t=0^f=0.8^o=1"
 
 
-def test_duplicate_pipeline():
+@pytest.mark.parametrize("index_mapping,size,mapping_out", [
+    (None, 395, "0"),
+    (5, 11, "5"),
+    (slice(3, 5, None), 6, "3-5-n"),
+    ([3, 5, 6, 7], 7, "h-6e582938"),
+])
+def test_duplicate_pipeline(index_mapping, size, mapping_out):
     """Test running the same pipeline twice
 
     When the pipeline is run on a file with the same pipeline
     identifier, data are just copied over. Nothing much fancy else.
     """
     path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
     path = path_orig.with_name("input.rtdc")
     path2 = path.with_name("path_intermediate.rtdc")
     with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
         pass
-    job = logic.DCNumPipelineJob(path_in=path, path_out=path2, debug=True)
+    job = logic.DCNumPipelineJob(
+        path_in=path,
+        path_out=path2,
+        data_kwargs={"index_mapping": index_mapping},
+        background_code="copy",
+        segmenter_code="thresh",
+        segmenter_kwargs={"thresh": -6,
+                          "kwargs_mask": {"closing_disk": 0}},
+        debug=True)
+    assert job.kwargs["data_kwargs"]["index_mapping"] == index_mapping
 
     # perform the initial pipeline
     with logic.DCNumJobRunner(job=job) as runner:
         runner.run()
     # Sanity checks for initial job
     with read.HDF5Data(job["path_out"]) as hd:
         # Check the logs
         logdat = " ".join(get_log(hd, time.strftime("dcnum-log-%Y")))
         assert "Starting background computation" in logdat
         assert "Finished background computation" in logdat
         assert "Starting segmentation and feature extraction" in logdat
         assert "Flushing data to disk" in logdat
         assert "Finished segmentation and feature extraction" in logdat
 
+    # get the first image for reference
+    with h5py.File(path) as h5:
+        if index_mapping is None:
+            idx0 = 0
+        else:
+            idx0 = read.get_mapping_indices(index_mapping)[0]
+        im0 = h5["/events/image"][idx0]
+
     # remove all logs just to be sure nothing interferes
     with h5py.File(path2, "a") as h5:
+        assert h5.attrs["pipeline:dcnum mapping"] == mapping_out
+        assert len(h5["events/deform"]) == size
         del h5["logs"]
 
-    # now when we do everything again, not a things should be done
-    job2 = logic.DCNumPipelineJob(path_in=path2,
-                                  path_out=path2.with_name("final_out.rtdc"),
-                                  no_basins_in_output=True,
-                                  debug=True)
+    # now when we do everything again, not a thing should be done
+    job2 = logic.DCNumPipelineJob(
+        path_in=path2,
+        path_out=path2.with_name("final_out.rtdc"),
+        no_basins_in_output=True,
+        background_code="copy",
+        segmenter_code="thresh",
+        segmenter_kwargs={"thresh": -6,
+                          "kwargs_mask": {"closing_disk": 0}},
+        debug=True)
     with logic.DCNumJobRunner(job=job2) as runner2:
         runner2.run()
     # Real check for second run (not the `not`s [sic]!)
     with read.HDF5Data(job2["path_out"]) as hd:
         # Check the logs
         logdat = " ".join(get_log(hd, time.strftime("dcnum-log-%Y")))
         assert "Starting background computation" not in logdat
@@ -106,15 +136,17 @@
         assert "Flushing data to disk" not in logdat
         assert "Finished segmentation and feature extraction" not in logdat
 
     with h5py.File(job2["path_out"]) as h5:
         assert "deform" in h5["events"]
         assert "image" in h5["events"]
         assert "image_bg" in h5["events"]
-        assert len(h5["events/deform"]) == 395
+        assert len(h5["events/deform"]) == size
+        assert h5.attrs["pipeline:dcnum mapping"] == "0"
+        assert np.all(h5["events/image"][0] == im0)
 
 
 def test_duplicate_transfer_basin_data():
     """task_transfer_basin_data should not copy basin data from input"""
     path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
     path = path_orig.with_name("input.rtdc")
     path2 = path.with_name("path_intermediate.rtdc")
@@ -300,21 +332,93 @@
 
     with read.HDF5Data(path) as hd:
         assert len(hd) == 200, "sanity check"
 
     # this is the default pipeline
     gen_id = ppid.DCNUM_PPID_GENERATION
     dat_id = "hdf:p=0.2645"
-    bg_id = "sparsemed:k=200^s=1^t=0^f=0.8"
-    seg_id = "thresh:t=-6:cle=1^f=1^clo=2"
-    feat_id = "legacy:b=1^h=1"
+    bg_id = "sparsemed:k=200^s=1^t=0^f=0.8^o=1"
+    seg_id = "thresh:t=-6:cle=1^f=1^clo=0"
+    feat_id = "legacy:b=1^h=1^v=1"
+    gate_id = "norm:o=0^s=10"
+    jobid = "|".join([gen_id, dat_id, bg_id, seg_id, feat_id, gate_id])
+
+    job = logic.DCNumPipelineJob(
+        path_in=path,
+        debug=debug,
+        segmenter_kwargs={"kwargs_mask": {"closing_disk": 0}},
+    )
+    assert job.get_ppid() == jobid
+
+    with logic.DCNumJobRunner(job=job) as runner:
+        assert len(runner.draw) == 200
+        runner.run()
+
+        assert job["path_out"].exists(), "output file must exist"
+        assert runner.path_temp_in.exists(), "tmp input still exists"
+
+    assert not runner.path_temp_in.exists(), "tmp input file mustn't exist"
+    assert not runner.path_temp_out.exists(), "tmp out file must not exist"
+
+    with read.HDF5Data(job["path_out"]) as hd:
+        assert "image" in hd
+        assert "image_bg" in hd
+        assert "deform" in hd
+        assert "inert_ratio_prnc" in hd
+        assert len(hd) == 395
+        assert hd["nevents"][0] == 1
+        assert hd["nevents"][1] == 2
+        assert np.all(hd["nevents"][:11] == [1, 2, 2, 2, 2, 3, 3, 3, 3, 3, 3])
+        assert np.all(hd["frame"][:11] == [1, 2, 2, 4, 4, 5, 5, 5, 6, 6, 6])
+        assert np.allclose(hd["area_um"][2], 36.694151125,
+                           atol=0.5, rtol=0)
+        assert np.allclose(hd["deform"][2], 0.29053587689236526,
+                           atol=0.001, rtol=0)
+
+    with h5py.File(job["path_out"]) as h5:
+        assert h5.attrs["pipeline:dcnum generation"] == gen_id
+        assert h5.attrs["pipeline:dcnum data"] == dat_id
+        assert h5.attrs["pipeline:dcnum background"] == bg_id
+        assert h5.attrs["pipeline:dcnum segmenter"] == seg_id
+        assert h5.attrs["pipeline:dcnum feature"] == feat_id
+        assert h5.attrs["pipeline:dcnum gate"] == gate_id
+        assert h5.attrs["pipeline:dcnum yield"] == 395
+        assert h5.attrs["experiment:event count"] == 395
+        pp_hash = h5.attrs["pipeline:dcnum hash"]
+        # test for general metadata
+        assert h5.attrs["experiment:sample"] == "data"
+        assert h5.attrs["experiment:date"] == "2022-04-21"
+        assert h5.attrs["experiment:run identifier"] == f"dcn-{pp_hash[:7]}"
+
+
+@pytest.mark.parametrize("debug", [True, False])
+def test_simple_pipeline_no_offset_correction(debug):
+    path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
+    path = path_orig.with_name("input.rtdc")
+    with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
+        pass
+
+    with read.HDF5Data(path) as hd:
+        assert len(hd) == 200, "sanity check"
+
+    # this is the default pipeline
+    gen_id = ppid.DCNUM_PPID_GENERATION
+    dat_id = "hdf:p=0.2645"
+    bg_id = "sparsemed:k=200^s=1^t=0^f=0.8^o=0"
+    seg_id = "thresh:t=-6:cle=1^f=1^clo=0"
+    feat_id = "legacy:b=1^h=1^v=1"
     gate_id = "norm:o=0^s=10"
     jobid = "|".join([gen_id, dat_id, bg_id, seg_id, feat_id, gate_id])
 
-    job = logic.DCNumPipelineJob(path_in=path, debug=debug)
+    job = logic.DCNumPipelineJob(
+        path_in=path,
+        debug=debug,
+        background_kwargs={"offset_correction": False},
+        segmenter_kwargs={"kwargs_mask": {"closing_disk": 0}},
+    )
     assert job.get_ppid() == jobid
 
     with logic.DCNumJobRunner(job=job) as runner:
         assert len(runner.draw) == 200
         runner.run()
 
         assert job["path_out"].exists(), "output file must exist"
@@ -367,15 +471,15 @@
         runner.join()
 
 
 @pytest.mark.parametrize("attr,oldval,newbg", [
     # Changes that trigger computation of new background
     ["pipeline:dcnum generation", "1", True],
     ["pipeline:dcnum data", "hdf:p=0.2656", True],
-    ["pipeline:dcnum background", "sparsemed:k=100^s=1^t=0^f=0.8", True],
+    ["pipeline:dcnum background", "sparsemed:k=100^s=1^t=0^f=0.8^o=1", True],
     # Changes that don't trigger background computation
     ["pipeline:dcnum segmenter", "thresh:t=-1:cle=1^f=1^clo=2", False],
     ["pipeline:dcnum feature", "thresh:t=-1:cle=1^f=1^clo=2", False],
     ["pipeline:dcnum gate", "norm:o=0^s=5", False],
     ["pipeline:dcnum yield", 5000, False],
     ["pipeline:dcnum hash", "asdasd", False],
 ])
@@ -398,17 +502,18 @@
     with h5py.File(path, "a") as h5:
         # marker for identifying recomputation of background
         h5["events/image_bg"][:, 0, 0] = 200
 
         # Set the default values
         h5.attrs["pipeline:dcnum generation"] = ppid.DCNUM_PPID_GENERATION
         h5.attrs["pipeline:dcnum data"] = "hdf:p=0.2645"
-        h5.attrs["pipeline:dcnum background"] = "sparsemed:k=200^s=1^t=0^f=0.8"
+        h5.attrs["pipeline:dcnum background"] = \
+            "sparsemed:k=200^s=1^t=0^f=0.8^o=1"
         h5.attrs["pipeline:dcnum segmenter"] = "thresh:t=-6:cle=1^f=1^clo=2"
-        h5.attrs["pipeline:dcnum feature"] = "legacy:b=1^h=1"
+        h5.attrs["pipeline:dcnum feature"] = "legacy:b=1^h=1^v=1"
         h5.attrs["pipeline:dcnum gate"] = "norm:o=0^s=10"
         h5.attrs["pipeline:dcnum yield"] = h5["events/image"].shape[0]
 
         if attr == "pipeline:dcnum hash":
             # set just the pipeline hash
             h5.attrs["pipeline:dcnum hash"] = oldval
         else:
@@ -445,17 +550,17 @@
     path = path_orig.with_name("input.rtdc")
     with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
         pass
 
     # this is the default pipeline
     gen_id = ppid.DCNUM_PPID_GENERATION
     dat_id = "hdf:p=0.2645"
-    bg_id = "sparsemed:k=200^s=1^t=0^f=0.8"
+    bg_id = "sparsemed:k=200^s=1^t=0^f=0.8^o=1"
     seg_id = "thresh:t=-6:cle=1^f=1^clo=2"
-    feat_id = "legacy:b=1^h=1"
+    feat_id = "legacy:b=1^h=1^v=1"
     gate_id = "norm:o=0^s=10"
     jobid = "|".join([gen_id, dat_id, bg_id, seg_id, feat_id, gate_id])
 
     job = logic.DCNumPipelineJob(path_in=path, debug=True)
     assert job.get_ppid() == jobid
 
     with logic.DCNumJobRunner(job=job) as runner:
```

### Comparing `dcnum-0.17.2/tests/test_meta_paths.py` & `dcnum-0.18.0/tests/test_meta_paths.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_meta_ppid_base.py` & `dcnum-0.18.0/tests/test_meta_ppid_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,20 +29,20 @@
         return cls.__name__
 
 
 def test_compute_pipeline_hash():
     pp_hash = ppid.compute_pipeline_hash(
         gen_id="7",
         dat_id="hdf:p=0.34",
-        bg_id="sparsemed:k=200^s=1^t=0^f=0.8",
+        bg_id="sparsemed:k=200^s=1^t=0^f=0.8^o=1",
         seg_id="thresh:t=-3:cle=1^f=1^clo=2",
-        feat_id="legacy:b=1^h=0",
+        feat_id="legacy:b=1^h=0^v=1",
         gate_id="norm:o=0^s=11",
     )
-    assert pp_hash == "ec11977fc233e133c29642736161f201"
+    assert pp_hash == "2e56aa93fcb264381c90a8fd181b3fbc"
 
 
 @pytest.mark.parametrize("in_list,out_list", [
     (["camera", "campus"],
      ["came", "camp"]),
     (["cole", "coleman"],
      ["cole", "colem"]),
```

### Comparing `dcnum-0.17.2/tests/test_meta_ppid_bg.py` & `dcnum-0.18.0/tests/test_meta_ppid_bg.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,39 +4,41 @@
 
 import pytest
 
 
 @pytest.mark.filterwarnings(
     "ignore::dcnum.write.writer.CreatingFileWithoutBasinWarning")
 @pytest.mark.parametrize("bg_ppid", [
-    "sparsemed:k=200^s=1^t=0^f=0.8",
-    "sparsemed:k=210^s=1^t=0^f=0.8",
-    "sparsemed:k=200^s=2^t=0^f=0.8",
-    "sparsemed:k=200^s=1^t=0.1^f=0.8",
-    "sparsemed:k=200^s=1^t=0^f=0.9",
+    "sparsemed:k=200^s=1^t=0^f=0.8^o=1",
+    "sparsemed:k=210^s=1^t=0^f=0.8^o=1",
+    "sparsemed:k=200^s=2^t=0^f=0.8^o=1",
+    "sparsemed:k=200^s=1^t=0.1^f=0.8^o=1",
+    "sparsemed:k=200^s=1^t=0^f=0.9^o=1",
+    "sparsemed:k=200^s=1^t=0^f=0.9^o=0",
 ])
 def test_ppid_decoding_sparsemed(bg_ppid, tmp_path):
     input_data = np.arange(5 * 7).reshape(1, 5, 7) * np.ones((120, 1, 1))
     path_out = tmp_path / "test.h5"
     bg_class = fbg.get_available_background_methods()["sparsemed"]
     kwargs = bg_class.get_ppkw_from_ppid(bg_ppid)
     with bg_class(input_data=input_data,
                   output_path=path_out,
                   **kwargs) as bg_inst:
         assert bg_inst.get_ppid() == bg_ppid
 
 
 def test_ppid_decoding_sparsemed_check_kwargs():
-    bg_ppid = "sparsemed:k=210^s=1^t=0^f=0.8"
+    bg_ppid = "sparsemed:k=210^s=1^t=0^f=0.8^o=0"
     bg_class = fbg.get_available_background_methods()["sparsemed"]
     kwargs = bg_class.get_ppkw_from_ppid(bg_ppid)
     assert kwargs["kernel_size"] == 210
     assert np.allclose(kwargs["split_time"], 1.0)
     assert np.allclose(kwargs["thresh_cleansing"], 0.0)
     assert np.allclose(kwargs["frac_cleansing"], 0.8)
+    assert np.allclose(kwargs["offset_correction"], False)
 
 
 @pytest.mark.parametrize("bg_code",
                          fbg.get_available_background_methods().keys())
 def test_ppid_required_method_definitions(bg_code):
     bg_class = fbg.get_available_background_methods()[bg_code]
     assert hasattr(bg_class, "get_ppid")
@@ -52,8 +54,8 @@
     input_data = np.arange(5 * 7).reshape(1, 5, 7) * np.ones((120, 1, 1))
     path_out = tmp_path / "test.h5"
     scls = fbg.get_available_background_methods()["sparsemed"]
     with scls(input_data=input_data,
               output_path=path_out,
               thresh_cleansing=.22) as sthr:
         assert sthr.get_ppid_code() == "sparsemed"
-        assert sthr.get_ppid() == "sparsemed:k=200^s=1^t=0.22^f=0.8"
+        assert sthr.get_ppid() == "sparsemed:k=200^s=1^t=0.22^f=0.8^o=1"
```

### Comparing `dcnum-0.17.2/tests/test_meta_ppid_data.py` & `dcnum-0.18.0/tests/test_meta_ppid_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_meta_ppid_feat.py` & `dcnum-0.18.0/tests/test_meta_ppid_feat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dcnum.feat import QueueEventExtractor
 
 
 def test_ppid_decoding_extr_check_kwargs():
-    extr_ppid = "legacy:b=1^h=0"
+    extr_ppid = "legacy:b=1^h=0^v=1"
     kwargs = QueueEventExtractor.get_ppkw_from_ppid(extr_ppid)
     assert kwargs["haralick"] is False
     assert kwargs["brightness"] is True
 
 
 def test_ppid_encoding_extr_check_kwargs():
     kwargs = {"haralick": True, "brightness": False}
     ppid = QueueEventExtractor.get_ppid_from_ppkw(kwargs)
-    assert ppid == "legacy:b=0^h=1"
+    assert ppid == "legacy:b=0^h=1^v=1"
 
 
 def test_ppid_required_method_definitions():
     extr_code = "legacy"
     extr_class = QueueEventExtractor
     assert hasattr(extr_class, "get_ppid")
     assert hasattr(extr_class, "get_ppid_code")
```

### Comparing `dcnum-0.17.2/tests/test_meta_ppid_gate.py` & `dcnum-0.18.0/tests/test_meta_ppid_gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_meta_ppid_segm.py` & `dcnum-0.18.0/tests/test_meta_ppid_segm.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_read_basin.py` & `dcnum-0.18.0/tests/test_read_basin.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_read_concat_hdf5.py` & `dcnum-0.18.0/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_read_hdf5.py` & `dcnum-0.18.0/tests/test_read_hdf5.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,17 +169,17 @@
 
 
 def test_meta_nest():
     path = retrieve_data(
         "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
     with read.HDF5Data(path) as hd:
         meta = hd.meta_nest
-        print(meta)
         assert meta["imaging"]["pixel size"] == .2645
         assert meta["experiment"]["time"] == '15:24:17'
+        # no volume yet in this file:
         assert meta["user"]["dcevent ppid feature"] == 'legacy:b=1^h=1'
 
 
 def test_pixel_size_getset(tmp_path):
     path = tmp_path / "test.hdf5"
     with h5py.File(path, "w") as hw:
         hw["events/image"] = np.random.rand(10, 80, 180)
```

### Comparing `dcnum-0.17.2/tests/test_segm_base.py` & `dcnum-0.18.0/tests/test_segm_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pytest
 
 from dcnum import segm
 from dcnum.meta import ppid
 import numpy as np
 
+
 data_path = pathlib.Path(__file__).parent / "data"
 SEGM_METH = segm.get_available_segmenters()
 SEGM_KEYS = sorted(SEGM_METH.keys())
 
 
 class MockImageData:
     mask = np.array([
@@ -99,15 +100,15 @@
     assert np.sum(labels4 != 0) == 31
     assert len(np.unique(labels4)) == 4  # (bg, filled, border, other)
     assert np.sum(labels4 == 1) == 9
     assert np.sum(labels4 == 2) == 10
     assert np.sum(labels4 == 3) == 12
 
 
-def test_segmenter_labeled_mask_closing_disk():
+def test_segmenter_labeled_mask_fill_holes():
     mask = np.array([
         [0, 0, 0, 0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0, 0, 0],
         [0, 0, 1, 1, 1, 0, 0, 0, 0],
         [0, 0, 1, 0, 1, 0, 0, 0, 0],  # filled, 1
         [0, 0, 1, 1, 1, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0, 0, 0],
@@ -124,51 +125,51 @@
         [0, 0, 0, 0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0, 0, 0],
         ], dtype=bool)
 
     sm1 = segm.segm_thresh.SegmentThresh(thresh=-6,
                                          kwargs_mask={"clear_border": True,
                                                       "fill_holes": True,
-                                                      "closing_disk": 1,
+                                                      "closing_disk": 0,
                                                       })
     labels1 = sm1.segment_frame(-10 * mask)
     assert np.sum(labels1 != 0) == 32
     assert len(np.unique(labels1)) == 3  # (bg, filled, other)
     assert np.sum(labels1 == 1) == 9
     # due to the relabeling done in `fill_holes`, the index of "other" is "3"
     assert np.sum(labels1 == 2) == 23
 
     sm2 = segm.segm_thresh.SegmentThresh(thresh=-6,
                                          kwargs_mask={"clear_border": True,
                                                       "fill_holes": False,
-                                                      "closing_disk": 1,
+                                                      "closing_disk": 0,
                                                       })
     labels2 = sm2.segment_frame(-10 * mask)
     _, l2a, l2b = np.unique(labels2)
-    assert np.sum(labels2 != 0) == 27
+    assert np.sum(labels2 != 0) == 23
     assert len(np.unique(labels2)) == 3  # (bg, filled, other)
-    assert np.sum(labels2 == l2a) == 9
-    assert np.sum(labels2 == l2b) == 18
+    assert np.sum(labels2 == l2a) == 8
+    assert np.sum(labels2 == l2b) == 15
 
     sm3 = segm.segm_thresh.SegmentThresh(thresh=-6,
                                          kwargs_mask={"clear_border": False,
                                                       "fill_holes": False,
-                                                      "closing_disk": 1,
+                                                      "closing_disk": 0,
                                                       })
     labels3 = sm3.segment_frame(-10 * mask)
-    assert np.sum(labels3 != 0) == 35
+    assert np.sum(labels3 != 0) == 31
     assert len(np.unique(labels3)) == 4  # (bg, filled, border, other)
-    assert np.sum(labels3 == 1) == 9
+    assert np.sum(labels3 == 1) == 8
     assert np.sum(labels3 == 2) == 8
-    assert np.sum(labels3 == 3) == 18
+    assert np.sum(labels3 == 3) == 15
 
     sm4 = segm.segm_thresh.SegmentThresh(thresh=-6,
                                          kwargs_mask={"clear_border": False,
                                                       "fill_holes": True,
-                                                      "closing_disk": 1,
+                                                      "closing_disk": 0,
                                                       })
     labels4 = sm4.segment_frame(-10 * mask)
     assert np.sum(labels4 != 0) == 40
     assert len(np.unique(labels4)) == 4  # (bg, filled, border, other)
     assert np.sum(labels4 == 1) == 9
     assert np.sum(labels4 == 2) == 8
     assert np.sum(labels4 == 3) == 23
@@ -202,15 +203,19 @@
                                 fill_holes=True,
                                 closing_disk=False)
     assert np.allclose(labels, labels_2)
     assert labels_2.dtype == np.int32
 
 
 def test_segmenter_segment_chunk():
-    with segm.segm_thresh.SegmentThresh(thresh=-12, debug=True) as sm:
+    with segm.segm_thresh.SegmentThresh(
+            thresh=-12,
+            kwargs_mask={"closing_disk": 0},
+            debug=True
+    ) as sm:
         image_data = MockImageData()
         labels_1 = np.copy(sm.segment_chunk(image_data, 0))  # below threshold
         assert sm.image_array.min() == -10
         labels_2 = np.copy(sm.segment_chunk(image_data, 10))  # above threshold
         assert sm.image_array.min() == -20
         assert np.all(labels_1 == 0)
         assert not np.all(labels_2 == 0)
@@ -269,7 +274,112 @@
     assert np.sum(lbs) > 0
     assert np.sum(lbs > 0) == 9
     assert lbs[:, 0].sum() == 0
     assert lbs[:, -1].sum() == 0
     assert lbs[0, :].sum() == 0
     assert lbs[-1, :].sum() == 0
     assert lbs[3, 3] == 3
+
+
+def test_segmenter_labeled_mask_clear_border():
+    lab0 = np.array([
+        [2, 0, 0, 0, 0, 0, 0, 0],  # bad seed position for floodfill
+        [0, 2, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 1, 1, 1, 0, 0, 0],
+        [0, 0, 1, 0, 1, 0, 0, 0],  # filled, 1
+        [0, 0, 1, 1, 1, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        ], dtype=int)
+
+    sm = segm.segm_thresh.SegmentThresh(thresh=-6)
+
+    labels = sm.process_mask(lab0,
+                             clear_border=False,
+                             fill_holes=True,
+                             closing_disk=False)
+
+    assert np.sum(labels == 0) > 20, "background should be largest"
+    assert np.sum(labels == 1) == 9
+
+
+def test_segmenter_labeled_mask_clear_border2():
+    lab0 = np.array([
+        [2, 2, 2, 0, 0, 0, 0, 0],  # bad seed position for floodfill
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 1, 1, 1, 0, 0, 0],
+        [0, 0, 1, 0, 1, 0, 0, 0],  # filled, 1
+        [0, 0, 1, 1, 1, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        ], dtype=int)
+
+    sm = segm.segm_thresh.SegmentThresh(thresh=-6)
+
+    labels = sm.process_mask(lab0,
+                             clear_border=False,
+                             fill_holes=True,
+                             closing_disk=False)
+
+    assert np.sum(labels == 0) > 20, "background should be largest"
+    assert np.sum(labels == 1) == 9
+
+
+def test_segmenter_labeled_mask_spurious_noise_closing():
+    lab0 = np.array([
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 2, 0, 0, 0],  # noise, 2
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 1, 1, 1, 1, 1, 0, 0],
+        [0, 1, 1, 1, 1, 1, 0, 0],
+        [0, 1, 1, 0, 1, 1, 0, 0],  # filled, 1
+        [0, 1, 1, 1, 1, 1, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 3, 3, 0, 0, 0, 0],  # noise, 3
+        [0, 0, 0, 0, 0, 0, 0, 0],
+        ], dtype=int)
+
+    # Structuring element disk 1:
+    # [0, 1, 0],
+    # [1, 1, 1],
+    # [0, 1, 0],
+
+    # After erosion:
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+    # [0, 0, 1, 1, 1, 0, 0, 0],
+    # [0, 0, 1, 1, 1, 0, 0, 0],
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+
+    # After dilation:
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+    # [0, 0, 1, 1, 1, 0, 0, 0],
+    # [0, 1, 1, 1, 1, 1, 0, 0],
+    # [0, 1, 1, 1, 1, 1, 0, 0],
+    # [0, 0, 1, 1, 1, 0, 0, 0],
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+    # [0, 0, 0, 0, 0, 0, 0, 0],
+
+    sm = segm.segm_thresh.SegmentThresh(thresh=-6)
+
+    labels = sm.process_mask(lab0,
+                             clear_border=False,
+                             fill_holes=True,
+                             closing_disk=1)
+
+    assert np.sum(labels == 0) > 20, "background should be largest"
+    assert np.sum(labels == 1) == 16
+    assert np.sum(labels) == 16, "only one label"
```

### Comparing `dcnum-0.17.2/tests/test_segm_thresh.py` & `dcnum-0.18.0/tests/test_segm_thresh.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,44 +12,40 @@
 
 data_path = pathlib.Path(__file__).parent / "data"
 
 
 def test_segm_thresh_basic():
     """Basic thresholding segmenter
 
-    The segmenter is equivalent to the old dcevent legacy segmenter with
-    the options legacy:t=-6^bl=0^bi=0^d=1:cle=1^f=1^clo=3
-    (no blur, no binaryops, clear borders, fill holes, closing disk 3).
-    Since in the dcevent pipeline, the data are gated and small objects
-    are removed, we have to do this here manually before comparing mask
-    images.
+    The data in "fmt-hdf5_cytoshot_full-features_2024.zip" were
+    created in 2024 using ChipStream and the threshold segmenter.
     """
     path = retrieve_data(
-        data_path / "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
+        data_path / "fmt-hdf5_cytoshot_full-features_2024.zip")
 
     # Get all the relevant information
     with h5py.File(path) as h5:
         image = h5["events/image"][:]
         image_bg = h5["events/image_bg"][:]
         mask = h5["events/mask"][:]
         frame = h5["events/frame"][:]
+        bg_off = h5["events/bg_off"][:]
 
     # Concatenate the masks
     frame_u, indices = np.unique(frame, return_index=True)
     image_u = image[indices]
-    image_bg_u = image_bg[indices]
+    image_bg_u = image_bg[indices] + bg_off[indices].reshape(-1, 1, 1)
     mask_u = np.zeros_like(image_u, dtype=bool)
     for ii, fr in enumerate(frame):
         idx = np.where(frame_u == fr)[0]
         mask_u[idx] = np.logical_or(mask_u[idx], mask[ii])
 
     image_u_c = np.array(image_u, dtype=int) - image_bg_u
 
-    sm = segm.segm_thresh.SegmentThresh(thresh=-6,
-                                        kwargs_mask={"closing_disk": 3})
+    sm = segm.segm_thresh.SegmentThresh()
     assert sm.requires_background_correction
 
     for ii in range(len(frame_u)):
         labels_seg = sm.segment_frame(image_u_c[ii])
         mask_seg = np.array(labels_seg, dtype=bool)
         # Remove small objects, because this is not implemented in the
         # segmenter class as it would be part of gating.
@@ -63,39 +59,38 @@
     assert cls.get_ppid_from_ppkw(segm_kwargs) == "thresh:t=-6:cle=1^f=1^clo=3"
 
 
 @pytest.mark.parametrize("worker_type", ["thread", "process"])
 def test_segm_thresh_segment_batch(worker_type):
     debug = worker_type == "thread"
     path = retrieve_data(
-        data_path / "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
+        data_path / "fmt-hdf5_cytoshot_full-features_2024.zip")
 
     # Get all the relevant information
     with h5py.File(path) as h5:
         image = h5["events/image"][:]
         image_bg = h5["events/image_bg"][:]
         mask = h5["events/mask"][:]
         frame = h5["events/frame"][:]
+        bg_off = h5["events/bg_off"][:]
 
     # Concatenate the masks
     frame_u, indices = np.unique(frame, return_index=True)
     image_u = image[indices]
-    image_bg_u = image_bg[indices]
+    image_bg_u = image_bg[indices] + bg_off[indices].reshape(-1, 1, 1)
     mask_u = np.zeros_like(image_u, dtype=bool)
     for ii, fr in enumerate(frame):
         idx = np.where(frame_u == fr)[0]
         mask_u[idx] = np.logical_or(mask_u[idx], mask[ii])
 
     image_u_c = np.array(image_u, dtype=int) - image_bg_u
 
-    sm = segm.segm_thresh.SegmentThresh(thresh=-6,
-                                        debug=debug,
-                                        kwargs_mask={"closing_disk": 3})
+    sm = segm.segm_thresh.SegmentThresh(debug=debug)
 
-    labels_seg = sm.segment_batch(image_u_c, start=0, stop=5)
+    labels_seg = sm.segment_batch(image_u_c, start=0, stop=11)
     assert labels_seg is sm.labels_array
     assert np.all(np.array(labels_seg, dtype=bool) == sm.mask_array)
     # tell workers to stop
     sm.join_workers()
 
     for ii in range(len(frame_u)):
         mask_seg = np.array(labels_seg[ii], dtype=bool)
@@ -111,15 +106,15 @@
 
     # Create fake data
     mask = np.zeros((121, 80, 200), dtype=bool)
     mask[:, 10:71, 100:161] = morphology.disk(30).reshape(-1, 61, 61)
     image = -10 * mask
 
     sm = segm.segm_thresh.SegmentThresh(thresh=-6,
-                                        kwargs_mask={"closing_disk": 3},
+                                        kwargs_mask={"closing_disk": 0},
                                         debug=debug)
 
     labels_seg_1 = np.copy(
         sm.segment_batch(image, start=0, stop=101))
 
     assert labels_seg_1.dtype == np.uint16  # uint8 is not enough
     assert sm.mp_batch_index.value == 0
```

### Comparing `dcnum-0.17.2/tests/test_write_deque_writer_thread.py` & `dcnum-0.18.0/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_write_queue_collector_thread.py` & `dcnum-0.18.0/tests/test_write_queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.17.2/tests/test_write_writer.py` & `dcnum-0.18.0/tests/test_write_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,28 @@
     with read.HDF5Data(path_wrt) as hd:
         assert len(hd.basins) == 1
         assert len(hd.basins[0]["features"]) == 48
         assert len(hd.basins[0]["paths"]) == 2
         assert np.allclose(hd["deform"][0], 0.07405636775888857)
 
 
+def test_open_from_h5py_object(tmp_path):
+    path = tmp_path / "test.rtdc"
+    with write.HDF5Writer(path) as hw:
+        hw.store_feature_chunk("userdef1", np.arange(10))
+
+    with h5py.File(path, "a") as h5:
+        with write.HDF5Writer(h5, "a") as hw:
+            hw.store_feature_chunk("userdef1", np.arange(10, 20))
+        assert h5.id, "file should not be closed"
+
+    with h5py.File(path) as h5:
+        assert np.all(h5["events"]["userdef1"] == np.arange(20))
+
+
 def test_writer_basic():
     path = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
     path_wrt = path.with_name("written.hdf5")
     with h5py.File(path) as h5, write.HDF5Writer(path_wrt) as hw:
         deform = h5["events"]["deform"][:]
         image = h5["events"]["image"][:]
```

