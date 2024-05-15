# Comparing `tmp/pytorch-lifestream-0.5.3.tar.gz` & `tmp/pytorch-lifestream-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-lifestream-0.5.3.tar", last modified: Wed Dec 13 22:46:50 2023, max compression
+gzip compressed data, was "pytorch-lifestream-0.6.0.tar", last modified: Wed May 15 08:24:40 2024, max compression
```

## Comparing `pytorch-lifestream-0.5.3.tar` & `pytorch-lifestream-0.6.0.tar`

### file list

```diff
@@ -1,332 +1,342 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.928257 pytorch-lifestream-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11397 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2023-12-13 22:46:50.928257 pytorch-lifestream-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.876257 pytorch-lifestream-0.5.3/ptls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12563 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/custom_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.880257 pytorch-lifestream-0.5.3/ptls/data_load/
--rw-r--r--   0 runner    (1001) docker     (127)    16884 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.880257 pytorch-lifestream-0.5.3/ptls/data_load/augmentations/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/augmentations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/augmentations/all_time_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/augmentations/build_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/augmentations/drop_day.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/augmentations/dropout_trx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/augmentations/random_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/augmentations/seq_len_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/augmentations/sequence_pair_augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.884257 pytorch-lifestream-0.5.3/ptls/data_load/data_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/data_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12776 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/data_module/cls_data_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/data_module/coles_data_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/data_module/cpc_data_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/data_module/cpc_v2_data_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/data_module/emb_data_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/data_module/emb_valid_data_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/data_module/map_augmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/data_module/nsp_data_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8407 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/data_module/rtd_data_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/data_module/seq_to_target_data_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8773 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/data_module/sop_data_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.884257 pytorch-lifestream-0.5.3/ptls/data_load/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/datasets/augmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/datasets/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/datasets/duckdb_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/datasets/memory_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/datasets/parquet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/datasets/parquet_file_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/datasets/persist_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/fast_tensor_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/feature_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/filter_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.888257 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/category_size_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/feature_bin_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/feature_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/feature_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/feature_type_cast.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/filter_non_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/id_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/id_filter_df.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/iterable_seq_len_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/iterable_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/seq_len_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/take_first_trx.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/target_empty_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/target_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/target_join.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/target_move.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/to_torch_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/list_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/padded_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/partitioned_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/data_load/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.888257 pytorch-lifestream-0.5.3/ptls/frames/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/abs_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.888257 pytorch-lifestream-0.5.3/ptls/frames/bert/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.888257 pytorch-lifestream-0.5.3/ptls/frames/bert/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/datasets/mlm_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/datasets/mlm_indexed_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/datasets/nsp_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/datasets/rtd_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/datasets/sop_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.892257 pytorch-lifestream-0.5.3/ptls/frames/bert/losses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/losses/query_soft_max.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.892257 pytorch-lifestream-0.5.3/ptls/frames/bert/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/modules/mlm_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/modules/mlm_nsp_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/modules/rtd_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/bert/modules/sop_nsp_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.892257 pytorch-lifestream-0.5.3/ptls/frames/coles/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/coles_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/coles_dataset_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/coles_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/coles_supervised_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/coles_supervised_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.896257 pytorch-lifestream-0.5.3/ptls/frames/coles/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/losses/barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/losses/binomial_deviance_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/losses/centroid_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/losses/complex_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/losses/contrastive_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/losses/histogram_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/losses/margin_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/losses/softmax_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/losses/triplet_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/losses/vicreg_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.896257 pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/all_positive_pair_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/all_triplets_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/distance_weighted_pair_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/hard_negative_pair_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/hard_triplet_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/pair_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/random_negative_triplet_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/semi_hard_triplet_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/triplet_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9481 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/coles/split_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.896257 pytorch-lifestream-0.5.3/ptls/frames/cpc/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/cpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.896257 pytorch-lifestream-0.5.3/ptls/frames/cpc/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/cpc/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/cpc/datasets/cpc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/cpc/datasets/cpc_v2_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.896257 pytorch-lifestream-0.5.3/ptls/frames/cpc/losses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/cpc/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/cpc/losses/cpc_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.900257 pytorch-lifestream-0.5.3/ptls/frames/cpc/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/cpc/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/cpc/metrics/cpc_accuracy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.900257 pytorch-lifestream-0.5.3/ptls/frames/cpc/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/cpc/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/cpc/modules/cpc_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/cpc/modules/cpc_v2_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.900257 pytorch-lifestream-0.5.3/ptls/frames/gpt/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/gpt/gpt_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/gpt/gpt_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/inference_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/ptls_data_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.900257 pytorch-lifestream-0.5.3/ptls/frames/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/supervised/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/supervised/seq_to_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/supervised/seq_to_target_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.900257 pytorch-lifestream-0.5.3/ptls/frames/tabformer/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/tabformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/tabformer/tabformer_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11436 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/frames/tabformer/tabformer_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/make_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    19617 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/make_datasets_spark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.900257 pytorch-lifestream-0.5.3/ptls/metric_learn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/metric_learn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.904257 pytorch-lifestream-0.5.3/ptls/metric_learn/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/metric_learn/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/metric_learn/dataset/complex_target_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/metric_learn/dataset/splitting_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/metric_learn/dataset/target_enumerator_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/metric_learn/ml_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/metric_learn/read_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.904257 pytorch-lifestream-0.5.3/ptls/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/binarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/head.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/pb.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/pb_feature_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.904257 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/abs_seq_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/agg_feature_seq_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/custom_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/gpt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/longformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/rnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/rnn_seq_encoder_distribution_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/statistics_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9062 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/seq_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.908257 pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/float_positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/noisy_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/scalers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/tabformer_feature_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/trx_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/trx_encoder_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/trx_encoder_ohe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/trx_mean_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/pl_fit_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/pl_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/pl_inference_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/pl_train_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.908257 pytorch-lifestream-0.5.3/ptls/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.908257 pytorch-lifestream-0.5.3/ptls/preprocessing/base/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/base/col_category_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/base/col_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/base/data_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.912257 pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/category_identity_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/col_identity_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/col_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/event_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/frequency_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/user_group_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pandas_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.912257 pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/category_identity_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/col_identity_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/col_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/event_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/frequency_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/user_group_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/preprocessing/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/size_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/swa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/tb_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.912257 pytorch-lifestream-0.5.3/ptls_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.912257 pytorch-lifestream-0.5.3/ptls_tests/metric_learning_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/metric_learning_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/metric_learning_tests/test_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_custom_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.916257 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.916257 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_augmentations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_augmentations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_augmentations/test_all_time_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_augmentations/test_dropout_trx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_augmentations/test_random_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_augmentations/test_seq_len_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_feature_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.920257 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_category_size_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_feature_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_id_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_id_filter_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_iterable_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_seq_len_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_target_empty_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_target_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_target_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_target_move.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_to_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_list_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_padded_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_distribution_target_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.920257 pytorch-lifestream-0.5.3/ptls_tests/test_frames/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.920257 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_bert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_bert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.920257 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_bert/test_datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_bert/test_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_bert/test_datasets/test_mlm_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_bert/test_mlm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.920257 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/test_coles_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.920257 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/test_sampling_strategies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/test_sampling_strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/test_sampling_strategies/test_pair_selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/test_sampling_strategies/test_triplet_selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_common_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_cpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_inference_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.920257 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_supervised/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_supervised/test_seq_to_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_supervised/test_seq_to_target_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_list_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.924257 pytorch-lifestream-0.5.3/ptls_tests/test_nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_head.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_pb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.924257 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_agg_feature_seq_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_longformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_rnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_rnn_seq_distribution_targets_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_statistics_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11575 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.924257 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/test_batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/test_noisy_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/test_trx_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/test_trx_encoder_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/test_trx_mean_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/test_trx_ohe_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_pl_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_pl_api_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_ranking_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/test_size_reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.924257 pytorch-lifestream-0.5.3/ptls_tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/ptls_tests/utils/data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 22:46:50.928257 pytorch-lifestream-0.5.3/pytorch_lifestream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2023-12-13 22:46:50.000000 pytorch-lifestream-0.5.3/pytorch_lifestream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12370 2023-12-13 22:46:50.000000 pytorch-lifestream-0.5.3/pytorch_lifestream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 22:46:50.000000 pytorch-lifestream-0.5.3/pytorch_lifestream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-13 22:46:50.000000 pytorch-lifestream-0.5.3/pytorch_lifestream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-13 22:46:50.000000 pytorch-lifestream-0.5.3/pytorch_lifestream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 22:46:50.928257 pytorch-lifestream-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2023-12-13 22:44:12.000000 pytorch-lifestream-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.269624 pytorch-lifestream-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-15 08:24:40.269624 pytorch-lifestream-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.221624 pytorch-lifestream-0.6.0/ptls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12563 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/custom_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.225624 pytorch-lifestream-0.6.0/ptls/data_load/
+-rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.225624 pytorch-lifestream-0.6.0/ptls/data_load/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/augmentations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/augmentations/all_time_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/augmentations/build_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/augmentations/drop_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/augmentations/dropout_trx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/augmentations/random_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/augmentations/seq_len_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/augmentations/sequence_pair_augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.229624 pytorch-lifestream-0.6.0/ptls/data_load/data_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/data_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12776 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/data_module/cls_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/data_module/coles_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/data_module/cpc_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/data_module/cpc_v2_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/data_module/emb_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/data_module/emb_valid_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/data_module/map_augmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/data_module/nsp_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/data_module/rtd_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/data_module/seq_to_target_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/data_module/sop_data_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.229624 pytorch-lifestream-0.6.0/ptls/data_load/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/datasets/augmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/datasets/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/datasets/duckdb_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/datasets/memory_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/datasets/parquet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/datasets/parquet_file_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/datasets/persist_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/fast_tensor_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/feature_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/filter_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.233624 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/add_modal_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/category_size_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/delete_nan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/feature_bin_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/feature_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/feature_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/feature_type_cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/filter_non_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/id_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/id_filter_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/iterable_seq_len_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/iterable_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/seq_len_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/take_first_trx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/target_empty_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/target_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/target_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/target_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/time_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/to_torch_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/list_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/padded_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/partitioned_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/data_load/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.233624 pytorch-lifestream-0.6.0/ptls/frames/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/abs_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.233624 pytorch-lifestream-0.6.0/ptls/frames/bert/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.233624 pytorch-lifestream-0.6.0/ptls/frames/bert/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/datasets/mlm_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/datasets/mlm_indexed_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/datasets/nsp_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/datasets/rtd_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/datasets/sop_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.233624 pytorch-lifestream-0.6.0/ptls/frames/bert/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/losses/query_soft_max.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.237624 pytorch-lifestream-0.6.0/ptls/frames/bert/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/modules/mlm_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/modules/mlm_nsp_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/modules/rtd_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/bert/modules/sop_nsp_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.237624 pytorch-lifestream-0.6.0/ptls/frames/coles/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/coles_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/coles_dataset_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/coles_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/coles_supervised_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/coles_supervised_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.241624 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/binomial_deviance_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/centroid_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/complex_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/contrastive_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/histogram_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/margin_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/softmax_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/triplet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/losses/vicreg_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/multimodal_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/multimodal_inference_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/multimodal_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/multimodal_supervised_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.241624 pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/all_positive_pair_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/all_triplets_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/distance_weighted_pair_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/hard_negative_pair_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/hard_triplet_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/pair_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/random_negative_triplet_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/semi_hard_triplet_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/triplet_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/coles/split_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.241624 pytorch-lifestream-0.6.0/ptls/frames/cpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/cpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.241624 pytorch-lifestream-0.6.0/ptls/frames/cpc/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/cpc/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/cpc/datasets/cpc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/cpc/datasets/cpc_v2_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.241624 pytorch-lifestream-0.6.0/ptls/frames/cpc/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/cpc/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/cpc/losses/cpc_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.241624 pytorch-lifestream-0.6.0/ptls/frames/cpc/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/cpc/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/cpc/metrics/cpc_accuracy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.241624 pytorch-lifestream-0.6.0/ptls/frames/cpc/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/cpc/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/cpc/modules/cpc_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/cpc/modules/cpc_v2_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.245624 pytorch-lifestream-0.6.0/ptls/frames/gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/gpt/gpt_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/gpt/gpt_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/inference_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/ptls_data_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.245624 pytorch-lifestream-0.6.0/ptls/frames/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/supervised/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/supervised/seq_to_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/supervised/seq_to_target_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.245624 pytorch-lifestream-0.6.0/ptls/frames/tabformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/tabformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/tabformer/tabformer_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11436 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/frames/tabformer/tabformer_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/make_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19751 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/make_datasets_spark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.245624 pytorch-lifestream-0.6.0/ptls/metric_learn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/metric_learn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.245624 pytorch-lifestream-0.6.0/ptls/metric_learn/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/metric_learn/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/metric_learn/dataset/complex_target_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/metric_learn/dataset/splitting_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/metric_learn/dataset/target_enumerator_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/metric_learn/ml_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/metric_learn/read_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.245624 pytorch-lifestream-0.6.0/ptls/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/binarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/pb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/pb_feature_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.249624 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/abs_seq_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/agg_feature_seq_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/custom_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/gpt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/longformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/rnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/rnn_seq_encoder_distribution_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/statistics_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/seq_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.249624 pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/float_positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/noisy_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/scalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/tabformer_feature_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/trx_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/trx_encoder_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/trx_encoder_ohe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/trx_mean_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/pl_fit_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/pl_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/pl_inference_multimodal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/pl_inference_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/pl_train_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.253624 pytorch-lifestream-0.6.0/ptls/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.253624 pytorch-lifestream-0.6.0/ptls/preprocessing/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/base/col_category_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/base/col_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/base/data_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.253624 pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/category_identity_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/col_identity_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/col_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/event_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/frequency_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/user_group_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pandas_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.253624 pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/category_identity_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/col_identity_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/col_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/event_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/frequency_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/user_group_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/preprocessing/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/size_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/swa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/tb_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.257624 pytorch-lifestream-0.6.0/ptls_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.257624 pytorch-lifestream-0.6.0/ptls_tests/metric_learning_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/metric_learning_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/metric_learning_tests/test_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_custom_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.257624 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.257624 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_augmentations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_augmentations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_augmentations/test_all_time_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_augmentations/test_dropout_trx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_augmentations/test_random_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_augmentations/test_seq_len_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_feature_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.261624 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_category_size_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_feature_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_id_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_id_filter_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_iterable_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_seq_len_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_target_empty_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_target_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_target_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_target_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_list_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_padded_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_distribution_target_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.261624 pytorch-lifestream-0.6.0/ptls_tests/test_frames/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.261624 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_bert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_bert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.261624 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_bert/test_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_bert/test_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_bert/test_datasets/test_mlm_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_bert/test_mlm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.261624 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/test_coles_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.265624 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/test_sampling_strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/test_sampling_strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/test_sampling_strategies/test_pair_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/test_sampling_strategies/test_triplet_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_common_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_inference_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.265624 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_supervised/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_supervised/test_seq_to_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_supervised/test_seq_to_target_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_list_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_make_datasets_spark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.265624 pytorch-lifestream-0.6.0/ptls_tests/test_nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_pb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.265624 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_agg_feature_seq_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_longformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_rnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_rnn_seq_distribution_targets_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_statistics_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.269624 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/test_batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/test_noisy_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/test_trx_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/test_trx_encoder_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/test_trx_mean_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/test_trx_ohe_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_pl_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_pl_api_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_ranking_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/test_size_reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.269624 pytorch-lifestream-0.6.0/ptls_tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/ptls_tests/utils/data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:24:40.269624 pytorch-lifestream-0.6.0/pytorch_lifestream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-15 08:24:40.000000 pytorch-lifestream-0.6.0/pytorch_lifestream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-05-15 08:24:40.000000 pytorch-lifestream-0.6.0/pytorch_lifestream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:24:40.000000 pytorch-lifestream-0.6.0/pytorch_lifestream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-15 08:24:40.000000 pytorch-lifestream-0.6.0/pytorch_lifestream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 08:24:40.000000 pytorch-lifestream-0.6.0/pytorch_lifestream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:24:40.269624 pytorch-lifestream-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-15 08:21:50.000000 pytorch-lifestream-0.6.0/setup.py
```

### Comparing `pytorch-lifestream-0.5.3/LICENSE` & `pytorch-lifestream-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/PKG-INFO` & `pytorch-lifestream-0.6.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: pytorch-lifestream
-Version: 0.5.3
+Version: 0.6.0
 Summary: Lifestream data analysis with PyTorch
 Author: 
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-`PyTorch-LifeStream` or PTLS a library built upon [PyTorch](https://pytorch.org/) for building embeddings on discrete event sequences using self-supervision. It can process terabyte-size volumes of raw events like game history events, clickstream data, purchase history or card transactions.
+![ptls-logo](ptls-banner.png)
+
+
+[![GitHub license](https://img.shields.io/github/license/dllllb/pytorch-lifestream.svg)](https://github.com/dllllb/pytorch-lifestream/blob/master/LICENSE)
+[![PyPI version](https://badge.fury.io/py/pytorch-lifestream.svg)](https://badge.fury.io/py/pytorch-lifestream)
+[![GitHub issues](https://img.shields.io/github/issues/dllllb/pytorch-lifestream.svg)](https://github.com/dllllb/pytorch-lifestream/issues)
+[![Telegram](https://img.shields.io/badge/chat-on%20Telegram-2ba2d9.svg)](https://t.me/pytorch_lifestream)
+
+`pytorch-lifestream` or ptls a library built upon [PyTorch](https://pytorch.org/) for building embeddings on discrete event sequences using self-supervision. It can process terabyte-size volumes of raw events like game history events, clickstream data, purchase history or card transactions.
 
 It supports various methods of self-supervised training, adapted for event sequences:
 
 - Contrastive Learning for Event Sequences ([CoLES](https://arxiv.org/abs/2002.08232))
 - Contrastive Predictive Coding ([CPC](https://arxiv.org/abs/1807.03748))
 - Replaced Token Detection (RTD) from [ELECTRA](https://arxiv.org/abs/2003.10555)
 - Next Sequence Prediction (NSP) from [BERT](https://arxiv.org/abs/1810.04805)
@@ -43,33 +51,34 @@
 
 ```sh
 # Ubuntu 20.04
 
 sudo apt install python3.8 python3-venv
 pip3 install pipenv
 
-pipenv sync  --dev # install packages exactly as specified in Pipfile.lock
+pipenv sync --dev # install packages exactly as specified in Pipfile.lock
 pipenv shell
 pytest
 
 ```
 
 ## Demo notebooks
 
 - Supervised model training [notebook](demo/supervised-sequence-to-target.ipynb)
 - Self-supervided training and embeddings for downstream task [notebook](demo/coles-emb.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dllllb/pytorch-lifestream/blob/master/demo/coles-emb.ipynb)
+- Self-supervided training and embeddings for clients' transactions [notebook](demo/transaction-emb.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dllllb/pytorch-lifestream/blob/master/demo/transaction-emb.ipynb)
 - Self-supervided embeddings in CatBoost [notebook](demo/coles-catboost.ipynb)
 - Self-supervided training and fine-tuning [notebook](demo/coles-finetune.ipynb)
 - Self-supervised TrxEncoder only training with Masked Language Model task and fine-tuning [notebook](demo/mlm-emb.ipynb)
 - Pandas data preprocessing options [notebook](demo/preprocessing-demo.ipynb)
 - PySpark and Parquet for data preprocessing [notebook](demo/pyspark-parquet.ipynb)
 - Fast inference on large dataset [notebook](demo/extended_inference.ipynb)
 - Supervised multilabel classification [notebook](demo/multilabel-classification.ipynb)
 - Text features demo:
-  - Using pretrained encoder to text features[notebook](demo/coles-pretrained-embeddings.ipynb)
+  - Using pretrained encoder to text features [notebook](demo/coles-pretrained-embeddings.ipynb)
 
 ## Docs
 
 [Documentation](https://dllllb.github.io/pytorch-lifestream/)
 
 Library description [index](docs/index.md)
 
@@ -86,7 +95,25 @@
 - [American Express - Default Prediction Kaggle contest report](https://habr.com/ru/articles/704440/) (in Russian)
 
 ## How to contribute
 
 1. Make your chages via Fork and Pull request.
 2. Write unit test for new code in `ptls_tests`.
 3. Check unit test via `pytest`: [Example](.#install-from-source).
+
+## Citation
+
+We have a [paper](https://arxiv.org/abs/2002.08232) you can cite it:
+```bibtex
+@inproceedings{
+   Babaev_2022, series={SIGMOD/PODS ’22},
+   title={CoLES: Contrastive Learning for Event Sequences with Self-Supervision},
+   url={http://dx.doi.org/10.1145/3514221.3526129},
+   DOI={10.1145/3514221.3526129},
+   booktitle={Proceedings of the 2022 International Conference on Management of Data},
+   publisher={ACM},
+   author={Babaev, Dmitrii and Ovsov, Nikita and Kireev, Ivan and Ivanova, Maria and Gusev, Gleb and Nazarov, Ivan and Tuzhilin, Alexander},
+   year={2022},
+   month=jun, collection={SIGMOD/PODS ’22}
+}
+
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytorch-lifestream-0.5.3/README.md` & `pytorch-lifestream-0.6.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-`PyTorch-LifeStream` or PTLS a library built upon [PyTorch](https://pytorch.org/) for building embeddings on discrete event sequences using self-supervision. It can process terabyte-size volumes of raw events like game history events, clickstream data, purchase history or card transactions.
+![ptls-logo](ptls-banner.png)
+
+
+[![GitHub license](https://img.shields.io/github/license/dllllb/pytorch-lifestream.svg)](https://github.com/dllllb/pytorch-lifestream/blob/master/LICENSE)
+[![PyPI version](https://badge.fury.io/py/pytorch-lifestream.svg)](https://badge.fury.io/py/pytorch-lifestream)
+[![GitHub issues](https://img.shields.io/github/issues/dllllb/pytorch-lifestream.svg)](https://github.com/dllllb/pytorch-lifestream/issues)
+[![Telegram](https://img.shields.io/badge/chat-on%20Telegram-2ba2d9.svg)](https://t.me/pytorch_lifestream)
+
+`pytorch-lifestream` or ptls a library built upon [PyTorch](https://pytorch.org/) for building embeddings on discrete event sequences using self-supervision. It can process terabyte-size volumes of raw events like game history events, clickstream data, purchase history or card transactions.
 
 It supports various methods of self-supervised training, adapted for event sequences:
 
 - Contrastive Learning for Event Sequences ([CoLES](https://arxiv.org/abs/2002.08232))
 - Contrastive Predictive Coding ([CPC](https://arxiv.org/abs/1807.03748))
 - Replaced Token Detection (RTD) from [ELECTRA](https://arxiv.org/abs/2003.10555)
 - Next Sequence Prediction (NSP) from [BERT](https://arxiv.org/abs/1810.04805)
@@ -30,33 +38,34 @@
 
 ```sh
 # Ubuntu 20.04
 
 sudo apt install python3.8 python3-venv
 pip3 install pipenv
 
-pipenv sync  --dev # install packages exactly as specified in Pipfile.lock
+pipenv sync --dev # install packages exactly as specified in Pipfile.lock
 pipenv shell
 pytest
 
 ```
 
 ## Demo notebooks
 
 - Supervised model training [notebook](demo/supervised-sequence-to-target.ipynb)
 - Self-supervided training and embeddings for downstream task [notebook](demo/coles-emb.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dllllb/pytorch-lifestream/blob/master/demo/coles-emb.ipynb)
+- Self-supervided training and embeddings for clients' transactions [notebook](demo/transaction-emb.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dllllb/pytorch-lifestream/blob/master/demo/transaction-emb.ipynb)
 - Self-supervided embeddings in CatBoost [notebook](demo/coles-catboost.ipynb)
 - Self-supervided training and fine-tuning [notebook](demo/coles-finetune.ipynb)
 - Self-supervised TrxEncoder only training with Masked Language Model task and fine-tuning [notebook](demo/mlm-emb.ipynb)
 - Pandas data preprocessing options [notebook](demo/preprocessing-demo.ipynb)
 - PySpark and Parquet for data preprocessing [notebook](demo/pyspark-parquet.ipynb)
 - Fast inference on large dataset [notebook](demo/extended_inference.ipynb)
 - Supervised multilabel classification [notebook](demo/multilabel-classification.ipynb)
 - Text features demo:
-  - Using pretrained encoder to text features[notebook](demo/coles-pretrained-embeddings.ipynb)
+  - Using pretrained encoder to text features [notebook](demo/coles-pretrained-embeddings.ipynb)
 
 ## Docs
 
 [Documentation](https://dllllb.github.io/pytorch-lifestream/)
 
 Library description [index](docs/index.md)
 
@@ -73,7 +82,25 @@
 - [American Express - Default Prediction Kaggle contest report](https://habr.com/ru/articles/704440/) (in Russian)
 
 ## How to contribute
 
 1. Make your chages via Fork and Pull request.
 2. Write unit test for new code in `ptls_tests`.
 3. Check unit test via `pytest`: [Example](.#install-from-source).
+
+## Citation
+
+We have a [paper](https://arxiv.org/abs/2002.08232) you can cite it:
+```bibtex
+@inproceedings{
+   Babaev_2022, series={SIGMOD/PODS ’22},
+   title={CoLES: Contrastive Learning for Event Sequences with Self-Supervision},
+   url={http://dx.doi.org/10.1145/3514221.3526129},
+   DOI={10.1145/3514221.3526129},
+   booktitle={Proceedings of the 2022 International Conference on Management of Data},
+   publisher={ACM},
+   author={Babaev, Dmitrii and Ovsov, Nikita and Kireev, Ivan and Ivanova, Maria and Gusev, Gleb and Nazarov, Ivan and Tuzhilin, Alexander},
+   year={2022},
+   month=jun, collection={SIGMOD/PODS ’22}
+}
+
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytorch-lifestream-0.5.3/ptls/custom_layers.py` & `pytorch-lifestream-0.6.0/ptls/custom_layers.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/__init__.py` & `pytorch-lifestream-0.6.0/ptls/data_load/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/augmentations/all_time_shuffle.py` & `pytorch-lifestream-0.6.0/ptls/data_load/augmentations/all_time_shuffle.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/augmentations/build_augmentations.py` & `pytorch-lifestream-0.6.0/ptls/data_load/augmentations/build_augmentations.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/augmentations/drop_day.py` & `pytorch-lifestream-0.6.0/ptls/data_load/augmentations/drop_day.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/augmentations/dropout_trx.py` & `pytorch-lifestream-0.6.0/ptls/data_load/augmentations/dropout_trx.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/augmentations/random_slice.py` & `pytorch-lifestream-0.6.0/ptls/data_load/augmentations/random_slice.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/augmentations/seq_len_limit.py` & `pytorch-lifestream-0.6.0/ptls/data_load/augmentations/seq_len_limit.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/data_module/cls_data_module.py` & `pytorch-lifestream-0.6.0/ptls/data_load/data_module/cls_data_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/data_module/coles_data_module.py` & `pytorch-lifestream-0.6.0/ptls/data_load/data_module/coles_data_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/data_module/cpc_data_module.py` & `pytorch-lifestream-0.6.0/ptls/data_load/data_module/cpc_data_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/data_module/cpc_v2_data_module.py` & `pytorch-lifestream-0.6.0/ptls/data_load/data_module/cpc_v2_data_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/data_module/emb_data_module.py` & `pytorch-lifestream-0.6.0/ptls/data_load/data_module/emb_data_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/data_module/emb_valid_data_module.py` & `pytorch-lifestream-0.6.0/ptls/data_load/data_module/emb_valid_data_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/data_module/map_augmentation_dataset.py` & `pytorch-lifestream-0.6.0/ptls/data_load/data_module/map_augmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/data_module/nsp_data_module.py` & `pytorch-lifestream-0.6.0/ptls/data_load/data_module/nsp_data_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/data_module/rtd_data_module.py` & `pytorch-lifestream-0.6.0/ptls/data_load/data_module/rtd_data_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/data_module/seq_to_target_data_module.py` & `pytorch-lifestream-0.6.0/ptls/data_load/data_module/seq_to_target_data_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/data_module/sop_data_module.py` & `pytorch-lifestream-0.6.0/ptls/data_load/data_module/sop_data_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/datasets/augmentation_dataset.py` & `pytorch-lifestream-0.6.0/ptls/data_load/datasets/augmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/datasets/dataloaders.py` & `pytorch-lifestream-0.6.0/ptls/data_load/datasets/dataloaders.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/datasets/duckdb_dataset.py` & `pytorch-lifestream-0.6.0/ptls/data_load/datasets/duckdb_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
         field_names = [self.col_id] + event_fields
         
         query = f"""
             SELECT {self.col_id}, {fields}
             FROM {self.data_read_func}
             GROUP BY {self.col_id}
+            ORDER BY {self.col_id}
             """
     
         rel = duckdb.sql(query)
 
         while(True):
             recs = rel.fetchmany(1000)
             if not recs:
```

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/datasets/memory_dataset.py` & `pytorch-lifestream-0.6.0/ptls/data_load/datasets/memory_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/datasets/parquet_file_scan.py` & `pytorch-lifestream-0.6.0/ptls/data_load/datasets/parquet_file_scan.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/fast_tensor_data_loader.py` & `pytorch-lifestream-0.6.0/ptls/data_load/fast_tensor_data_loader.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/feature_dict.py` & `pytorch-lifestream-0.6.0/ptls/data_load/feature_dict.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/filter_dataset.py` & `pytorch-lifestream-0.6.0/ptls/data_load/filter_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/__init__.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/category_size_clip.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/category_size_clip.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/feature_bin_scaler.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/feature_bin_scaler.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/feature_filter.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/feature_filter.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/filter_non_array.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/filter_non_array.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/id_filter.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/id_filter.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/id_filter_df.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/id_filter_df.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/iterable_shuffle.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/iterable_shuffle.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/seq_len_filter.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/seq_len_filter.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/take_first_trx.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/take_first_trx.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/target_empty_filter.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/target_empty_filter.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/target_extractor.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/target_extractor.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/target_join.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/target_join.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/target_move.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/target_move.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing/to_torch_tensor.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing/to_torch_tensor.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/iterable_processing_dataset.py` & `pytorch-lifestream-0.6.0/ptls/data_load/iterable_processing_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/list_splitter.py` & `pytorch-lifestream-0.6.0/ptls/data_load/list_splitter.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/padded_batch.py` & `pytorch-lifestream-0.6.0/ptls/data_load/padded_batch.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/partitioned_dataset.py` & `pytorch-lifestream-0.6.0/ptls/data_load/partitioned_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/data_load/utils.py` & `pytorch-lifestream-0.6.0/ptls/data_load/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,21 +31,23 @@
             lambda a, b: ((a[1] is not None and a[1] == b or a[1] is None) and a[0], b),
             map(len, new_x_.values()), (True, None))[0]
 
     seq_col = next(k for k, v in batch[0].items() if FeatureDict.is_seq_feature(k, v))
     lengths = torch.LongTensor([len(rec[seq_col]) for rec in batch])
     new_x = {}
     for k, v in new_x_.items():
-        if type(v[0]) is torch.Tensor:
+        if isinstance(v[0], torch.Tensor):
             if k.startswith('target'):
                 new_x[k] = torch.stack(v, dim=0)
             else:
                 new_x[k] = torch.nn.utils.rnn.pad_sequence(v, batch_first=True)
-        elif type(v[0]) is np.ndarray:
+        elif isinstance(v[0], np.ndarray):
             new_x[k] = v  # list of arrays[object]
+        elif isinstance(v[0], list):
+            new_x[k] = np.array(v, dtype=object)
         else:
             v = np.array(v)
             if v.dtype.kind == 'i':
                 new_x[k] = torch.from_numpy(v).long()
             elif v.dtype.kind == 'f':
                 new_x[k] = torch.from_numpy(v).float()
             elif v.dtype.kind == 'b':
```

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/abs_module.py` & `pytorch-lifestream-0.6.0/ptls/frames/abs_module.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             raise AssertionError('batch is not a tuple')
         return loss
 
     def validation_step(self, batch, _):
         y_h, y = self.shared_step(*batch)
         self._validation_metric(y_h, y)
 
-    def validation_epoch_end(self, outputs):
+    def on_validation_epoch_end(self):
         self.log(f'valid/{self.metric_name}', self._validation_metric.compute(), prog_bar=True)
         self._validation_metric.reset()
 
     def configure_optimizers(self):
         optimizer = self._optimizer_partial(self.parameters())
         scheduler = self._lr_scheduler_partial(optimizer)
```

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/bert/__init__.py` & `pytorch-lifestream-0.6.0/ptls/frames/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/bert/datasets/mlm_dataset.py` & `pytorch-lifestream-0.6.0/ptls/frames/bert/datasets/mlm_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/bert/datasets/mlm_indexed_dataset.py` & `pytorch-lifestream-0.6.0/ptls/frames/bert/datasets/mlm_indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/bert/datasets/nsp_dataset.py` & `pytorch-lifestream-0.6.0/ptls/frames/bert/datasets/nsp_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/bert/datasets/rtd_dataset.py` & `pytorch-lifestream-0.6.0/ptls/frames/bert/datasets/rtd_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/bert/datasets/sop_dataset.py` & `pytorch-lifestream-0.6.0/ptls/frames/bert/datasets/sop_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/bert/losses/query_soft_max.py` & `pytorch-lifestream-0.6.0/ptls/frames/bert/losses/query_soft_max.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/bert/modules/mlm_module.py` & `pytorch-lifestream-0.6.0/ptls/frames/bert/modules/mlm_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,14 @@
 
     def validation_step(self, batch, batch_idx):
         x_trx = batch
         z_trx = self.trx_encoder(x_trx)  # PB: B, T, H
         loss_mlm = self.loss_mlm(z_trx, is_train_step=False)
         self.valid_mlm_loss(loss_mlm)
 
-    def training_epoch_end(self, _):
+    def on_training_epoch_end(self):
         self.log(f'mlm/train_mlm_loss', self.train_mlm_loss, prog_bar=False)
         # self.train_mlm_loss reset not required here
 
-    def validation_epoch_end(self, _):
+    def on_validation_epoch_end(self):
         self.log(f'mlm/valid_mlm_loss', self.valid_mlm_loss, prog_bar=True)
         # self.valid_mlm_loss reset not required here
```

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/bert/modules/mlm_nsp_module.py` & `pytorch-lifestream-0.6.0/ptls/frames/bert/modules/mlm_nsp_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,19 +221,19 @@
     def validation_step(self, batch, batch_idx):
         x_trx, y = batch
         z_trx = self.trx_encoder(x_trx)  # PB: B, T, H
         loss_mlm, loss_nsp = self.loss(z_trx, y, is_train_step=False)
         self.valid_nsp_loss(loss_nsp)
         self.valid_mlm_loss(loss_mlm)
 
-    def training_epoch_end(self, _):
+    def on_training_epoch_end(self):
         self.log(f'mlm/train_mlm_loss', self.train_mlm_loss, prog_bar=False)
         self.log(f'nsp/train_nsp_loss', self.train_nsp_loss, prog_bar=False)
 
-    def validation_epoch_end(self, _):
+    def on_validation_epoch_end(self):
         self.log(f'mlm/valid_mlm_loss', self.valid_mlm_loss, prog_bar=True)
         self.log(f'nsp/valid_nsp_loss', self.valid_nsp_loss, prog_bar=False)
    
     @property
     def seq_encoder(self):
         return MLMNSPInferenceModule(pretrained_model=self)
```

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/bert/modules/rtd_module.py` & `pytorch-lifestream-0.6.0/ptls/frames/bert/modules/rtd_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/bert/modules/sop_nsp_module.py` & `pytorch-lifestream-0.6.0/ptls/frames/bert/modules/sop_nsp_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/coles_dataset.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/coles_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/coles_dataset_time.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/coles_dataset_time.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/coles_module.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/coles_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/coles_supervised_dataset.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/coles_supervised_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/coles_supervised_module.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/coles_supervised_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,10 +120,10 @@
         return self.contrastive_loss_w * loss + self.supervised_loss_w * l_loss
         # return self.supervised_loss_w * l_loss
 
     def validation_step(self, batch, _):
         y_h, y, l = self.shared_step(*batch)
         self._validation_metric(y_h, y)
 
-    def validation_epoch_end(self, outputs):
+    def on_validation_epoch_end(self):
         self.log(f'valid/{self.metric_name}', self._validation_metric.compute(), prog_bar=True)
         self._validation_metric.reset()
```

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/losses/barlow_twins_loss.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/losses/barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/losses/binomial_deviance_loss.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/losses/binomial_deviance_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/losses/centroid_loss.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/losses/centroid_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/losses/complex_loss.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/losses/complex_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/losses/histogram_loss.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/losses/histogram_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/losses/margin_loss.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/losses/margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/losses/softmax_loss.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/losses/softmax_loss.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 import torch
+import torch.distributed as dist
 
+from ptls.frames.coles.losses.dist_utils import all_gather_and_cat
 
 class SoftmaxLoss(torch.nn.Module):
     """Also known as NCE loss
     All positive pairs as `anchor`-`pos_sample` concated with all possible `neg_samples` from batch.
     Softmax is applied ower `distances` between `anchor` ans pos or neg samples.
     `distances` is a dot product.
     Loss minimize `-log()` for `anchor-pos` position.
     
     Params:
         temperature:
             `softmax(distances / temperature)` - scale a sub-exponent expression.
             default 0.05 value is for l2-normalized `embeddings` where dot product distance is in range [-1, 1]
     """
-    def __init__(self, temperature=0.05):
+    def __init__(self, temperature=0.05, distributed_mode = False):
         super().__init__()
         
         self.temperature = temperature
+        self.distributed_mode = distributed_mode
         
     def forward(self, embeddings, classes):
+        if dist.is_initialized() and self.distributed_mode:
+            dist.barrier()
+            embeddings = all_gather_and_cat(embeddings)
+            classes = classes + (classes.max()+1) * dist.get_rank()
+            classes = all_gather_and_cat(classes)
         d = torch.einsum('bh,kh->bk', embeddings, embeddings) / self.temperature
         
         ix_pos = classes.unsqueeze(1) == classes.unsqueeze(0)
         ix_pos.fill_diagonal_(0)
         ix_a, ix_pos = ix_pos.nonzero(as_tuple=True)
         
         _, ix_neg = (classes[ix_a].unsqueeze(1) != classes.unsqueeze(0)).nonzero(as_tuple=True)
```

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/losses/triplet_loss.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/losses/triplet_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/losses/vicreg_loss.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/losses/vicreg_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/metric.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/all_positive_pair_selector.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/all_positive_pair_selector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/all_triplets_selector.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/all_triplets_selector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/distance_weighted_pair_selector.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/distance_weighted_pair_selector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/hard_negative_pair_selector.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/hard_negative_pair_selector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/hard_triplet_selector.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/hard_triplet_selector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/random_negative_triplet_selector.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/random_negative_triplet_selector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/sampling_strategies/semi_hard_triplet_selector.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/sampling_strategies/semi_hard_triplet_selector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/coles/split_strategy.py` & `pytorch-lifestream-0.6.0/ptls/frames/coles/split_strategy.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/cpc/datasets/cpc_dataset.py` & `pytorch-lifestream-0.6.0/ptls/frames/cpc/datasets/cpc_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/cpc/datasets/cpc_v2_dataset.py` & `pytorch-lifestream-0.6.0/ptls/frames/cpc/datasets/cpc_v2_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/cpc/losses/cpc_loss.py` & `pytorch-lifestream-0.6.0/ptls/frames/cpc/losses/cpc_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/cpc/modules/cpc_module.py` & `pytorch-lifestream-0.6.0/ptls/frames/cpc/modules/cpc_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/cpc/modules/cpc_v2_module.py` & `pytorch-lifestream-0.6.0/ptls/frames/cpc/modules/cpc_v2_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/gpt/gpt_module.py` & `pytorch-lifestream-0.6.0/ptls/frames/gpt/gpt_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,19 +127,19 @@
         out = self.forward(batch)  # PB: B, T, H
         out = out.payload if isinstance(out, PaddedBatch) else out
         labels = batch.payload
 
         loss_gpt = self.loss_gpt(out, labels, is_train_step=False)
         self.valid_gpt_loss(loss_gpt)
 
-    def training_epoch_end(self, _):
+    def on_training_epoch_end(self):
         self.log(f'gpt/train_gpt_loss', self.train_gpt_loss, prog_bar=False, sync_dist=True, rank_zero_only=True)
         # self.train_gpt_loss reset not required here
 
-    def validation_epoch_end(self, _):
+    def on_validation_epoch_end(self):
         self.log(f'gpt/valid_gpt_loss', self.valid_gpt_loss, prog_bar=True, sync_dist=True, rank_zero_only=True)
         # self.valid_gpt_loss reset not required here
 
     def configure_optimizers(self):
         optim = torch.optim.NAdam(self.parameters(),
                                  lr=self.hparams.max_lr,
                                  weight_decay=self.hparams.weight_decay,
@@ -185,8 +185,8 @@
             out = self.stat_pooler(out)
         elif self.model.hparams.inference_pooling_strategy=='out':
             out = self.last_step(out)
         else:
             raise
         if self.model.hparams.norm_predict:
             out = out / (out.pow(2).sum(dim=-1, keepdim=True) + 1e-9).pow(0.5)
-        return out
+        return out
```

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/ptls_data_module.py` & `pytorch-lifestream-0.6.0/ptls/frames/ptls_data_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/supervised/metrics.py` & `pytorch-lifestream-0.6.0/ptls/frames/supervised/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,19 @@
     def compute(self):
         y1, y = torch.cat(self.y1).float().cpu(), torch.cat(self.y).float().cpu()
         q = torch.linspace(0, 1, self.n_buckets + 1).float().cpu()[1:]
         b1 = torch.quantile(y1, q, interpolation="nearest")
         b = torch.quantile(y, q, interpolation="nearest")
         y1 = torch.bucketize(y1, b1, out_int32=True)
         y = torch.bucketize(y, b, out_int32=True)
-        return torchmetrics.functional.accuracy(y1, y)
+        num_classes = y.max().item() + 1
+        if hasattr(torchmetrics.functional.classification, "multiclass_accuracy"):
+            return torchmetrics.functional.classification.multiclass_accuracy(y1, y, num_classes=num_classes)
+        else:
+            return torchmetrics.functional.classification.accuracy(y1, y, num_classes=num_classes)
 
 
 class JSDiv(torchmetrics.Metric):
     """
     Jensen-Shannon divergence for distribution-like target:
         0 <= JSD(P||Q) = H(P/2 + Q/2) - H(P)/2 - H(Q)/2 <= ln(2)
     """
```

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/supervised/seq_to_target.py` & `pytorch-lifestream-0.6.0/ptls/frames/supervised/seq_to_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,40 +123,40 @@
         train_update_n_steps = self.hparams.train_update_n_steps
         if train_update_n_steps is None or \
                 train_update_n_steps is not None and self.global_step % train_update_n_steps == 0:
             for name, mf in self.train_metrics.items():
                 mf(y_h, y)
         return loss
 
-    def training_epoch_end(self, outputs):
+    def on_training_epoch_end(self):
         for name, mf in self.train_metrics.items():
             self.log(f'train/{name}', mf.compute(), prog_bar=False)
         for name, mf in self.train_metrics.items():
             mf.reset()
 
     def validation_step(self, batch, _):
         x, y = batch
         y_h = self(x)
         self.log('val_loss', self.loss(y_h, y))
         for name, mf in self.valid_metrics.items():
             mf(y_h, y)
 
-    def validation_epoch_end(self, outputs):
+    def on_validation_epoch_end(self):
         for name, mf in self.valid_metrics.items():
             self.log(f'valid/{name}', mf.compute(), prog_bar=True)
         for name, mf in self.valid_metrics.items():
             mf.reset()
 
     def test_step(self, batch, _):
         x, y = batch
         y_h = self(x)
         for name, mf in self.test_metrics.items():
             mf(y_h, y)
 
-    def test_epoch_end(self, outputs):
+    def on_test_epoch_end(self):
         for name, mf in self.test_metrics.items():
             value = mf.compute().item()
             self.log(f'test/{name}', value, prog_bar=False)
         for name, mf in self.test_metrics.items():
             mf.reset()
 
     def predict_step(self, batch, batch_idx, dataloader_idx=0):
```

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/supervised/seq_to_target_dataset.py` & `pytorch-lifestream-0.6.0/ptls/frames/supervised/seq_to_target_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/frames/tabformer/tabformer_module.py` & `pytorch-lifestream-0.6.0/ptls/frames/tabformer/tabformer_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
     def forward(self, z: PaddedBatch):
         out = self._seq_encoder(z)
         if self.hparams.norm_predict:
             out = self.fn_norm_predict(out)
         return out
 
-    def get_masks_and_labels(self, batch: PaddedBatch) -> Tuple(torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor):
+    def get_masks_and_labels(self, batch: PaddedBatch) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
         feature_tensors, random_words = [], []
         for field_name, noisy_emb_module in self.trx_encoder.embeddings.items():
             feature_tensors += [batch.payload[field_name].unsqueeze(0)]
             random_words += [noisy_emb_module(torch.randint(1, noisy_emb_module.num_embeddings, batch.seq_len_mask.shape, dtype=torch.long).to(batch.device)).unsqueeze(0)]
         feature_tensors = torch.cat(feature_tensors)
         random_words = torch.cat(random_words).permute(1, 2, 0, 3)
         pad_mask_tensors = batch.seq_len_mask.unsqueeze(0).repeat((feature_tensors.shape[0], 1, 1))
@@ -202,19 +202,19 @@
         payload = self.feature_encoder(payload)
 
         z_trx._payload = payload
 
         loss_tabformer = self.loss_tabformer(z_trx, tabf_labels, is_train_step=False)
         self.valid_tabformer_loss(loss_tabformer)
 
-    def training_epoch_end(self, _):
+    def on_training_epoch_end(self):
         self.log(f'tabformer/train_tabformer_loss', self.train_tabformer_loss, prog_bar=False)
         # self.train_tabformer_loss reset not required here
 
-    def validation_epoch_end(self, _):
+    def on_validation_epoch_end(self):
         self.log(f'tabformer/valid_tabformer_loss', self.valid_tabformer_loss, prog_bar=True)
         # self.valid_tabformer_loss reset not required here
 
     @property
     def seq_encoder(self):
         return TabformerInferenceModule(pretrained_model=self)
```

### Comparing `pytorch-lifestream-0.5.3/ptls/loss.py` & `pytorch-lifestream-0.6.0/ptls/loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/make_datasets.py` & `pytorch-lifestream-0.6.0/ptls/make_datasets.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/make_datasets_spark.py` & `pytorch-lifestream-0.6.0/ptls/make_datasets_spark.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,28 +188,28 @@
             Window.partitionBy(col_client_id).orderBy(F.col('event_time').desc())))
         df = df.filter(F.col('_rn') <= max_trx_count)
         df = df.drop('_cn')
         df = df.drop('_rn')
         return df
 
     def collect_lists(self, df, col_id):
-        col_list = [col for col in df.columns if col != col_id]
+        col_list = ['event_time'] + [col for col in df.columns if col != col_id and col != 'event_time']
+        unpack_col_list = [col_id] + [F.col(f'_struct.{col}').alias(col) for col in col_list]
 
         if self.config.save_partitioned_data:
             df = df.withColumn('mon_id', (F.col('event_time') / 30).cast('int'))
             col_id = [col_id, 'mon_id']
+            unpack_col_list.append('mon_id')
 
-        df = df \
-            .withColumn('trx_count', F.count(F.lit(1)).over(Window.partitionBy(col_id))) \
-            .withColumn('_rn', F.row_number().over(Window.partitionBy(col_id).orderBy('event_time')))
-
-        for col in col_list:
-            df = df.withColumn(col, F.collect_list(col).over(Window.partitionBy(col_id).orderBy('_rn'))) \
-
-        df = df.filter('_rn = trx_count').drop('_rn')
+        # Put columns into structs and collect structs.
+        df = df.groupBy(col_id).agg(F.sort_array(F.collect_list(F.struct(*col_list))).alias('_struct'))
+        # Unpack structs.
+        df = df.select(*unpack_col_list).drop('_struct').persist()
+        # Get counts.
+        df = df.withColumn('trx_count', F.size(F.col('event_time')).cast('long'))
         return df
 
     def join_dict(self, df, df_dict_name, col_id):
         path = self.path_to_file(df_dict_name)
         df_dict = self.spark_read_file(path)
         df = df.join(df_dict, on=col_id, how='left')
```

### Comparing `pytorch-lifestream-0.5.3/ptls/metric_learn/dataset/__init__.py` & `pytorch-lifestream-0.6.0/ptls/metric_learn/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/metric_learn/dataset/complex_target_dataset.py` & `pytorch-lifestream-0.6.0/ptls/metric_learn/dataset/complex_target_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/metric_learn/dataset/splitting_dataset.py` & `pytorch-lifestream-0.6.0/ptls/metric_learn/dataset/splitting_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/metric_learn/ml_models.py` & `pytorch-lifestream-0.6.0/ptls/metric_learn/ml_models.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/metric_learn/read_processing.py` & `pytorch-lifestream-0.6.0/ptls/metric_learn/read_processing.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/models.py` & `pytorch-lifestream-0.6.0/ptls/models.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/__init__.py` & `pytorch-lifestream-0.6.0/ptls/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/binarization.py` & `pytorch-lifestream-0.6.0/ptls/nn/binarization.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/head.py` & `pytorch-lifestream-0.6.0/ptls/nn/head.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/pb.py` & `pytorch-lifestream-0.6.0/ptls/nn/pb.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/__init__.py` & `pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/agg_feature_seq_encoder.py` & `pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/agg_feature_seq_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/containers.py` & `pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/containers.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/custom_encoder.py` & `pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/custom_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/gpt_encoder.py` & `pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/gpt_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/longformer_encoder.py` & `pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/longformer_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/rnn_encoder.py` & `pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/rnn_seq_encoder_distribution_target.py` & `pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/rnn_seq_encoder_distribution_target.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/statistics_encoder.py` & `pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/statistics_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/transformer_encoder.py` & `pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/seq_encoder/utils.py` & `pytorch-lifestream-0.6.0/ptls/nn/seq_encoder/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/seq_step.py` & `pytorch-lifestream-0.6.0/ptls/nn/seq_step.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/batch_norm.py` & `pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/batch_norm.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/encoders.py` & `pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/encoders.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/float_positional_encoding.py` & `pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/float_positional_encoding.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/noisy_embedding.py` & `pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/noisy_embedding.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/scalers.py` & `pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/scalers.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/tabformer_feature_encoder.py` & `pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/tabformer_feature_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/trx_encoder.py` & `pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/trx_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/trx_encoder_base.py` & `pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/trx_encoder_base.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/trx_encoder_ohe.py` & `pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/trx_encoder_ohe.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/nn/trx_encoder/trx_mean_encoder.py` & `pytorch-lifestream-0.6.0/ptls/nn/trx_encoder/trx_mean_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/pl_fit_target.py` & `pytorch-lifestream-0.6.0/ptls/pl_fit_target.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/pl_inference.py` & `pytorch-lifestream-0.6.0/ptls/pl_inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,17 +56,29 @@
         dataset=dataset_inference,
         collate_fn=collate_feature_dict,
         shuffle=False,
         num_workers=conf.inference.get('num_workers', 0),
         batch_size=conf.inference.get('batch_size', 128),
     )
 
-    gpus = 1 if torch.cuda.is_available() else 0
-    gpus = conf.inference.get('gpus', gpus)
-    df_scores = pl.Trainer(gpus=gpus, max_epochs=-1).predict(model, inference_dl)
+    if torch.cuda.is_available():
+        accelerator = "cuda"
+        devices = 1
+    else:
+        accelerator = "cpu"
+        devices = 0
+    user_defined_gpus = conf.inference.get("devices", conf.inference.get("gpus", None))
+    if user_defined_gpus is not None:
+        if user_defined_gpus:
+            accelerator = "gpu"
+            devices = user_defined_gpus
+        else:
+            accelerator = "cpu"
+            devices = 0
+    df_scores = pl.Trainer(accelerator=accelerator, devices=devices, max_epochs=-1).predict(model, inference_dl)
     df_scores = pd.concat(df_scores, axis=0)
     logger.info(f'df_scores examples: {df_scores.shape}:')
 
     save_scores(df_scores, conf.inference.output)
 
 
 if __name__ == '__main__':
```

### Comparing `pytorch-lifestream-0.5.3/ptls/pl_inference_spark.py` & `pytorch-lifestream-0.6.0/ptls/pl_inference_spark.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/pl_train_module.py` & `pytorch-lifestream-0.6.0/ptls/pl_train_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     dm = hydra.utils.instantiate(conf.data_module)
 
     _trainer_params = conf.trainer
     _trainer_params_additional = {}
     _use_best_epoch = _trainer_params.get('use_best_epoch', False)
 
     if 'callbacks' in _trainer_params:
-        logger.warning(f'Overwrite `trainer.callbacks`, was "{_trainer_params.checkpoint_callback}"')
+        logger.warning(f'Overwrite `trainer.callbacks`, was `{_trainer_params.get("enable_checkpointing", _trainer_params.get("checkpoint_callback", None))}`')
     _trainer_params_callbacks = []
 
     if _use_best_epoch:
         checkpoint_callback = ModelCheckpoint(monitor=model.metric_name, mode='max')
         logger.info(f'Create ModelCheckpoint callback with monitor="{model.metric_name}"')
         _trainer_params_callbacks.append(checkpoint_callback)
 
@@ -45,14 +45,17 @@
         del _trainer_params.checkpoints_every_n_val_epochs
 
     if 'logger_name' in conf:
         _trainer_params_additional['logger'] = TensorBoardLogger(
             save_dir='lightning_logs',
             name=conf.get('logger_name'),
         )
+    if not isinstance(_trainer_params.get('strategy', ''), str): # if strategy not exist or str do nothing, 
+        _trainer_params_additional['strategy'] = hydra.utils.instantiate(_trainer_params.strategy)
+        del _trainer_params.strategy
 
     lr_monitor = LearningRateMonitor(logging_interval='step')
     _trainer_params_callbacks.append(lr_monitor)
 
     if len(_trainer_params_callbacks) > 0:
         _trainer_params_additional['callbacks'] = _trainer_params_callbacks
     trainer = pl.Trainer(**_trainer_params, **_trainer_params_additional)
```

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/base/col_transformer.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/base/col_transformer.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/base/data_preprocessor.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/base/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/category_identity_encoder.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/category_identity_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/col_identity_transformer.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/col_identity_transformer.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/col_transformer.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/col_transformer.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/event_time.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/event_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 
 from ptls.preprocessing.base import ColTransformer
 from ptls.preprocessing.pandas.col_transformer import ColTransformerPandasMixin
 
 
 def dt_to_timestamp(x: pd.Series):
-    return pd.to_datetime(x).astype('datetime64[s]').astype('int64') // 1000000000
+    return pd.to_datetime(x).astype('datetime64[ns]').astype('int64') // 1000000000
 
 
 def timestamp_to_dt(x: pd.Series):
     return pd.to_datetime(x, unit='s')
 
 
 class DatetimeToTimestamp(ColTransformerPandasMixin, ColTransformer):
```

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/frequency_encoder.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/frequency_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pandas/user_group_transformer.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pandas/user_group_transformer.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pandas_preprocessor.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pandas_preprocessor.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/category_identity_encoder.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/category_identity_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/col_identity_transformer.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/col_identity_transformer.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/col_transformer.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/col_transformer.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/event_time.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/event_time.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark/frequency_encoder.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark/frequency_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/pyspark_preprocessor.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/pyspark_preprocessor.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/preprocessing/util.py` & `pytorch-lifestream-0.6.0/ptls/preprocessing/util.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/size_reduction.py` & `pytorch-lifestream-0.6.0/ptls/size_reduction.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/swa.py` & `pytorch-lifestream-0.6.0/ptls/swa.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/tb_interface.py` & `pytorch-lifestream-0.6.0/ptls/tb_interface.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls/util.py` & `pytorch-lifestream-0.6.0/ptls/util.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/metric_learning_tests/test_collate.py` & `pytorch-lifestream-0.6.0/ptls_tests/metric_learning_tests/test_collate.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_custom_layers.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_custom_layers.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/__init__.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test__init__.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from ptls.data_load import padded_collate, ZeroDownSampler, DropoutTrxDataset, TrxDataset, LastKTrxDataset
 from ptls.data_load import augmentation_chain
 from ptls_tests.utils.data_generation import gen_trx_data
 
 
 def test_padded_collate():
     data = [
-        ({'a': torch.LongTensor([1, 2, 3, 4])}, torch.LongTensor([0])),
-        ({'a': torch.LongTensor([1, 2])},  torch.LongTensor([0])),
-        ({'a': torch.LongTensor([1])},  torch.LongTensor([1])),
+        ({'a': torch.tensor([1, 2, 3, 4])}, torch.tensor(0)),
+        ({'a': torch.tensor([1, 2])},  torch.tensor(0)),
+        ({'a': torch.tensor([1])},  torch.tensor(1)),
     ]
 
     tt = torch.LongTensor([
         [1, 2, 3, 4],
         [1, 2, 0, 0],
         [1, 0, 0, 0]])
```

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_augmentations/test_all_time_shuffle.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_augmentations/test_all_time_shuffle.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_augmentations/test_dropout_trx.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_augmentations/test_dropout_trx.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_augmentations/test_random_slice.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_augmentations/test_random_slice.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_augmentations/test_seq_len_limit.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_augmentations/test_seq_len_limit.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_duckdb.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_feature_dict.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_feature_dict.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_category_size_clip.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_category_size_clip.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_id_filter.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_id_filter.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_id_filter_df.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_id_filter_df.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_iterable_shuffle.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_iterable_shuffle.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_seq_len_filter.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_seq_len_filter.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_target_empty_filter.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_target_empty_filter.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_target_extractor.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_target_extractor.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_target_join.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_target_join.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_target_move.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_target_move.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_iterable_processing/test_to_torch.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_iterable_processing/test_to_torch.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_list_splitter.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_list_splitter.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_padded_batch.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_padded_batch.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_data_load/test_utils.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_data_load/test_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_distribution_target_loss.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_distribution_target_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_bert/test_datasets/test_mlm_dataset.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_bert/test_datasets/test_mlm_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_bert/test_mlm.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_bert/test_mlm.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/test_coles_module.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/test_coles_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,9 +55,9 @@
             **params['rnn'],
         ),
         head=Head(use_norm_encoder=True),
         optimizer_partial=partial(torch.optim.Adam),
         lr_scheduler_partial=partial(torch.optim.lr_scheduler.StepLR, step_size=1, gamma=1.0),
     )
     dl = RandomEventData(params['data_module'])
-    trainer = pl.Trainer(max_epochs=1, logger=None, checkpoint_callback=False)
+    trainer = pl.Trainer(max_epochs=1, logger=None, enable_checkpointing=False)
     trainer.fit(model, dl)
```

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/test_losses.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/test_losses.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/test_metrics.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/test_metrics.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/test_sampling_strategies/test_pair_selectors.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/test_sampling_strategies/test_pair_selectors.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_coles/test_sampling_strategies/test_triplet_selectors.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_coles/test_sampling_strategies/test_triplet_selectors.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_common_usage.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_common_usage.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_cpc.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_cpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,12 +67,12 @@
     test_data = gen_trx_data((torch.rand(100)*60+1).long())
     valid_ds = TrxDataset(test_data)
 
     train_loader = create_train_loader(train_ds, config['train'])
     valid_loader = create_validation_loader(valid_ds, config['valid'])
 
     trainer = pl.Trainer(
-        gpus=None,
+        accelerator="cpu",
         max_steps=50,
-        checkpoint_callback=False,
+        enable_checkpointing=False,
     )
     trainer.fit(pl_module, train_loader, valid_loader)
```

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_supervised/test_metrics.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_supervised/test_metrics.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_supervised/test_seq_to_target.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_supervised/test_seq_to_target.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,33 @@
 
 from ptls.frames.supervised import SequenceToTarget
 from ptls.loss import BCELoss
 from ptls.nn import PBLinear, RnnSeqEncoder, TransformerSeqEncoder, TrxEncoder
 from ptls_tests.test_data_load import RandomEventData
 
 
+def accuracy_metric(*args, **kwargs):
+    kwargs["task"] = kwargs.get("task", "multiclass")
+    try:
+        return torchmetrics.classification.Accuracy(*args, **kwargs)
+    except TypeError:
+        if kwargs.pop("task", None) == "binary":
+            kwargs["num_classes"] = 2
+        return torchmetrics.classification.Accuracy(*args, **kwargs)
+
+def auroc_metric(*args, **kwargs):
+    kwargs["task"] = kwargs.get("task", "multiclass")
+    try:
+        return torchmetrics.classification.AUROC(*args, **kwargs)
+    except TypeError:
+        if kwargs.pop("task", None) == "binary":
+            kwargs["num_classes"] = 2
+        return torchmetrics.classification.AUROC(*args, **kwargs)
+
+
 def get_rnn_params():
     return dict(
         seq_encoder=RnnSeqEncoder(
             trx_encoder=TrxEncoder(
                 norm_embeddings=False,
                 embeddings_noise=0.1,
                 embeddings={
@@ -79,54 +98,54 @@
     model = SequenceToTarget(
         head=torch.nn.Sequential(
             torch.nn.Linear(16, 1),
             torch.nn.Sigmoid(),
             torch.nn.Flatten(start_dim=0),
         ),
         loss=BCELoss(),
-        metric_list=torchmetrics.AUROC(num_classes=2),
+        metric_list=auroc_metric(task="binary"),
         **get_rnn_params(),
     )
     dl = RandomEventData(tst_params_data(), target_type='bin_cls')
-    trainer = pl.Trainer(max_epochs=1, logger=None, checkpoint_callback=False)
+    trainer = pl.Trainer(max_epochs=1, logger=None, enable_checkpointing=False)
     trainer.fit(model, dl)
     print(trainer.logged_metrics)
 
 
 def test_train_loop_rnn_milti_classification():
     model = SequenceToTarget(
         head=torch.nn.Sequential(
             torch.nn.Linear(16, 4),
             torch.nn.LogSoftmax(dim=1),
         ),
         loss=torch.nn.NLLLoss(),
         metric_list={
-            'auroc': torchmetrics.AUROC(num_classes=4),
-            'accuracy': torchmetrics.Accuracy(),
+            'auroc': auroc_metric(num_classes=4),
+            'accuracy': accuracy_metric(num_classes=4),
         },
         **get_rnn_params(),
     )
     dl = RandomEventData(tst_params_data(), target_type='multi_cls')
-    trainer = pl.Trainer(max_epochs=1, logger=None, checkpoint_callback=False)
+    trainer = pl.Trainer(max_epochs=1, logger=None, enable_checkpointing=False)
     trainer.fit(model, dl)
     print(trainer.logged_metrics)
 
 
 def test_train_loop_rnn_regression():
     model = SequenceToTarget(
         head=torch.nn.Sequential(
             torch.nn.Linear(16, 1),
             torch.nn.Flatten(start_dim=0),
         ),
         loss=torch.nn.MSELoss(),
-        metric_list=torchmetrics.MeanSquaredError(compute_on_step=False, squared=False),
+        metric_list=torchmetrics.MeanSquaredError(squared=False),
         **get_rnn_params(),
     )
     dl = RandomEventData(tst_params_data(), target_type='regression')
-    trainer = pl.Trainer(max_epochs=1, logger=None, checkpoint_callback=False)
+    trainer = pl.Trainer(max_epochs=1, logger=None, enable_checkpointing=False)
     trainer.fit(model, dl)
     print(trainer.logged_metrics)
 
 
 def test_train_loop_transf():
     trx_encoder = TrxEncoder(
         norm_embeddings=False,
@@ -147,59 +166,60 @@
         seq_encoder=seq_encoder,
         head=torch.nn.Sequential(
             torch.nn.Linear(seq_encoder.embedding_size, 1),
             torch.nn.Sigmoid(),
             torch.nn.Flatten(start_dim=0),
         ),
         loss=BCELoss(),
-        metric_list=torchmetrics.AUROC(num_classes=2),
+        metric_list=auroc_metric(task="binary"),
         optimizer_partial=partial(torch.optim.Adam, lr=0.004),
         lr_scheduler_partial=partial(torch.optim.lr_scheduler.StepLR, step_size=10, gamma=0.8),
     )
     dl = RandomEventData(tst_params_data())
-    trainer = pl.Trainer(max_epochs=1, logger=None, checkpoint_callback=False)
+    trainer = pl.Trainer(max_epochs=1, logger=None, enable_checkpointing=False)
     trainer.fit(model, dl)
 
 # SequenceToTarget.metric_list
 def test_seq_to_target_metric_list_single_metric():
-    model = SequenceToTarget(metric_list=torchmetrics.Accuracy(), seq_encoder=None)
+    model = SequenceToTarget(metric_list=accuracy_metric(num_classes=2), seq_encoder=None)
     metric_name = next(iter(model.valid_metrics.keys()))
-    assert metric_name == 'Accuracy'
+    assert metric_name in {'Accuracy', 'MulticlassAccuracy'}
 
 
 def test_seq_to_target_metric_list_list_with_metric():
     model = SequenceToTarget(metric_list=[
-        torchmetrics.Accuracy(),
-        torchmetrics.AUROC(num_classes=2),
+        accuracy_metric(num_classes=2),
+        auroc_metric(num_classes=2),
     ], seq_encoder=None)
-    assert 'Accuracy' in model.valid_metrics
-    assert 'AUROC' in model.valid_metrics
+    assert 'Accuracy' in model.valid_metrics or 'MulticlassAccuracy' in model.valid_metrics
+    assert 'AUROC' in model.valid_metrics or 'MulticlassAUROC' in model.valid_metrics
 
 
 def test_seq_to_target_metric_list_dict_with_single_metric():
     model = SequenceToTarget(metric_list={
-        'acc': torchmetrics.Accuracy(),
+        'acc': accuracy_metric(num_classes=2),
     }, seq_encoder=None)
     metric_name = next(iter(model.valid_metrics.keys()))
     assert metric_name == 'acc'
 
 
 def test_seq_to_target_metric_list_dict_with_metric():
     model = SequenceToTarget(metric_list={
-        'acc': torchmetrics.Accuracy(),
-        'auroc': torchmetrics.AUROC(num_classes=2),
+        'acc': accuracy_metric(num_classes=2),
+        'auroc': auroc_metric(num_classes=2),
     }, seq_encoder=None)
     assert 'acc' in model.valid_metrics
     assert 'auroc' in model.valid_metrics
 
 
 def test_seq_to_target_metric_list_dict_config_with_metric():
-    conf = omegaconf.OmegaConf.create("""
+    conf = omegaconf.OmegaConf.create(f"""
         auroc:
-            _target_: torchmetrics.AUROC
+            _target_: torchmetrics.classification.{'MulticlassAUROC' if hasattr(torchmetrics.classification, 'MulticlassAUROC') else 'AUROC'}
             num_classes: 2
         acc:
-            _target_: torchmetrics.Accuracy
+            _target_: torchmetrics.classification.{'MulticlassAccuracy' if hasattr(torchmetrics.classification, 'MulticlassAccuracy') else 'Accuracy'}
+            num_classes: 2
     """)
     model = SequenceToTarget(metric_list=hydra.utils.instantiate(conf), seq_encoder=None)
     assert 'acc' in model.valid_metrics
     assert 'auroc' in model.valid_metrics
```

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_frames/test_supervised/test_seq_to_target_dataset.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_frames/test_supervised/test_seq_to_target_dataset.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_head.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_head.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_pb.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_pb.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_agg_feature_seq_encoder.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_agg_feature_seq_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_containers.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_containers.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_longformer_encoder.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_longformer_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_rnn_encoder.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_rnn_seq_distribution_targets_encoder.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_rnn_seq_distribution_targets_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_statistics_encoder.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_statistics_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_transformer_encoder.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_encoder/test_utils.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_encoder/test_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_seq_step.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_seq_step.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/test_batch_norm.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/test_batch_norm.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/test_noisy_embedding.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/test_noisy_embedding.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/test_trx_encoder.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/test_trx_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/test_trx_encoder_base.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/test_trx_encoder_base.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/test_trx_mean_encoder.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/test_trx_mean_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_nn/test_trx_encoder/test_trx_ohe_encoder.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_nn/test_trx_encoder/test_trx_ohe_encoder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_pl_api.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_pl_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,16 @@
         seq_encoder=seq_encoder,
         optimizer_partial=partial(torch.optim.Adam),
         lr_scheduler_partial=partial(torch.optim.lr_scheduler.StepLR, step_size=1, gamma=1.0),
     )
 
     trainer = pl.Trainer(
         max_epochs=1,
-        gpus=0 if torch.cuda.is_available() else 0,
+        accelerator="cuda" if torch.cuda.is_available() else "cpu",
+        devices=1 if torch.cuda.is_available() else "auto",
         logger=False
     )
     trainer.fit(model, train_dl)
 
     test_dl = inference_data_loader(test, num_workers=0, batch_size=4)
 
     filtered_ds = MemoryMapDataset(test, [
```

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_pl_api_duckdb.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_pl_api_duckdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,24 +65,25 @@
         optimizer_partial=partial(torch.optim.Adam),
         lr_scheduler_partial=partial(torch.optim.lr_scheduler.StepLR, step_size=1, gamma=1.0),
         loss=ContrastiveLoss(margin=0.5, sampling_strategy=HardNegativePairSelector(2))
     )
 
     trainer = pl.Trainer(
         max_epochs=1,
-        gpus=0 if torch.cuda.is_available() else 0,
+        accelerator="cuda" if torch.cuda.is_available() else "cpu",
+        devices=1 if torch.cuda.is_available() else "auto",
         logger=False
     )
     trainer.fit(model, train_dl)
 
     test_data = f"""
         (SELECT * FROM read_csv_auto('{Path(__file__).parent / 'age-transactions.csv'}')
         WHERE hash(client_id) % 5 == 0)
         """
-    
+
     test_ds = DuckDbDataset(
         data_read_func = test_data,
         col_id = 'client_id',
         col_event_time = 'trans_date',
         col_event_fields = ['amount_rur', 'small_group'],
         i_filters=[
             FilterNonArray(),
```

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_ranking_loss.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_ranking_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/test_size_reduction.py` & `pytorch-lifestream-0.6.0/ptls_tests/test_size_reduction.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/ptls_tests/utils/data_generation.py` & `pytorch-lifestream-0.6.0/ptls_tests/utils/data_generation.py`

 * *Files identical despite different names*

### Comparing `pytorch-lifestream-0.5.3/pytorch_lifestream.egg-info/PKG-INFO` & `pytorch-lifestream-0.6.0/pytorch_lifestream.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: pytorch-lifestream
-Version: 0.5.3
+Version: 0.6.0
 Summary: Lifestream data analysis with PyTorch
 Author: 
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-`PyTorch-LifeStream` or PTLS a library built upon [PyTorch](https://pytorch.org/) for building embeddings on discrete event sequences using self-supervision. It can process terabyte-size volumes of raw events like game history events, clickstream data, purchase history or card transactions.
+![ptls-logo](ptls-banner.png)
+
+
+[![GitHub license](https://img.shields.io/github/license/dllllb/pytorch-lifestream.svg)](https://github.com/dllllb/pytorch-lifestream/blob/master/LICENSE)
+[![PyPI version](https://badge.fury.io/py/pytorch-lifestream.svg)](https://badge.fury.io/py/pytorch-lifestream)
+[![GitHub issues](https://img.shields.io/github/issues/dllllb/pytorch-lifestream.svg)](https://github.com/dllllb/pytorch-lifestream/issues)
+[![Telegram](https://img.shields.io/badge/chat-on%20Telegram-2ba2d9.svg)](https://t.me/pytorch_lifestream)
+
+`pytorch-lifestream` or ptls a library built upon [PyTorch](https://pytorch.org/) for building embeddings on discrete event sequences using self-supervision. It can process terabyte-size volumes of raw events like game history events, clickstream data, purchase history or card transactions.
 
 It supports various methods of self-supervised training, adapted for event sequences:
 
 - Contrastive Learning for Event Sequences ([CoLES](https://arxiv.org/abs/2002.08232))
 - Contrastive Predictive Coding ([CPC](https://arxiv.org/abs/1807.03748))
 - Replaced Token Detection (RTD) from [ELECTRA](https://arxiv.org/abs/2003.10555)
 - Next Sequence Prediction (NSP) from [BERT](https://arxiv.org/abs/1810.04805)
@@ -43,33 +51,34 @@
 
 ```sh
 # Ubuntu 20.04
 
 sudo apt install python3.8 python3-venv
 pip3 install pipenv
 
-pipenv sync  --dev # install packages exactly as specified in Pipfile.lock
+pipenv sync --dev # install packages exactly as specified in Pipfile.lock
 pipenv shell
 pytest
 
 ```
 
 ## Demo notebooks
 
 - Supervised model training [notebook](demo/supervised-sequence-to-target.ipynb)
 - Self-supervided training and embeddings for downstream task [notebook](demo/coles-emb.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dllllb/pytorch-lifestream/blob/master/demo/coles-emb.ipynb)
+- Self-supervided training and embeddings for clients' transactions [notebook](demo/transaction-emb.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dllllb/pytorch-lifestream/blob/master/demo/transaction-emb.ipynb)
 - Self-supervided embeddings in CatBoost [notebook](demo/coles-catboost.ipynb)
 - Self-supervided training and fine-tuning [notebook](demo/coles-finetune.ipynb)
 - Self-supervised TrxEncoder only training with Masked Language Model task and fine-tuning [notebook](demo/mlm-emb.ipynb)
 - Pandas data preprocessing options [notebook](demo/preprocessing-demo.ipynb)
 - PySpark and Parquet for data preprocessing [notebook](demo/pyspark-parquet.ipynb)
 - Fast inference on large dataset [notebook](demo/extended_inference.ipynb)
 - Supervised multilabel classification [notebook](demo/multilabel-classification.ipynb)
 - Text features demo:
-  - Using pretrained encoder to text features[notebook](demo/coles-pretrained-embeddings.ipynb)
+  - Using pretrained encoder to text features [notebook](demo/coles-pretrained-embeddings.ipynb)
 
 ## Docs
 
 [Documentation](https://dllllb.github.io/pytorch-lifestream/)
 
 Library description [index](docs/index.md)
 
@@ -86,7 +95,25 @@
 - [American Express - Default Prediction Kaggle contest report](https://habr.com/ru/articles/704440/) (in Russian)
 
 ## How to contribute
 
 1. Make your chages via Fork and Pull request.
 2. Write unit test for new code in `ptls_tests`.
 3. Check unit test via `pytest`: [Example](.#install-from-source).
+
+## Citation
+
+We have a [paper](https://arxiv.org/abs/2002.08232) you can cite it:
+```bibtex
+@inproceedings{
+   Babaev_2022, series={SIGMOD/PODS ’22},
+   title={CoLES: Contrastive Learning for Event Sequences with Self-Supervision},
+   url={http://dx.doi.org/10.1145/3514221.3526129},
+   DOI={10.1145/3514221.3526129},
+   booktitle={Proceedings of the 2022 International Conference on Management of Data},
+   publisher={ACM},
+   author={Babaev, Dmitrii and Ovsov, Nikita and Kireev, Ivan and Ivanova, Maria and Gusev, Gleb and Nazarov, Ivan and Tuzhilin, Alexander},
+   year={2022},
+   month=jun, collection={SIGMOD/PODS ’22}
+}
+
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytorch-lifestream-0.5.3/pytorch_lifestream.egg-info/SOURCES.txt` & `pytorch-lifestream-0.6.0/pytorch_lifestream.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ptls/custom_layers.py
 ptls/loss.py
 ptls/make_datasets.py
 ptls/make_datasets_spark.py
 ptls/models.py
 ptls/pl_fit_target.py
 ptls/pl_inference.py
+ptls/pl_inference_multimodal.py
 ptls/pl_inference_spark.py
 ptls/pl_train_module.py
 ptls/size_reduction.py
 ptls/swa.py
 ptls/tb_interface.py
 ptls/util.py
 ptls/data_load/__init__.py
@@ -50,15 +51,17 @@
 ptls/data_load/datasets/dataloaders.py
 ptls/data_load/datasets/duckdb_dataset.py
 ptls/data_load/datasets/memory_dataset.py
 ptls/data_load/datasets/parquet_dataset.py
 ptls/data_load/datasets/parquet_file_scan.py
 ptls/data_load/datasets/persist_dataset.py
 ptls/data_load/iterable_processing/__init__.py
+ptls/data_load/iterable_processing/add_modal_name.py
 ptls/data_load/iterable_processing/category_size_clip.py
+ptls/data_load/iterable_processing/delete_nan.py
 ptls/data_load/iterable_processing/feature_bin_scaler.py
 ptls/data_load/iterable_processing/feature_filter.py
 ptls/data_load/iterable_processing/feature_rename.py
 ptls/data_load/iterable_processing/feature_type_cast.py
 ptls/data_load/iterable_processing/filter_non_array.py
 ptls/data_load/iterable_processing/id_filter.py
 ptls/data_load/iterable_processing/id_filter_df.py
@@ -66,14 +69,15 @@
 ptls/data_load/iterable_processing/iterable_shuffle.py
 ptls/data_load/iterable_processing/seq_len_filter.py
 ptls/data_load/iterable_processing/take_first_trx.py
 ptls/data_load/iterable_processing/target_empty_filter.py
 ptls/data_load/iterable_processing/target_extractor.py
 ptls/data_load/iterable_processing/target_join.py
 ptls/data_load/iterable_processing/target_move.py
+ptls/data_load/iterable_processing/time_proc.py
 ptls/data_load/iterable_processing/to_torch_tensor.py
 ptls/frames/__init__.py
 ptls/frames/abs_module.py
 ptls/frames/inference_module.py
 ptls/frames/ptls_data_module.py
 ptls/frames/bert/__init__.py
 ptls/frames/bert/datasets/__init__.py
@@ -92,21 +96,26 @@
 ptls/frames/coles/__init__.py
 ptls/frames/coles/coles_dataset.py
 ptls/frames/coles/coles_dataset_time.py
 ptls/frames/coles/coles_module.py
 ptls/frames/coles/coles_supervised_dataset.py
 ptls/frames/coles/coles_supervised_module.py
 ptls/frames/coles/metric.py
+ptls/frames/coles/multimodal_dataset.py
+ptls/frames/coles/multimodal_inference_dataset.py
+ptls/frames/coles/multimodal_module.py
+ptls/frames/coles/multimodal_supervised_dataset.py
 ptls/frames/coles/split_strategy.py
 ptls/frames/coles/losses/__init__.py
 ptls/frames/coles/losses/barlow_twins_loss.py
 ptls/frames/coles/losses/binomial_deviance_loss.py
 ptls/frames/coles/losses/centroid_loss.py
 ptls/frames/coles/losses/complex_loss.py
 ptls/frames/coles/losses/contrastive_loss.py
+ptls/frames/coles/losses/dist_utils.py
 ptls/frames/coles/losses/histogram_loss.py
 ptls/frames/coles/losses/margin_loss.py
 ptls/frames/coles/losses/softmax_loss.py
 ptls/frames/coles/losses/triplet_loss.py
 ptls/frames/coles/losses/vicreg_loss.py
 ptls/frames/coles/sampling_strategies/__init__.py
 ptls/frames/coles/sampling_strategies/all_positive_pair_selector.py
@@ -199,14 +208,15 @@
 ptls/preprocessing/pyspark/frequency_encoder.py
 ptls/preprocessing/pyspark/user_group_transformer.py
 ptls_tests/__init__.py
 ptls_tests/test_custom_layers.py
 ptls_tests/test_distribution_target_loss.py
 ptls_tests/test_list_subset.py
 ptls_tests/test_loss.py
+ptls_tests/test_make_datasets_spark.py
 ptls_tests/test_pl_api.py
 ptls_tests/test_pl_api_duckdb.py
 ptls_tests/test_ranking_loss.py
 ptls_tests/test_size_reduction.py
 ptls_tests/metric_learning_tests/__init__.py
 ptls_tests/metric_learning_tests/test_collate.py
 ptls_tests/test_data_load/__init__.py
```

### Comparing `pytorch-lifestream-0.5.3/setup.py` & `pytorch-lifestream-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,28 +3,34 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='pytorch-lifestream',
-    version='0.5.3',
+    version='0.6.0',
     author='',
     author_email='',
     description='Lifestream data analysis with PyTorch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
     install_requires=[
-        'pytorch-lightning==1.6.*',
-        'torch==1.12.*',
-        'numpy==1.23.*',
-        'torchmetrics==0.9.*',
+        'duckdb',
+        'hydra-core>=1.1.2',
+        'numpy>=1.21.5',
         'omegaconf',
+        'pandas>=1.3.5',
+        'pyarrow>=6.0.1',
+        'pytorch-lightning>=1.6.0',
+        'scikit-learn>=1.0.2',
+        'torch>=1.12.0',
+        'torchmetrics>=0.9.0',
+        'transformers',
     ],
 )
```

