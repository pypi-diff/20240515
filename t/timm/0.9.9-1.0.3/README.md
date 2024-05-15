# Comparing `tmp/timm-0.9.9.tar.gz` & `tmp/timm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timm-0.9.9.tar", last modified: Fri Nov  3 21:50:05 2023, max compression
+gzip compressed data, was "timm-1.0.3.tar", last modified: Wed May 15 18:10:46 2024, max compression
```

## Comparing `timm-0.9.9.tar` & `timm-1.0.3.tar`

### file list

```diff
@@ -1,284 +1,273 @@
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.908449 timm-0.9.9/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11343 2023-02-24 22:35:42.000000 timm-0.9.9/LICENSE
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       95 2023-03-31 00:49:24.000000 timm-0.9.9/MANIFEST.in
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    59684 2023-11-03 21:50:05.908449 timm-0.9.9/PKG-INFO
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    58566 2023-11-03 21:34:49.000000 timm-0.9.9/README.md
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      551 2023-03-31 00:49:24.000000 timm-0.9.9/pyproject.toml
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      126 2023-11-03 21:50:05.908449 timm-0.9.9/setup.cfg
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1935 2023-03-31 00:49:24.000000 timm-0.9.9/setup.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.888449 timm-0.9.9/timm/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      292 2023-03-31 00:49:24.000000 timm-0.9.9/timm/__init__.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.888449 timm-0.9.9/timm/data/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      819 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/__init__.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.892449 timm-0.9.9/timm/data/_info/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   118210 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet12k_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   218430 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet21k_goog_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    64070 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet21k_goog_to_12k_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   119937 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet21k_goog_to_22k_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   112210 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet21k_miil_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   104500 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet21k_miil_w21_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   218410 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet22k_ms_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    63625 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet22k_ms_to_12k_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   119938 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet22k_ms_to_22k_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   218410 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet22k_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    64070 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet22k_to_12k_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      774 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet_a_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2000 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet_a_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      769 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet_r_indices.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2000 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet_r_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   388478 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet_real_labels.json
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)  1748917 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet_synset_to_definition.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   741457 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet_synset_to_lemma.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10000 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/_info/imagenet_synsets.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    35550 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/auto_augment.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4531 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/config.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      442 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/constants.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5833 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/dataset.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6989 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/dataset_factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2391 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/dataset_info.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5540 2023-02-24 22:35:42.000000 timm-0.9.9/timm/data/distributed_sampler.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4167 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/imagenet_info.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11849 2023-04-28 20:49:14.000000 timm-0.9.9/timm/data/loader.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14634 2023-08-03 23:44:25.000000 timm-0.9.9/timm/data/mixup.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4964 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/random_erasing.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.892449 timm-0.9.9/timm/data/readers/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       72 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/readers/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      895 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/readers/class_map.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1482 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/readers/img_extensions.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      487 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/readers/reader.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1364 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/readers/reader_factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2431 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/readers/reader_hfds.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3315 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/readers/reader_image_folder.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9182 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/readers/reader_image_in_tar.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2644 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/readers/reader_image_tar.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17858 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/readers/reader_tfds.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    16724 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/readers/reader_wds.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      303 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/readers/shared_count.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1800 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/real_labels.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9169 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/tf_preprocessing.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11992 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/transforms.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9840 2023-03-31 00:49:24.000000 timm-0.9.9/timm/data/transforms_factory.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.896449 timm-0.9.9/timm/layers/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3827 2023-10-31 17:20:37.000000 timm-0.9.9/timm/layers/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4882 2023-11-03 18:13:21.000000 timm-0.9.9/timm/layers/activations.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2529 2023-11-02 20:50:57.000000 timm-0.9.9/timm/layers/activations_jit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5886 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/activations_me.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6309 2023-10-31 17:20:37.000000 timm-0.9.9/timm/layers/adaptive_avgmax_pool.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3458 2023-10-19 18:56:45.000000 timm-0.9.9/timm/layers/attention_pool.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4934 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/attention_pool2d.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1594 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/blur_pool.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6895 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/bottleneck_attn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4426 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/cbam.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7486 2023-04-28 20:49:14.000000 timm-0.9.9/timm/layers/classifier.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5199 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/cond_conv2d.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4175 2023-04-12 15:57:13.000000 timm-0.9.9/timm/layers/config.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3216 2023-04-28 20:49:14.000000 timm-0.9.9/timm/layers/conv2d_same.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3836 2023-04-28 20:49:14.000000 timm-0.9.9/timm/layers/conv_bn_act.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5416 2023-11-03 18:13:21.000000 timm-0.9.9/timm/layers/create_act.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3514 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/create_attn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1622 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/create_conv2d.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1568 2023-11-03 18:13:21.000000 timm-0.9.9/timm/layers/create_norm.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3836 2023-11-03 18:13:21.000000 timm-0.9.9/timm/layers/create_norm_act.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6872 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/drop.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6386 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/eca.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13862 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/evo_norm.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4008 2023-05-10 14:38:22.000000 timm-0.9.9/timm/layers/fast_norm.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2540 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/filter_response_norm.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1109 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/format.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3824 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/gather_excite.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2445 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/global_context.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1319 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/grn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10662 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/halo_attn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1053 2023-10-29 22:34:22.000000 timm-0.9.9/timm/layers/helpers.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3374 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/inplace_abn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2439 2023-08-20 18:50:19.000000 timm-0.9.9/timm/layers/interpolate.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5941 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/lambda_layer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      743 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/linear.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1737 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/median_pool.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1843 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/mixed_conv2d.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7008 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/ml_decoder.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8457 2023-10-19 00:38:07.000000 timm-0.9.9/timm/layers/mlp.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6218 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/non_local_attn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6040 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/norm.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17418 2023-04-28 20:49:14.000000 timm-0.9.9/timm/layers/norm_act.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2877 2023-04-28 20:49:14.000000 timm-0.9.9/timm/layers/padding.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1741 2023-04-12 15:57:13.000000 timm-0.9.9/timm/layers/patch_dropout.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9598 2023-08-29 16:12:50.000000 timm-0.9.9/timm/layers/patch_embed.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3045 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/pool2d_same.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2584 2023-08-29 16:12:50.000000 timm-0.9.9/timm/layers/pos_embed.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    19449 2023-09-02 18:19:46.000000 timm-0.9.9/timm/layers/pos_embed_rel.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14452 2023-08-29 16:12:50.000000 timm-0.9.9/timm/layers/pos_embed_sincos.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5387 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/selective_kernel.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2620 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/separable_conv.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1775 2023-04-28 20:49:14.000000 timm-0.9.9/timm/layers/space_to_depth.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3076 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/split_attn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3441 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/split_batchnorm.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4327 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/squeeze_excite.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5887 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/std_conv.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1996 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/test_time_pool.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      335 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/trace_utils.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      163 2023-10-31 17:20:37.000000 timm-0.9.9/timm/layers/typing.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4765 2023-03-31 00:49:24.000000 timm-0.9.9/timm/layers/weight_init.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.896449 timm-0.9.9/timm/loss/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      245 2023-02-24 22:35:42.000000 timm-0.9.9/timm/loss/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3343 2023-03-31 00:49:24.000000 timm-0.9.9/timm/loss/asymmetric_loss.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2030 2023-02-24 22:35:42.000000 timm-0.9.9/timm/loss/binary_cross_entropy.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1145 2023-02-24 22:35:42.000000 timm-0.9.9/timm/loss/cross_entropy.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1595 2023-02-24 22:35:42.000000 timm-0.9.9/timm/loss/jsd.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.904449 timm-0.9.9/timm/models/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3246 2023-09-02 18:19:46.000000 timm-0.9.9/timm/models/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18177 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/_builder.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    12092 2023-08-03 23:44:25.000000 timm-0.9.9/timm/models/_efficientnet_blocks.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    20021 2023-10-31 17:20:37.000000 timm-0.9.9/timm/models/_efficientnet_builder.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5069 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/_factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15540 2023-10-17 16:33:57.000000 timm-0.9.9/timm/models/_features.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4972 2023-08-20 18:50:19.000000 timm-0.9.9/timm/models/_features_fx.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5948 2023-10-29 22:34:22.000000 timm-0.9.9/timm/models/_helpers.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15332 2023-11-03 18:39:04.000000 timm-0.9.9/timm/models/_hub.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10503 2023-10-17 16:33:57.000000 timm-0.9.9/timm/models/_manipulate.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3525 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/_pretrained.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4171 2023-03-31 00:49:24.000000 timm-0.9.9/timm/models/_prune.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.904449 timm-0.9.9/timm/models/_pruned/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8734 2023-03-31 00:49:24.000000 timm-0.9.9/timm/models/_pruned/ecaresnet101d_pruned.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4520 2023-03-31 00:49:24.000000 timm-0.9.9/timm/models/_pruned/ecaresnet50d_pruned.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18596 2023-03-31 00:49:24.000000 timm-0.9.9/timm/models/_pruned/efficientnet_b1_pruned.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18676 2023-03-31 00:49:24.000000 timm-0.9.9/timm/models/_pruned/efficientnet_b2_pruned.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    21133 2023-03-31 00:49:24.000000 timm-0.9.9/timm/models/_pruned/efficientnet_b3_pruned.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13506 2023-04-06 15:39:02.000000 timm-0.9.9/timm/models/_registry.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    25579 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/beit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18985 2023-05-11 22:52:53.000000 timm-0.9.9/timm/models/byoanet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    85786 2023-08-29 16:12:50.000000 timm-0.9.9/timm/models/byobnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18131 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/cait.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    30015 2023-08-10 18:12:17.000000 timm-0.9.9/timm/models/coat.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15301 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/convit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4598 2023-09-27 17:21:16.000000 timm-0.9.9/timm/models/convmixer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    49907 2023-11-03 21:33:43.000000 timm-0.9.9/timm/models/convnext.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    24271 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/crossvit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    40028 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/cspnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    23064 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/davit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18550 2023-08-29 16:12:50.000000 timm-0.9.9/timm/models/deit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15634 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/densenet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18599 2023-05-10 22:09:19.000000 timm-0.9.9/timm/models/dla.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13621 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/dpn.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    21277 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/edgenext.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    19024 2023-09-27 17:21:16.000000 timm-0.9.9/timm/models/efficientformer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    24873 2023-08-20 18:50:19.000000 timm-0.9.9/timm/models/efficientformer_v2.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   102119 2023-10-17 16:33:57.000000 timm-0.9.9/timm/models/efficientnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    20740 2023-09-02 18:19:46.000000 timm-0.9.9/timm/models/efficientvit_mit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    23405 2023-09-02 18:19:46.000000 timm-0.9.9/timm/models/efficientvit_msra.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    40768 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/eva.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      150 2023-03-31 00:49:24.000000 timm-0.9.9/timm/models/factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    48143 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/fastvit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      151 2023-03-31 00:49:24.000000 timm-0.9.9/timm/models/features.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    24033 2023-10-17 16:33:57.000000 timm-0.9.9/timm/models/focalnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      154 2023-03-31 00:49:24.000000 timm-0.9.9/timm/models/fx_features.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    21393 2023-10-17 16:33:57.000000 timm-0.9.9/timm/models/gcvit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14559 2023-09-27 17:21:16.000000 timm-0.9.9/timm/models/ghostnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7697 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/hardcorenas.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      223 2023-03-31 00:49:24.000000 timm-0.9.9/timm/models/helpers.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    33100 2023-08-03 23:44:25.000000 timm-0.9.9/timm/models/hrnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      146 2023-05-14 15:02:18.000000 timm-0.9.9/timm/models/hub.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15052 2023-08-29 16:12:50.000000 timm-0.9.9/timm/models/inception_next.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    12077 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/inception_resnet_v2.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17104 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/inception_v3.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11076 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/inception_v4.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.904449 timm-0.9.9/timm/models/layers/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3432 2023-05-11 22:52:53.000000 timm-0.9.9/timm/models/layers/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    32443 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/levit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    84981 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/maxxvit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    35053 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/metaformer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    24231 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/mlp_mixer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    33974 2023-10-31 17:20:37.000000 timm-0.9.9/timm/models/mobilenetv3.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    25734 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/mobilevit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    35675 2023-09-27 17:21:16.000000 timm-0.9.9/timm/models/mvitv2.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    26627 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/nasnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    21505 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/nest.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    41085 2023-11-02 16:47:33.000000 timm-0.9.9/timm/models/nfnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14946 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/pit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15389 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/pnasnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17286 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/pvt_v2.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      151 2023-03-31 00:49:24.000000 timm-0.9.9/timm/models/registry.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    44020 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/regnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    16340 2023-09-27 17:21:16.000000 timm-0.9.9/timm/models/repghost.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    16386 2023-10-20 18:50:18.000000 timm-0.9.9/timm/models/repvit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7691 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/res2net.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9635 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/resnest.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    95853 2023-10-31 17:20:37.000000 timm-0.9.9/timm/models/resnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    30449 2023-10-20 20:24:36.000000 timm-0.9.9/timm/models/resnetv2.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11918 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/rexnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13254 2023-08-03 23:44:25.000000 timm-0.9.9/timm/models/selecsls.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18165 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/senet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17254 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/sequencer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8777 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/sknet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    34520 2023-10-31 17:20:37.000000 timm-0.9.9/timm/models/swin_transformer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    33673 2023-09-27 17:20:03.000000 timm-0.9.9/timm/models/swin_transformer_v2.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    41811 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/swin_transformer_v2_cr.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    23778 2023-09-27 17:21:16.000000 timm-0.9.9/timm/models/tiny_vit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    13362 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/tnt.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    12893 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/tresnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    19038 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/twins.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11004 2023-04-28 20:49:14.000000 timm-0.9.9/timm/models/vgg.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    18982 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/visformer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)   116863 2023-11-03 18:13:21.000000 timm-0.9.9/timm/models/vision_transformer.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17397 2023-08-29 16:12:50.000000 timm-0.9.9/timm/models/vision_transformer_hybrid.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    23878 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/vision_transformer_relpos.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    25122 2023-10-19 00:38:07.000000 timm-0.9.9/timm/models/vision_transformer_sam.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    30366 2023-08-03 23:44:25.000000 timm-0.9.9/timm/models/volo.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15477 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/vovnet.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8098 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/xception.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14086 2023-05-10 14:38:22.000000 timm-0.9.9/timm/models/xception_aligned.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    37768 2023-09-27 17:21:16.000000 timm-0.9.9/timm/models/xcit.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.904449 timm-0.9.9/timm/optim/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      530 2023-08-03 23:44:25.000000 timm-0.9.9/timm/optim/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9827 2023-02-24 22:35:42.000000 timm-0.9.9/timm/optim/adabelief.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7459 2023-02-24 22:35:42.000000 timm-0.9.9/timm/optim/adafactor.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6535 2023-02-24 22:35:42.000000 timm-0.9.9/timm/optim/adahessian.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3574 2023-02-24 22:35:42.000000 timm-0.9.9/timm/optim/adamp.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5147 2023-02-24 22:35:42.000000 timm-0.9.9/timm/optim/adamw.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5071 2023-03-31 00:49:24.000000 timm-0.9.9/timm/optim/adan.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9184 2023-02-24 22:35:42.000000 timm-0.9.9/timm/optim/lamb.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5256 2023-02-24 22:35:42.000000 timm-0.9.9/timm/optim/lars.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7099 2023-03-31 00:49:24.000000 timm-0.9.9/timm/optim/lion.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2687 2023-08-03 23:44:25.000000 timm-0.9.9/timm/optim/lookahead.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6893 2023-02-24 22:35:42.000000 timm-0.9.9/timm/optim/madgrad.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3929 2023-08-03 23:44:25.000000 timm-0.9.9/timm/optim/nadam.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    12369 2023-08-03 23:44:25.000000 timm-0.9.9/timm/optim/nadamw.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4856 2023-02-24 22:35:42.000000 timm-0.9.9/timm/optim/nvnovograd.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    15424 2023-08-03 23:44:25.000000 timm-0.9.9/timm/optim/optim_factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3468 2023-02-24 22:35:42.000000 timm-0.9.9/timm/optim/radam.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6143 2023-02-24 22:35:42.000000 timm-0.9.9/timm/optim/rmsprop_tf.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2296 2023-02-24 22:35:42.000000 timm-0.9.9/timm/optim/sgdp.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.904449 timm-0.9.9/timm/scheduler/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      330 2023-03-31 00:49:24.000000 timm-0.9.9/timm/scheduler/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3843 2023-03-31 00:49:24.000000 timm-0.9.9/timm/scheduler/cosine_lr.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1930 2023-03-31 00:49:24.000000 timm-0.9.9/timm/scheduler/multistep_lr.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3573 2023-03-31 00:49:24.000000 timm-0.9.9/timm/scheduler/plateau_lr.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3673 2023-03-31 00:49:24.000000 timm-0.9.9/timm/scheduler/poly_lr.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5408 2023-03-31 00:49:24.000000 timm-0.9.9/timm/scheduler/scheduler.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6622 2023-03-31 00:49:24.000000 timm-0.9.9/timm/scheduler/scheduler_factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1732 2023-03-31 00:49:24.000000 timm-0.9.9/timm/scheduler/step_lr.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3607 2023-03-31 00:49:24.000000 timm-0.9.9/timm/scheduler/tanh_lr.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.908449 timm-0.9.9/timm/utils/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      786 2023-08-29 16:12:50.000000 timm-0.9.9/timm/utils/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1624 2023-02-24 22:35:42.000000 timm-0.9.9/timm/utils/agc.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6133 2023-02-24 22:35:42.000000 timm-0.9.9/timm/utils/checkpoint_saver.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      796 2023-02-24 22:35:42.000000 timm-0.9.9/timm/utils/clip_grad.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2029 2023-04-28 20:49:14.000000 timm-0.9.9/timm/utils/cuda.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1762 2023-02-24 22:35:42.000000 timm-0.9.9/timm/utils/decay_batch.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4256 2023-03-31 00:49:24.000000 timm-0.9.9/timm/utils/distributed.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2203 2023-02-24 22:35:42.000000 timm-0.9.9/timm/utils/jit.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1015 2023-02-24 22:35:42.000000 timm-0.9.9/timm/utils/log.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      901 2023-02-24 22:35:42.000000 timm-0.9.9/timm/utils/metrics.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1105 2023-03-31 00:49:24.000000 timm-0.9.9/timm/utils/misc.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10420 2023-08-29 16:12:50.000000 timm-0.9.9/timm/utils/model.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5670 2023-02-24 22:35:42.000000 timm-0.9.9/timm/utils/model_ema.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3342 2023-04-28 20:49:14.000000 timm-0.9.9/timm/utils/onnx.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      178 2023-02-24 22:35:42.000000 timm-0.9.9/timm/utils/random.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1300 2023-03-31 00:49:24.000000 timm-0.9.9/timm/utils/summary.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       22 2023-11-03 18:16:00.000000 timm-0.9.9/timm/version.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-11-03 21:50:05.888449 timm-0.9.9/timm.egg-info/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    59684 2023-11-03 21:50:05.000000 timm-0.9.9/timm.egg-info/PKG-INFO
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7263 2023-11-03 21:50:05.000000 timm-0.9.9/timm.egg-info/SOURCES.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)        1 2023-11-03 21:50:05.000000 timm-0.9.9/timm.egg-info/dependency_links.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       58 2023-11-03 21:50:05.000000 timm-0.9.9/timm.egg-info/requires.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)        5 2023-11-03 21:50:05.000000 timm-0.9.9/timm.egg-info/top_level.txt
+-rw-r--r--   0        0        0    11343 2024-05-15 17:56:47.070268 timm-1.0.3/LICENSE
+-rw-r--r--   0        0        0    42161 2024-05-15 17:57:47.894225 timm-1.0.3/README.md
+-rw-r--r--   0        0        0     2058 2024-05-15 18:10:46.349658 timm-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 17:56:47.086268 timm-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1849 2024-05-15 17:56:47.086268 timm-1.0.3/tests/test_layers.py
+-rw-r--r--   0        0        0    26498 2024-05-15 17:56:47.086268 timm-1.0.3/tests/test_models.py
+-rw-r--r--   0        0        0    24702 2024-05-15 17:56:47.086268 timm-1.0.3/tests/test_optim.py
+-rw-r--r--   0        0        0     1978 2024-05-15 17:56:47.086268 timm-1.0.3/tests/test_utils.py
+-rw-r--r--   0        0        0      292 2024-05-15 17:56:47.086268 timm-1.0.3/timm/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-15 17:56:47.086268 timm-1.0.3/timm/data/__init__.py
+-rw-r--r--   0        0        0   118210 2024-05-15 17:56:47.086268 timm-1.0.3/timm/data/_info/imagenet12k_synsets.txt
+-rw-r--r--   0        0        0   218430 2024-05-15 17:56:47.086268 timm-1.0.3/timm/data/_info/imagenet21k_goog_synsets.txt
+-rw-r--r--   0        0        0    64070 2024-05-15 17:56:47.086268 timm-1.0.3/timm/data/_info/imagenet21k_goog_to_12k_indices.txt
+-rw-r--r--   0        0        0   119937 2024-05-15 17:56:47.086268 timm-1.0.3/timm/data/_info/imagenet21k_goog_to_22k_indices.txt
+-rw-r--r--   0        0        0   112210 2024-05-15 17:56:47.086268 timm-1.0.3/timm/data/_info/imagenet21k_miil_synsets.txt
+-rw-r--r--   0        0        0   104500 2024-05-15 17:56:47.086268 timm-1.0.3/timm/data/_info/imagenet21k_miil_w21_synsets.txt
+-rw-r--r--   0        0        0   218420 2024-05-15 17:56:47.086268 timm-1.0.3/timm/data/_info/imagenet22k_ms_synsets.txt
+-rw-r--r--   0        0        0    63625 2024-05-15 17:56:47.090268 timm-1.0.3/timm/data/_info/imagenet22k_ms_to_12k_indices.txt
+-rw-r--r--   0        0        0   119938 2024-05-15 17:56:47.090268 timm-1.0.3/timm/data/_info/imagenet22k_ms_to_22k_indices.txt
+-rw-r--r--   0        0        0   218410 2024-05-15 17:56:47.090268 timm-1.0.3/timm/data/_info/imagenet22k_synsets.txt
+-rw-r--r--   0        0        0    64070 2024-05-15 17:56:47.090268 timm-1.0.3/timm/data/_info/imagenet22k_to_12k_indices.txt
+-rw-r--r--   0        0        0      774 2024-05-15 17:56:47.090268 timm-1.0.3/timm/data/_info/imagenet_a_indices.txt
+-rw-r--r--   0        0        0     2000 2024-05-15 17:56:47.090268 timm-1.0.3/timm/data/_info/imagenet_a_synsets.txt
+-rw-r--r--   0        0        0      769 2024-05-15 17:56:47.090268 timm-1.0.3/timm/data/_info/imagenet_r_indices.txt
+-rw-r--r--   0        0        0     2000 2024-05-15 17:56:47.090268 timm-1.0.3/timm/data/_info/imagenet_r_synsets.txt
+-rw-r--r--   0        0        0   388478 2024-05-15 17:56:47.090268 timm-1.0.3/timm/data/_info/imagenet_real_labels.json
+-rw-r--r--   0        0        0  1748917 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/_info/imagenet_synset_to_definition.txt
+-rw-r--r--   0        0        0   741457 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/_info/imagenet_synset_to_lemma.txt
+-rw-r--r--   0        0        0    10000 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/_info/imagenet_synsets.txt
+-rw-r--r--   0        0        0    35550 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/auto_augment.py
+-rw-r--r--   0        0        0     4616 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/config.py
+-rw-r--r--   0        0        0      442 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/constants.py
+-rw-r--r--   0        0        0     6210 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/dataset.py
+-rw-r--r--   0        0        0     8180 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/dataset_factory.py
+-rw-r--r--   0        0        0     2391 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/dataset_info.py
+-rw-r--r--   0        0        0     5540 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/distributed_sampler.py
+-rw-r--r--   0        0        0     4167 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/imagenet_info.py
+-rw-r--r--   0        0        0    15511 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/loader.py
+-rw-r--r--   0        0        0    14634 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/mixup.py
+-rw-r--r--   0        0        0     4964 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/random_erasing.py
+-rw-r--r--   0        0        0       72 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/readers/__init__.py
+-rw-r--r--   0        0        0      895 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/readers/class_map.py
+-rw-r--r--   0        0        0     1482 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/readers/img_extensions.py
+-rw-r--r--   0        0        0      487 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/readers/reader.py
+-rw-r--r--   0        0        0     1732 2024-05-15 17:56:47.098268 timm-1.0.3/timm/data/readers/reader_factory.py
+-rw-r--r--   0        0        0     2608 2024-05-15 17:56:47.102268 timm-1.0.3/timm/data/readers/reader_hfds.py
+-rw-r--r--   0        0        0     8282 2024-05-15 17:56:47.102268 timm-1.0.3/timm/data/readers/reader_hfids.py
+-rw-r--r--   0        0        0     3508 2024-05-15 17:56:47.102268 timm-1.0.3/timm/data/readers/reader_image_folder.py
+-rw-r--r--   0        0        0     9182 2024-05-15 17:56:47.102268 timm-1.0.3/timm/data/readers/reader_image_in_tar.py
+-rw-r--r--   0        0        0     2644 2024-05-15 17:56:47.102268 timm-1.0.3/timm/data/readers/reader_image_tar.py
+-rw-r--r--   0        0        0    17909 2024-05-15 17:56:47.102268 timm-1.0.3/timm/data/readers/reader_tfds.py
+-rw-r--r--   0        0        0    16947 2024-05-15 17:56:47.102268 timm-1.0.3/timm/data/readers/reader_wds.py
+-rw-r--r--   0        0        0      303 2024-05-15 17:56:47.102268 timm-1.0.3/timm/data/readers/shared_count.py
+-rw-r--r--   0        0        0     1800 2024-05-15 17:56:47.102268 timm-1.0.3/timm/data/real_labels.py
+-rw-r--r--   0        0        0     9169 2024-05-15 17:56:47.102268 timm-1.0.3/timm/data/tf_preprocessing.py
+-rw-r--r--   0        0        0    18852 2024-05-15 17:56:47.102268 timm-1.0.3/timm/data/transforms.py
+-rw-r--r--   0        0        0    19051 2024-05-15 17:56:47.102268 timm-1.0.3/timm/data/transforms_factory.py
+-rw-r--r--   0        0        0     3842 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/__init__.py
+-rw-r--r--   0        0        0     4882 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/activations.py
+-rw-r--r--   0        0        0     5504 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/activations_me.py
+-rw-r--r--   0        0        0     6583 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/adaptive_avgmax_pool.py
+-rw-r--r--   0        0        0     3458 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/attention_pool.py
+-rw-r--r--   0        0        0     4934 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/attention_pool2d.py
+-rw-r--r--   0        0        0     1594 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/blur_pool.py
+-rw-r--r--   0        0        0     6895 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/bottleneck_attn.py
+-rw-r--r--   0        0        0     4426 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/cbam.py
+-rw-r--r--   0        0        0     7522 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/classifier.py
+-rw-r--r--   0        0        0     5199 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/cond_conv2d.py
+-rw-r--r--   0        0        0     4175 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/config.py
+-rw-r--r--   0        0        0     3216 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/conv2d_same.py
+-rw-r--r--   0        0        0     3836 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/conv_bn_act.py
+-rw-r--r--   0        0        0     4434 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/create_act.py
+-rw-r--r--   0        0        0     3514 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/create_attn.py
+-rw-r--r--   0        0        0     1622 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/create_conv2d.py
+-rw-r--r--   0        0        0     1581 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/create_norm.py
+-rw-r--r--   0        0        0     3836 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/create_norm_act.py
+-rw-r--r--   0        0        0     6973 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/drop.py
+-rw-r--r--   0        0        0     6386 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/eca.py
+-rw-r--r--   0        0        0    13862 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/evo_norm.py
+-rw-r--r--   0        0        0     4008 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/fast_norm.py
+-rw-r--r--   0        0        0     2540 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/filter_response_norm.py
+-rw-r--r--   0        0        0     1109 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/format.py
+-rw-r--r--   0        0        0     3824 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/gather_excite.py
+-rw-r--r--   0        0        0     2445 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/global_context.py
+-rw-r--r--   0        0        0     1624 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/grid.py
+-rw-r--r--   0        0        0     1319 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/grn.py
+-rw-r--r--   0        0        0    10662 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/halo_attn.py
+-rw-r--r--   0        0        0     1053 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/helpers.py
+-rw-r--r--   0        0        0     3374 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/inplace_abn.py
+-rw-r--r--   0        0        0     2439 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/interpolate.py
+-rw-r--r--   0        0        0     5958 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/lambda_layer.py
+-rw-r--r--   0        0        0      743 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/linear.py
+-rw-r--r--   0        0        0     1737 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/median_pool.py
+-rw-r--r--   0        0        0     1843 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/mixed_conv2d.py
+-rw-r--r--   0        0        0     6701 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/ml_decoder.py
+-rw-r--r--   0        0        0     8457 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/mlp.py
+-rw-r--r--   0        0        0     6218 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/non_local_attn.py
+-rw-r--r--   0        0        0     6022 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/norm.py
+-rw-r--r--   0        0        0    17418 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/norm_act.py
+-rw-r--r--   0        0        0     2877 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/padding.py
+-rw-r--r--   0        0        0     1741 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/patch_dropout.py
+-rw-r--r--   0        0        0    10324 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/patch_embed.py
+-rw-r--r--   0        0        0     3045 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/pool2d_same.py
+-rw-r--r--   0        0        0     2584 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/pos_embed.py
+-rw-r--r--   0        0        0    19370 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/pos_embed_rel.py
+-rw-r--r--   0        0        0    14465 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/pos_embed_sincos.py
+-rw-r--r--   0        0        0     5387 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/selective_kernel.py
+-rw-r--r--   0        0        0     2620 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/separable_conv.py
+-rw-r--r--   0        0        0     1068 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/space_to_depth.py
+-rw-r--r--   0        0        0     3076 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/split_attn.py
+-rw-r--r--   0        0        0     3441 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/split_batchnorm.py
+-rw-r--r--   0        0        0     4327 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/squeeze_excite.py
+-rw-r--r--   0        0        0     5887 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/std_conv.py
+-rw-r--r--   0        0        0     1996 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/test_time_pool.py
+-rw-r--r--   0        0        0      335 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/trace_utils.py
+-rw-r--r--   0        0        0      163 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/typing.py
+-rw-r--r--   0        0        0     4765 2024-05-15 17:56:47.102268 timm-1.0.3/timm/layers/weight_init.py
+-rw-r--r--   0        0        0      245 2024-05-15 17:56:47.102268 timm-1.0.3/timm/loss/__init__.py
+-rw-r--r--   0        0        0     3240 2024-05-15 17:56:47.102268 timm-1.0.3/timm/loss/asymmetric_loss.py
+-rw-r--r--   0        0        0     2483 2024-05-15 17:56:47.102268 timm-1.0.3/timm/loss/binary_cross_entropy.py
+-rw-r--r--   0        0        0     1145 2024-05-15 17:56:47.102268 timm-1.0.3/timm/loss/cross_entropy.py
+-rw-r--r--   0        0        0     1595 2024-05-15 17:56:47.102268 timm-1.0.3/timm/loss/jsd.py
+-rw-r--r--   0        0        0     3333 2024-05-15 17:56:47.102268 timm-1.0.3/timm/models/__init__.py
+-rw-r--r--   0        0        0    19879 2024-05-15 17:56:47.102268 timm-1.0.3/timm/models/_builder.py
+-rw-r--r--   0        0        0    12092 2024-05-15 17:56:47.102268 timm-1.0.3/timm/models/_efficientnet_blocks.py
+-rw-r--r--   0        0        0    20021 2024-05-15 17:56:47.102268 timm-1.0.3/timm/models/_efficientnet_builder.py
+-rw-r--r--   0        0        0     5188 2024-05-15 17:56:47.102268 timm-1.0.3/timm/models/_factory.py
+-rw-r--r--   0        0        0    19720 2024-05-15 17:56:47.102268 timm-1.0.3/timm/models/_features.py
+-rw-r--r--   0        0        0     5687 2024-05-15 17:56:47.102268 timm-1.0.3/timm/models/_features_fx.py
+-rw-r--r--   0        0        0     5948 2024-05-15 17:56:47.102268 timm-1.0.3/timm/models/_helpers.py
+-rw-r--r--   0        0        0    16141 2024-05-15 17:56:47.102268 timm-1.0.3/timm/models/_hub.py
+-rw-r--r--   0        0        0    10503 2024-05-15 17:56:47.102268 timm-1.0.3/timm/models/_manipulate.py
+-rw-r--r--   0        0        0     3525 2024-05-15 17:56:47.102268 timm-1.0.3/timm/models/_pretrained.py
+-rw-r--r--   0        0        0     4171 2024-05-15 17:56:47.102268 timm-1.0.3/timm/models/_prune.py
+-rw-r--r--   0        0        0     8734 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/_pruned/ecaresnet101d_pruned.txt
+-rw-r--r--   0        0        0     4520 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/_pruned/ecaresnet50d_pruned.txt
+-rw-r--r--   0        0        0    18596 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/_pruned/efficientnet_b1_pruned.txt
+-rw-r--r--   0        0        0    18676 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/_pruned/efficientnet_b2_pruned.txt
+-rw-r--r--   0        0        0    21133 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/_pruned/efficientnet_b3_pruned.txt
+-rw-r--r--   0        0        0    14117 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/_registry.py
+-rw-r--r--   0        0        0    29295 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/beit.py
+-rw-r--r--   0        0        0    18985 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/byoanet.py
+-rw-r--r--   0        0        0    89753 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/byobnet.py
+-rw-r--r--   0        0        0    21376 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/cait.py
+-rw-r--r--   0        0        0    30017 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/coat.py
+-rw-r--r--   0        0        0    15320 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/convit.py
+-rw-r--r--   0        0        0     4649 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/convmixer.py
+-rw-r--r--   0        0        0    52338 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/convnext.py
+-rw-r--r--   0        0        0    24285 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/crossvit.py
+-rw-r--r--   0        0        0    40060 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/cspnet.py
+-rw-r--r--   0        0        0    23281 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/davit.py
+-rw-r--r--   0        0        0    18512 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/deit.py
+-rw-r--r--   0        0        0    15942 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/densenet.py
+-rw-r--r--   0        0        0    18599 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/dla.py
+-rw-r--r--   0        0        0    13593 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/dpn.py
+-rw-r--r--   0        0        0    20900 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/edgenext.py
+-rw-r--r--   0        0        0    21956 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/efficientformer.py
+-rw-r--r--   0        0        0    24873 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/efficientformer_v2.py
+-rw-r--r--   0        0        0   105265 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/efficientnet.py
+-rw-r--r--   0        0        0    34173 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/efficientvit_mit.py
+-rw-r--r--   0        0        0    23437 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/efficientvit_msra.py
+-rw-r--r--   0        0        0    48500 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/eva.py
+-rw-r--r--   0        0        0      150 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/factory.py
+-rw-r--r--   0        0        0    48418 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/fastvit.py
+-rw-r--r--   0        0        0      151 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/features.py
+-rw-r--r--   0        0        0    24087 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/focalnet.py
+-rw-r--r--   0        0        0      154 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/fx_features.py
+-rw-r--r--   0        0        0    21447 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/gcvit.py
+-rw-r--r--   0        0        0    14559 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/ghostnet.py
+-rw-r--r--   0        0        0     7697 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/hardcorenas.py
+-rw-r--r--   0        0        0      223 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/helpers.py
+-rw-r--r--   0        0        0    23366 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/hgnet.py
+-rw-r--r--   0        0        0    33596 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/hiera.py
+-rw-r--r--   0        0        0    33271 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/hrnet.py
+-rw-r--r--   0        0        0      146 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/hub.py
+-rw-r--r--   0        0        0    15052 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/inception_next.py
+-rw-r--r--   0        0        0    12077 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/inception_resnet_v2.py
+-rw-r--r--   0        0        0    17104 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/inception_v3.py
+-rw-r--r--   0        0        0    11076 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/inception_v4.py
+-rw-r--r--   0        0        0     3374 2024-05-15 17:56:47.106268 timm-1.0.3/timm/models/layers/__init__.py
+-rw-r--r--   0        0        0    34910 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/levit.py
+-rw-r--r--   0        0        0    87847 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/maxxvit.py
+-rw-r--r--   0        0        0    35053 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/metaformer.py
+-rw-r--r--   0        0        0    27269 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/mlp_mixer.py
+-rw-r--r--   0        0        0    35969 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/mobilenetv3.py
+-rw-r--r--   0        0        0    25734 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/mobilevit.py
+-rw-r--r--   0        0        0    39149 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/mvitv2.py
+-rw-r--r--   0        0        0    26627 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/nasnet.py
+-rw-r--r--   0        0        0    21505 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/nest.py
+-rw-r--r--   0        0        0    22760 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/nextvit.py
+-rw-r--r--   0        0        0    41085 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/nfnet.py
+-rw-r--r--   0        0        0    14967 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/pit.py
+-rw-r--r--   0        0        0    15389 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/pnasnet.py
+-rw-r--r--   0        0        0    17311 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/pvt_v2.py
+-rw-r--r--   0        0        0      151 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/registry.py
+-rw-r--r--   0        0        0    46496 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/regnet.py
+-rw-r--r--   0        0        0    16340 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/repghost.py
+-rw-r--r--   0        0        0    16436 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/repvit.py
+-rw-r--r--   0        0        0     7691 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/res2net.py
+-rw-r--r--   0        0        0     9635 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/resnest.py
+-rw-r--r--   0        0        0    98006 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/resnet.py
+-rw-r--r--   0        0        0    30481 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/resnetv2.py
+-rw-r--r--   0        0        0    11918 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/rexnet.py
+-rw-r--r--   0        0        0    13254 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/selecsls.py
+-rw-r--r--   0        0        0    18165 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/senet.py
+-rw-r--r--   0        0        0    17286 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/sequencer.py
+-rw-r--r--   0        0        0     8777 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/sknet.py
+-rw-r--r--   0        0        0    37091 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/swin_transformer.py
+-rw-r--r--   0        0        0    37364 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/swin_transformer_v2.py
+-rw-r--r--   0        0        0    43936 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/swin_transformer_v2_cr.py
+-rw-r--r--   0        0        0    23796 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/tiny_vit.py
+-rw-r--r--   0        0        0    13412 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/tnt.py
+-rw-r--r--   0        0        0    12951 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/tresnet.py
+-rw-r--r--   0        0        0    21959 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/twins.py
+-rw-r--r--   0        0        0    11004 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/vgg.py
+-rw-r--r--   0        0        0    18982 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/visformer.py
+-rw-r--r--   0        0        0   138934 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/vision_transformer.py
+-rw-r--r--   0        0        0    18543 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/vision_transformer_hybrid.py
+-rw-r--r--   0        0        0    28504 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/vision_transformer_relpos.py
+-rw-r--r--   0        0        0    28249 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/vision_transformer_sam.py
+-rw-r--r--   0        0        0    34218 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/volo.py
+-rw-r--r--   0        0        0    15509 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/vovnet.py
+-rw-r--r--   0        0        0     8098 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/xception.py
+-rw-r--r--   0        0        0    15330 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/xception_aligned.py
+-rw-r--r--   0        0        0    41577 2024-05-15 17:56:47.110267 timm-1.0.3/timm/models/xcit.py
+-rw-r--r--   0        0        0      530 2024-05-15 17:56:47.110267 timm-1.0.3/timm/optim/__init__.py
+-rw-r--r--   0        0        0     9827 2024-05-15 17:56:47.110267 timm-1.0.3/timm/optim/adabelief.py
+-rw-r--r--   0        0        0     7459 2024-05-15 17:56:47.110267 timm-1.0.3/timm/optim/adafactor.py
+-rw-r--r--   0        0        0     6535 2024-05-15 17:56:47.110267 timm-1.0.3/timm/optim/adahessian.py
+-rw-r--r--   0        0        0     3574 2024-05-15 17:56:47.110267 timm-1.0.3/timm/optim/adamp.py
+-rw-r--r--   0        0        0     5147 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/adamw.py
+-rw-r--r--   0        0        0     5071 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/adan.py
+-rw-r--r--   0        0        0     9184 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/lamb.py
+-rw-r--r--   0        0        0     5256 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/lars.py
+-rw-r--r--   0        0        0     7099 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/lion.py
+-rw-r--r--   0        0        0     2687 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/lookahead.py
+-rw-r--r--   0        0        0     6893 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/madgrad.py
+-rw-r--r--   0        0        0     3929 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/nadam.py
+-rw-r--r--   0        0        0    12369 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/nadamw.py
+-rw-r--r--   0        0        0     4856 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/nvnovograd.py
+-rw-r--r--   0        0        0    15868 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/optim_factory.py
+-rw-r--r--   0        0        0     3468 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/radam.py
+-rw-r--r--   0        0        0     6143 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/rmsprop_tf.py
+-rw-r--r--   0        0        0     2296 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/sgdp.py
+-rw-r--r--   0        0        0     9046 2024-05-15 17:56:47.114268 timm-1.0.3/timm/optim/sgdw.py
+-rw-r--r--   0        0        0      330 2024-05-15 17:56:47.114268 timm-1.0.3/timm/scheduler/__init__.py
+-rw-r--r--   0        0        0     3887 2024-05-15 17:56:47.114268 timm-1.0.3/timm/scheduler/cosine_lr.py
+-rw-r--r--   0        0        0     1950 2024-05-15 17:56:47.114268 timm-1.0.3/timm/scheduler/multistep_lr.py
+-rw-r--r--   0        0        0     3603 2024-05-15 17:56:47.114268 timm-1.0.3/timm/scheduler/plateau_lr.py
+-rw-r--r--   0        0        0     3717 2024-05-15 17:56:47.114268 timm-1.0.3/timm/scheduler/poly_lr.py
+-rw-r--r--   0        0        0     5426 2024-05-15 17:56:47.114268 timm-1.0.3/timm/scheduler/scheduler.py
+-rw-r--r--   0        0        0     6787 2024-05-15 17:56:47.114268 timm-1.0.3/timm/scheduler/scheduler_factory.py
+-rw-r--r--   0        0        0     1777 2024-05-15 17:56:47.114268 timm-1.0.3/timm/scheduler/step_lr.py
+-rw-r--r--   0        0        0     3651 2024-05-15 17:56:47.114268 timm-1.0.3/timm/scheduler/tanh_lr.py
+-rw-r--r--   0        0        0      846 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/__init__.py
+-rw-r--r--   0        0        0     1624 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/agc.py
+-rw-r--r--   0        0        0     2823 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/attention_extract.py
+-rw-r--r--   0        0        0     6133 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/checkpoint_saver.py
+-rw-r--r--   0        0        0      796 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/clip_grad.py
+-rw-r--r--   0        0        0     2029 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/cuda.py
+-rw-r--r--   0        0        0     1762 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/decay_batch.py
+-rw-r--r--   0        0        0     5762 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/distributed.py
+-rw-r--r--   0        0        0     2203 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/jit.py
+-rw-r--r--   0        0        0     1015 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/log.py
+-rw-r--r--   0        0        0      901 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/metrics.py
+-rw-r--r--   0        0        0     1105 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/misc.py
+-rw-r--r--   0        0        0    10420 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/model.py
+-rw-r--r--   0        0        0    11244 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/model_ema.py
+-rw-r--r--   0        0        0     3922 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/onnx.py
+-rw-r--r--   0        0        0      178 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/random.py
+-rw-r--r--   0        0        0     1325 2024-05-15 17:56:47.114268 timm-1.0.3/timm/utils/summary.py
+-rw-r--r--   0        0        0       22 2024-05-15 17:57:07.974253 timm-1.0.3/timm/version.py
+-rw-r--r--   0        0        0    43575 1970-01-01 00:00:00.000000 timm-1.0.3/PKG-INFO
```

### Comparing `timm-0.9.9/LICENSE` & `timm-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/__init__.py` & `timm-1.0.3/timm/data/__init__.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet12k_synsets.txt` & `timm-1.0.3/timm/data/_info/imagenet12k_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet21k_goog_synsets.txt` & `timm-1.0.3/timm/data/_info/imagenet21k_goog_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet21k_goog_to_12k_indices.txt` & `timm-1.0.3/timm/data/_info/imagenet21k_goog_to_12k_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet21k_goog_to_22k_indices.txt` & `timm-1.0.3/timm/data/_info/imagenet21k_goog_to_22k_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet21k_miil_synsets.txt` & `timm-1.0.3/timm/data/_info/imagenet21k_miil_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet21k_miil_w21_synsets.txt` & `timm-1.0.3/timm/data/_info/imagenet21k_miil_w21_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet22k_ms_synsets.txt` & `timm-1.0.3/timm/data/_info/imagenet22k_ms_synsets.txt`

 * *Files 0% similar despite different names*

```diff
@@ -844,14 +844,15 @@
 n04371774
 n04372370
 n04376876
 n04380533
 n04389033
 n04392985
 n04398044
+n04399382
 n04404412
 n04409515
 n04417672
 n04418357
 n04423845
 n04428191
 n04429376
```

### Comparing `timm-0.9.9/timm/data/_info/imagenet22k_ms_to_12k_indices.txt` & `timm-1.0.3/timm/data/_info/imagenet22k_ms_to_12k_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet22k_ms_to_22k_indices.txt` & `timm-1.0.3/timm/data/_info/imagenet22k_ms_to_22k_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet22k_synsets.txt` & `timm-1.0.3/timm/data/_info/imagenet22k_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet22k_to_12k_indices.txt` & `timm-1.0.3/timm/data/_info/imagenet22k_to_12k_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet_a_indices.txt` & `timm-1.0.3/timm/data/_info/imagenet_a_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet_a_synsets.txt` & `timm-1.0.3/timm/data/_info/imagenet_a_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet_r_indices.txt` & `timm-1.0.3/timm/data/_info/imagenet_r_indices.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet_r_synsets.txt` & `timm-1.0.3/timm/data/_info/imagenet_r_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet_real_labels.json` & `timm-1.0.3/timm/data/_info/imagenet_real_labels.json`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet_synset_to_definition.txt` & `timm-1.0.3/timm/data/_info/imagenet_synset_to_definition.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet_synset_to_lemma.txt` & `timm-1.0.3/timm/data/_info/imagenet_synset_to_lemma.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/_info/imagenet_synsets.txt` & `timm-1.0.3/timm/data/_info/imagenet_synsets.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/auto_augment.py` & `timm-1.0.3/timm/data/auto_augment.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/config.py` & `timm-1.0.3/timm/data/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     pretrained_cfg = pretrained_cfg or {}
     if not pretrained_cfg and model is not None and hasattr(model, 'pretrained_cfg'):
         pretrained_cfg = model.pretrained_cfg
     data_config = {}
 
     # Resolve input/image size
     in_chans = 3
-    if args.get('chans', None) is not None:
+    if args.get('in_chans', None) is not None:
+        in_chans = args['in_chans']
+    elif args.get('chans', None) is not None:
         in_chans = args['chans']
 
     input_size = (in_chans, 224, 224)
     if args.get('input_size', None) is not None:
         assert isinstance(args['input_size'], (tuple, list))
         assert len(args['input_size']) == 3
         input_size = tuple(args['input_size'])
```

### Comparing `timm-0.9.9/timm/data/dataset.py` & `timm-1.0.3/timm/data/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     def __init__(
             self,
             root,
             reader=None,
             split='train',
             class_map=None,
             load_bytes=False,
-            img_mode='RGB',
+            input_img_mode='RGB',
             transform=None,
             target_transform=None,
     ):
         if reader is None or isinstance(reader, str):
             reader = create_reader(
                 reader or '',
                 root=root,
                 split=split,
                 class_map=class_map
             )
         self.reader = reader
         self.load_bytes = load_bytes
-        self.img_mode = img_mode
+        self.input_img_mode = input_img_mode
         self.transform = transform
         self.target_transform = target_transform
         self._consecutive_errors = 0
 
     def __getitem__(self, index):
         img, target = self.reader[index]
 
@@ -55,16 +55,16 @@
             self._consecutive_errors += 1
             if self._consecutive_errors < _ERROR_RETRY:
                 return self.__getitem__((index + 1) % len(self.reader))
             else:
                 raise e
         self._consecutive_errors = 0
 
-        if self.img_mode and not self.load_bytes:
-            img = img.convert(self.img_mode)
+        if self.input_img_mode and not self.load_bytes:
+            img = img.convert(self.input_img_mode)
         if self.transform is not None:
             img = self.transform(img)
 
         if target is None:
             target = -1
         elif self.target_transform is not None:
             target = self.target_transform(target)
@@ -86,33 +86,43 @@
     def __init__(
             self,
             root,
             reader=None,
             split='train',
             class_map=None,
             is_training=False,
-            batch_size=None,
+            batch_size=1,
+            num_samples=None,
             seed=42,
             repeats=0,
             download=False,
+            input_img_mode='RGB',
+            input_key=None,
+            target_key=None,
             transform=None,
             target_transform=None,
+            max_steps=None,
     ):
         assert reader is not None
         if isinstance(reader, str):
             self.reader = create_reader(
                 reader,
                 root=root,
                 split=split,
                 class_map=class_map,
                 is_training=is_training,
                 batch_size=batch_size,
+                num_samples=num_samples,
                 seed=seed,
                 repeats=repeats,
                 download=download,
+                input_img_mode=input_img_mode,
+                input_key=input_key,
+                target_key=target_key,
+                max_steps=max_steps,
             )
         else:
             self.reader = reader
         self.transform = transform
         self.target_transform = target_transform
         self._consecutive_errors = 0
```

### Comparing `timm-0.9.9/timm/data/dataset_factory.py` & `timm-1.0.3/timm/data/dataset_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Dataset Factory
 
 Hacked together by / Copyright 2021, Ross Wightman
 """
 import os
+from typing import Optional
 
 from torchvision.datasets import CIFAR100, CIFAR10, MNIST, KMNIST, FashionMNIST, ImageFolder
 try:
     from torchvision.datasets import Places365
     has_places365 = True
 except ImportError:
     has_places365 = False
@@ -56,30 +57,32 @@
         root = _try(_TRAIN_SYNONYM)
     elif split_name in _EVAL_SYNONYM:
         root = _try(_EVAL_SYNONYM)
     return root
 
 
 def create_dataset(
-        name,
-        root,
-        split='validation',
-        search_split=True,
-        class_map=None,
-        load_bytes=False,
-        is_training=False,
-        download=False,
-        batch_size=None,
-        seed=42,
-        repeats=0,
-        **kwargs
+        name: str,
+        root: Optional[str] = None,
+        split: str = 'validation',
+        search_split: bool = True,
+        class_map: dict = None,
+        load_bytes: bool = False,
+        is_training: bool = False,
+        download: bool = False,
+        batch_size: int = 1,
+        num_samples: Optional[int] = None,
+        seed: int = 42,
+        repeats: int = 0,
+        input_img_mode: str = 'RGB',
+        **kwargs,
 ):
     """ Dataset factory method
 
-    In parenthesis after each arg are the type of dataset supported for each arg, one of:
+    In parentheses after each arg are the type of dataset supported for each arg, one of:
       * folder - default, timm folder (or tar) based ImageDataset
       * torch - torchvision based datasets
       * HFDS - Hugging Face Datasets
       * TFDS - Tensorflow-datasets wrapper in IterabeDataset interface via IterableImageDataset
       * WDS - Webdataset
       * all - any of the above
 
@@ -93,19 +96,21 @@
         load_bytes: load data, return images as undecoded bytes (folder)
         download: download dataset if not present and supported (HFDS, TFDS, torch)
         is_training: create dataset in train mode, this is different from the split.
             For Iterable / TDFS it enables shuffle, ignored for other datasets. (TFDS, WDS)
         batch_size: batch size hint for (TFDS, WDS)
         seed: seed for iterable datasets (TFDS, WDS)
         repeats: dataset repeats per iteration i.e. epoch (TFDS, WDS)
+        input_img_mode: Input image color conversion mode e.g. 'RGB', 'L' (folder, TFDS, WDS, HFDS)
         **kwargs: other args to pass to dataset
 
     Returns:
         Dataset object
     """
+    kwargs = {k: v for k, v in kwargs.items() if v is not None}
     name = name.lower()
     if name.startswith('torch/'):
         name = name.split('/', 2)[-1]
         torch_kwargs = dict(root=root, download=download, **kwargs)
         if name in _TORCH_BASIC_DS:
             ds_class = _TORCH_BASIC_DS[name]
             use_train = split in _TRAIN_SYNONYM
@@ -147,40 +152,73 @@
                 root = _search_split(root, split)
             ds = ImageFolder(root, **kwargs)
         else:
             assert False, f"Unknown torchvision dataset {name}"
     elif name.startswith('hfds/'):
         # NOTE right now, HF datasets default arrow format is a random-access Dataset,
         # There will be a IterableDataset variant too, TBD
-        ds = ImageDataset(root, reader=name, split=split, class_map=class_map, **kwargs)
+        ds = ImageDataset(
+            root,
+            reader=name,
+            split=split,
+            class_map=class_map,
+            input_img_mode=input_img_mode,
+            **kwargs,
+        )
+    elif name.startswith('hfids/'):
+        ds = IterableImageDataset(
+            root,
+            reader=name,
+            split=split,
+            class_map=class_map,
+            is_training=is_training,
+            download=download,
+            batch_size=batch_size,
+            num_samples=num_samples,
+            repeats=repeats,
+            seed=seed,
+            input_img_mode=input_img_mode,
+            **kwargs
+        )
     elif name.startswith('tfds/'):
         ds = IterableImageDataset(
             root,
             reader=name,
             split=split,
             class_map=class_map,
             is_training=is_training,
             download=download,
             batch_size=batch_size,
+            num_samples=num_samples,
             repeats=repeats,
             seed=seed,
+            input_img_mode=input_img_mode,
             **kwargs
         )
     elif name.startswith('wds/'):
         ds = IterableImageDataset(
             root,
             reader=name,
             split=split,
             class_map=class_map,
             is_training=is_training,
             batch_size=batch_size,
+            num_samples=num_samples,
             repeats=repeats,
             seed=seed,
+            input_img_mode=input_img_mode,
             **kwargs
         )
     else:
         # FIXME support more advance split cfg for ImageFolder/Tar datasets in the future
         if search_split and os.path.isdir(root):
             # look for split specific sub-folder in root
             root = _search_split(root, split)
-        ds = ImageDataset(root, reader=name, class_map=class_map, load_bytes=load_bytes, **kwargs)
+        ds = ImageDataset(
+            root,
+            reader=name,
+            class_map=class_map,
+            load_bytes=load_bytes,
+            input_img_mode=input_img_mode,
+            **kwargs,
+        )
     return ds
```

### Comparing `timm-0.9.9/timm/data/dataset_info.py` & `timm-1.0.3/timm/data/dataset_info.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/distributed_sampler.py` & `timm-1.0.3/timm/data/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/imagenet_info.py` & `timm-1.0.3/timm/data/imagenet_info.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/loader.py` & `timm-1.0.3/timm/data/loader.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 Hacked together by / Copyright 2019, Ross Wightman
 """
 import logging
 import random
 from contextlib import suppress
 from functools import partial
 from itertools import repeat
-from typing import Callable
+from typing import Callable, Optional, Tuple, Union
 
 import torch
 import torch.utils.data
 import numpy as np
 
 from .constants import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
-from .dataset import IterableImageDataset
+from .dataset import IterableImageDataset, ImageDataset
 from .distributed_sampler import OrderedDistributedSampler, RepeatAugSampler
 from .random_erasing import RandomErasing
 from .mixup import FastCollateMixup
 from .transforms_factory import create_transform
 
 _logger = logging.getLogger(__name__)
 
@@ -183,74 +183,130 @@
         # random / torch seed already called in dataloader iter class w/ worker_info.seed
         # to reproduce some old results (same seed + hparam combo), partial seeding is required (skip numpy re-seed)
         if worker_seeding == 'all':
             np.random.seed(worker_info.seed % (2 ** 32 - 1))
 
 
 def create_loader(
-        dataset,
-        input_size,
-        batch_size,
-        is_training=False,
-        use_prefetcher=True,
-        no_aug=False,
-        re_prob=0.,
-        re_mode='const',
-        re_count=1,
-        re_split=False,
-        scale=None,
-        ratio=None,
-        hflip=0.5,
-        vflip=0.,
-        color_jitter=0.4,
-        auto_augment=None,
-        num_aug_repeats=0,
-        num_aug_splits=0,
-        interpolation='bilinear',
-        mean=IMAGENET_DEFAULT_MEAN,
-        std=IMAGENET_DEFAULT_STD,
-        num_workers=1,
-        distributed=False,
-        crop_pct=None,
-        crop_mode=None,
-        collate_fn=None,
-        pin_memory=False,
-        fp16=False,  # deprecated, use img_dtype
-        img_dtype=torch.float32,
-        device=torch.device('cuda'),
-        tf_preprocessing=False,
-        use_multi_epochs_loader=False,
-        persistent_workers=True,
-        worker_seeding='all',
+        dataset: Union[ImageDataset, IterableImageDataset],
+        input_size: Union[int, Tuple[int, int], Tuple[int, int, int]],
+        batch_size: int,
+        is_training: bool = False,
+        no_aug: bool = False,
+        re_prob: float = 0.,
+        re_mode: str = 'const',
+        re_count: int = 1,
+        re_split: bool = False,
+        train_crop_mode: Optional[str] = None,
+        scale: Optional[Tuple[float, float]] = None,
+        ratio: Optional[Tuple[float, float]] = None,
+        hflip: float = 0.5,
+        vflip: float = 0.,
+        color_jitter: float = 0.4,
+        color_jitter_prob: Optional[float] = None,
+        grayscale_prob: float = 0.,
+        gaussian_blur_prob: float = 0.,
+        auto_augment: Optional[str] = None,
+        num_aug_repeats: int = 0,
+        num_aug_splits: int = 0,
+        interpolation: str = 'bilinear',
+        mean: Tuple[float, ...] = IMAGENET_DEFAULT_MEAN,
+        std: Tuple[float, ...] = IMAGENET_DEFAULT_STD,
+        num_workers: int = 1,
+        distributed: bool = False,
+        crop_pct: Optional[float] = None,
+        crop_mode: Optional[str] = None,
+        crop_border_pixels: Optional[int] = None,
+        collate_fn: Optional[Callable] = None,
+        pin_memory: bool = False,
+        fp16: bool = False,  # deprecated, use img_dtype
+        img_dtype: torch.dtype = torch.float32,
+        device: torch.device = torch.device('cuda'),
+        use_prefetcher: bool = True,
+        use_multi_epochs_loader: bool = False,
+        persistent_workers: bool = True,
+        worker_seeding: str = 'all',
+        tf_preprocessing: bool = False,
 ):
+    """
+
+    Args:
+        dataset: The image dataset to load.
+        input_size: Target input size (channels, height, width) tuple or size scalar.
+        batch_size: Number of samples in a batch.
+        is_training: Return training (random) transforms.
+        no_aug: Disable augmentation for training (useful for debug).
+        re_prob: Random erasing probability.
+        re_mode: Random erasing fill mode.
+        re_count: Number of random erasing regions.
+        re_split: Control split of random erasing across batch size.
+        scale: Random resize scale range (crop area, < 1.0 => zoom in).
+        ratio: Random aspect ratio range (crop ratio for RRC, ratio adjustment factor for RKR).
+        hflip: Horizontal flip probability.
+        vflip: Vertical flip probability.
+        color_jitter: Random color jitter component factors (brightness, contrast, saturation, hue).
+            Scalar is applied as (scalar,) * 3 (no hue).
+        color_jitter_prob: Apply color jitter with this probability if not None (for SimlCLR-like aug
+        grayscale_prob: Probability of converting image to grayscale (for SimCLR-like aug).
+        gaussian_blur_prob: Probability of applying gaussian blur (for SimCLR-like aug).
+        auto_augment: Auto augment configuration string (see auto_augment.py).
+        num_aug_repeats: Enable special sampler to repeat same augmentation across distributed GPUs.
+        num_aug_splits: Enable mode where augmentations can be split across the batch.
+        interpolation: Image interpolation mode.
+        mean: Image normalization mean.
+        std: Image normalization standard deviation.
+        num_workers: Num worker processes per DataLoader.
+        distributed: Enable dataloading for distributed training.
+        crop_pct: Inference crop percentage (output size / resize size).
+        crop_mode: Inference crop mode. One of ['squash', 'border', 'center']. Defaults to 'center' when None.
+        crop_border_pixels: Inference crop border of specified # pixels around edge of original image.
+        collate_fn: Override default collate_fn.
+        pin_memory: Pin memory for device transfer.
+        fp16: Deprecated argument for half-precision input dtype. Use img_dtype.
+        img_dtype: Data type for input image.
+        device: Device to transfer inputs and targets to.
+        use_prefetcher: Use efficient pre-fetcher to load samples onto device.
+        use_multi_epochs_loader:
+        persistent_workers: Enable persistent worker processes.
+        worker_seeding: Control worker random seeding at init.
+        tf_preprocessing: Use TF 1.0 inference preprocessing for testing model ports.
+
+    Returns:
+        DataLoader
+    """
     re_num_splits = 0
     if re_split:
         # apply RE to second half of batch if no aug split otherwise line up with aug split
         re_num_splits = num_aug_splits or 2
     dataset.transform = create_transform(
         input_size,
         is_training=is_training,
-        use_prefetcher=use_prefetcher,
         no_aug=no_aug,
+        train_crop_mode=train_crop_mode,
         scale=scale,
         ratio=ratio,
         hflip=hflip,
         vflip=vflip,
         color_jitter=color_jitter,
+        color_jitter_prob=color_jitter_prob,
+        grayscale_prob=grayscale_prob,
+        gaussian_blur_prob=gaussian_blur_prob,
         auto_augment=auto_augment,
         interpolation=interpolation,
         mean=mean,
         std=std,
         crop_pct=crop_pct,
         crop_mode=crop_mode,
-        tf_preprocessing=tf_preprocessing,
+        crop_border_pixels=crop_border_pixels,
         re_prob=re_prob,
         re_mode=re_mode,
         re_count=re_count,
         re_num_splits=re_num_splits,
+        tf_preprocessing=tf_preprocessing,
+        use_prefetcher=use_prefetcher,
         separate=num_aug_splits > 0,
     )
 
     if isinstance(dataset, IterableImageDataset):
         # give Iterable datasets early knowledge of num_workers so that sample estimates
         # are correct before worker processes are launched
         dataset.set_loader_cfg(num_workers=num_workers)
```

### Comparing `timm-0.9.9/timm/data/mixup.py` & `timm-1.0.3/timm/data/mixup.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/random_erasing.py` & `timm-1.0.3/timm/data/random_erasing.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/readers/class_map.py` & `timm-1.0.3/timm/data/readers/class_map.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/readers/img_extensions.py` & `timm-1.0.3/timm/data/readers/img_extensions.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/readers/reader_factory.py` & `timm-1.0.3/timm/data/readers/reader_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 import os
+from typing import Optional
 
 from .reader_image_folder import ReaderImageFolder
 from .reader_image_in_tar import ReaderImageInTar
 
 
-def create_reader(name, root, split='train', **kwargs):
+def create_reader(
+        name: str,
+        root: Optional[str] = None,
+        split: str = 'train',
+        **kwargs,
+):
+    kwargs = {k: v for k, v in kwargs.items() if v is not None}
     name = name.lower()
     name = name.split('/', 1)
     prefix = ''
     if len(name) > 1:
         prefix = name[0]
     name = name[-1]
 
     # FIXME improve the selection right now just tfds prefix or fallback path, will need options to
     # explicitly select other options shortly
     if prefix == 'hfds':
-        from .reader_hfds import ReaderHfds  # defer tensorflow import
-        reader = ReaderHfds(root, name, split=split, **kwargs)
+        from .reader_hfds import ReaderHfds  # defer Hf datasets import
+        reader = ReaderHfds(name=name, root=root, split=split, **kwargs)
+    elif prefix == 'hfids':
+        from .reader_hfids import ReaderHfids  # defer HF datasets import
+        reader = ReaderHfids(name=name, root=root, split=split, **kwargs)
     elif prefix == 'tfds':
         from .reader_tfds import ReaderTfds  # defer tensorflow import
-        reader = ReaderTfds(root, name, split=split, **kwargs)
+        reader = ReaderTfds(name=name, root=root, split=split, **kwargs)
     elif prefix == 'wds':
         from .reader_wds import ReaderWds
         kwargs.pop('download', False)
-        reader = ReaderWds(root, name, split=split, **kwargs)
+        reader = ReaderWds(root=root, name=name, split=split, **kwargs)
     else:
         assert os.path.exists(root)
         # default fallback path (backwards compat), use image tar if root is a .tar file, otherwise image folder
         # FIXME support split here or in reader?
         if os.path.isfile(root) and os.path.splitext(root)[1] == '.tar':
             reader = ReaderImageInTar(root, **kwargs)
         else:
```

### Comparing `timm-0.9.9/timm/data/readers/reader_hfds.py` & `timm-1.0.3/timm/data/readers/reader_hfds.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """ Dataset reader that wraps Hugging Face datasets
 
 Hacked together by / Copyright 2022 Ross Wightman
 """
 import io
 import math
+from typing import Optional
+
 import torch
 import torch.distributed as dist
 from PIL import Image
 
 try:
     import datasets
 except ImportError as e:
     print("Please install Hugging Face datasets package `pip install datasets`.")
-    exit(1)
+    raise e
 from .class_map import load_class_map
 from .reader import Reader
 
 
 def get_class_labels(info, label_key='label'):
     if 'label' not in info.features:
         return {}
@@ -25,47 +27,49 @@
     return class_to_idx
 
 
 class ReaderHfds(Reader):
 
     def __init__(
             self,
-            root,
-            name,
-            split='train',
-            class_map=None,
-            label_key='label',
-            download=False,
+            name: str,
+            root: Optional[str] = None,
+            split: str = 'train',
+            class_map: dict = None,
+            image_key: str = 'image',
+            target_key: str = 'label',
+            download: bool = False,
     ):
         """
         """
         super().__init__()
         self.root = root
         self.split = split
         self.dataset = datasets.load_dataset(
             name,  # 'name' maps to path arg in hf datasets
             split=split,
             cache_dir=self.root,  # timm doesn't expect hidden cache dir for datasets, specify a path
         )
         # leave decode for caller, plus we want easy access to original path names...
-        self.dataset = self.dataset.cast_column('image', datasets.Image(decode=False))
+        self.dataset = self.dataset.cast_column(image_key, datasets.Image(decode=False))
 
-        self.label_key = label_key
+        self.image_key = image_key
+        self.label_key = target_key
         self.remap_class = False
         if class_map:
             self.class_to_idx = load_class_map(class_map)
             self.remap_class = True
         else:
             self.class_to_idx = get_class_labels(self.dataset.info, self.label_key)
         self.split_info = self.dataset.info.splits[split]
         self.num_samples = self.split_info.num_examples
 
     def __getitem__(self, index):
         item = self.dataset[index]
-        image = item['image']
+        image = item[self.image_key]
         if 'bytes' in image and image['bytes']:
             image = io.BytesIO(image['bytes'])
         else:
             assert 'path' in image and image['path']
             image = open(image['path'], 'rb')
         label = item[self.label_key]
         if self.remap_class:
@@ -73,8 +77,8 @@
         return image, label
 
     def __len__(self):
         return len(self.dataset)
 
     def _filename(self, index, basename=False, absolute=False):
         item = self.dataset[index]
-        return item['image']['path']
+        return item[self.image_key]['path']
```

### Comparing `timm-0.9.9/timm/data/readers/reader_image_folder.py` & `timm-1.0.3/timm/data/readers/reader_image_folder.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,22 +57,31 @@
 
 
 class ReaderImageFolder(Reader):
 
     def __init__(
             self,
             root,
-            class_map=''):
+            class_map='',
+            input_key=None,
+    ):
         super().__init__()
 
         self.root = root
         class_to_idx = None
         if class_map:
             class_to_idx = load_class_map(class_map, root)
-        self.samples, self.class_to_idx = find_images_and_targets(root, class_to_idx=class_to_idx)
+        find_types = None
+        if input_key:
+            find_types = input_key.split(';')
+        self.samples, self.class_to_idx = find_images_and_targets(
+            root,
+            class_to_idx=class_to_idx,
+            types=find_types,
+        )
         if len(self.samples) == 0:
             raise RuntimeError(
                 f'Found 0 images in subfolders of {root}. '
                 f'Supported image extensions are {", ".join(get_img_extensions())}')
 
     def __getitem__(self, index):
         path, target = self.samples[index]
```

### Comparing `timm-0.9.9/timm/data/readers/reader_image_in_tar.py` & `timm-1.0.3/timm/data/readers/reader_image_in_tar.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/readers/reader_image_tar.py` & `timm-1.0.3/timm/data/readers/reader_image_tar.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/readers/reader_tfds.py` & `timm-1.0.3/timm/data/readers/reader_tfds.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from https://github.com/tensorflow/datasets
 https://www.tensorflow.org/datasets/catalog/overview#image_classification
 
 Hacked together by / Copyright 2020 Ross Wightman
 """
 import math
 import os
+import sys
 from typing import Optional
 
 import torch
 import torch.distributed as dist
 from PIL import Image
 
 try:
@@ -28,31 +29,31 @@
     # NOTE uncomment below if having file limit issues on dataset build (or alter your OS defaults)
     # import resource
     # low, high = resource.getrlimit(resource.RLIMIT_NOFILE)
     # resource.setrlimit(resource.RLIMIT_NOFILE, (high, high))
 except ImportError as e:
     print(e)
     print("Please install tensorflow_datasets package `pip install tensorflow-datasets`.")
-    exit(1)
+    raise e
 
 from .class_map import load_class_map
 from .reader import Reader
 from .shared_count import SharedCount
 
 
 MAX_TP_SIZE = int(os.environ.get('TFDS_TP_SIZE', 8))  # maximum TF threadpool size, for jpeg decodes and queuing activities
 SHUFFLE_SIZE = int(os.environ.get('TFDS_SHUFFLE_SIZE', 8192))  # samples to shuffle in DS queue
 PREFETCH_SIZE = int(os.environ.get('TFDS_PREFETCH_SIZE', 2048))  # samples to prefetch
 
 
 @tfds.decode.make_decoder()
-def decode_example(serialized_image, feature, dct_method='INTEGER_ACCURATE'):
+def decode_example(serialized_image, feature, dct_method='INTEGER_ACCURATE', channels=3):
     return tf.image.decode_jpeg(
         serialized_image,
-        channels=3,
+        channels=channels,
         dct_method=dct_method,
     )
 
 
 def even_split_indices(split, n, num_samples):
     partitions = [round(i * num_samples / n) for i in range(n + 1)]
     return [f"{split}[{partitions[i]}:{partitions[i + 1]}]" for i in range(n)]
@@ -88,26 +89,26 @@
         to specify TF augmentation fn and return augmented batches w/ some modifications to other downstream
         components.
 
     """
 
     def __init__(
             self,
-            root,
             name,
+            root=None,
             split='train',
             class_map=None,
             is_training=False,
-            batch_size=None,
+            batch_size=1,
             download=False,
             repeats=0,
             seed=42,
-            input_name='image',
+            input_key='image',
             input_img_mode='RGB',
-            target_name='label',
+            target_key='label',
             target_img_mode='',
             prefetch_size=None,
             shuffle_size=None,
             max_threadpool_size=None
     ):
         """ Tensorflow-datasets Wrapper
 
@@ -116,53 +117,50 @@
             name: tfds dataset name (eg `imagenet2012`)
             split: tfds dataset split (can use all TFDS split strings eg `train[:10%]`)
             is_training: training mode, shuffle enabled, dataset len rounded by batch_size
             batch_size: batch_size to use to unsure total samples % batch_size == 0 in training across all dis nodes
             download: download and build TFDS dataset if set, otherwise must use tfds CLI
             repeats: iterate through (repeat) the dataset this many times per iteration (once if 0 or 1)
             seed: common seed for shard shuffle across all distributed/worker instances
-            input_name: name of Feature to return as data (input)
+            input_key: name of Feature to return as data (input)
             input_img_mode: image mode if input is an image (currently PIL mode string)
-            target_name: name of Feature to return as target (label)
+            target_key: name of Feature to return as target (label)
             target_img_mode: image mode if target is an image (currently PIL mode string)
             prefetch_size: override default tf.data prefetch buffer size
             shuffle_size: override default tf.data shuffle buffer size
             max_threadpool_size: override default threadpool size for tf.data
         """
         super().__init__()
         self.root = root
         self.split = split
         self.is_training = is_training
-        if self.is_training:
-            assert batch_size is not None, \
-                "Must specify batch_size in training mode for reasonable behaviour w/ TFDS wrapper"
         self.batch_size = batch_size
         self.repeats = repeats
         self.common_seed = seed  # a seed that's fixed across all worker / distributed instances
 
         # performance settings
         self.prefetch_size = prefetch_size or PREFETCH_SIZE
         self.shuffle_size = shuffle_size or SHUFFLE_SIZE
         self.max_threadpool_size = max_threadpool_size or MAX_TP_SIZE
 
         # TFDS builder and split information
-        self.input_name = input_name  # FIXME support tuples / lists of inputs and targets and full range of Feature
+        self.input_key = input_key  # FIXME support tuples / lists of inputs and targets and full range of Feature
         self.input_img_mode = input_img_mode
-        self.target_name = target_name
-        self.target_img_mode = target_img_mode
+        self.target_key = target_key
+        self.target_img_mode = target_img_mode  # for dense pixel targets
         self.builder = tfds.builder(name, data_dir=root)
         # NOTE: the tfds command line app can be used download & prepare datasets if you don't enable download flag
         if download:
             self.builder.download_and_prepare()
         self.remap_class = False
         if class_map:
             self.class_to_idx = load_class_map(class_map)
             self.remap_class = True
         else:
-            self.class_to_idx = get_class_labels(self.builder.info) if self.target_name == 'label' else {}
+            self.class_to_idx = get_class_labels(self.builder.info) if self.target_key == 'label' else {}
         self.split_info = self.builder.info.splits[split]
         self.num_samples = self.split_info.num_examples
 
         # Distributed world state
         self.dist_rank = 0
         self.dist_num_replicas = 1
         if dist.is_available() and dist.is_initialized() and dist.get_world_size() > 1:
@@ -254,15 +252,15 @@
             shuffle_seed=self.common_seed + self.epoch_count.value,
             shuffle_reshuffle_each_iteration=True,
             input_context=input_context,
         )
         ds = self.builder.as_dataset(
             split=self.subsplit or self.split,
             shuffle_files=self.is_training,
-            decoders=dict(image=decode_example()),
+            decoders=dict(image=decode_example(channels=1 if self.input_img_mode == 'L' else 3)),
             read_config=read_config,
         )
         # avoid overloading threading w/ combo of TF ds threads + PyTorch workers
         options = tf.data.Options()
         thread_member = 'threading' if hasattr(options, 'threading') else 'experimental_threading'
         getattr(options, thread_member).private_threadpool_size = max(1, self.max_threadpool_size // self.num_workers)
         getattr(options, thread_member).max_intra_op_parallelism = 1
@@ -278,15 +276,15 @@
         self.init_count += 1
 
     def _num_samples_per_worker(self):
         num_worker_samples = \
             max(1, self.repeats) * self.num_samples / max(self.global_num_workers, self.dist_num_replicas)
         if self.is_training or self.dist_num_replicas > 1:
             num_worker_samples = math.ceil(num_worker_samples)
-        if self.is_training and self.batch_size is not None:
+        if self.is_training:
             num_worker_samples = math.ceil(num_worker_samples / self.batch_size) * self.batch_size
         return int(num_worker_samples)
 
     def __iter__(self):
         if self.ds is None or self.reinit_each_iter:
             self._lazy_init()
 
@@ -296,19 +294,22 @@
         #   2. determine loop ending condition in training w/ repeat enabled so that only full batch_size
         #     batches are produced (underlying tfds iter wraps around)
         target_sample_count = self._num_samples_per_worker()
 
         # Iterate until exhausted or sample count hits target when training (ds.repeat enabled)
         sample_count = 0
         for sample in self.ds:
-            input_data = sample[self.input_name]
+            input_data = sample[self.input_key]
             if self.input_img_mode:
+                if self.input_img_mode == 'L' and input_data.ndim == 3:
+                    input_data = input_data[:, :, 0]
                 input_data = Image.fromarray(input_data, mode=self.input_img_mode)
-            target_data = sample[self.target_name]
+            target_data = sample[self.target_key]
             if self.target_img_mode:
+                # dense pixel target
                 target_data = Image.fromarray(target_data, mode=self.target_img_mode)
             elif self.remap_class:
                 target_data = self.class_to_idx[target_data]
             yield input_data, target_data
             sample_count += 1
             if self.is_training and sample_count >= target_sample_count:
                 # Need to break out of loop when repeat() is enabled for training w/ oversampling
```

### Comparing `timm-0.9.9/timm/data/readers/reader_wds.py` & `timm-1.0.3/timm/data/readers/reader_wds.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,48 +18,51 @@
 import torch.distributed as dist
 import yaml
 from PIL import Image
 from torch.utils.data import Dataset, IterableDataset, get_worker_info
 
 try:
     import webdataset as wds
-    from webdataset.filters import _shuffle
+    from webdataset.filters import _shuffle, getfirst
     from webdataset.shardlists import expand_urls
     from webdataset.tariterators import base_plus_ext, url_opener, tar_file_expander, valid_sample
 except ImportError:
     wds = None
     expand_urls = None
 
 from .class_map import load_class_map
 from .reader import Reader
 from .shared_count import SharedCount
 
 _logger = logging.getLogger(__name__)
 
-SHUFFLE_SIZE = int(os.environ.get('WDS_SHUFFLE_SIZE', 8192))
+SAMPLE_SHUFFLE_SIZE = int(os.environ.get('WDS_SHUFFLE_SIZE', 8192))
+SAMPLE_INITIAL_SIZE = int(os.environ.get('WDS_INITIAL_SIZE', 2048))
 
 
-def _load_info(root, basename='info'):
-    info_json = os.path.join(root, basename + '.json')
-    info_yaml = os.path.join(root, basename + '.yaml')
+def _load_info(root, names=('_info.json', 'info.json')):
+    if isinstance(names, str):
+        names = (names,)
+    tried = []
     err_str = ''
-    try:
-        with wds.gopen(info_json) as f:
-            info_dict = json.load(f)
-        return info_dict
-    except Exception as e:
-        err_str = str(e)
-    try:
-        with wds.gopen(info_yaml) as f:
-            info_dict = yaml.safe_load(f)
-        return info_dict
-    except Exception:
-        pass
+    for n in names:
+        full_path = os.path.join(root, n)
+        try:
+            tried.append(full_path)
+            with wds.gopen(full_path) as f:
+                if n.endswith('.json'):
+                    info_dict = json.load(f)
+                else:
+                    info_dict = yaml.safe_load(f)
+            return info_dict
+        except Exception as e:
+            err_str = str(e)
+
     _logger.warning(
-        f'Dataset info file not found at {info_json} or {info_yaml}. Error: {err_str}. '
+        f'Dataset info file not found at {tried}. Error: {err_str}. '
         'Falling back to provided split and size arg.')
     return {}
 
 
 @dataclass
 class SplitInfo:
     num_samples: int
@@ -117,23 +120,26 @@
         split_info = info['splits'][split]
         split_info = _info_convert(split_info)
 
     return split_info
 
 
 def log_and_continue(exn):
-    """Call in an exception handler to ignore any exception, isssue a warning, and continue."""
+    """Call in an exception handler to ignore exceptions, isssue a warning, and continue."""
     _logger.warning(f'Handling webdataset error ({repr(exn)}). Ignoring.')
+    # NOTE: try force an exit on errors that are clearly code / config and not transient
+    if isinstance(exn, TypeError):
+        raise exn
     return True
 
 
 def _decode(
         sample,
         image_key='jpg',
-        image_format='RGB',
+        image_mode='RGB',
         target_key='cls',
         alt_label=''
 ):
     """ Custom sample decode
     * decode and convert PIL Image
     * cls byte string label to int
     * pass through JSON byte string (if it exists) without parse
@@ -146,67 +152,39 @@
         if class_label < 0:
             # skipped labels currently encoded as -1, may change to a null/None value
             return None
     else:
         class_label = int(sample[target_key])
 
     # decode image
-    with io.BytesIO(sample[image_key]) as b:
+    img = getfirst(sample, image_key)
+    with io.BytesIO(img) as b:
         img = Image.open(b)
         img.load()
-    if image_format:
-        img = img.convert(image_format)
+    if image_mode:
+        img = img.convert(image_mode)
 
     # json passed through in undecoded state
     decoded = dict(jpg=img, cls=class_label, json=sample.get('json', None))
     return decoded
 
 
-def _decode_samples(
-        data,
-        image_key='jpg',
-        image_format='RGB',
-        target_key='cls',
-        alt_label='',
-        handler=log_and_continue):
-    """Decode samples with skip."""
-    for sample in data:
-        try:
-            result = _decode(
-                sample,
-                image_key=image_key,
-                image_format=image_format,
-                target_key=target_key,
-                alt_label=alt_label
-            )
-        except Exception as exn:
-            if handler(exn):
-                continue
-            else:
-                break
-
-        # null results are skipped
-        if result is not None:
-            if isinstance(sample, dict) and isinstance(result, dict):
-                result["__key__"] = sample.get("__key__")
-            yield result
-
-
 def pytorch_worker_seed():
     """get dataloader worker seed from pytorch"""
     worker_info = get_worker_info()
     if worker_info is not None:
         # favour the seed already created for pytorch dataloader workers if it exists
         return worker_info.seed
     # fallback to wds rank based seed
     return wds.utils.pytorch_worker_seed()
 
 
 if wds is not None:
     # conditional to avoid mandatory wds import (via inheritance of wds.PipelineStage)
+
     class detshuffle2(wds.PipelineStage):
         def __init__(
                 self,
                 bufsize=1000,
                 initial=100,
                 seed=0,
                 epoch=-1,
@@ -280,52 +258,58 @@
             index = self.rng.randint(0, len(self.urls) - 1)
             yield dict(url=self.urls[index])
 
 
 class ReaderWds(Reader):
     def __init__(
             self,
-            root,
-            name,
-            split,
-            is_training=False,
-            batch_size=None,
-            repeats=0,
-            seed=42,
-            class_map=None,
-            input_name='jpg',
-            input_image='RGB',
-            target_name='cls',
-            target_image='',
-            prefetch_size=None,
-            shuffle_size=None,
+            root: str,
+            name: Optional[str] = None,
+            split: str = 'train',
+            is_training: bool = False,
+            num_samples: Optional[int] = None,
+            batch_size: int = 1,
+            repeats: int = 0,
+            seed: int = 42,
+            class_map: Optional[dict] = None,
+            input_key: str = 'jpg;png;webp',
+            input_img_mode: str = 'RGB',
+            target_key: str = 'cls',
+            target_img_mode: str = '',
+            filename_key: str = 'filename',
+            sample_shuffle_size: Optional[int] = None,
+            smaple_initial_size: Optional[int] = None,
     ):
         super().__init__()
         if wds is None:
             raise RuntimeError(
                 'Please install webdataset 0.2.x package `pip install git+https://github.com/webdataset/webdataset`.')
         self.root = root
         self.is_training = is_training
         self.batch_size = batch_size
         self.repeats = repeats
         self.common_seed = seed  # a seed that's fixed across all worker / distributed instances
         self.shard_shuffle_size = 500
-        self.sample_shuffle_size = shuffle_size or SHUFFLE_SIZE
+        self.sample_shuffle_size = sample_shuffle_size or SAMPLE_SHUFFLE_SIZE
+        self.sample_initial_size = smaple_initial_size or SAMPLE_INITIAL_SIZE
 
-        self.image_key = input_name
-        self.image_format = input_image
-        self.target_key = target_name
-        self.filename_key = 'filename'
+        self.input_key = input_key
+        self.input_img_mode = input_img_mode
+        self.target_key = target_key
+        self.filename_key = filename_key
         self.key_ext = '.JPEG'  # extension to add to key for original filenames (DS specific, default ImageNet)
 
         self.info = _load_info(self.root)
         self.split_info = _parse_split_info(split, self.info)
-        self.num_samples = self.split_info.num_samples
+        if num_samples is not None:
+            self.num_samples = num_samples
+        else:
+            self.num_samples = self.split_info.num_samples
         if not self.num_samples:
-            raise RuntimeError(f'Invalid split definition, no samples found.')
+            raise RuntimeError(f'Invalid split definition, num_samples not specified.')
         self.remap_class = False
         if class_map:
             self.class_to_idx = load_class_map(class_map)
             self.remap_class = True
         else:
             self.class_to_idx = {}
 
@@ -342,15 +326,15 @@
         self.worker_seed = seed  # seed unique to each worker instance
         self.num_workers = 1
         self.global_worker_id = 0
         self.global_num_workers = 1
         self.init_count = 0
         self.epoch_count = SharedCount()
 
-        # DataPipeline is lazy init, majority of WDS DataPipeline could be init here, BUT, shuffle seed
+        # DataPipeline is lazy init, the majority of WDS DataPipeline could be init here, BUT, shuffle seed
         # is not handled in manner where it can be deterministic for each worker AND initialized up front
         self.ds = None
 
     def set_epoch(self, count):
         self.epoch_count.value = count
 
     def set_loader_cfg(
@@ -378,35 +362,45 @@
 
         # init data pipeline
         abs_shard_filenames = [os.path.join(self.root, f) for f in self.split_info.filenames]
         pipeline = [wds.SimpleShardList(abs_shard_filenames)]
         # at this point we have an iterator over all the shards
         if self.is_training:
             pipeline.extend([
-                detshuffle2(self.shard_shuffle_size, seed=self.common_seed, epoch=self.epoch_count),
+                detshuffle2(
+                    self.shard_shuffle_size,
+                    seed=self.common_seed,
+                    epoch=self.epoch_count,
+                ),
                 self._split_by_node_and_worker,
                 # at this point, we have an iterator over the shards assigned to each worker
                 wds.tarfile_to_samples(handler=log_and_continue),
                 wds.shuffle(
-                    self.sample_shuffle_size,
-                    rng=random.Random(self.worker_seed)),  # this is why we lazy-init whole DataPipeline
+                    bufsize=self.sample_shuffle_size,
+                    initial=self.sample_initial_size,
+                    rng=random.Random(self.worker_seed) # this is why we lazy-init whole DataPipeline
+                ),
             ])
         else:
             pipeline.extend([
                 self._split_by_node_and_worker,
                 # at this point, we have an iterator over the shards assigned to each worker
                 wds.tarfile_to_samples(handler=log_and_continue),
             ])
         pipeline.extend([
-            partial(
-                _decode_samples,
-                image_key=self.image_key,
-                image_format=self.image_format,
-                alt_label=self.split_info.alt_label
-            )
+            wds.map(
+                partial(
+                    _decode,
+                    image_key=self.input_key,
+                    image_mode=self.input_img_mode,
+                    alt_label=self.split_info.alt_label,
+                ),
+                handler=log_and_continue,
+            ),
+            wds.rename(image=self.input_key, target=self.target_key)
         ])
         self.ds = wds.DataPipeline(*pipeline)
 
     def _split_by_node_and_worker(self, src):
         if self.global_num_workers > 1:
             for s in islice(src, self.global_worker_id, None, self.global_num_workers):
                 yield s
@@ -414,15 +408,15 @@
             for s in src:
                 yield s
 
     def _num_samples_per_worker(self):
         num_worker_samples = self.num_samples / max(self.global_num_workers, self.dist_num_replicas)
         if self.is_training or self.dist_num_replicas > 1:
             num_worker_samples = math.ceil(num_worker_samples)
-        if self.is_training and self.batch_size is not None:
+        if self.is_training:
             num_worker_samples = math.ceil(num_worker_samples / self.batch_size) * self.batch_size
         return int(num_worker_samples)
 
     def __iter__(self):
         if self.ds is None:
             self._lazy_init()
 
@@ -435,18 +429,18 @@
             ds = self.ds.with_epoch(num_worker_samples)
         else:
             ds = self.ds
 
         i = 0
         # _logger.info(f'start {i}, {self.worker_id}')  # FIXME temporary debug
         for sample in ds:
-            target = sample[self.target_key]
+            target = sample['target']
             if self.remap_class:
                 target = self.class_to_idx[target]
-            yield sample[self.image_key], target
+            yield sample['image'], target
             i += 1
         # _logger.info(f'end {i}, {self.worker_id}')  # FIXME temporary debug
 
     def __len__(self):
         num_samples = self._num_samples_per_worker() * self.num_workers
         return num_samples
```

### Comparing `timm-0.9.9/timm/data/real_labels.py` & `timm-1.0.3/timm/data/real_labels.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/data/tf_preprocessing.py` & `timm-1.0.3/timm/data/tf_preprocessing.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/__init__.py` & `timm-1.0.3/timm/layers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .evo_norm import EvoNorm2dB0, EvoNorm2dB1, EvoNorm2dB2,\
     EvoNorm2dS0, EvoNorm2dS0a, EvoNorm2dS1, EvoNorm2dS1a, EvoNorm2dS2, EvoNorm2dS2a
 from .fast_norm import is_fast_norm, set_fast_norm, fast_group_norm, fast_layer_norm
 from .filter_response_norm import FilterResponseNormTlu2d, FilterResponseNormAct2d
 from .format import Format, get_channel_dim, get_spatial_dim, nchw_to, nhwc_to
 from .gather_excite import GatherExcite
 from .global_context import GlobalContext
+from .grid import ndgrid, meshgrid
 from .helpers import to_ntuple, to_2tuple, to_3tuple, to_4tuple, make_divisible, extend_tuple
 from .inplace_abn import InplaceAbn
 from .linear import Linear
 from .mixed_conv2d import MixedConv2d
 from .mlp import Mlp, GluMlp, GatedMlp, SwiGLU, SwiGLUPacked, ConvMlp, GlobalResponseNormMlp
 from .non_local_attn import NonLocalAttn, BatNonLocalAttn
 from .norm import GroupNorm, GroupNorm1, LayerNorm, LayerNorm2d, RmsNorm
@@ -42,15 +43,15 @@
     resize_rel_pos_bias_table, resize_rel_pos_bias_table_simple, resize_rel_pos_bias_table_levit
 from .pos_embed_sincos import pixel_freq_bands, freq_bands, build_sincos2d_pos_embed, build_fourier_pos_embed, \
     build_rotary_pos_embed, apply_rot_embed, apply_rot_embed_cat, apply_rot_embed_list, apply_keep_indices_nlc, \
     FourierEmbed, RotaryEmbedding, RotaryEmbeddingCat
 from .squeeze_excite import SEModule, SqueezeExcite, EffectiveSEModule, EffectiveSqueezeExcite
 from .selective_kernel import SelectiveKernel
 from .separable_conv import SeparableConv2d, SeparableConvNormAct
-from .space_to_depth import SpaceToDepthModule, SpaceToDepth, DepthToSpace
+from .space_to_depth import SpaceToDepth, DepthToSpace
 from .split_attn import SplitAttn
 from .split_batchnorm import SplitBatchNorm2d, convert_splitbn_model
 from .std_conv import StdConv2d, StdConv2dSame, ScaledStdConv2d, ScaledStdConv2dSame
 from .test_time_pool import TestTimePoolHead, apply_test_time_pool
 from .trace_utils import _assert, _float_to_int
 from .typing import LayerType, PadType
 from .weight_init import trunc_normal_, trunc_normal_tf_, variance_scaling_, lecun_normal_
```

### Comparing `timm-0.9.9/timm/layers/activations.py` & `timm-1.0.3/timm/layers/activations.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/activations_me.py` & `timm-1.0.3/timm/layers/activations_me.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,218 +1,208 @@
 """ Activations (memory-efficient w/ custom autograd)
 
 A collection of activations fn and modules with a common interface so that they can
 easily be swapped. All have an `inplace` arg even if not used.
 
-These activations are not compatible with jit scripting or ONNX export of the model, please use either
-the JIT or basic versions of the activations.
+These activations are not compatible with jit scripting or ONNX export of the model, please use
+basic versions of the activations.
 
 Hacked together by / Copyright 2020 Ross Wightman
 """
 
 import torch
 from torch import nn as nn
 from torch.nn import functional as F
 
 
-@torch.jit.script
-def swish_jit_fwd(x):
+def swish_fwd(x):
     return x.mul(torch.sigmoid(x))
 
 
-@torch.jit.script
-def swish_jit_bwd(x, grad_output):
+def swish_bwd(x, grad_output):
     x_sigmoid = torch.sigmoid(x)
     return grad_output * (x_sigmoid * (1 + x * (1 - x_sigmoid)))
 
 
-class SwishJitAutoFn(torch.autograd.Function):
-    """ torch.jit.script optimised Swish w/ memory-efficient checkpoint
+class SwishAutoFn(torch.autograd.Function):
+    """ optimised Swish w/ memory-efficient checkpoint
     Inspired by conversation btw Jeremy Howard & Adam Pazske
     https://twitter.com/jeremyphoward/status/1188251041835315200
     """
     @staticmethod
     def symbolic(g, x):
         return g.op("Mul", x, g.op("Sigmoid", x))
 
     @staticmethod
     def forward(ctx, x):
         ctx.save_for_backward(x)
-        return swish_jit_fwd(x)
+        return swish_fwd(x)
 
     @staticmethod
     def backward(ctx, grad_output):
         x = ctx.saved_tensors[0]
-        return swish_jit_bwd(x, grad_output)
+        return swish_bwd(x, grad_output)
 
 
 def swish_me(x, inplace=False):
-    return SwishJitAutoFn.apply(x)
+    return SwishAutoFn.apply(x)
 
 
 class SwishMe(nn.Module):
     def __init__(self, inplace: bool = False):
         super(SwishMe, self).__init__()
 
     def forward(self, x):
-        return SwishJitAutoFn.apply(x)
+        return SwishAutoFn.apply(x)
 
 
-@torch.jit.script
-def mish_jit_fwd(x):
+def mish_fwd(x):
     return x.mul(torch.tanh(F.softplus(x)))
 
 
-@torch.jit.script
-def mish_jit_bwd(x, grad_output):
+def mish_bwd(x, grad_output):
     x_sigmoid = torch.sigmoid(x)
     x_tanh_sp = F.softplus(x).tanh()
     return grad_output.mul(x_tanh_sp + x * x_sigmoid * (1 - x_tanh_sp * x_tanh_sp))
 
 
-class MishJitAutoFn(torch.autograd.Function):
+class MishAutoFn(torch.autograd.Function):
     """ Mish: A Self Regularized Non-Monotonic Neural Activation Function - https://arxiv.org/abs/1908.08681
-    A memory efficient, jit scripted variant of Mish
+    A memory efficient variant of Mish
     """
     @staticmethod
     def forward(ctx, x):
         ctx.save_for_backward(x)
-        return mish_jit_fwd(x)
+        return mish_fwd(x)
 
     @staticmethod
     def backward(ctx, grad_output):
         x = ctx.saved_tensors[0]
-        return mish_jit_bwd(x, grad_output)
+        return mish_bwd(x, grad_output)
 
 
 def mish_me(x, inplace=False):
-    return MishJitAutoFn.apply(x)
+    return MishAutoFn.apply(x)
 
 
 class MishMe(nn.Module):
     def __init__(self, inplace: bool = False):
         super(MishMe, self).__init__()
 
     def forward(self, x):
-        return MishJitAutoFn.apply(x)
+        return MishAutoFn.apply(x)
 
 
-@torch.jit.script
-def hard_sigmoid_jit_fwd(x, inplace: bool = False):
+def hard_sigmoid_fwd(x, inplace: bool = False):
     return (x + 3).clamp(min=0, max=6).div(6.)
 
 
-@torch.jit.script
-def hard_sigmoid_jit_bwd(x, grad_output):
+def hard_sigmoid_bwd(x, grad_output):
     m = torch.ones_like(x) * ((x >= -3.) & (x <= 3.)) / 6.
     return grad_output * m
 
 
-class HardSigmoidJitAutoFn(torch.autograd.Function):
+class HardSigmoidAutoFn(torch.autograd.Function):
     @staticmethod
     def forward(ctx, x):
         ctx.save_for_backward(x)
-        return hard_sigmoid_jit_fwd(x)
+        return hard_sigmoid_fwd(x)
 
     @staticmethod
     def backward(ctx, grad_output):
         x = ctx.saved_tensors[0]
-        return hard_sigmoid_jit_bwd(x, grad_output)
+        return hard_sigmoid_bwd(x, grad_output)
 
 
 def hard_sigmoid_me(x, inplace: bool = False):
-    return HardSigmoidJitAutoFn.apply(x)
+    return HardSigmoidAutoFn.apply(x)
 
 
 class HardSigmoidMe(nn.Module):
     def __init__(self, inplace: bool = False):
         super(HardSigmoidMe, self).__init__()
 
     def forward(self, x):
-        return HardSigmoidJitAutoFn.apply(x)
+        return HardSigmoidAutoFn.apply(x)
 
 
-@torch.jit.script
-def hard_swish_jit_fwd(x):
+def hard_swish_fwd(x):
     return x * (x + 3).clamp(min=0, max=6).div(6.)
 
 
-@torch.jit.script
-def hard_swish_jit_bwd(x, grad_output):
+def hard_swish_bwd(x, grad_output):
     m = torch.ones_like(x) * (x >= 3.)
     m = torch.where((x >= -3.) & (x <= 3.),  x / 3. + .5, m)
     return grad_output * m
 
 
-class HardSwishJitAutoFn(torch.autograd.Function):
-    """A memory efficient, jit-scripted HardSwish activation"""
+class HardSwishAutoFn(torch.autograd.Function):
+    """A memory efficient HardSwish activation"""
     @staticmethod
     def forward(ctx, x):
         ctx.save_for_backward(x)
-        return hard_swish_jit_fwd(x)
+        return hard_swish_fwd(x)
 
     @staticmethod
     def backward(ctx, grad_output):
         x = ctx.saved_tensors[0]
-        return hard_swish_jit_bwd(x, grad_output)
+        return hard_swish_bwd(x, grad_output)
 
     @staticmethod
     def symbolic(g, self):
         input = g.op("Add", self, g.op('Constant', value_t=torch.tensor(3, dtype=torch.float)))
         hardtanh_ = g.op("Clip", input, g.op('Constant', value_t=torch.tensor(0, dtype=torch.float)), g.op('Constant', value_t=torch.tensor(6, dtype=torch.float)))
         hardtanh_ = g.op("Div", hardtanh_, g.op('Constant', value_t=torch.tensor(6, dtype=torch.float)))
         return g.op("Mul", self, hardtanh_)
 
 
 def hard_swish_me(x, inplace=False):
-    return HardSwishJitAutoFn.apply(x)
+    return HardSwishAutoFn.apply(x)
 
 
 class HardSwishMe(nn.Module):
     def __init__(self, inplace: bool = False):
         super(HardSwishMe, self).__init__()
 
     def forward(self, x):
-        return HardSwishJitAutoFn.apply(x)
+        return HardSwishAutoFn.apply(x)
 
 
-@torch.jit.script
-def hard_mish_jit_fwd(x):
+def hard_mish_fwd(x):
     return 0.5 * x * (x + 2).clamp(min=0, max=2)
 
 
-@torch.jit.script
-def hard_mish_jit_bwd(x, grad_output):
+def hard_mish_bwd(x, grad_output):
     m = torch.ones_like(x) * (x >= -2.)
     m = torch.where((x >= -2.) & (x <= 0.), x + 1., m)
     return grad_output * m
 
 
-class HardMishJitAutoFn(torch.autograd.Function):
-    """ A memory efficient, jit scripted variant of Hard Mish
+class HardMishAutoFn(torch.autograd.Function):
+    """ A memory efficient variant of Hard Mish
     Experimental, based on notes by Mish author Diganta Misra at
       https://github.com/digantamisra98/H-Mish/blob/0da20d4bc58e696b6803f2523c58d3c8a82782d0/README.md
     """
     @staticmethod
     def forward(ctx, x):
         ctx.save_for_backward(x)
-        return hard_mish_jit_fwd(x)
+        return hard_mish_fwd(x)
 
     @staticmethod
     def backward(ctx, grad_output):
         x = ctx.saved_tensors[0]
-        return hard_mish_jit_bwd(x, grad_output)
+        return hard_mish_bwd(x, grad_output)
 
 
 def hard_mish_me(x, inplace: bool = False):
-    return HardMishJitAutoFn.apply(x)
+    return HardMishAutoFn.apply(x)
 
 
 class HardMishMe(nn.Module):
     def __init__(self, inplace: bool = False):
         super(HardMishMe, self).__init__()
 
     def forward(self, x):
-        return HardMishJitAutoFn.apply(x)
+        return HardMishAutoFn.apply(x)
```

### Comparing `timm-0.9.9/timm/layers/adaptive_avgmax_pool.py` & `timm-1.0.3/timm/layers/adaptive_avgmax_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -130,38 +130,43 @@
             pool_type: str = 'fast',
             flatten: bool = False,
             input_fmt: str = 'NCHW',
     ):
         super(SelectAdaptivePool2d, self).__init__()
         assert input_fmt in ('NCHW', 'NHWC')
         self.pool_type = pool_type or ''  # convert other falsy values to empty string for consistent TS typing
+        pool_type = pool_type.lower()
         if not pool_type:
             self.pool = nn.Identity()  # pass through
             self.flatten = nn.Flatten(1) if flatten else nn.Identity()
         elif pool_type.startswith('fast') or input_fmt != 'NCHW':
             assert output_size == 1, 'Fast pooling and non NCHW input formats require output_size == 1.'
-            if pool_type.endswith('avgmax'):
-                self.pool = FastAdaptiveAvgMaxPool(flatten, input_fmt=input_fmt)
-            elif pool_type.endswith('catavgmax'):
+            if pool_type.endswith('catavgmax'):
                 self.pool = FastAdaptiveCatAvgMaxPool(flatten, input_fmt=input_fmt)
+            elif pool_type.endswith('avgmax'):
+                self.pool = FastAdaptiveAvgMaxPool(flatten, input_fmt=input_fmt)
             elif pool_type.endswith('max'):
                 self.pool = FastAdaptiveMaxPool(flatten, input_fmt=input_fmt)
-            else:
+            elif pool_type == 'fast' or pool_type.endswith('avg'):
                 self.pool = FastAdaptiveAvgPool(flatten, input_fmt=input_fmt)
+            else:
+                assert False, 'Invalid pool type: %s' % pool_type
             self.flatten = nn.Identity()
         else:
             assert input_fmt == 'NCHW'
             if pool_type == 'avgmax':
                 self.pool = AdaptiveAvgMaxPool2d(output_size)
             elif pool_type == 'catavgmax':
                 self.pool = AdaptiveCatAvgMaxPool2d(output_size)
             elif pool_type == 'max':
                 self.pool = nn.AdaptiveMaxPool2d(output_size)
-            else:
+            elif pool_type == 'avg':
                 self.pool = nn.AdaptiveAvgPool2d(output_size)
+            else:
+                assert False, 'Invalid pool type: %s' % pool_type
             self.flatten = nn.Flatten(1) if flatten else nn.Identity()
 
     def is_identity(self):
         return not self.pool_type
 
     def forward(self, x):
         x = self.pool(x)
```

### Comparing `timm-0.9.9/timm/layers/attention_pool.py` & `timm-1.0.3/timm/layers/attention_pool.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/attention_pool2d.py` & `timm-1.0.3/timm/layers/attention_pool2d.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/blur_pool.py` & `timm-1.0.3/timm/layers/blur_pool.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/bottleneck_attn.py` & `timm-1.0.3/timm/layers/bottleneck_attn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/cbam.py` & `timm-1.0.3/timm/layers/cbam.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/classifier.py` & `timm-1.0.3/timm/layers/classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             input_fmt=input_fmt,
         )
         self.global_pool = global_pool
         self.drop = nn.Dropout(drop_rate)
         self.fc = fc
         self.flatten = nn.Flatten(1) if use_conv and pool_type else nn.Identity()
 
-    def reset(self, num_classes, pool_type=None):
+    def reset(self, num_classes: int, pool_type: Optional[str] = None):
         if pool_type is not None and pool_type != self.global_pool.pool_type:
             self.global_pool, self.fc = create_classifier(
                 self.in_features,
                 num_classes,
                 pool_type=pool_type,
                 use_conv=self.use_conv,
                 input_fmt=self.input_fmt,
@@ -176,18 +176,18 @@
             ]))
             self.num_features = hidden_size
         else:
             self.pre_logits = nn.Identity()
         self.drop = nn.Dropout(drop_rate)
         self.fc = linear_layer(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
 
-    def reset(self, num_classes, global_pool=None):
-        if global_pool is not None:
-            self.global_pool = SelectAdaptivePool2d(pool_type=global_pool)
-            self.flatten = nn.Flatten(1) if global_pool else nn.Identity()
+    def reset(self, num_classes: int, pool_type: Optional[str] = None):
+        if pool_type is not None:
+            self.global_pool = SelectAdaptivePool2d(pool_type=pool_type)
+            self.flatten = nn.Flatten(1) if pool_type else nn.Identity()
         self.use_conv = self.global_pool.is_identity()
         linear_layer = partial(nn.Conv2d, kernel_size=1) if self.use_conv else nn.Linear
         if self.hidden_size:
             if ((isinstance(self.pre_logits.fc, nn.Conv2d) and not self.use_conv) or
                     (isinstance(self.pre_logits.fc, nn.Linear) and self.use_conv)):
                 with torch.no_grad():
                     new_fc = linear_layer(self.in_features, self.hidden_size)
```

### Comparing `timm-0.9.9/timm/layers/cond_conv2d.py` & `timm-1.0.3/timm/layers/cond_conv2d.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/config.py` & `timm-1.0.3/timm/layers/config.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/conv2d_same.py` & `timm-1.0.3/timm/layers/conv2d_same.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/conv_bn_act.py` & `timm-1.0.3/timm/layers/conv_bn_act.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/create_act.py` & `timm-1.0.3/timm/layers/create_act.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """ Activation Factory
 Hacked together by / Copyright 2020 Ross Wightman
 """
 from typing import Union, Callable, Type
 
 from .activations import *
-from .activations_jit import *
 from .activations_me import *
-from .config import is_exportable, is_scriptable, is_no_jit
+from .config import is_exportable, is_scriptable
 
 # PyTorch has an optimized, native 'silu' (aka 'swish') operator as of PyTorch 1.7.
 # Also hardsigmoid, hardswish, and soon mish. This code will use native version if present.
 # Eventually, the custom SiLU, Mish, Hard*, layers will be removed and only native variants will be used.
 _has_silu = 'silu' in dir(torch.nn.functional)
 _has_hardswish = 'hardswish' in dir(torch.nn.functional)
 _has_hardsigmoid = 'hardsigmoid' in dir(torch.nn.functional)
@@ -33,33 +32,24 @@
     sigmoid=sigmoid,
     tanh=tanh,
     hard_sigmoid=F.hardsigmoid if _has_hardsigmoid else hard_sigmoid,
     hard_swish=F.hardswish if _has_hardswish else hard_swish,
     hard_mish=hard_mish,
 )
 
-_ACT_FN_JIT = dict(
-    silu=F.silu if _has_silu else swish_jit,
-    swish=F.silu if _has_silu else swish_jit,
-    mish=F.mish if _has_mish else mish_jit,
-    hard_sigmoid=F.hardsigmoid if _has_hardsigmoid else hard_sigmoid_jit,
-    hard_swish=F.hardswish if _has_hardswish else hard_swish_jit,
-    hard_mish=hard_mish_jit,
-)
-
 _ACT_FN_ME = dict(
     silu=F.silu if _has_silu else swish_me,
     swish=F.silu if _has_silu else swish_me,
     mish=F.mish if _has_mish else mish_me,
     hard_sigmoid=F.hardsigmoid if _has_hardsigmoid else hard_sigmoid_me,
     hard_swish=F.hardswish if _has_hardswish else hard_swish_me,
     hard_mish=hard_mish_me,
 )
 
-_ACT_FNS = (_ACT_FN_ME, _ACT_FN_JIT, _ACT_FN_DEFAULT)
+_ACT_FNS = (_ACT_FN_ME, _ACT_FN_DEFAULT)
 for a in _ACT_FNS:
     a.setdefault('hardsigmoid', a.get('hard_sigmoid'))
     a.setdefault('hardswish', a.get('hard_swish'))
 
 
 _ACT_LAYER_DEFAULT = dict(
     silu=nn.SiLU if _has_silu else Swish,
@@ -79,55 +69,43 @@
     tanh=Tanh,
     hard_sigmoid=nn.Hardsigmoid if _has_hardsigmoid else HardSigmoid,
     hard_swish=nn.Hardswish if _has_hardswish else HardSwish,
     hard_mish=HardMish,
     identity=nn.Identity,
 )
 
-_ACT_LAYER_JIT = dict(
-    silu=nn.SiLU if _has_silu else SwishJit,
-    swish=nn.SiLU if _has_silu else SwishJit,
-    mish=nn.Mish if _has_mish else MishJit,
-    hard_sigmoid=nn.Hardsigmoid if _has_hardsigmoid else HardSigmoidJit,
-    hard_swish=nn.Hardswish if _has_hardswish else HardSwishJit,
-    hard_mish=HardMishJit,
-)
-
 _ACT_LAYER_ME = dict(
     silu=nn.SiLU if _has_silu else SwishMe,
     swish=nn.SiLU if _has_silu else SwishMe,
     mish=nn.Mish if _has_mish else MishMe,
     hard_sigmoid=nn.Hardsigmoid if _has_hardsigmoid else HardSigmoidMe,
     hard_swish=nn.Hardswish if _has_hardswish else HardSwishMe,
     hard_mish=HardMishMe,
 )
 
-_ACT_LAYERS = (_ACT_LAYER_ME, _ACT_LAYER_JIT, _ACT_LAYER_DEFAULT)
+_ACT_LAYERS = (_ACT_LAYER_ME, _ACT_LAYER_DEFAULT)
 for a in _ACT_LAYERS:
     a.setdefault('hardsigmoid', a.get('hard_sigmoid'))
     a.setdefault('hardswish', a.get('hard_swish'))
 
 
 def get_act_fn(name: Union[Callable, str] = 'relu'):
     """ Activation Function Factory
     Fetching activation fns by name with this function allows export or torch script friendly
     functions to be returned dynamically based on current config.
     """
     if not name:
         return None
     if isinstance(name, Callable):
         return name
-    if not (is_no_jit() or is_exportable() or is_scriptable()):
+    if not (is_exportable() or is_scriptable()):
         # If not exporting or scripting the model, first look for a memory-efficient version with
         # custom autograd, then fallback
         if name in _ACT_FN_ME:
             return _ACT_FN_ME[name]
-    if not (is_no_jit() or is_exportable()):
-        if name in _ACT_FN_JIT:
-            return _ACT_FN_JIT[name]
     return _ACT_FN_DEFAULT[name]
 
 
 def get_act_layer(name: Union[Type[nn.Module], str] = 'relu'):
     """ Activation Layer Factory
     Fetching activation layers by name with this function allows export or torch script friendly
     functions to be returned dynamically based on current config.
@@ -135,24 +113,21 @@
     if name is None:
         return None
     if not isinstance(name, str):
         # callable, module, etc
         return name
     if not name:
         return None
-    if not (is_no_jit() or is_exportable() or is_scriptable()):
+    if not (is_exportable() or is_scriptable()):
         if name in _ACT_LAYER_ME:
             return _ACT_LAYER_ME[name]
-    if not (is_no_jit() or is_exportable()):
-        if name in _ACT_LAYER_JIT:
-            return _ACT_LAYER_JIT[name]
     return _ACT_LAYER_DEFAULT[name]
 
 
-def create_act_layer(name: Union[nn.Module, str], inplace=None, **kwargs):
+def create_act_layer(name: Union[Type[nn.Module], str], inplace=None, **kwargs):
     act_layer = get_act_layer(name)
     if act_layer is None:
         return None
     if inplace is None:
         return act_layer(**kwargs)
     try:
         return act_layer(inplace=inplace, **kwargs)
```

### Comparing `timm-0.9.9/timm/layers/create_attn.py` & `timm-1.0.3/timm/layers/create_attn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/create_conv2d.py` & `timm-1.0.3/timm/layers/create_conv2d.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/create_norm.py` & `timm-1.0.3/timm/layers/create_norm.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import functools
 import types
 from typing import Type
 
 import torch.nn as nn
 
 from .norm import GroupNorm, GroupNorm1, LayerNorm, LayerNorm2d, RmsNorm
-from torchvision.ops import FrozenBatchNorm2d
+from torchvision.ops.misc import FrozenBatchNorm2d
 
 _NORM_MAP = dict(
     batchnorm=nn.BatchNorm2d,
     batchnorm2d=nn.BatchNorm2d,
     batchnorm1d=nn.BatchNorm1d,
     groupnorm=GroupNorm,
     groupnorm1=GroupNorm1,
@@ -43,15 +43,15 @@
     if isinstance(norm_layer, functools.partial):
         norm_kwargs.update(norm_layer.keywords)
         norm_layer = norm_layer.func
 
     if isinstance(norm_layer, str):
         if not norm_layer:
             return None
-        layer_name = norm_layer.replace('_', '')
+        layer_name = norm_layer.replace('_', '').lower()
         norm_layer = _NORM_MAP[layer_name]
     else:
         norm_layer = norm_layer
 
     if norm_kwargs:
         norm_layer = functools.partial(norm_layer, **norm_kwargs)  # bind/rebind args
     return norm_layer
```

### Comparing `timm-0.9.9/timm/layers/create_norm_act.py` & `timm-1.0.3/timm/layers/create_norm_act.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/drop.py` & `timm-1.0.3/timm/layers/drop.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,32 +14,40 @@
 
 Hacked together by / Copyright 2020 Ross Wightman
 """
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from .grid import ndgrid
+
 
 def drop_block_2d(
-        x, drop_prob: float = 0.1, block_size: int = 7, gamma_scale: float = 1.0,
-        with_noise: bool = False, inplace: bool = False, batchwise: bool = False):
+        x,
+        drop_prob: float = 0.1,
+        block_size: int = 7,
+        gamma_scale: float = 1.0,
+        with_noise: bool = False,
+        inplace: bool = False,
+        batchwise: bool = False
+):
     """ DropBlock. See https://arxiv.org/pdf/1810.12890.pdf
 
     DropBlock with an experimental gaussian noise option. This layer has been tested on a few training
     runs with success, but needs further validation and possibly optimization for lower runtime impact.
     """
     B, C, H, W = x.shape
     total_size = W * H
     clipped_block_size = min(block_size, min(W, H))
     # seed_drop_rate, the gamma parameter
     gamma = gamma_scale * drop_prob * total_size / clipped_block_size ** 2 / (
             (W - block_size + 1) * (H - block_size + 1))
 
     # Forces the block to be inside the feature map.
-    w_i, h_i = torch.meshgrid(torch.arange(W).to(x.device), torch.arange(H).to(x.device))
+    w_i, h_i = ndgrid(torch.arange(W, device=x.device), torch.arange(H, device=x.device))
     valid_block = ((w_i >= clipped_block_size // 2) & (w_i < W - (clipped_block_size - 1) // 2)) & \
                   ((h_i >= clipped_block_size // 2) & (h_i < H - (clipped_block_size - 1) // 2))
     valid_block = torch.reshape(valid_block, (1, 1, H, W)).to(dtype=x.dtype)
 
     if batchwise:
         # one mask for whole batch, quite a bit faster
         uniform_noise = torch.rand((1, C, H, W), dtype=x.dtype, device=x.device)
@@ -64,16 +72,21 @@
             x.mul_(block_mask * normalize_scale)
         else:
             x = x * block_mask * normalize_scale
     return x
 
 
 def drop_block_fast_2d(
-        x: torch.Tensor, drop_prob: float = 0.1, block_size: int = 7,
-        gamma_scale: float = 1.0, with_noise: bool = False, inplace: bool = False):
+        x: torch.Tensor,
+        drop_prob: float = 0.1,
+        block_size: int = 7,
+        gamma_scale: float = 1.0,
+        with_noise: bool = False,
+        inplace: bool = False,
+):
     """ DropBlock. See https://arxiv.org/pdf/1810.12890.pdf
 
     DropBlock with an experimental gaussian noise option. Simplied from above without concern for valid
     block mask at edges.
     """
     B, C, H, W = x.shape
     total_size = W * H
```

### Comparing `timm-0.9.9/timm/layers/eca.py` & `timm-1.0.3/timm/layers/eca.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/evo_norm.py` & `timm-1.0.3/timm/layers/evo_norm.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/fast_norm.py` & `timm-1.0.3/timm/layers/fast_norm.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/filter_response_norm.py` & `timm-1.0.3/timm/layers/filter_response_norm.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/format.py` & `timm-1.0.3/timm/layers/format.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/gather_excite.py` & `timm-1.0.3/timm/layers/gather_excite.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/global_context.py` & `timm-1.0.3/timm/layers/global_context.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/grn.py` & `timm-1.0.3/timm/layers/grn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/halo_attn.py` & `timm-1.0.3/timm/layers/halo_attn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/helpers.py` & `timm-1.0.3/timm/layers/helpers.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/inplace_abn.py` & `timm-1.0.3/timm/layers/inplace_abn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/interpolate.py` & `timm-1.0.3/timm/layers/interpolate.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/lambda_layer.py` & `timm-1.0.3/timm/layers/lambda_layer.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 
 Hacked together by / Copyright 2021 Ross Wightman
 """
 import torch
 from torch import nn
 import torch.nn.functional as F
 
+from .grid import ndgrid
 from .helpers import to_2tuple, make_divisible
 from .weight_init import trunc_normal_
 
 
 def rel_pos_indices(size):
     size = to_2tuple(size)
-    pos = torch.stack(torch.meshgrid(torch.arange(size[0]), torch.arange(size[1]))).flatten(1)
+    pos = torch.stack(ndgrid(torch.arange(size[0]), torch.arange(size[1]))).flatten(1)
     rel_pos = pos[:, None, :] - pos[:, :, None]
     rel_pos[0] += size[0] - 1
     rel_pos[1] += size[1] - 1
     return rel_pos  # 2, H * W, H * W
 
 
 class LambdaLayer(nn.Module):
```

### Comparing `timm-0.9.9/timm/layers/linear.py` & `timm-1.0.3/timm/layers/linear.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/median_pool.py` & `timm-1.0.3/timm/layers/median_pool.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/mixed_conv2d.py` & `timm-1.0.3/timm/layers/mixed_conv2d.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/ml_decoder.py` & `timm-1.0.3/timm/layers/ml_decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,47 +69,35 @@
         tgt = self.norm2(tgt)
         tgt2 = self.linear2(self.dropout(self.activation(self.linear1(tgt))))
         tgt = tgt + self.dropout3(tgt2)
         tgt = self.norm3(tgt)
         return tgt
 
 
-# @torch.jit.script
 # class ExtrapClasses(object):
 #     def __init__(self, num_queries: int, group_size: int):
 #         self.num_queries = num_queries
 #         self.group_size = group_size
 #
 #     def __call__(self, h: torch.Tensor, class_embed_w: torch.Tensor, class_embed_b: torch.Tensor, out_extrap:
 #     torch.Tensor):
 #         # h = h.unsqueeze(-1).expand(-1, -1, -1, self.group_size)
 #         h = h[..., None].repeat(1, 1, 1, self.group_size) # torch.Size([bs, 5, 768, groups])
 #         w = class_embed_w.view((self.num_queries, h.shape[2], self.group_size))
 #         out = (h * w).sum(dim=2) + class_embed_b
 #         out = out.view((h.shape[0], self.group_size * self.num_queries))
 #         return out
 
-@torch.jit.script
-class GroupFC(object):
-    def __init__(self, embed_len_decoder: int):
-        self.embed_len_decoder = embed_len_decoder
-
-    def __call__(self, h: torch.Tensor, duplicate_pooling: torch.Tensor, out_extrap: torch.Tensor):
-        for i in range(self.embed_len_decoder):
-            h_i = h[:, i, :]
-            w_i = duplicate_pooling[i, :, :]
-            out_extrap[:, i, :] = torch.matmul(h_i, w_i)
-
-
 class MLDecoder(nn.Module):
     def __init__(self, num_classes, num_of_groups=-1, decoder_embedding=768, initial_num_features=2048):
         super(MLDecoder, self).__init__()
         embed_len_decoder = 100 if num_of_groups < 0 else num_of_groups
         if embed_len_decoder > num_classes:
             embed_len_decoder = num_classes
+        self.embed_len_decoder = embed_len_decoder
 
         # switching to 768 initial embeddings
         decoder_embedding = 768 if decoder_embedding < 0 else decoder_embedding
         self.embed_standart = nn.Linear(initial_num_features, decoder_embedding)
 
         # decoder
         decoder_dropout = 0.1
@@ -127,15 +115,14 @@
         self.num_classes = num_classes
         self.duplicate_factor = int(num_classes / embed_len_decoder + 0.999)
         self.duplicate_pooling = torch.nn.Parameter(
             torch.Tensor(embed_len_decoder, decoder_embedding, self.duplicate_factor))
         self.duplicate_pooling_bias = torch.nn.Parameter(torch.Tensor(num_classes))
         torch.nn.init.xavier_normal_(self.duplicate_pooling)
         torch.nn.init.constant_(self.duplicate_pooling_bias, 0)
-        self.group_fc = GroupFC(embed_len_decoder)
 
     def forward(self, x):
         if len(x.shape) == 4:  # [bs,2048, 7,7]
             embedding_spatial = x.flatten(2).transpose(1, 2)
         else:  # [bs, 197,468]
             embedding_spatial = x
         embedding_spatial_786 = self.embed_standart(embedding_spatial)
@@ -145,12 +132,15 @@
         query_embed = self.query_embed.weight
         # tgt = query_embed.unsqueeze(1).repeat(1, bs, 1)
         tgt = query_embed.unsqueeze(1).expand(-1, bs, -1)  # no allocation of memory with expand
         h = self.decoder(tgt, embedding_spatial_786.transpose(0, 1))  # [embed_len_decoder, batch, 768]
         h = h.transpose(0, 1)
 
         out_extrap = torch.zeros(h.shape[0], h.shape[1], self.duplicate_factor, device=h.device, dtype=h.dtype)
-        self.group_fc(h, self.duplicate_pooling, out_extrap)
+        for i in range(self.embed_len_decoder):  # group FC
+            h_i = h[:, i, :]
+            w_i = self.duplicate_pooling[i, :, :]
+            out_extrap[:, i, :] = torch.matmul(h_i, w_i)
         h_out = out_extrap.flatten(1)[:, :self.num_classes]
         h_out += self.duplicate_pooling_bias
         logits = h_out
         return logits
```

### Comparing `timm-0.9.9/timm/layers/mlp.py` & `timm-1.0.3/timm/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/non_local_attn.py` & `timm-1.0.3/timm/layers/non_local_attn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/norm.py` & `timm-1.0.3/timm/layers/norm.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,14 @@
     # jit is oh so lovely :/
     if torch.jit.is_scripting():
         return tensor.is_contiguous()
     else:
         return tensor.is_contiguous(memory_format=torch.contiguous_format)
 
 
-@torch.jit.script
 def _layer_norm_cf(x: torch.Tensor, weight: torch.Tensor, bias: torch.Tensor, eps: float):
     s, u = torch.var_mean(x, dim=1, unbiased=False, keepdim=True)
     x = (x - u) * torch.rsqrt(s + eps)
     x = x * weight[:, None, None] + bias[:, None, None]
     return x
```

### Comparing `timm-0.9.9/timm/layers/norm_act.py` & `timm-1.0.3/timm/layers/norm_act.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/padding.py` & `timm-1.0.3/timm/layers/padding.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/patch_dropout.py` & `timm-1.0.3/timm/layers/patch_dropout.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/patch_embed.py` & `timm-1.0.3/timm/layers/patch_embed.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Based on code in:
   * https://github.com/google-research/vision_transformer
   * https://github.com/google-research/big_vision/tree/main/big_vision
 
 Hacked together by / Copyright 2020 Ross Wightman
 """
 import logging
+import math
 from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 from torch import nn as nn
 import torch.nn.functional as F
 
 from .format import Format, nchw_to
@@ -61,14 +62,29 @@
             self.output_fmt = Format.NCHW
         self.strict_img_size = strict_img_size
         self.dynamic_img_pad = dynamic_img_pad
 
         self.proj = nn.Conv2d(in_chans, embed_dim, kernel_size=patch_size, stride=patch_size, bias=bias)
         self.norm = norm_layer(embed_dim) if norm_layer else nn.Identity()
 
+    def feat_ratio(self, as_scalar=True) -> Union[Tuple[int, int], int]:
+        if as_scalar:
+            return max(self.patch_size)
+        else:
+            return self.patch_size
+
+    def dynamic_feat_size(self, img_size: Tuple[int, int]) -> Tuple[int, int]:
+        """ Get grid (feature) size for given image size taking account of dynamic padding.
+        NOTE: must be torchscript compatible so using fixed tuple indexing
+        """
+        if self.dynamic_img_pad:
+            return math.ceil(img_size[0] / self.patch_size[0]), math.ceil(img_size[1] / self.patch_size[1])
+        else:
+            return img_size[0] // self.patch_size[0], img_size[1] // self.patch_size[1]
+
     def forward(self, x):
         B, C, H, W = x.shape
         if self.img_size is not None:
             if self.strict_img_size:
                 _assert(H == self.img_size[0], f"Input height ({H}) doesn't match model ({self.img_size[0]}).")
                 _assert(W == self.img_size[1], f"Input width ({W}) doesn't match model ({self.img_size[1]}).")
             elif not self.dynamic_img_pad:
@@ -123,21 +139,21 @@
     def forward(self, x) -> Tuple[torch.Tensor, List[int]]:
         B, C, H, W = x.shape
         if self.img_size is not None:
             _assert(H % self.patch_size[0] == 0, f"Input image height ({H}) must be divisible by patch size ({self.patch_size[0]}).")
             _assert(W % self.patch_size[1] == 0, f"Input image width ({W}) must be divisible by patch size ({self.patch_size[1]}).")
 
         x = self.proj(x)
-        grid_size = x.shape[-2:]
+        feat_size = x.shape[-2:]
         if self.flatten:
             x = x.flatten(2).transpose(1, 2)  # NCHW -> NLC
         elif self.output_fmt != Format.NCHW:
             x = nchw_to(x, self.output_fmt)
         x = self.norm(x)
-        return x, grid_size
+        return x, feat_size
 
 
 def resample_patch_embed(
         patch_embed,
         new_size: List[int],
         interpolation: str = 'bicubic',
         antialias: bool = True,
@@ -192,15 +208,15 @@
         for i in range(np.prod(_old_size)):
             basis_vec = np.zeros(_old_size)
             basis_vec[np.unravel_index(i, _old_size)] = 1.
             mat.append(resize(basis_vec, _new_size).reshape(-1))
         return np.stack(mat).T
 
     resize_mat = get_resize_mat(old_size, new_size)
-    resize_mat_pinv = torch.Tensor(np.linalg.pinv(resize_mat.T))
+    resize_mat_pinv = torch.tensor(np.linalg.pinv(resize_mat.T), device=patch_embed.device)
 
     def resample_kernel(kernel):
         resampled_kernel = resize_mat_pinv @ kernel.reshape(-1)
         return resampled_kernel.reshape(new_size)
 
     v_resample_kernel = vmap(vmap(resample_kernel, 0, 0), 1, 1)
     orig_dtype = patch_embed.dtype
```

### Comparing `timm-0.9.9/timm/layers/pool2d_same.py` & `timm-1.0.3/timm/layers/pool2d_same.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/pos_embed.py` & `timm-1.0.3/timm/layers/pos_embed.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/pos_embed_rel.py` & `timm-1.0.3/timm/layers/pos_embed_rel.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 from typing import Optional, Tuple
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from .grid import ndgrid
 from .interpolate import RegularGridInterpolator
 from .mlp import Mlp
 from .weight_init import trunc_normal_
 
 _USE_SCIPY = int(os.environ.get('TIMM_USE_SCIPY_INTERP', 0)) > 0
 
 
@@ -22,40 +23,35 @@
         k_size: Optional[Tuple[int, int]] = None,
         class_token: bool = False,
 ) -> torch.Tensor:
     # Adapted with significant modifications from Swin / BeiT codebases
     # get pair-wise relative position index for each token inside the window
     assert k_size is None, 'Different q & k sizes not currently supported'  # FIXME
 
-    coords = torch.stack(
-        torch.meshgrid([
-            torch.arange(q_size[0]),
-            torch.arange(q_size[1])
-        ])
-    ).flatten(1)  # 2, Wh, Ww
+    coords = torch.stack(ndgrid(torch.arange(q_size[0]), torch.arange(q_size[1]))).flatten(1)  # 2, Wh, Ww
     relative_coords = coords[:, :, None] - coords[:, None, :]  # 2, Wh*Ww, Wh*Ww
     relative_coords = relative_coords.permute(1, 2, 0)  # Qh*Qw, Kh*Kw, 2
     relative_coords[:, :, 0] += q_size[0] - 1  # shift to start from 0
     relative_coords[:, :, 1] += q_size[1] - 1
     relative_coords[:, :, 0] *= 2 * q_size[1] - 1
     num_relative_distance = (2 * q_size[0] - 1) * (2 * q_size[1] - 1)
 
     # else:
     #     # FIXME different q vs k sizes is a WIP, need to better offset the two grids?
     #     q_coords = torch.stack(
-    #         torch.meshgrid([
+    #         ndgrid(
     #             torch.arange(q_size[0]),
     #             torch.arange(q_size[1])
-    #         ])
+    #         )
     #     ).flatten(1)  # 2, Wh, Ww
     #     k_coords = torch.stack(
-    #         torch.meshgrid([
+    #         ndgrid(
     #             torch.arange(k_size[0]),
     #             torch.arange(k_size[1])
-    #         ])
+    #         )
     #     ).flatten(1)
     #     relative_coords = q_coords[:, :, None] - k_coords[:, None, :]  # 2, Wh*Ww, Wh*Ww
     #     relative_coords = relative_coords.permute(1, 2, 0)  # Qh*Qw, Kh*Kw, 2
     #     relative_coords[:, :, 0] += max(q_size[0], k_size[0]) - 1  # shift to start from 0
     #     relative_coords[:, :, 1] += max(q_size[1], k_size[1]) - 1
     #     relative_coords[:, :, 0] *= k_size[1] + q_size[1] - 1
     #     relative_position_index = relative_coords.sum(-1)  # Qh*Qw, Kh*Kw
@@ -228,15 +224,15 @@
         yx = [torch.tensor(y), torch.tensor(x)]
         # print("Original positions = %s" % str(x))
 
         ty = dst_size[0] // 2.0
         tx = dst_size[1] // 2.0
         dy = torch.arange(-ty, ty + 0.1, 1.0)
         dx = torch.arange(-tx, tx + 0.1, 1.0)
-        dyx = torch.meshgrid([dy, dx])
+        dyx = ndgrid(dy, dx)
         # print("Target positions = %s" % str(dx))
 
         all_rel_pos_bias = []
         for i in range(num_attn_heads):
             if has_flat_shape:
                 z = rel_pos_bias[:, i].view(src_size[0], src_size[1]).float()
             else:
@@ -307,17 +303,17 @@
 def gen_relative_log_coords(
         win_size: Tuple[int, int],
         pretrained_win_size: Tuple[int, int] = (0, 0),
         mode='swin',
 ):
     assert mode in ('swin', 'cr')
     # as per official swin-v2 impl, supporting timm specific 'cr' log coords as well
-    relative_coords_h = torch.arange(-(win_size[0] - 1), win_size[0], dtype=torch.float32)
-    relative_coords_w = torch.arange(-(win_size[1] - 1), win_size[1], dtype=torch.float32)
-    relative_coords_table = torch.stack(torch.meshgrid([relative_coords_h, relative_coords_w]))
+    relative_coords_h = torch.arange(-(win_size[0] - 1), win_size[0]).to(torch.float32)
+    relative_coords_w = torch.arange(-(win_size[1] - 1), win_size[1]).to(torch.float32)
+    relative_coords_table = torch.stack(ndgrid(relative_coords_h, relative_coords_w))
     relative_coords_table = relative_coords_table.permute(1, 2, 0).contiguous()  # 2*Wh-1, 2*Ww-1, 2
     if mode == 'swin':
         if pretrained_win_size[0] > 0:
             relative_coords_table[:, :, 0] /= (pretrained_win_size[0] - 1)
             relative_coords_table[:, :, 1] /= (pretrained_win_size[1] - 1)
         else:
             relative_coords_table[:, :, 0] /= (win_size[0] - 1)
```

### Comparing `timm-0.9.9/timm/layers/pos_embed_sincos.py` & `timm-1.0.3/timm/layers/pos_embed_sincos.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 """
 import math
 from typing import List, Tuple, Optional, Union
 
 import torch
 from torch import nn as nn
 
+from .grid import ndgrid
 from .trace_utils import _assert
 
 
 def pixel_freq_bands(
         num_bands: int,
         max_freq: float = 224.,
         linear_bands: bool = True,
-        dtype: torch.dtype = torch.float32,
         device: Optional[torch.device] = None,
 ):
     if linear_bands:
-        bands = torch.linspace(1.0, max_freq / 2, num_bands, dtype=dtype, device=device)
+        bands = torch.linspace(1.0, max_freq / 2, num_bands, dtype=torch.float32, device=device)
     else:
-        bands = 2 ** torch.linspace(0, math.log(max_freq, 2) - 1, num_bands, dtype=dtype, device=device)
+        bands = 2 ** torch.linspace(0, math.log(max_freq, 2) - 1, num_bands, dtype=torch.float32, device=device)
     return bands * torch.pi
 
 
 def freq_bands(
         num_bands: int,
         temperature: float = 10000.,
         step: int = 2,
-        dtype: torch.dtype = torch.float32,
         device: Optional[torch.device] = None,
 ) -> torch.Tensor:
-    bands = 1. / (temperature ** (torch.arange(0, num_bands, step, dtype=dtype, device=device) / num_bands))
+    exp = torch.arange(0, num_bands, step, dtype=torch.int64, device=device).to(torch.float32) / num_bands
+    bands = 1. / (temperature ** exp)
     return bands
 
 
 def build_sincos2d_pos_embed(
         feat_shape: List[int],
         dim: int = 64,
         temperature: float = 10000.,
@@ -57,26 +57,28 @@
         device:
 
     Returns:
 
     """
     assert dim % 4 == 0, 'Embed dimension must be divisible by 4 for sin-cos 2D position embedding'
     pos_dim = dim // 4
-    bands = freq_bands(pos_dim, temperature=temperature, step=1, dtype=dtype, device=device)
+    bands = freq_bands(pos_dim, temperature=temperature, step=1, device=device)
 
     if reverse_coord:
         feat_shape = feat_shape[::-1]  # stack W, H instead of H, W
-    grid = torch.stack(torch.meshgrid(
-        [torch.arange(s, device=device, dtype=dtype) for s in feat_shape])).flatten(1).transpose(0, 1)
+    grid = torch.stack(ndgrid([
+        torch.arange(s, device=device, dtype=torch.int64).to(torch.float32)
+        for s in feat_shape
+    ])).flatten(1).transpose(0, 1)
     pos2 = grid.unsqueeze(-1) * bands.unsqueeze(0)
     # FIXME add support for unflattened spatial dim?
 
     stack_dim = 2 if interleave_sin_cos else 1  # stack sin, cos, sin, cos  instead of sin sin cos cos
     pos_emb = torch.stack([torch.sin(pos2), torch.cos(pos2)], dim=stack_dim).flatten(1)
-    return pos_emb
+    return pos_emb.to(dtype=dtype)
 
 
 def build_fourier_pos_embed(
         feat_shape: List[int],
         bands: Optional[torch.Tensor] = None,
         num_bands: int = 64,
         max_res: int = 224,
@@ -108,45 +110,43 @@
     """
     if bands is None:
         if in_pixels:
             bands = pixel_freq_bands(
                 num_bands,
                 float(max_res),
                 linear_bands=linear_bands,
-                dtype=dtype,
                 device=device,
             )
         else:
             bands = freq_bands(
                 num_bands,
                 temperature=temperature,
                 step=1,
-                dtype=dtype,
                 device=device,
             )
     else:
         if device is None:
             device = bands.device
         if dtype is None:
             dtype = bands.dtype
 
     if in_pixels:
-        t = [torch.linspace(-1., 1., steps=s, device=device, dtype=dtype) for s in feat_shape]
+        t = [torch.linspace(-1., 1., steps=s, device=device, dtype=torch.float32) for s in feat_shape]
     else:
-        t = [torch.arange(s, device=device, dtype=dtype) for s in feat_shape]
+        t = [torch.arange(s, device=device, dtype=torch.int64).to(torch.float32) for s in feat_shape]
 
     if ref_feat_shape is not None:
         # eva's scheme for resizing rope embeddings (ref shape = pretrain)
         t = [x / f * r for x, f, r in zip(t, feat_shape, ref_feat_shape)]
 
-    grid = torch.stack(torch.meshgrid(t), dim=-1)
+    grid = torch.stack(ndgrid(t), dim=-1)
     grid = grid.unsqueeze(-1)
     pos = grid * bands
 
-    pos_sin, pos_cos = pos.sin(), pos.cos()
+    pos_sin, pos_cos = pos.sin().to(dtype=dtype), pos.cos().to(dtype)
     out = [grid, pos_sin, pos_cos] if include_grid else [pos_sin, pos_cos]
     return out
 
 
 class FourierEmbed(nn.Module):
 
     def __init__(
```

### Comparing `timm-0.9.9/timm/layers/selective_kernel.py` & `timm-1.0.3/timm/layers/selective_kernel.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/separable_conv.py` & `timm-1.0.3/timm/layers/separable_conv.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/space_to_depth.py` & `timm-1.0.3/timm/layers/space_to_depth.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,37 +14,14 @@
         N, C, H, W = x.size()
         x = x.view(N, C, H // self.bs, self.bs, W // self.bs, self.bs)  # (N, C, H//bs, bs, W//bs, bs)
         x = x.permute(0, 3, 5, 1, 2, 4).contiguous()  # (N, bs, bs, C, H//bs, W//bs)
         x = x.view(N, C * self.bs * self.bs, H // self.bs, W // self.bs)  # (N, C*bs^2, H//bs, W//bs)
         return x
 
 
-@torch.jit.script
-class SpaceToDepthJit:
-    def __call__(self, x: torch.Tensor):
-        # assuming hard-coded that block_size==4 for acceleration
-        N, C, H, W = x.size()
-        x = x.view(N, C, H // 4, 4, W // 4, 4)  # (N, C, H//bs, bs, W//bs, bs)
-        x = x.permute(0, 3, 5, 1, 2, 4).contiguous()  # (N, bs, bs, C, H//bs, W//bs)
-        x = x.view(N, C * 16, H // 4, W // 4)  # (N, C*bs^2, H//bs, W//bs)
-        return x
-
-
-class SpaceToDepthModule(nn.Module):
-    def __init__(self, no_jit=False):
-        super().__init__()
-        if not no_jit:
-            self.op = SpaceToDepthJit()
-        else:
-            self.op = SpaceToDepth()
-
-    def forward(self, x):
-        return self.op(x)
-
-
 class DepthToSpace(nn.Module):
 
     def __init__(self, block_size):
         super().__init__()
         self.bs = block_size
 
     def forward(self, x):
```

### Comparing `timm-0.9.9/timm/layers/split_attn.py` & `timm-1.0.3/timm/layers/split_attn.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/split_batchnorm.py` & `timm-1.0.3/timm/layers/split_batchnorm.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/squeeze_excite.py` & `timm-1.0.3/timm/layers/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/std_conv.py` & `timm-1.0.3/timm/layers/std_conv.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/test_time_pool.py` & `timm-1.0.3/timm/layers/test_time_pool.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/layers/weight_init.py` & `timm-1.0.3/timm/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/loss/binary_cross_entropy.py` & `timm-1.0.3/timm/loss/binary_cross_entropy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,65 @@
 """ Binary Cross Entropy w/ a few extras
 
 Hacked together by / Copyright 2021 Ross Wightman
 """
-from typing import Optional
+from typing import Optional, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 
 class BinaryCrossEntropy(nn.Module):
     """ BCE with optional one-hot from dense targets, label smoothing, thresholding
     NOTE for experiments comparing CE to BCE /w label smoothing, may remove
     """
     def __init__(
-            self, smoothing=0.1, target_threshold: Optional[float] = None, weight: Optional[torch.Tensor] = None,
-            reduction: str = 'mean', pos_weight: Optional[torch.Tensor] = None):
+            self,
+            smoothing=0.1,
+            target_threshold: Optional[float] = None,
+            weight: Optional[torch.Tensor] = None,
+            reduction: str = 'mean',
+            sum_classes: bool = False,
+            pos_weight: Optional[Union[torch.Tensor, float]] = None,
+    ):
         super(BinaryCrossEntropy, self).__init__()
         assert 0. <= smoothing < 1.0
+        if pos_weight is not None:
+            if not isinstance(pos_weight, torch.Tensor):
+                pos_weight = torch.tensor(pos_weight)
         self.smoothing = smoothing
         self.target_threshold = target_threshold
-        self.reduction = reduction
+        self.reduction = 'none' if sum_classes else reduction
+        self.sum_classes = sum_classes
         self.register_buffer('weight', weight)
         self.register_buffer('pos_weight', pos_weight)
 
     def forward(self, x: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        assert x.shape[0] == target.shape[0]
+        batch_size = x.shape[0]
+        assert batch_size == target.shape[0]
+
         if target.shape != x.shape:
             # NOTE currently assume smoothing or other label softening is applied upstream if targets are already sparse
             num_classes = x.shape[-1]
             # FIXME should off/on be different for smoothing w/ BCE? Other impl out there differ
             off_value = self.smoothing / num_classes
             on_value = 1. - self.smoothing + off_value
             target = target.long().view(-1, 1)
             target = torch.full(
-                (target.size()[0], num_classes),
+                (batch_size, num_classes),
                 off_value,
                 device=x.device, dtype=x.dtype).scatter_(1, target, on_value)
+
         if self.target_threshold is not None:
             # Make target 0, or 1 if threshold set
             target = target.gt(self.target_threshold).to(dtype=target.dtype)
-        return F.binary_cross_entropy_with_logits(
+
+        loss = F.binary_cross_entropy_with_logits(
             x, target,
             self.weight,
             pos_weight=self.pos_weight,
-            reduction=self.reduction)
+            reduction=self.reduction,
+        )
+        if self.sum_classes:
+            loss = loss.sum(-1).mean()
+        return loss
```

### Comparing `timm-0.9.9/timm/loss/cross_entropy.py` & `timm-1.0.3/timm/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/loss/jsd.py` & `timm-1.0.3/timm/loss/jsd.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/__init__.py` & `timm-1.0.3/timm/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,31 @@
 from .efficientvit_msra import *
 from .eva import *
 from .fastvit import *
 from .focalnet import *
 from .gcvit import *
 from .ghostnet import *
 from .hardcorenas import *
+from .hgnet import *
+from .hiera import *
 from .hrnet import *
 from .inception_next import *
 from .inception_resnet_v2 import *
 from .inception_v3 import *
 from .inception_v4 import *
 from .levit import *
 from .maxxvit import *
 from .metaformer import *
 from .mlp_mixer import *
 from .mobilenetv3 import *
 from .mobilevit import *
 from .mvitv2 import *
 from .nasnet import *
 from .nest import *
+from .nextvit import *
 from .nfnet import *
 from .pit import *
 from .pnasnet import *
 from .pvt_v2 import *
 from .regnet import *
 from .repghost import *
 from .repvit import *
@@ -74,15 +77,15 @@
 from .xception_aligned import *
 from .xcit import *
 
 from ._builder import build_model_with_cfg, load_pretrained, load_custom_pretrained, resolve_pretrained_cfg, \
     set_pretrained_download_progress, set_pretrained_check_hash
 from ._factory import create_model, parse_model_name, safe_model_name
 from ._features import FeatureInfo, FeatureHooks, FeatureHookNet, FeatureListNet, FeatureDictNet
-from ._features_fx import FeatureGraphNet, GraphExtractNet, create_feature_extractor, \
+from ._features_fx import FeatureGraphNet, GraphExtractNet, create_feature_extractor, get_graph_node_names, \
     register_notrace_module, is_notrace_module, get_notrace_modules, \
     register_notrace_function, is_notrace_function, get_notrace_functions
 from ._helpers import clean_state_dict, load_state_dict, load_checkpoint, remap_state_dict, resume_checkpoint
 from ._hub import load_model_config_from_hf, load_state_dict_from_hf, push_to_hf_hub
 from ._manipulate import model_parameters, named_apply, named_modules, named_modules_with_params, \
     group_modules, group_parameters, checkpoint_seq, adapt_input_conv
 from ._pretrained import PretrainedCfg, DefaultCfg, filter_pretrained_cfg
```

### Comparing `timm-0.9.9/timm/models/_builder.py` & `timm-1.0.3/timm/models/_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import dataclasses
 import logging
 import os
 from copy import deepcopy
-from typing import Optional, Dict, Callable, Any, Tuple
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from torch import nn as nn
 from torch.hub import load_state_dict_from_url
 
-from timm.models._features import FeatureListNet, FeatureHookNet
+from timm.models._features import FeatureListNet, FeatureDictNet, FeatureHookNet, FeatureGetterNet
 from timm.models._features_fx import FeatureGraphNet
 from timm.models._helpers import load_state_dict
-from timm.models._hub import has_hf_hub, download_cached_file, check_cached_file, load_state_dict_from_hf
+from timm.models._hub import has_hf_hub, download_cached_file, check_cached_file, load_state_dict_from_hf,\
+    load_custom_from_hf
 from timm.models._manipulate import adapt_input_conv
 from timm.models._pretrained import PretrainedCfg
 from timm.models._prune import adapt_model_from_file
 from timm.models._registry import get_pretrained_cfg
 
 _logger = logging.getLogger(__name__)
 
@@ -181,15 +182,20 @@
                 map_location='cpu',
                 progress=_DOWNLOAD_PROGRESS,
                 check_hash=_CHECK_HASH,
             )
     elif load_from == 'hf-hub':
         _logger.info(f'Loading pretrained weights from Hugging Face hub ({pretrained_loc})')
         if isinstance(pretrained_loc, (list, tuple)):
-            state_dict = load_state_dict_from_hf(*pretrained_loc)
+            custom_load = pretrained_cfg.get('custom_load', False)
+            if isinstance(custom_load, str) and custom_load == 'hf':
+                load_custom_from_hf(*pretrained_loc, model)
+                return
+            else:
+                state_dict = load_state_dict_from_hf(*pretrained_loc)
         else:
             state_dict = load_state_dict_from_hf(pretrained_loc)
     else:
         model_name = pretrained_cfg.get('architecture', 'this model')
         raise RuntimeError(f"No pretrained weights exist for {model_name}. Use `pretrained=False` for random init.")
 
     if filter_fn is not None:
@@ -230,15 +236,23 @@
             for classifier_name in classifiers:
                 # special case for pretrained weights with an extra background class in pretrained weights
                 classifier_weight = state_dict[classifier_name + '.weight']
                 state_dict[classifier_name + '.weight'] = classifier_weight[label_offset:]
                 classifier_bias = state_dict[classifier_name + '.bias']
                 state_dict[classifier_name + '.bias'] = classifier_bias[label_offset:]
 
-    model.load_state_dict(state_dict, strict=strict)
+    load_result = model.load_state_dict(state_dict, strict=strict)
+    if load_result.missing_keys:
+        _logger.info(
+            f'Missing keys ({", ".join(load_result.missing_keys)}) discovered while loading pretrained weights.'
+            f' This is expected if model is being adapted.')
+    if load_result.unexpected_keys:
+        _logger.warning(
+            f'Unexpected keys ({", ".join(load_result.unexpected_keys)}) found while loading pretrained weights.'
+            f' This may be expected if model is being adapted.')
 
 
 def pretrained_cfg_for_features(pretrained_cfg):
     pretrained_cfg = deepcopy(pretrained_cfg)
     # remove default pretrained cfg fields that don't have much relevance for feature backbone
     to_remove = ('num_classes', 'classifier', 'global_pool')  # add default final pool size?
     for tr in to_remove:
@@ -249,15 +263,15 @@
 def _filter_kwargs(kwargs, names):
     if not kwargs or not names:
         return
     for n in names:
         kwargs.pop(n, None)
 
 
-def _update_default_kwargs(pretrained_cfg, kwargs, kwargs_filter):
+def _update_default_model_kwargs(pretrained_cfg, kwargs, kwargs_filter):
     """ Update the default_cfg and kwargs before passing to model
 
     Args:
         pretrained_cfg: input pretrained cfg (updated in-place)
         kwargs: keyword args passed to model build fn (updated in-place)
         kwargs_filter: keyword arg keys that must be removed before model __init__
     """
@@ -276,14 +290,19 @@
                 assert len(input_size) == 3
                 kwargs.setdefault(n, input_size[-2:])
         elif n == 'in_chans':
             input_size = pretrained_cfg.get('input_size', None)
             if input_size is not None:
                 assert len(input_size) == 3
                 kwargs.setdefault(n, input_size[0])
+        elif n == 'num_classes':
+            default_val = pretrained_cfg.get(n, None)
+            # if default is < 0, don't pass through to model
+            if default_val is not None and default_val >= 0:
+                kwargs.setdefault(n, pretrained_cfg[n])
         else:
             default_val = pretrained_cfg.get(n, None)
             if default_val is not None:
                 kwargs.setdefault(n, pretrained_cfg[n])
 
     # Filter keyword args for task specific model variants (some 'features only' models, etc.)
     _filter_kwargs(kwargs, names=kwargs_filter)
@@ -342,23 +361,23 @@
     This helper fn aids in the construction of a model including:
       * handling default_cfg and associated pretrained weight loading
       * passing through optional model_cfg for models with config based arch spec
       * features_only model adaptation
       * pruning config / model adaptation
 
     Args:
-        model_cls (nn.Module): model class
-        variant (str): model variant name
-        pretrained (bool): load pretrained weights
-        pretrained_cfg (dict): model's pretrained weight/task config
-        model_cfg (Optional[Dict]): model's architecture config
-        feature_cfg (Optional[Dict]: feature extraction adapter config
-        pretrained_strict (bool): load pretrained weights strictly
-        pretrained_filter_fn (Optional[Callable]): filter callable for pretrained weights
-        kwargs_filter (Optional[Tuple]): kwargs to filter before passing to model
+        model_cls: model class
+        variant: model variant name
+        pretrained: load pretrained weights
+        pretrained_cfg: model's pretrained weight/task config
+        model_cfg: model's architecture config
+        feature_cfg: feature extraction adapter config
+        pretrained_strict: load pretrained weights strictly
+        pretrained_filter_fn: filter callable for pretrained weights
+        kwargs_filter: kwargs to filter before passing to model
         **kwargs: model args passed through to model __init__
     """
     pruned = kwargs.pop('pruned', False)
     features = False
     feature_cfg = feature_cfg or {}
 
     # resolve and update model pretrained config and model kwargs
@@ -367,22 +386,24 @@
         pretrained_cfg=pretrained_cfg,
         pretrained_cfg_overlay=pretrained_cfg_overlay
     )
 
     # FIXME converting back to dict, PretrainedCfg use should be propagated further, but not into model
     pretrained_cfg = pretrained_cfg.to_dict()
 
-    _update_default_kwargs(pretrained_cfg, kwargs, kwargs_filter)
+    _update_default_model_kwargs(pretrained_cfg, kwargs, kwargs_filter)
 
     # Setup for feature extraction wrapper done at end of this fn
     if kwargs.pop('features_only', False):
         features = True
         feature_cfg.setdefault('out_indices', (0, 1, 2, 3, 4))
         if 'out_indices' in kwargs:
             feature_cfg['out_indices'] = kwargs.pop('out_indices')
+        if 'feature_cls' in kwargs:
+            feature_cfg['feature_cls'] = kwargs.pop('feature_cls')
 
     # Instantiate the model
     if model_cfg is None:
         model = model_cls(**kwargs)
     else:
         model = model_cls(cfg=model_cfg, **kwargs)
     model.pretrained_cfg = pretrained_cfg
@@ -401,26 +422,42 @@
             in_chans=kwargs.get('in_chans', 3),
             filter_fn=pretrained_filter_fn,
             strict=pretrained_strict,
         )
 
     # Wrap the model in a feature extraction module if enabled
     if features:
-        feature_cls = FeatureListNet
-        output_fmt = getattr(model, 'output_fmt', None)
-        if output_fmt is not None:
-            feature_cfg.setdefault('output_fmt', output_fmt)
+        use_getter = False
         if 'feature_cls' in feature_cfg:
             feature_cls = feature_cfg.pop('feature_cls')
             if isinstance(feature_cls, str):
                 feature_cls = feature_cls.lower()
+
+                # flatten_sequential only valid for some feature extractors
+                if feature_cls not in ('dict', 'list', 'hook'):
+                    feature_cfg.pop('flatten_sequential', None)
+
                 if 'hook' in feature_cls:
                     feature_cls = FeatureHookNet
+                elif feature_cls == 'list':
+                    feature_cls = FeatureListNet
+                elif feature_cls == 'dict':
+                    feature_cls = FeatureDictNet
                 elif feature_cls == 'fx':
                     feature_cls = FeatureGraphNet
+                elif feature_cls == 'getter':
+                    use_getter = True
+                    feature_cls = FeatureGetterNet
                 else:
                     assert False, f'Unknown feature class {feature_cls}'
+        else:
+            feature_cls = FeatureListNet
+
+        output_fmt = getattr(model, 'output_fmt', None)
+        if output_fmt is not None and not use_getter:  # don't set default for intermediate feat getter
+            feature_cfg.setdefault('output_fmt', output_fmt)
+
         model = feature_cls(model, **feature_cfg)
         model.pretrained_cfg = pretrained_cfg_for_features(pretrained_cfg)  # add back pretrained cfg
         model.default_cfg = model.pretrained_cfg  # alias for rename backwards compat (default_cfg -> pretrained_cfg)
 
     return model
```

### Comparing `timm-0.9.9/timm/models/_efficientnet_blocks.py` & `timm-1.0.3/timm/models/_efficientnet_blocks.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/_efficientnet_builder.py` & `timm-1.0.3/timm/models/_efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/_factory.py` & `timm-1.0.3/timm/models/_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,18 @@
     kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
     model_source, model_name = parse_model_name(model_name)
     if model_source == 'hf-hub':
         assert not pretrained_cfg, 'pretrained_cfg should not be set when sourcing model from Hugging Face Hub.'
         # For model names specified in the form `hf-hub:path/architecture_name@revision`,
         # load model weights + pretrained_cfg from Hugging Face hub.
-        pretrained_cfg, model_name = load_model_config_from_hf(model_name)
+        pretrained_cfg, model_name, model_args = load_model_config_from_hf(model_name)
+        if model_args:
+            for k, v in model_args.items():
+                kwargs.setdefault(k, v)
     else:
         model_name, pretrained_tag = split_model_name_tag(model_name)
         if pretrained_tag and not pretrained_cfg:
             # a valid pretrained_cfg argument takes priority over tag in model name
             pretrained_cfg = pretrained_tag
 
     if not is_model(model_name):
```

### Comparing `timm-0.9.9/timm/models/_features.py` & `timm-1.0.3/timm/models/_features.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,80 +7,139 @@
 https://github.com/pytorch/vision/blob/d88d8961ae51507d0cb680329d985b1488b1b76b/torchvision/models/_utils.py
 
 Hacked together by / Copyright 2020 Ross Wightman
 """
 from collections import OrderedDict, defaultdict
 from copy import deepcopy
 from functools import partial
-from typing import Dict, List, Sequence, Tuple, Union
+from typing import Dict, List, Optional, Sequence, Set, Tuple, Union
 
 import torch
 import torch.nn as nn
 from torch.utils.checkpoint import checkpoint
 
 from timm.layers import Format
 
 
-__all__ = ['FeatureInfo', 'FeatureHooks', 'FeatureDictNet', 'FeatureListNet', 'FeatureHookNet']
+__all__ = [
+    'FeatureInfo', 'FeatureHooks', 'FeatureDictNet', 'FeatureListNet', 'FeatureHookNet', 'FeatureGetterNet',
+    'feature_take_indices'
+]
+
+
+def _take_indices(
+        num_blocks: int,
+        n: Optional[Union[int, List[int], Tuple[int]]],
+) -> Tuple[Set[int], int]:
+    if isinstance(n, int):
+        assert n >= 0
+        take_indices = {x for x in range(num_blocks - n, num_blocks)}
+    else:
+        take_indices = {num_blocks + idx if idx < 0 else idx for idx in n}
+    return take_indices, max(take_indices)
+
+
+def _take_indices_jit(
+        num_blocks: int,
+        n: Union[int, List[int], Tuple[int]],
+) -> Tuple[List[int], int]:
+    if isinstance(n, int):
+        assert n >= 0
+        take_indices = [num_blocks - n + i for i in range(n)]
+    elif isinstance(n, tuple):
+        # splitting this up is silly, but needed for torchscript type resolution of n
+        take_indices = [num_blocks + idx if idx < 0 else idx for idx in n]
+    else:
+        take_indices = [num_blocks + idx if idx < 0 else idx for idx in n]
+    return take_indices, max(take_indices)
+
+
+def feature_take_indices(
+        num_blocks: int,
+        indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+) -> Tuple[List[int], int]:
+    if indices is None:
+        indices = num_blocks  # all blocks if None
+    if torch.jit.is_scripting():
+        return _take_indices_jit(num_blocks, indices)
+    else:
+        # NOTE non-jit returns Set[int] instead of List[int] but torchscript can't handle that anno
+        return _take_indices(num_blocks, indices)
+
+
+def _out_indices_as_tuple(x: Union[int, Tuple[int, ...]]) -> Tuple[int, ...]:
+    if isinstance(x, int):
+        # if indices is an int, take last N features
+        return tuple(range(-x, 0))
+    return tuple(x)
+
+
+OutIndicesT = Union[int, Tuple[int, ...]]
 
 
 class FeatureInfo:
 
-    def __init__(self, feature_info: List[Dict], out_indices: Tuple[int]):
+    def __init__(
+            self,
+            feature_info: List[Dict],
+            out_indices: OutIndicesT,
+    ):
+        out_indices = _out_indices_as_tuple(out_indices)
         prev_reduction = 1
         for i, fi in enumerate(feature_info):
             # sanity check the mandatory fields, there may be additional fields depending on the model
             assert 'num_chs' in fi and fi['num_chs'] > 0
             assert 'reduction' in fi and fi['reduction'] >= prev_reduction
             prev_reduction = fi['reduction']
             assert 'module' in fi
             fi.setdefault('index', i)
         self.out_indices = out_indices
         self.info = feature_info
 
-    def from_other(self, out_indices: Tuple[int]):
+    def from_other(self, out_indices: OutIndicesT):
+        out_indices = _out_indices_as_tuple(out_indices)
         return FeatureInfo(deepcopy(self.info), out_indices)
 
-    def get(self, key, idx=None):
+    def get(self, key: str, idx: Optional[Union[int, List[int]]] = None):
         """ Get value by key at specified index (indices)
         if idx == None, returns value for key at each output index
         if idx is an integer, return value for that feature module index (ignoring output indices)
-        if idx is a list/tupple, return value for each module index (ignoring output indices)
+        if idx is a list/tuple, return value for each module index (ignoring output indices)
         """
         if idx is None:
             return [self.info[i][key] for i in self.out_indices]
         if isinstance(idx, (tuple, list)):
             return [self.info[i][key] for i in idx]
         else:
             return self.info[idx][key]
 
-    def get_dicts(self, keys=None, idx=None):
+    def get_dicts(self, keys: Optional[List[str]] = None, idx: Optional[Union[int, List[int]]] = None):
         """ return info dicts for specified keys (or all if None) at specified indices (or out_indices if None)
         """
         if idx is None:
             if keys is None:
                 return [self.info[i] for i in self.out_indices]
             else:
                 return [{k: self.info[i][k] for k in keys} for i in self.out_indices]
         if isinstance(idx, (tuple, list)):
             return [self.info[i] if keys is None else {k: self.info[i][k] for k in keys} for i in idx]
         else:
             return self.info[idx] if keys is None else {k: self.info[idx][k] for k in keys}
 
-    def channels(self, idx=None):
+    def channels(self, idx: Optional[Union[int, List[int]]] = None):
         """ feature channels accessor
         """
         return self.get('num_chs', idx)
 
-    def reduction(self, idx=None):
+    def reduction(self, idx: Optional[Union[int, List[int]]] = None):
         """ feature reduction (output stride) accessor
         """
         return self.get('reduction', idx)
 
-    def module_name(self, idx=None):
+    def module_name(self, idx: Optional[Union[int, List[int]]] = None):
         """ feature module name accessor
         """
         return self.get('module', idx)
 
     def __getitem__(self, item):
         return self.info[item]
 
@@ -95,34 +154,38 @@
     internal nodes in a model by node name.
 
     FIXME This works well in eager Python but needs redesign for torchscript.
     """
 
     def __init__(
             self,
-            hooks: Sequence[str],
+            hooks: Sequence[Union[str, Dict]],
             named_modules: dict,
             out_map: Sequence[Union[int, str]] = None,
             default_hook_type: str = 'forward',
     ):
         # setup feature hooks
         self._feature_outputs = defaultdict(OrderedDict)
+        self._handles = []
         modules = {k: v for k, v in named_modules}
         for i, h in enumerate(hooks):
-            hook_name = h['module']
+            hook_name = h if isinstance(h, str) else h['module']
             m = modules[hook_name]
             hook_id = out_map[i] if out_map else hook_name
             hook_fn = partial(self._collect_output_hook, hook_id)
-            hook_type = h.get('hook_type', default_hook_type)
+            hook_type = default_hook_type
+            if isinstance(h, dict):
+                hook_type = h.get('hook_type', default_hook_type)
             if hook_type == 'forward_pre':
-                m.register_forward_pre_hook(hook_fn)
+                handle = m.register_forward_pre_hook(hook_fn)
             elif hook_type == 'forward':
-                m.register_forward_hook(hook_fn)
+                handle = m.register_forward_hook(hook_fn)
             else:
                 assert False, "Unsupported hook type"
+            self._handles.append(handle)
 
     def _collect_output_hook(self, hook_id, *args):
         x = args[-1]  # tensor we want is last argument, output for fwd, input for fwd_pre
         if isinstance(x, tuple):
             x = x[0]  # unwrap input tuple
         self._feature_outputs[x.device][hook_id] = x
 
@@ -142,15 +205,15 @@
                 combined = [name, child_name]
                 ml.append(('_'.join(combined), '.'.join(combined), child_module))
         else:
             ml.append((name, name, module))
     return ml
 
 
-def _get_feature_info(net, out_indices):
+def _get_feature_info(net, out_indices: OutIndicesT):
     feature_info = getattr(net, 'feature_info')
     if isinstance(feature_info, FeatureInfo):
         return feature_info.from_other(out_indices)
     elif isinstance(feature_info, (list, tuple)):
         return FeatureInfo(net.feature_info, out_indices)
     else:
         assert False, "Provided feature_info is not valid"
@@ -178,15 +241,15 @@
     one Sequential container deep (`model.features.1`, with flatten_sequent=True) can be captured.
     All Sequential containers that are directly assigned to the original model will have their
     modules assigned to this module with the name `model.features.1` being changed to `model.features_1`
     """
     def __init__(
             self,
             model: nn.Module,
-            out_indices: Tuple[int, ...] = (0, 1, 2, 3, 4),
+            out_indices: OutIndicesT = (0, 1, 2, 3, 4),
             out_map: Sequence[Union[int, str]] = None,
             output_fmt: str = 'NCHW',
             feature_concat: bool = False,
             flatten_sequential: bool = False,
     ):
         """
         Args:
@@ -253,15 +316,15 @@
     """ Feature extractor with list return
 
     A specialization of FeatureDictNet that always returns features as a list (values() of dict).
     """
     def __init__(
             self,
             model: nn.Module,
-            out_indices: Tuple[int, ...] = (0, 1, 2, 3, 4),
+            out_indices: OutIndicesT = (0, 1, 2, 3, 4),
             output_fmt: str = 'NCHW',
             feature_concat: bool = False,
             flatten_sequential: bool = False,
     ):
         """
         Args:
             model: Model from which to extract features.
@@ -294,19 +357,19 @@
     FeatureList/FeatureDict case by folding first to second (Sequential only) level modules into this one.
 
     FIXME this does not currently work with Torchscript, see FeatureHooks class
     """
     def __init__(
             self,
             model: nn.Module,
-            out_indices: Tuple[int, ...] = (0, 1, 2, 3, 4),
-            out_map: Sequence[Union[int, str]] = None,
+            out_indices: OutIndicesT = (0, 1, 2, 3, 4),
+            out_map: Optional[Sequence[Union[int, str]]] = None,
             return_dict: bool = False,
             output_fmt: str = 'NCHW',
-            no_rewrite: bool = False,
+            no_rewrite: Optional[bool] = None,
             flatten_sequential: bool = False,
             default_hook_type: str = 'forward',
     ):
         """
 
         Args:
             model: Model from which to extract features.
@@ -320,15 +383,16 @@
         """
         super().__init__()
         assert not torch.jit.is_scripting()
         self.feature_info = _get_feature_info(model, out_indices)
         self.return_dict = return_dict
         self.output_fmt = Format(output_fmt)
         self.grad_checkpointing = False
-
+        if no_rewrite is None:
+            no_rewrite = not flatten_sequential
         layers = OrderedDict()
         hooks = []
         if no_rewrite:
             assert not flatten_sequential
             if hasattr(model, 'reset_classifier'):  # make sure classifier is removed?
                 model.reset_classifier(0)
             layers['body'] = model
@@ -362,7 +426,59 @@
                 # NOTE: first_or_last module could be static, but recalc in is_scripting guard to avoid jit issues
                 first_or_last_module = i == 0 or i == max(len(self) - 1, 0)
                 x = module(x) if first_or_last_module else checkpoint(module, x)
             else:
                 x = module(x)
         out = self.hooks.get_output(x.device)
         return out if self.return_dict else list(out.values())
+
+
+class FeatureGetterNet(nn.ModuleDict):
+    """ FeatureGetterNet
+
+    Wrap models with a feature getter method, like 'get_intermediate_layers'
+
+    """
+    def __init__(
+            self,
+            model: nn.Module,
+            out_indices: OutIndicesT = 4,
+            out_map: Optional[Sequence[Union[int, str]]] = None,
+            return_dict: bool = False,
+            output_fmt: str = 'NCHW',
+            norm: bool = False,
+            prune: bool = True,
+    ):
+        """
+
+        Args:
+            model: Model to wrap.
+            out_indices: Indices of features to extract.
+            out_map: Remap feature names for dict output (WIP, not supported).
+            return_dict: Return features as dictionary instead of list (WIP, not supported).
+            norm: Apply final model norm to all output features (if possible).
+        """
+        super().__init__()
+        if prune and hasattr(model, 'prune_intermediate_layers'):
+            # replace out_indices after they've been normalized, -ve indices will be invalid after prune
+            out_indices = model.prune_intermediate_layers(
+                out_indices,
+                prune_norm=not norm,
+            )
+            out_indices = list(out_indices)
+        self.feature_info = _get_feature_info(model, out_indices)
+        self.model = model
+        self.out_indices = out_indices
+        self.out_map = out_map
+        self.return_dict = return_dict
+        self.output_fmt = Format(output_fmt)
+        self.norm = norm
+
+    def forward(self, x):
+        features = self.model.forward_intermediates(
+            x,
+            indices=self.out_indices,
+            norm=self.norm,
+            output_fmt=self.output_fmt,
+            intermediates_only=True,
+        )
+        return features
```

### Comparing `timm-0.9.9/timm/models/_features_fx.py` & `timm-1.0.3/timm/models/_features_fx.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 """ PyTorch FX Based Feature Extraction Helpers
 Using https://pytorch.org/vision/stable/feature_extraction.html
 """
-from typing import Callable, List, Dict, Union, Type
+from typing import Callable, Dict, List, Optional, Union, Tuple, Type
 
 import torch
 from torch import nn
 
 from ._features import _get_feature_info, _get_return_layers
 
 try:
+    # NOTE we wrap torchvision fns to use timm leaf / no trace definitions
     from torchvision.models.feature_extraction import create_feature_extractor as _create_feature_extractor
+    from torchvision.models.feature_extraction import get_graph_node_names as _get_graph_node_names
     has_fx_feature_extraction = True
 except ImportError:
     has_fx_feature_extraction = False
 
 # Layers we went to treat as leaf modules
-from timm.layers import Conv2dSame, ScaledStdConv2dSame, CondConv2d, StdConv2dSame
+from timm.layers import Conv2dSame, ScaledStdConv2dSame, CondConv2d, StdConv2dSame, Format
 from timm.layers.non_local_attn import BilinearAttnTransform
 from timm.layers.pool2d_same import MaxPool2dSame, AvgPool2dSame
 from timm.layers.norm_act import (
     BatchNormAct2d,
     SyncBatchNormAct,
     FrozenBatchNormAct2d,
     GroupNormAct,
     GroupNorm1Act,
     LayerNormAct,
     LayerNormAct2d
 )
 
 __all__ = ['register_notrace_module', 'is_notrace_module', 'get_notrace_modules',
            'register_notrace_function', 'is_notrace_function', 'get_notrace_functions',
-           'create_feature_extractor', 'FeatureGraphNet', 'GraphExtractNet']
+           'create_feature_extractor', 'get_graph_node_names', 'FeatureGraphNet', 'GraphExtractNet']
 
 
 # NOTE: By default, any modules from timm.models.layers that we want to treat as leaf modules go here
 # BUT modules from timm.models should use the registration mechanism below
 _leaf_modules = {
     BilinearAttnTransform,  # reason: flow control t <= 1
     # Reason: get_same_padding has a max which raises a control flow error
@@ -88,31 +90,45 @@
     return func in _autowrap_functions
 
 
 def get_notrace_functions():
     return list(_autowrap_functions)
 
 
+def get_graph_node_names(model: nn.Module) -> Tuple[List[str], List[str]]:
+    return _get_graph_node_names(
+        model,
+        tracer_kwargs={'leaf_modules': list(_leaf_modules), 'autowrap_functions': list(_autowrap_functions)}
+    )
+
+
 def create_feature_extractor(model: nn.Module, return_nodes: Union[Dict[str, str], List[str]]):
     assert has_fx_feature_extraction, 'Please update to PyTorch 1.10+, torchvision 0.11+ for FX feature extraction'
     return _create_feature_extractor(
         model, return_nodes,
         tracer_kwargs={'leaf_modules': list(_leaf_modules), 'autowrap_functions': list(_autowrap_functions)}
     )
 
 
 class FeatureGraphNet(nn.Module):
     """ A FX Graph based feature extractor that works with the model feature_info metadata
     """
-    def __init__(self, model, out_indices, out_map=None):
+    def __init__(
+            self,
+            model: nn.Module,
+            out_indices: Tuple[int, ...],
+            out_map: Optional[Dict] = None,
+            output_fmt: str = 'NCHW',
+    ):
         super().__init__()
         assert has_fx_feature_extraction, 'Please update to PyTorch 1.10+, torchvision 0.11+ for FX feature extraction'
         self.feature_info = _get_feature_info(model, out_indices)
         if out_map is not None:
             assert len(out_map) == len(out_indices)
+        self.output_fmt = Format(output_fmt)
         return_nodes = _get_return_layers(self.feature_info, out_map)
         self.graph_module = create_feature_extractor(model, return_nodes)
 
     def forward(self, x):
         return list(self.graph_module(x).values())
 
 
@@ -125,15 +141,20 @@
       * create_feature_extractor can be used directly if dictionary output is acceptable
 
     Args:
         model: model to extract features from
         return_nodes: node names to return features from (dict or list)
         squeeze_out: if only one output, and output in list format, flatten to single tensor
     """
-    def __init__(self, model, return_nodes: Union[Dict[str, str], List[str]], squeeze_out: bool = True):
+    def __init__(
+            self,
+            model: nn.Module,
+            return_nodes: Union[Dict[str, str], List[str]],
+            squeeze_out: bool = True,
+    ):
         super().__init__()
         self.squeeze_out = squeeze_out
         self.graph_module = create_feature_extractor(model, return_nodes)
 
     def forward(self, x) -> Union[List[torch.Tensor], torch.Tensor]:
         out = list(self.graph_module(x).values())
         if self.squeeze_out and len(out) == 1:
```

### Comparing `timm-0.9.9/timm/models/_helpers.py` & `timm-1.0.3/timm/models/_helpers.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/_hub.py` & `timm-1.0.3/timm/models/_hub.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import hashlib
 import json
 import logging
 import os
-import sys
 from functools import partial
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Iterable, Optional, Union
 
 import torch
 from torch.hub import HASH_REGEX, download_url_to_file, urlparse
@@ -18,17 +17,17 @@
 
 try:
     import safetensors.torch
     _has_safetensors = True
 except ImportError:
     _has_safetensors = False
 
-if sys.version_info >= (3, 8):
+try:
     from typing import Literal
-else:
+except ImportError:
     from typing_extensions import Literal
 
 from timm import __version__
 from timm.models._pretrained import filter_pretrained_cfg
 
 try:
     from huggingface_hub import (
@@ -160,16 +159,17 @@
 
     # label meta-data in base config overrides saved pretrained_cfg on load
     if 'label_names' in hf_config:
         pretrained_cfg['label_names'] = hf_config.pop('label_names')
     if 'label_descriptions' in hf_config:
         pretrained_cfg['label_descriptions'] = hf_config.pop('label_descriptions')
 
+    model_args = hf_config.get('model_args', {})
     model_name = hf_config['architecture']
-    return pretrained_cfg, model_name
+    return pretrained_cfg, model_name, model_args
 
 
 def load_state_dict_from_hf(model_id: str, filename: str = HF_WEIGHTS_NAME):
     assert has_hf_hub(True)
     hf_model_id, hf_revision = hf_split(model_id)
 
     # Look for .safetensors alternatives and load from it if it exists
@@ -186,30 +186,41 @@
 
     # Otherwise, load using pytorch.load
     cached_file = hf_hub_download(hf_model_id, filename=filename, revision=hf_revision)
     _logger.debug(f"[{model_id}] Safe alternative not found for '{filename}'. Loading weights using default pytorch.")
     return torch.load(cached_file, map_location='cpu')
 
 
+def load_custom_from_hf(model_id: str, filename: str, model: torch.nn.Module):
+    assert has_hf_hub(True)
+    hf_model_id, hf_revision = hf_split(model_id)
+    cached_file = hf_hub_download(hf_model_id, filename=filename, revision=hf_revision)
+    return model.load_pretrained(cached_file)
+
+
 def save_config_for_hf(
         model,
         config_path: str,
-        model_config: Optional[dict] = None
+        model_config: Optional[dict] = None,
+        model_args: Optional[dict] = None
 ):
     model_config = model_config or {}
     hf_config = {}
     pretrained_cfg = filter_pretrained_cfg(model.pretrained_cfg, remove_source=True, remove_null=True)
     # set some values at root config level
     hf_config['architecture'] = pretrained_cfg.pop('architecture')
-    hf_config['num_classes'] = model_config.get('num_classes', model.num_classes)
-    hf_config['num_features'] = model_config.get('num_features', model.num_features)
-    global_pool_type = model_config.get('global_pool', getattr(model, 'global_pool', None))
+    hf_config['num_classes'] = model_config.pop('num_classes', model.num_classes)
+
+    # NOTE these attr saved for informational purposes, do not impact model build
+    hf_config['num_features'] = model_config.pop('num_features', model.num_features)
+    global_pool_type = model_config.pop('global_pool', getattr(model, 'global_pool', None))
     if isinstance(global_pool_type, str) and global_pool_type:
         hf_config['global_pool'] = global_pool_type
 
+    # Save class label info
     if 'labels' in model_config:
         _logger.warning(
             "'labels' as a config field for is deprecated. Please use 'label_names' and 'label_descriptions'."
             " Renaming provided 'labels' field to 'label_names'.")
         model_config.setdefault('label_names', model_config.pop('labels'))
 
     label_names = model_config.pop('label_names', None)
@@ -221,25 +232,29 @@
 
     label_descriptions = model_config.pop('label_descriptions', None)
     if label_descriptions:
         assert isinstance(label_descriptions, dict)
         # maps label names -> descriptions
         hf_config['label_descriptions'] = label_descriptions
 
+    if model_args:
+        hf_config['model_args'] = model_args
+
     hf_config['pretrained_cfg'] = pretrained_cfg
     hf_config.update(model_config)
 
     with config_path.open('w') as f:
         json.dump(hf_config, f, indent=2)
 
 
 def save_for_hf(
         model,
         save_directory: str,
         model_config: Optional[dict] = None,
+        model_args: Optional[dict] = None,
         safe_serialization: Union[bool, Literal["both"]] = False,
 ):
     assert has_hf_hub(True)
     save_directory = Path(save_directory)
     save_directory.mkdir(exist_ok=True, parents=True)
 
     # Save model weights, either safely (using safetensors), or using legacy pytorch approach or both.
@@ -247,27 +262,33 @@
     if safe_serialization is True or safe_serialization == "both":
         assert _has_safetensors, "`pip install safetensors` to use .safetensors"
         safetensors.torch.save_file(tensors, save_directory / HF_SAFE_WEIGHTS_NAME)
     if safe_serialization is False or safe_serialization == "both":
         torch.save(tensors, save_directory / HF_WEIGHTS_NAME)
 
     config_path = save_directory / 'config.json'
-    save_config_for_hf(model, config_path, model_config=model_config)
+    save_config_for_hf(
+        model,
+        config_path,
+        model_config=model_config,
+        model_args=model_args,
+    )
 
 
 def push_to_hf_hub(
-        model,
+        model: torch.nn.Module,
         repo_id: str,
         commit_message: str = 'Add model',
         token: Optional[str] = None,
         revision: Optional[str] = None,
         private: bool = False,
         create_pr: bool = False,
         model_config: Optional[dict] = None,
         model_card: Optional[dict] = None,
+        model_args: Optional[dict] = None,
         safe_serialization: Union[bool, Literal["both"]] = False,
 ):
     """
     Arguments:
         (...)
         safe_serialization (`bool` or `"both"`, *optional*, defaults to `False`):
             Whether to save the model using `safetensors` or the traditional PyTorch way (that uses `pickle`).
@@ -287,15 +308,21 @@
         has_readme = True
     except EntryNotFoundError:
         has_readme = False
 
     # Dump model and push to Hub
     with TemporaryDirectory() as tmpdir:
         # Save model weights and config.
-        save_for_hf(model, tmpdir, model_config=model_config, safe_serialization=safe_serialization)
+        save_for_hf(
+            model,
+            tmpdir,
+            model_config=model_config,
+            model_args=model_args,
+            safe_serialization=safe_serialization,
+        )
 
         # Add readme if it does not exist
         if not has_readme:
             model_card = model_card or {}
             model_name = repo_id.split('/')[-1]
             readme_path = Path(tmpdir) / "README.md"
             readme_text = generate_readme(model_card, model_name)
```

### Comparing `timm-0.9.9/timm/models/_manipulate.py` & `timm-1.0.3/timm/models/_manipulate.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/_pretrained.py` & `timm-1.0.3/timm/models/_pretrained.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/_prune.py` & `timm-1.0.3/timm/models/_prune.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/_pruned/ecaresnet101d_pruned.txt` & `timm-1.0.3/timm/models/_pruned/ecaresnet101d_pruned.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/_pruned/ecaresnet50d_pruned.txt` & `timm-1.0.3/timm/models/_pruned/ecaresnet50d_pruned.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/_pruned/efficientnet_b1_pruned.txt` & `timm-1.0.3/timm/models/_pruned/efficientnet_b1_pruned.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/_pruned/efficientnet_b2_pruned.txt` & `timm-1.0.3/timm/models/_pruned/efficientnet_b2_pruned.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/_pruned/efficientnet_b3_pruned.txt` & `timm-1.0.3/timm/models/_pruned/efficientnet_b3_pruned.txt`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/_registry.py` & `timm-1.0.3/timm/models/_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,20 @@
     model_name = fn.__name__
     if hasattr(mod, '__all__'):
         mod.__all__.append(model_name)
     else:
         mod.__all__ = [model_name]  # type: ignore
 
     # add entries to registry dict/sets
+    if model_name in _model_entrypoints:
+        warnings.warn(
+            f'Overwriting {model_name} in registry with {fn.__module__}.{model_name}. This is because the name being '
+            'registered conflicts with an existing name. Please check if this is not expected.',
+            stacklevel=2,
+        )
     _model_entrypoints[model_name] = fn
     _model_to_module[model_name] = module_name
     _module_to_models[module_name].add(model_name)
     if hasattr(mod, 'default_cfgs') and model_name in mod.default_cfgs:
         # this will catch all models that have entrypoint matching cfg key, but miss any aliasing
         # entrypoints or non-matching combos
         default_cfg = mod.default_cfgs[model_name]
@@ -174,15 +180,15 @@
         return ['.'.join([filter_base, '*']), filter]
     else:
         return [filter]
 
 
 def list_models(
         filter: Union[str, List[str]] = '',
-        module: str = '',
+        module: Union[str, List[str]] = '',
         pretrained: bool = False,
         exclude_filters: Union[str, List[str]] = '',
         name_matches_cfg: bool = False,
         include_tags: Optional[bool] = None,
 ) -> List[str]:
     """ Return list of available model names, sorted alphabetically
 
@@ -207,15 +213,24 @@
     else:
         include_filters = []
 
     if include_tags is None:
         # FIXME should this be default behaviour? or default to include_tags=True?
         include_tags = pretrained
 
-    all_models: Set[str] = _module_to_models[module] if module else set(_model_entrypoints.keys())
+    if not module:
+        all_models: Set[str] = set(_model_entrypoints.keys())
+    else:
+        if isinstance(module, str):
+            all_models: Set[str] = _module_to_models[module]
+        else:
+            assert isinstance(module, Sequence)
+            all_models: Set[str] = set()
+            for m in module:
+                all_models.update(_module_to_models[m])
     all_models = all_models - _deprecated_models.keys()  # remove deprecated models from listings
 
     if include_tags:
         # expand model names to include names w/ pretrained tags
         models_with_tags: Set[str] = set()
         for m in all_models:
             models_with_tags.update(_model_with_tags[m])
```

### Comparing `timm-0.9.9/timm/models/beit.py` & `timm-1.0.3/timm/models/beit.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,41 +35,39 @@
 # Based on timm and DeiT code bases
 # https://github.com/rwightman/pytorch-image-models/tree/master/timm
 # https://github.com/facebookresearch/deit/
 # https://github.com/facebookresearch/dino
 # --------------------------------------------------------'
 
 import math
-from typing import Callable, Optional, Tuple, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils.checkpoint import checkpoint
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import PatchEmbed, Mlp, SwiGLU, LayerNorm, DropPath, trunc_normal_, use_fused_attn
-from timm.layers import resample_patch_embed, resample_abs_pos_embed, resize_rel_pos_bias_table
+from timm.layers import resample_patch_embed, resample_abs_pos_embed, resize_rel_pos_bias_table, ndgrid
 
 
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._registry import generate_default_cfgs, register_model
-from .vision_transformer import checkpoint_filter_fn
 
 __all__ = ['Beit']
 
 
 def gen_relative_position_index(window_size: Tuple[int, int]) -> torch.Tensor:
     num_relative_distance = (2 * window_size[0] - 1) * (2 * window_size[1] - 1) + 3
     # cls to token & token 2 cls & cls to cls
     # get pair-wise relative position index for each token inside the window
     window_area = window_size[0] * window_size[1]
-    coords = torch.stack(torch.meshgrid(
-        [torch.arange(window_size[0]),
-         torch.arange(window_size[1])]))  # 2, Wh, Ww
+    coords = torch.stack(ndgrid(torch.arange(window_size[0]), torch.arange(window_size[1])))  # 2, Wh, Ww
     coords_flatten = torch.flatten(coords, 1)  # 2, Wh*Ww
     relative_coords = coords_flatten[:, :, None] - coords_flatten[:, None, :]  # 2, Wh*Ww, Wh*Ww
     relative_coords = relative_coords.permute(1, 2, 0).contiguous()  # Wh*Ww, Wh*Ww, 2
     relative_coords[:, :, 0] += window_size[0] - 1  # shift to start from 0
     relative_coords[:, :, 1] += window_size[1] - 1
     relative_coords[:, :, 0] *= 2 * window_size[1] - 1
     relative_position_index = torch.zeros(size=(window_area + 1,) * 2, dtype=relative_coords.dtype)
@@ -300,14 +298,15 @@
         self.patch_embed = PatchEmbed(
             img_size=img_size,
             patch_size=patch_size,
             in_chans=in_chans,
             embed_dim=embed_dim,
         )
         num_patches = self.patch_embed.num_patches
+        r = self.patch_embed.feat_ratio() if hasattr(self.patch_embed, 'feat_ratio') else patch_size
 
         self.cls_token = nn.Parameter(torch.zeros(1, 1, embed_dim))
         # self.mask_token = nn.Parameter(torch.zeros(1, 1, embed_dim))
         self.pos_embed = nn.Parameter(torch.zeros(1, num_patches + 1, embed_dim)) if use_abs_pos_emb else None
         self.pos_drop = nn.Dropout(p=pos_drop_rate)
 
         if use_shared_rel_pos_bias:
@@ -331,14 +330,16 @@
                 attn_drop=attn_drop_rate,
                 drop_path=dpr[i],
                 norm_layer=norm_layer,
                 init_values=init_values,
                 window_size=self.patch_embed.grid_size if use_rel_pos_bias else None,
             )
             for i in range(depth)])
+        self.feature_info = [
+            dict(module=f'blocks.{i}', num_chs=embed_dim, reduction=r) for i in range(depth)]
 
         use_fc_norm = self.global_pool == 'avg'
         self.norm = nn.Identity() if use_fc_norm else norm_layer(embed_dim)
         self.fc_norm = norm_layer(embed_dim) if use_fc_norm else nn.Identity()
         self.head_drop = nn.Dropout(drop_rate)
         self.head = nn.Linear(embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
@@ -390,20 +391,104 @@
         )
         return matcher
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             self.global_pool = global_pool
         self.head = nn.Linear(self.embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            return_prefix_tokens: bool = False,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if an int, if is a sequence, select by matching indices
+            return_prefix_tokens: Return both prefix and spatial intermediate tokens
+            norm: Apply norm layer to all intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW', 'NLC'), 'Output format must be one of NCHW or NLC.'
+        reshape = output_fmt == 'NCHW'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+
+        # forward pass
+        B, _, height, width = x.shape
+        x = self.patch_embed(x)
+        x = torch.cat((self.cls_token.expand(x.shape[0], -1, -1), x), dim=1)
+        if self.pos_embed is not None:
+            x = x + self.pos_embed
+        x = self.pos_drop(x)
+
+        rel_pos_bias = self.rel_pos_bias() if self.rel_pos_bias is not None else None
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            blocks = self.blocks
+        else:
+            blocks = self.blocks[:max_index + 1]
+        for i, blk in enumerate(blocks):
+            x = blk(x, shared_rel_pos_bias=rel_pos_bias)
+            if i in take_indices:
+                # normalize intermediates with final norm layer if enabled
+                intermediates.append(self.norm(x) if norm else x)
+
+        # process intermediates
+        if self.num_prefix_tokens:
+            # split prefix (e.g. class, distill) and spatial feature tokens
+            prefix_tokens = [y[:, 0:self.num_prefix_tokens] for y in intermediates]
+            intermediates = [y[:, self.num_prefix_tokens:] for y in intermediates]
+        if reshape:
+            # reshape to BCHW output format
+            H, W = self.patch_embed.dynamic_feat_size((height, width))
+            intermediates = [y.reshape(B, H, W, -1).permute(0, 3, 1, 2).contiguous() for y in intermediates]
+        if not torch.jit.is_scripting() and return_prefix_tokens:
+            # return_prefix not support in torchscript due to poor type handling
+            intermediates = list(zip(intermediates, prefix_tokens))
+
+        if intermediates_only:
+            return intermediates
+
+        x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+        self.blocks = self.blocks[:max_index + 1]  # truncate blocks
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.fc_norm = nn.Identity()
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.patch_embed(x)
         x = torch.cat((self.cls_token.expand(x.shape[0], -1, -1), x), dim=1)
         if self.pos_embed is not None:
             x = x + self.pos_embed
         x = self.pos_drop(x)
 
@@ -545,22 +630,21 @@
                     new_bias_shape=m.relative_position_bias_table.shape,
                 )
         out_dict[k] = v
     return out_dict
 
 
 def _create_beit(variant, pretrained=False, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError('features_only not implemented for BEiT models.')
-
+    out_indices = kwargs.pop('out_indices', 3)
     model = build_model_with_cfg(
         Beit, variant, pretrained,
-        # FIXME an updated filter fn needed to interpolate rel pos emb if fine tuning to diff model sizes
         pretrained_filter_fn=_beit_checkpoint_filter_fn,
-        **kwargs)
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
+        **kwargs,
+    )
     return model
 
 
 @register_model
 def beit_base_patch16_224(pretrained=False, **kwargs) -> Beit:
     model_args = dict(
         patch_size=16, embed_dim=768, depth=12, num_heads=12, mlp_ratio=4,
```

### Comparing `timm-0.9.9/timm/models/byoanet.py` & `timm-1.0.3/timm/models/byoanet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/byobnet.py` & `timm-1.0.3/timm/models/byobnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import ClassifierHead, ConvNormAct, BatchNormAct2d, DropPath, AvgPool2dSame, \
     create_conv2d, get_act_layer, get_norm_act_layer, get_attn, make_divisible, to_2tuple, EvoNorm2dS0a
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._manipulate import named_apply, checkpoint_seq
 from ._registry import generate_default_cfgs, register_model
 
 __all__ = ['ByobNet', 'ByoModelCfg', 'ByoBlockCfg', 'create_byob_stem', 'create_block']
 
 
 @dataclass
@@ -944,33 +945,45 @@
             stem_strides[-1] = 2
 
         num_act = num_rep if num_act is None else num_act
         # if num_act < num_rep, first convs in stack won't have bn + act
         stem_norm_acts = [False] * (num_rep - num_act) + [True] * num_act
         prev_chs = in_chs
         curr_stride = 1
+        last_feat_idx = -1
         for i, (ch, s, na) in enumerate(zip(stem_chs, stem_strides, stem_norm_acts)):
             layer_fn = layers.conv_norm_act if na else create_conv2d
             conv_name = f'conv{i + 1}'
             if i > 0 and s > 1:
-                self.feature_info.append(dict(num_chs=prev_chs, reduction=curr_stride, module=prev_feat))
+                last_feat_idx = i - 1
+                self.feature_info.append(dict(num_chs=prev_chs, reduction=curr_stride, module=prev_feat, stage=0))
             self.add_module(conv_name, layer_fn(prev_chs, ch, kernel_size=kernel_size, stride=s))
             prev_chs = ch
             curr_stride *= s
             prev_feat = conv_name
 
         if pool and 'max' in pool.lower():
-            self.feature_info.append(dict(num_chs=prev_chs, reduction=curr_stride, module=prev_feat))
+            last_feat_idx = i
+            self.feature_info.append(dict(num_chs=prev_chs, reduction=curr_stride, module=prev_feat, stage=0))
             self.add_module('pool', nn.MaxPool2d(3, 2, 1))
             curr_stride *= 2
             prev_feat = 'pool'
 
-        self.feature_info.append(dict(num_chs=prev_chs, reduction=curr_stride, module=prev_feat))
+        self.last_feat_idx = last_feat_idx if last_feat_idx >= 0 else None
+        self.feature_info.append(dict(num_chs=prev_chs, reduction=curr_stride, module=prev_feat, stage=0))
         assert curr_stride == stride
 
+    def forward_intermediates(self, x) -> Tuple[torch.Tensor, Optional[torch.Tensor]]:
+        intermediate: Optional[torch.Tensor] = None
+        for i, m in enumerate(self):
+            x = m(x)
+            if self.last_feat_idx is not None and i == self.last_feat_idx:
+                intermediate = x
+        return x, intermediate
+
 
 def create_byob_stem(
         in_chs: int,
         out_chs: int,
         stem_type: str = '',
         pool_type: str = '',
         feat_prefix: str = 'stem',
@@ -1004,15 +1017,15 @@
             stem = Stem(in_chs, out_chs, 3, num_rep=1, pool=pool_type, layers=layers)
         else:
             stem = layers.conv_norm_act(in_chs, out_chs, 3, stride=2)
 
     if isinstance(stem, Stem):
         feature_info = [dict(f, module='.'.join([feat_prefix, f['module']])) for f in stem.feature_info]
     else:
-        feature_info = [dict(num_chs=out_chs, reduction=2, module=feat_prefix)]
+        feature_info = [dict(num_chs=out_chs, reduction=2, module=feat_prefix, stage=0)]
     return stem, feature_info
 
 
 def reduce_feat_size(feat_size, stride=2):
     return None if feat_size is None else tuple([s // stride for s in feat_size])
 
 
@@ -1118,15 +1131,15 @@
             blocks += [create_block(block_cfg.type, **block_kwargs)]
             first_dilation = dilation
             prev_chs = out_chs
             if stride > 1 and block_idx == 0:
                 feat_size = reduce_feat_size(feat_size, stride)
 
         stages += [nn.Sequential(*blocks)]
-        prev_feat = dict(num_chs=prev_chs, reduction=net_stride, module=f'stages.{stage_idx}')
+        prev_feat = dict(num_chs=prev_chs, reduction=net_stride, module=f'stages.{stage_idx}', stage=stage_idx + 1)
 
     feature_info.append(prev_feat)
     return nn.Sequential(*stages), feature_info
 
 
 def get_layer_fns(cfg: ByoModelCfg):
     act = get_act_layer(cfg.act_layer)
@@ -1194,24 +1207,26 @@
             drop_path_rate,
             output_stride,
             stem_feat[-1],
             layers=layers,
             feat_size=feat_size,
         )
         self.feature_info.extend(stage_feat[:-1])
+        reduction = stage_feat[-1]['reduction']
 
         prev_chs = stage_feat[-1]['num_chs']
         if cfg.num_features:
             self.num_features = int(round(cfg.width_factor * cfg.num_features))
             self.final_conv = layers.conv_norm_act(prev_chs, self.num_features, 1)
         else:
             self.num_features = prev_chs
             self.final_conv = nn.Identity()
         self.feature_info += [
-            dict(num_chs=self.num_features, reduction=stage_feat[-1]['reduction'], module='final_conv')]
+            dict(num_chs=self.num_features, reduction=reduction, module='final_conv', stage=len(self.stages))]
+        self.stage_ends = [f['stage'] for f in self.feature_info]
 
         self.head = ClassifierHead(
             self.num_features,
             num_classes,
             pool_type=global_pool,
             drop_rate=self.drop_rate,
         )
@@ -1237,25 +1252,102 @@
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
     def reset_classifier(self, num_classes, global_pool='avg'):
         self.head.reset(num_classes, global_pool)
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+            exclude_final_conv: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to compatible intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+            exclude_final_conv: Exclude final_conv from last intermediate
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output shape must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.stage_ends), indices)
+        take_indices = [self.stage_ends[i] for i in take_indices]
+        max_index = self.stage_ends[max_index]
+        # forward pass
+        feat_idx = 0  # stem is index 0
+        if hasattr(self.stem, 'forward_intermediates'):
+            # returns last intermediate features in stem (before final stride in stride > 2 stems)
+            x, x_inter = self.stem.forward_intermediates(x)
+        else:
+            x, x_inter = self.stem(x), None
+        if feat_idx in take_indices:
+            intermediates.append(x if x_inter is None else x_inter)
+        last_idx = self.stage_ends[-1]
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            stages = self.stages
+        else:
+            stages = self.stages[:max_index]
+        for stage in stages:
+            feat_idx += 1
+            x = stage(x)
+            if not exclude_final_conv and feat_idx == last_idx:
+                # default feature_info for this model uses final_conv as the last feature output (if present)
+                x = self.final_conv(x)
+            if feat_idx in take_indices:
+                intermediates.append(x)
+
+        if intermediates_only:
+            return intermediates
+
+        if exclude_final_conv and feat_idx == last_idx:
+            x = self.final_conv(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.stage_ends), indices)
+        max_index = self.stage_ends[max_index]
+        self.stages = self.stages[:max_index]  # truncate blocks w/ stem as idx 0
+        if max_index < self.stage_ends[-1]:
+            self.final_conv = nn.Identity()
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
+
     def forward_features(self, x):
         x = self.stem(x)
         if self.grad_checkpointing and not torch.jit.is_scripting():
             x = checkpoint_seq(self.stages, x)
         else:
             x = self.stages(x)
         x = self.final_conv(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
-        return self.head(x, pre_logits=pre_logits)
+        return self.head(x, pre_logits=pre_logits) if pre_logits else self.head(x)
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
```

### Comparing `timm-0.9.9/timm/models/cait.py` & `timm-1.0.3/timm/models/cait.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 Original code and weights from https://github.com/facebookresearch/deit, copyright below
 
 Modifications and additions for timm hacked together by / Copyright 2021, Ross Wightman
 """
 # Copyright (c) 2015-present, Facebook, Inc.
 # All rights reserved.
 from functools import partial
+from typing import List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import PatchEmbed, Mlp, DropPath, trunc_normal_, use_fused_attn
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._manipulate import checkpoint_seq
 from ._registry import register_model, generate_default_cfgs
 
 __all__ = ['Cait', 'ClassAttn', 'LayerScaleBlockClassAttn', 'LayerScaleBlock', 'TalkingHeadAttn']
 
 
 class ClassAttn(nn.Module):
@@ -242,16 +244,16 @@
 
         self.patch_embed = patch_layer(
             img_size=img_size,
             patch_size=patch_size,
             in_chans=in_chans,
             embed_dim=embed_dim,
         )
-
         num_patches = self.patch_embed.num_patches
+        r = self.patch_embed.feat_ratio() if hasattr(self.patch_embed, 'feat_ratio') else patch_size
 
         self.cls_token = nn.Parameter(torch.zeros(1, 1, embed_dim))
         self.pos_embed = nn.Parameter(torch.zeros(1, num_patches, embed_dim))
         self.pos_drop = nn.Dropout(p=pos_drop_rate)
 
         dpr = [drop_path_rate for i in range(depth)]
         self.blocks = nn.Sequential(*[block_layers(
@@ -264,14 +266,15 @@
             drop_path=dpr[i],
             norm_layer=norm_layer,
             act_layer=act_layer,
             attn_block=attn_block,
             mlp_block=mlp_block,
             init_values=init_values,
         ) for i in range(depth)])
+        self.feature_info = [dict(num_chs=embed_dim, reduction=r, module=f'blocks.{i}') for i in range(depth)]
 
         self.blocks_token_only = nn.ModuleList([block_layers_token(
             dim=embed_dim,
             num_heads=num_heads,
             mlp_ratio=mlp_ratio_token_only,
             qkv_bias=qkv_bias,
             norm_layer=norm_layer,
@@ -279,15 +282,14 @@
             attn_block=attn_block_token_only,
             mlp_block=mlp_block_token_only,
             init_values=init_values,
         ) for _ in range(depth_token_only)])
 
         self.norm = norm_layer(embed_dim)
 
-        self.feature_info = [dict(num_chs=embed_dim, reduction=0, module='head')]
         self.head_drop = nn.Dropout(drop_rate)
         self.head = nn.Linear(embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
         trunc_normal_(self.pos_embed, std=.02)
         trunc_normal_(self.cls_token, std=.02)
         self.apply(self._init_weights)
 
@@ -325,21 +327,96 @@
                 return float('inf')
         return _matcher
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             assert global_pool in ('', 'token', 'avg')
             self.global_pool = global_pool
         self.head = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to all intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        """
+        assert output_fmt in ('NCHW', 'NLC'), 'Output format must be one of NCHW or NLC.'
+        reshape = output_fmt == 'NCHW'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+
+        # forward pass
+        B, _, height, width = x.shape
+        x = self.patch_embed(x)
+        x = x + self.pos_embed
+        x = self.pos_drop(x)
+
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            blocks = self.blocks
+        else:
+            blocks = self.blocks[:max_index + 1]
+        for i, blk in enumerate(blocks):
+            x = blk(x)
+            if i in take_indices:
+                # normalize intermediates with final norm layer if enabled
+                intermediates.append(self.norm(x) if norm else x)
+
+        # process intermediates
+        if reshape:
+            # reshape to BCHW output format
+            H, W = self.patch_embed.dynamic_feat_size((height, width))
+            intermediates = [y.reshape(B, H, W, -1).permute(0, 3, 1, 2).contiguous() for y in intermediates]
+
+        if intermediates_only:
+            return intermediates
+
+        # NOTE not supporting return of class tokens
+        cls_tokens = self.cls_token.expand(x.shape[0], -1, -1)
+        for i, blk in enumerate(self.blocks_token_only):
+            cls_tokens = blk(x, cls_tokens)
+        x = torch.cat((cls_tokens, x), dim=1)
+        x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+        self.blocks = self.blocks[:max_index + 1]  # truncate blocks
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.blocks_token_only = nn.ModuleList()  # prune token blocks with head
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.patch_embed(x)
         x = x + self.pos_embed
         x = self.pos_drop(x)
         if self.grad_checkpointing and not torch.jit.is_scripting():
             x = checkpoint_seq(self.blocks, x)
         else:
@@ -369,22 +446,21 @@
     checkpoint_no_module = {}
     for k, v in state_dict.items():
         checkpoint_no_module[k.replace('module.', '')] = v
     return checkpoint_no_module
 
 
 def _create_cait(variant, pretrained=False, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError('features_only not implemented for Vision Transformer models.')
-
+    out_indices = kwargs.pop('out_indices', 3)
     model = build_model_with_cfg(
         Cait,
         variant,
         pretrained,
         pretrained_filter_fn=checkpoint_filter_fn,
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
         **kwargs,
     )
     return model
 
 
 def _cfg(url='', **kwargs):
     return {
```

### Comparing `timm-0.9.9/timm/models/coat.py` & `timm-1.0.3/timm/models/coat.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 Paper: Co-Scale Conv-Attentional Image Transformers - https://arxiv.org/abs/2104.06399
 
 Official CoaT code at: https://github.com/mlpc-ucsd/CoaT
 
 Modified from timm/models/vision_transformer.py
 """
-from functools import partial
-from typing import Tuple, List, Union
+from typing import List, Optional, Union, Tuple
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import PatchEmbed, Mlp, DropPath, to_2tuple, trunc_normal_, _assert, LayerNorm
@@ -556,15 +555,15 @@
         )
         return matcher
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             assert global_pool in ('token', 'avg')
             self.global_pool = global_pool
         self.head = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
 
     def forward_features(self, x0):
```

### Comparing `timm-0.9.9/timm/models/convit.py` & `timm-1.0.3/timm/models/convit.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 #
 # This source code is licensed under the CC-by-NC license found in the
 # LICENSE file in the root directory of this source tree.
 #
 '''These modules are adapted from those of timm, see
 https://github.com/rwightman/pytorch-image-models/blob/master/timm/models/vision_transformer.py
 '''
-
-from functools import partial
+from typing import Optional
 
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import DropPath, trunc_normal_, PatchEmbed, Mlp, LayerNorm
 from ._builder import build_model_with_cfg
@@ -345,15 +344,15 @@
     def set_grad_checkpointing(self, enable=True):
         assert not enable, 'gradient checkpointing not supported'
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             assert global_pool in ('', 'token', 'avg')
             self.global_pool = global_pool
         self.head = nn.Linear(self.embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
     def forward_features(self, x):
```

### Comparing `timm-0.9.9/timm/models/convmixer.py` & `timm-1.0.3/timm/models/convmixer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """ ConvMixer
 
 """
+from typing import Optional
+
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import SelectAdaptivePool2d
 from ._registry import register_model, generate_default_cfgs
 from ._builder import build_model_with_cfg
@@ -71,15 +73,15 @@
     def set_grad_checkpointing(self, enable=True):
         self.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             self.pooling = SelectAdaptivePool2d(pool_type=global_pool, flatten=True)
         self.head = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
           
     def forward_features(self, x):
         x = self.stem(x)
```

### Comparing `timm-0.9.9/timm/models/convnext.py` & `timm-1.0.3/timm/models/convnext.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 # ConvNeXt-V2
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree (Attribution-NonCommercial 4.0 International (CC BY-NC 4.0))
 # No code was used directly from ConvNeXt-V2, however the weights are CC BY-NC 4.0 so beware if using commercially.
 
-from collections import OrderedDict
 from functools import partial
-from typing import Callable, Optional, Tuple, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD, OPENAI_CLIP_MEAN, OPENAI_CLIP_STD
 from timm.layers import trunc_normal_, AvgPool2dSame, DropPath, Mlp, GlobalResponseNormMlp, \
     LayerNorm2d, LayerNorm, create_conv2d, get_act_layer, make_divisible, to_ntuple
 from timm.layers import NormMlpClassifierHead, ClassifierHead
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._manipulate import named_apply, checkpoint_seq
 from ._registry import generate_default_cfgs, register_model, register_model_deprecations
 
 __all__ = ['ConvNeXt']  # model_registry will add each entrypoint fn to this
 
 
 class Downsample(nn.Module):
@@ -403,14 +403,79 @@
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
     def reset_classifier(self, num_classes=0, global_pool=None):
         self.head.reset(num_classes, global_pool)
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to compatible intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output shape must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.stages) + 1, indices)
+
+        # forward pass
+        feat_idx = 0  # stem is index 0
+        x = self.stem(x)
+        if feat_idx in take_indices:
+            intermediates.append(x)
+
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            stages = self.stages
+        else:
+            stages = self.stages[:max_index]
+        for stage in stages:
+            feat_idx += 1
+            x = stage(x)
+            if feat_idx in take_indices:
+                # NOTE not bothering to apply norm_pre when norm=True as almost no models have it enabled
+                intermediates.append(x)
+
+        if intermediates_only:
+            return intermediates
+
+        x = self.norm_pre(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.stages) + 1, indices)
+        self.stages = self.stages[:max_index]  # truncate blocks w/ stem as idx 0
+        if prune_norm:
+            self.norm_pre = nn.Identity()
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.stem(x)
         x = self.stages(x)
         x = self.norm_pre(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
```

### Comparing `timm-0.9.9/timm/models/crossvit.py` & `timm-1.0.3/timm/models/crossvit.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 
 
 """
 Modifed from Timm. https://github.com/rwightman/pytorch-image-models/blob/master/timm/models/vision_transformer.py
 
 """
 from functools import partial
-from typing import List
-from typing import Tuple
+from typing import List, Optional, Tuple
 
 import torch
 import torch.hub
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import DropPath, to_2tuple, trunc_normal_, _assert
@@ -415,15 +414,15 @@
     def set_grad_checkpointing(self, enable=True):
         assert not enable, 'gradient checkpointing not supported'
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             assert global_pool in ('token', 'avg')
             self.global_pool = global_pool
         self.head = nn.ModuleList(
             [nn.Linear(self.embed_dim[i], num_classes) if num_classes > 0 else nn.Identity() for i in
              range(self.num_branches)])
```

### Comparing `timm-0.9.9/timm/models/cspnet.py` & `timm-1.0.3/timm/models/cspnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -706,15 +706,15 @@
 
     def forward_features(self, x):
         x = self.stem(x)
         x = self.stages(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
-        return self.head(x, pre_logits=pre_logits)
+        return self.head(x, pre_logits=pre_logits) if pre_logits else self.head(x)
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
```

### Comparing `timm-0.9.9/timm/models/davit.py` & `timm-1.0.3/timm/models/davit.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 DaViT model defs and weights adapted from https://github.com/dingmyu/davit, original copyright below
 
 """
 # Copyright (c) 2022 Mingyu Ding
 # All rights reserved.
 # This source code is licensed under the MIT license
 from functools import partial
-from typing import Tuple
+from typing import Optional, Tuple
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
@@ -122,17 +122,17 @@
     def forward(self, x: Tensor):
         B, N, C = x.shape
 
         qkv = self.qkv(x).reshape(B, N, 3, self.num_heads, C // self.num_heads).permute(2, 0, 3, 1, 4)
         q, k, v = qkv.unbind(0)
 
         k = k * self.scale
-        attention = k.transpose(-1, -2) @ v
-        attention = attention.softmax(dim=-1)
-        x = (attention @ q.transpose(-1, -2)).transpose(-1, -2)
+        attn = k.transpose(-1, -2) @ v
+        attn = attn.softmax(dim=-1)
+        x = (attn @ q.transpose(-1, -2)).transpose(-1, -2)
         x = x.transpose(1, 2).reshape(B, N, C)
         x = self.proj(x)
         return x
 
 
 class ChannelBlock(nn.Module):
 
@@ -544,41 +544,48 @@
     def _init_weights(self, m):
         if isinstance(m, nn.Linear):
             trunc_normal_(m.weight, std=.02)
             if isinstance(m, nn.Linear) and m.bias is not None:
                 nn.init.constant_(m.bias, 0)
 
     @torch.jit.ignore
+    def group_matcher(self, coarse=False):
+        return dict(
+            stem=r'^stem',  # stem and embed
+            blocks=r'^stages\.(\d+)' if coarse else [
+                (r'^stages\.(\d+).downsample', (0,)),
+                (r'^stages\.(\d+)\.blocks\.(\d+)', None),
+                (r'^norm_pre', (99999,)),
+            ]
+        )
+
+    @torch.jit.ignore
     def set_grad_checkpointing(self, enable=True):
         self.grad_checkpointing = enable
         for stage in self.stages:
             stage.set_grad_checkpointing(enable=enable)
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
-    def reset_classifier(self, num_classes, global_pool=None):
-        self.head.reset(num_classes, global_pool=global_pool)
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
+        self.head.reset(num_classes, global_pool)
 
     def forward_features(self, x):
         x = self.stem(x)
         if self.grad_checkpointing and not torch.jit.is_scripting():
             x = checkpoint_seq(self.stages, x)
         else:
             x = self.stages(x)
         x = self.norm_pre(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
-        x = self.head.global_pool(x)
-        x = self.head.norm(x)
-        x = self.head.flatten(x)
-        x = self.head.drop(x)
-        return x if pre_logits else self.head.fc(x)
+        return self.head(x, pre_logits=True) if pre_logits else self.head(x)
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
@@ -644,45 +651,39 @@
     'davit_huge': _cfg(),
     'davit_giant': _cfg(),
 })
 
 
 @register_model
 def davit_tiny(pretrained=False, **kwargs) -> DaVit:
-    model_kwargs = dict(
-        depths=(1, 1, 3, 1), embed_dims=(96, 192, 384, 768), num_heads=(3, 6, 12, 24), **kwargs)
-    return _create_davit('davit_tiny', pretrained=pretrained, **model_kwargs)
+    model_args = dict(depths=(1, 1, 3, 1), embed_dims=(96, 192, 384, 768), num_heads=(3, 6, 12, 24))
+    return _create_davit('davit_tiny', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def davit_small(pretrained=False, **kwargs) -> DaVit:
-    model_kwargs = dict(
-        depths=(1, 1, 9, 1), embed_dims=(96, 192, 384, 768), num_heads=(3, 6, 12, 24), **kwargs)
-    return _create_davit('davit_small', pretrained=pretrained, **model_kwargs)
+    model_args = dict(depths=(1, 1, 9, 1), embed_dims=(96, 192, 384, 768), num_heads=(3, 6, 12, 24))
+    return _create_davit('davit_small', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def davit_base(pretrained=False, **kwargs) -> DaVit:
-    model_kwargs = dict(
-        depths=(1, 1, 9, 1), embed_dims=(128, 256, 512, 1024), num_heads=(4, 8, 16, 32), **kwargs)
-    return _create_davit('davit_base', pretrained=pretrained, **model_kwargs)
+    model_args = dict(depths=(1, 1, 9, 1), embed_dims=(128, 256, 512, 1024), num_heads=(4, 8, 16, 32))
+    return _create_davit('davit_base', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def davit_large(pretrained=False, **kwargs) -> DaVit:
-    model_kwargs = dict(
-        depths=(1, 1, 9, 1), embed_dims=(192, 384, 768, 1536), num_heads=(6, 12, 24, 48), **kwargs)
-    return _create_davit('davit_large', pretrained=pretrained, **model_kwargs)
+    model_args = dict(depths=(1, 1, 9, 1), embed_dims=(192, 384, 768, 1536), num_heads=(6, 12, 24, 48))
+    return _create_davit('davit_large', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def davit_huge(pretrained=False, **kwargs) -> DaVit:
-    model_kwargs = dict(
-        depths=(1, 1, 9, 1), embed_dims=(256, 512, 1024, 2048), num_heads=(8, 16, 32, 64), **kwargs)
-    return _create_davit('davit_huge', pretrained=pretrained, **model_kwargs)
+    model_args = dict(depths=(1, 1, 9, 1), embed_dims=(256, 512, 1024, 2048), num_heads=(8, 16, 32, 64))
+    return _create_davit('davit_huge', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def davit_giant(pretrained=False, **kwargs) -> DaVit:
-    model_kwargs = dict(
-        depths=(1, 1, 12, 3), embed_dims=(384, 768, 1536, 3072), num_heads=(12, 24, 48, 96), **kwargs)
-    return _create_davit('davit_giant', pretrained=pretrained, **model_kwargs)
+    model_args = dict(depths=(1, 1, 12, 3), embed_dims=(384, 768, 1536, 3072), num_heads=(12, 24, 48, 96))
+    return _create_davit('davit_giant', pretrained=pretrained, **dict(model_args, **kwargs))
```

### Comparing `timm-0.9.9/timm/models/deit.py` & `timm-1.0.3/timm/models/deit.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 paper: `DeiT III: Revenge of the ViT` - https://arxiv.org/abs/2204.07118
 
 Modifications copyright 2021, Ross Wightman
 """
 # Copyright (c) 2015-present, Facebook, Inc.
 # All rights reserved.
 from functools import partial
-from typing import Sequence, Union
+from typing import Optional
 
 import torch
 from torch import nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import resample_abs_pos_embed
 from timm.models.vision_transformer import VisionTransformer, trunc_normal_, checkpoint_filter_fn
 from ._builder import build_model_with_cfg
-from ._manipulate import checkpoint_seq
 from ._registry import generate_default_cfgs, register_model, register_model_deprecations
 
 __all__ = ['VisionTransformerDistilled']  # model_registry will add each entrypoint fn to this
 
 
 class VisionTransformerDistilled(VisionTransformer):
     """ Vision Transformer w/ Distillation Token and Head
@@ -60,15 +59,15 @@
                 (r'^norm', (99999,))]  # final norm w/ last block
         )
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head, self.head_dist
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         self.head = nn.Linear(self.embed_dim, num_classes) if num_classes > 0 else nn.Identity()
         self.head_dist = nn.Linear(self.embed_dim, self.num_classes) if num_classes > 0 else nn.Identity()
 
     @torch.jit.ignore
     def set_distilled_training(self, enable=True):
         self.distilled_training = enable
@@ -115,22 +114,22 @@
             return x, x_dist
         else:
             # during standard train / finetune, inference average the classifier predictions
             return (x + x_dist) / 2
 
 
 def _create_deit(variant, pretrained=False, distilled=False, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError('features_only not implemented for Vision Transformer models.')
+    out_indices = kwargs.pop('out_indices', 3)
     model_cls = VisionTransformerDistilled if distilled else VisionTransformer
     model = build_model_with_cfg(
         model_cls,
         variant,
         pretrained,
         pretrained_filter_fn=partial(checkpoint_filter_fn, adapt_layer_scale=True),
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
         **kwargs,
     )
     return model
 
 
 def _cfg(url='', **kwargs):
     return {
```

### Comparing `timm-0.9.9/timm/models/densenet.py` & `timm-1.0.3/timm/models/densenet.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import torch.utils.checkpoint as cp
 from torch.jit.annotations import List
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import BatchNormAct2d, get_norm_act_layer, BlurPool2d, create_classifier
 from ._builder import build_model_with_cfg
 from ._manipulate import MATCH_PREV_GROUP
-from ._registry import register_model, generate_default_cfgs
+from ._registry import register_model, generate_default_cfgs, register_model_deprecations
 
 __all__ = ['DenseNet']
 
 
 class DenseLayer(nn.Module):
     def __init__(
             self,
@@ -357,62 +357,65 @@
 
 
 @register_model
 def densenet121(pretrained=False, **kwargs) -> DenseNet:
     r"""Densenet-121 model from
     `"Densely Connected Convolutional Networks" <https://arxiv.org/pdf/1608.06993.pdf>`
     """
-    model = _create_densenet(
-        'densenet121', growth_rate=32, block_config=(6, 12, 24, 16), pretrained=pretrained, **kwargs)
+    model_args = dict(growth_rate=32, block_config=(6, 12, 24, 16))
+    model = _create_densenet('densenet121', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
 def densenetblur121d(pretrained=False, **kwargs) -> DenseNet:
     r"""Densenet-121 w/ blur-pooling & 3-layer 3x3 stem
     `"Densely Connected Convolutional Networks" <https://arxiv.org/pdf/1608.06993.pdf>`
     """
-    model = _create_densenet(
-        'densenetblur121d', growth_rate=32, block_config=(6, 12, 24, 16), pretrained=pretrained,
-        stem_type='deep', aa_layer=BlurPool2d, **kwargs)
+    model_args = dict(growth_rate=32, block_config=(6, 12, 24, 16), stem_type='deep', aa_layer=BlurPool2d)
+    model = _create_densenet('densenetblur121d', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
 def densenet169(pretrained=False, **kwargs) -> DenseNet:
     r"""Densenet-169 model from
     `"Densely Connected Convolutional Networks" <https://arxiv.org/pdf/1608.06993.pdf>`
     """
-    model = _create_densenet(
-        'densenet169', growth_rate=32, block_config=(6, 12, 32, 32), pretrained=pretrained, **kwargs)
+    model_args = dict(growth_rate=32, block_config=(6, 12, 32, 32))
+    model = _create_densenet('densenet169', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
 def densenet201(pretrained=False, **kwargs) -> DenseNet:
     r"""Densenet-201 model from
     `"Densely Connected Convolutional Networks" <https://arxiv.org/pdf/1608.06993.pdf>`
     """
-    model = _create_densenet(
-        'densenet201', growth_rate=32, block_config=(6, 12, 48, 32), pretrained=pretrained, **kwargs)
+    model_args = dict(growth_rate=32, block_config=(6, 12, 48, 32))
+    model = _create_densenet('densenet201', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
 def densenet161(pretrained=False, **kwargs) -> DenseNet:
     r"""Densenet-161 model from
     `"Densely Connected Convolutional Networks" <https://arxiv.org/pdf/1608.06993.pdf>`
     """
-    model = _create_densenet(
-        'densenet161', growth_rate=48, block_config=(6, 12, 36, 24), pretrained=pretrained, **kwargs)
+    model_args = dict(growth_rate=48, block_config=(6, 12, 36, 24))
+    model = _create_densenet('densenet161', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
 def densenet264d(pretrained=False, **kwargs) -> DenseNet:
     r"""Densenet-264 model from
     `"Densely Connected Convolutional Networks" <https://arxiv.org/pdf/1608.06993.pdf>`
     """
-    model = _create_densenet(
-        'densenet264d', growth_rate=48, block_config=(6, 12, 64, 48), stem_type='deep', pretrained=pretrained, **kwargs)
+    model_args = dict(growth_rate=48, block_config=(6, 12, 64, 48), stem_type='deep')
+    model = _create_densenet('densenet264d', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
+
+register_model_deprecations(__name__, {
+    'tv_densenet121': 'densenet121.tv_in1k',
+})
```

### Comparing `timm-0.9.9/timm/models/dla.py` & `timm-1.0.3/timm/models/dla.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/dpn.py` & `timm-1.0.3/timm/models/dpn.py`

 * *Files 6% similar despite different names*

```diff
@@ -313,59 +313,59 @@
     'dpn131.mx_in1k': _cfg(hf_hub_id='timm/'),
     'dpn107.mx_in1k': _cfg(hf_hub_id='timm/')
 })
 
 
 @register_model
 def dpn48b(pretrained=False, **kwargs) -> DPN:
-    model_kwargs = dict(
+    model_args = dict(
         small=True, num_init_features=10, k_r=128, groups=32,
         b=True, k_sec=(3, 4, 6, 3), inc_sec=(16, 32, 32, 64), act_layer='silu')
-    return _create_dpn('dpn48b', pretrained=pretrained, **dict(model_kwargs, **kwargs))
+    return _create_dpn('dpn48b', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def dpn68(pretrained=False, **kwargs) -> DPN:
-    model_kwargs = dict(
+    model_args = dict(
         small=True, num_init_features=10, k_r=128, groups=32,
         k_sec=(3, 4, 12, 3), inc_sec=(16, 32, 32, 64))
-    return _create_dpn('dpn68', pretrained=pretrained, **dict(model_kwargs, **kwargs))
+    return _create_dpn('dpn68', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def dpn68b(pretrained=False, **kwargs) -> DPN:
-    model_kwargs = dict(
+    model_args = dict(
         small=True, num_init_features=10, k_r=128, groups=32,
         b=True, k_sec=(3, 4, 12, 3), inc_sec=(16, 32, 32, 64))
-    return _create_dpn('dpn68b', pretrained=pretrained, **dict(model_kwargs, **kwargs))
+    return _create_dpn('dpn68b', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def dpn92(pretrained=False, **kwargs) -> DPN:
-    model_kwargs = dict(
+    model_args = dict(
         num_init_features=64, k_r=96, groups=32,
         k_sec=(3, 4, 20, 3), inc_sec=(16, 32, 24, 128))
-    return _create_dpn('dpn92', pretrained=pretrained, **dict(model_kwargs, **kwargs))
+    return _create_dpn('dpn92', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def dpn98(pretrained=False, **kwargs) -> DPN:
-    model_kwargs = dict(
+    model_args = dict(
         num_init_features=96, k_r=160, groups=40,
         k_sec=(3, 6, 20, 3), inc_sec=(16, 32, 32, 128))
-    return _create_dpn('dpn98', pretrained=pretrained, **dict(model_kwargs, **kwargs))
+    return _create_dpn('dpn98', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def dpn131(pretrained=False, **kwargs) -> DPN:
-    model_kwargs = dict(
+    model_args = dict(
         num_init_features=128, k_r=160, groups=40,
         k_sec=(4, 8, 28, 3), inc_sec=(16, 32, 32, 128))
-    return _create_dpn('dpn131', pretrained=pretrained, **dict(model_kwargs, **kwargs))
+    return _create_dpn('dpn131', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def dpn107(pretrained=False, **kwargs) -> DPN:
-    model_kwargs = dict(
+    model_args = dict(
         num_init_features=128, k_r=200, groups=50,
         k_sec=(4, 8, 20, 3), inc_sec=(20, 64, 64, 128))
-    return _create_dpn('dpn107', pretrained=pretrained, **dict(model_kwargs, **kwargs))
+    return _create_dpn('dpn107', pretrained=pretrained, **dict(model_args, **kwargs))
```

### Comparing `timm-0.9.9/timm/models/edgenext.py` & `timm-1.0.3/timm/models/edgenext.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,24 @@
  - https://arxiv.org/abs/2206.10589
 
 Original code and weights from https://github.com/mmaaz60/EdgeNeXt
 
 Modifications and additions for timm by / Copyright 2022, Ross Wightman
 """
 import math
-from collections import OrderedDict
 from functools import partial
 from typing import Tuple
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
-from timm.layers import trunc_normal_tf_, DropPath, LayerNorm2d, Mlp, SelectAdaptivePool2d, create_conv2d, \
-    use_fused_attn
+from timm.layers import trunc_normal_tf_, DropPath, LayerNorm2d, Mlp, create_conv2d, \
+    use_fused_attn, NormMlpClassifierHead, ClassifierHead
 from ._builder import build_model_with_cfg
 from ._features_fx import register_notrace_module
 from ._manipulate import named_apply, checkpoint_seq
 from ._registry import register_model, generate_default_cfgs
 
 __all__ = ['EdgeNeXt']  # model_registry will add each entrypoint fn to this
 
@@ -37,33 +36,33 @@
         self.hidden_dim = hidden_dim
         self.dim = dim
 
     def forward(self, shape: Tuple[int, int, int]):
         device = self.token_projection.weight.device
         dtype = self.token_projection.weight.dtype
         inv_mask = ~torch.zeros(shape).to(device=device, dtype=torch.bool)
-        y_embed = inv_mask.cumsum(1, dtype=dtype)
-        x_embed = inv_mask.cumsum(2, dtype=dtype)
+        y_embed = inv_mask.cumsum(1, dtype=torch.float32)
+        x_embed = inv_mask.cumsum(2, dtype=torch.float32)
         eps = 1e-6
         y_embed = y_embed / (y_embed[:, -1:, :] + eps) * self.scale
         x_embed = x_embed / (x_embed[:, :, -1:] + eps) * self.scale
 
-        dim_t = torch.arange(self.hidden_dim, dtype=dtype, device=device)
+        dim_t = torch.arange(self.hidden_dim, dtype=torch.int64, device=device).to(torch.float32)
         dim_t = self.temperature ** (2 * torch.div(dim_t, 2, rounding_mode='floor') / self.hidden_dim)
 
         pos_x = x_embed[:, :, :, None] / dim_t
         pos_y = y_embed[:, :, :, None] / dim_t
         pos_x = torch.stack(
             (pos_x[:, :, :, 0::2].sin(),
              pos_x[:, :, :, 1::2].cos()), dim=4).flatten(3)
         pos_y = torch.stack(
             (pos_y[:, :, :, 0::2].sin(),
              pos_y[:, :, :, 1::2].cos()), dim=4).flatten(3)
         pos = torch.cat((pos_y, pos_x), dim=3).permute(0, 3, 1, 2)
-        pos = self.token_projection(pos)
+        pos = self.token_projection(pos.to(dtype))
 
         return pos
 
 
 class ConvBlock(nn.Module):
     def __init__(
             self,
@@ -371,21 +370,31 @@
             # NOTE feature_info use currently assumes stage 0 == stride 1, rest are stride 2
             in_chs = dims[i]
             self.feature_info += [dict(num_chs=in_chs, reduction=curr_stride, module=f'stages.{i}')]
 
         self.stages = nn.Sequential(*stages)
 
         self.num_features = dims[-1]
-        self.norm_pre = norm_layer(self.num_features) if head_norm_first else nn.Identity()
-        self.head = nn.Sequential(OrderedDict([
-                ('global_pool', SelectAdaptivePool2d(pool_type=global_pool)),
-                ('norm', nn.Identity() if head_norm_first else norm_layer(self.num_features)),
-                ('flatten', nn.Flatten(1) if global_pool else nn.Identity()),
-                ('drop', nn.Dropout(self.drop_rate)),
-                ('fc', nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity())]))
+        if head_norm_first:
+            self.norm_pre = norm_layer(self.num_features)
+            self.head = ClassifierHead(
+                self.num_features,
+                num_classes,
+                pool_type=global_pool,
+                drop_rate=self.drop_rate,
+            )
+        else:
+            self.norm_pre = nn.Identity()
+            self.head = NormMlpClassifierHead(
+                self.num_features,
+                num_classes,
+                pool_type=global_pool,
+                drop_rate=self.drop_rate,
+                norm_layer=norm_layer,
+            )
 
         named_apply(partial(_init_weights, head_init_scale=head_init_scale), self)
 
     @torch.jit.ignore
     def group_matcher(self, coarse=False):
         return dict(
             stem=r'^stem',
@@ -402,32 +411,24 @@
             s.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
     def reset_classifier(self, num_classes=0, global_pool=None):
-        if global_pool is not None:
-            self.head.global_pool = SelectAdaptivePool2d(pool_type=global_pool)
-            self.head.flatten = nn.Flatten(1) if global_pool else nn.Identity()
-        self.head.fc = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
+        self.head.reset(num_classes, global_pool)
 
     def forward_features(self, x):
         x = self.stem(x)
         x = self.stages(x)
         x = self.norm_pre(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
-        # NOTE nn.Sequential in head broken down since can't call head[:-1](x) in torchscript :(
-        x = self.head.global_pool(x)
-        x = self.head.norm(x)
-        x = self.head.flatten(x)
-        x = self.head.drop(x)
-        return x if pre_logits else self.head.fc(x)
+        return self.head(x, pre_logits=True) if pre_logits else self.head(x)
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
@@ -524,51 +525,51 @@
 @register_model
 def edgenext_xx_small(pretrained=False, **kwargs) -> EdgeNeXt:
     # 1.33M & 260.58M @ 256 resolution
     # 71.23% Top-1 accuracy
     # No AA, Color Jitter=0.4, No Mixup & Cutmix, DropPath=0.0, BS=4096, lr=0.006, multi-scale-sampler
     # Jetson FPS=51.66 versus 47.67 for MobileViT_XXS
     # For A100: FPS @ BS=1: 212.13 & @ BS=256: 7042.06 versus FPS @ BS=1: 96.68 & @ BS=256: 4624.71 for MobileViT_XXS
-    model_kwargs = dict(depths=(2, 2, 6, 2), dims=(24, 48, 88, 168), heads=(4, 4, 4, 4), **kwargs)
-    return _create_edgenext('edgenext_xx_small', pretrained=pretrained, **model_kwargs)
+    model_args = dict(depths=(2, 2, 6, 2), dims=(24, 48, 88, 168), heads=(4, 4, 4, 4))
+    return _create_edgenext('edgenext_xx_small', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def edgenext_x_small(pretrained=False, **kwargs) -> EdgeNeXt:
     # 2.34M & 538.0M @ 256 resolution
     # 75.00% Top-1 accuracy
     # No AA, No Mixup & Cutmix, DropPath=0.0, BS=4096, lr=0.006, multi-scale-sampler
     # Jetson FPS=31.61 versus 28.49 for MobileViT_XS
     # For A100: FPS @ BS=1: 179.55 & @ BS=256: 4404.95 versus FPS @ BS=1: 94.55 & @ BS=256: 2361.53 for MobileViT_XS
-    model_kwargs = dict(depths=(3, 3, 9, 3), dims=(32, 64, 100, 192), heads=(4, 4, 4, 4), **kwargs)
-    return _create_edgenext('edgenext_x_small', pretrained=pretrained, **model_kwargs)
+    model_args = dict(depths=(3, 3, 9, 3), dims=(32, 64, 100, 192), heads=(4, 4, 4, 4))
+    return _create_edgenext('edgenext_x_small', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def edgenext_small(pretrained=False, **kwargs) -> EdgeNeXt:
     # 5.59M & 1260.59M @ 256 resolution
     # 79.43% Top-1 accuracy
     # AA=True, No Mixup & Cutmix, DropPath=0.1, BS=4096, lr=0.006, multi-scale-sampler
     # Jetson FPS=20.47 versus 18.86 for MobileViT_S
     # For A100: FPS @ BS=1: 172.33 & @ BS=256: 3010.25 versus FPS @ BS=1: 93.84 & @ BS=256: 1785.92 for MobileViT_S
-    model_kwargs = dict(depths=(3, 3, 9, 3), dims=(48, 96, 160, 304),  **kwargs)
-    return _create_edgenext('edgenext_small', pretrained=pretrained, **model_kwargs)
+    model_args = dict(depths=(3, 3, 9, 3), dims=(48, 96, 160, 304))
+    return _create_edgenext('edgenext_small', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def edgenext_base(pretrained=False, **kwargs) -> EdgeNeXt:
     # 18.51M & 3840.93M @ 256 resolution
     # 82.5% (normal) 83.7% (USI) Top-1 accuracy
     # AA=True, Mixup & Cutmix, DropPath=0.1, BS=4096, lr=0.006, multi-scale-sampler
     # Jetson FPS=xx.xx versus xx.xx for MobileViT_S
     # For A100: FPS @ BS=1: xxx.xx & @ BS=256: xxxx.xx
-    model_kwargs = dict(depths=[3, 3, 9, 3], dims=[80, 160, 288, 584], **kwargs)
-    return _create_edgenext('edgenext_base', pretrained=pretrained, **model_kwargs)
+    model_args = dict(depths=[3, 3, 9, 3], dims=[80, 160, 288, 584])
+    return _create_edgenext('edgenext_base', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def edgenext_small_rw(pretrained=False, **kwargs) -> EdgeNeXt:
-    model_kwargs = dict(
+    model_args = dict(
         depths=(3, 3, 9, 3), dims=(48, 96, 192, 384),
-        downsample_block=True, conv_bias=False, stem_type='overlap', **kwargs)
-    return _create_edgenext('edgenext_small_rw', pretrained=pretrained, **model_kwargs)
+        downsample_block=True, conv_bias=False, stem_type='overlap')
+    return _create_edgenext('edgenext_small_rw', pretrained=pretrained, **dict(model_args, **kwargs))
```

### Comparing `timm-0.9.9/timm/models/efficientformer.py` & `timm-1.0.3/timm/models/efficientformer.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,22 +8,23 @@
   year={2022}
 }
 
 Based on Apache 2.0 licensed code at https://github.com/snap-research/EfficientFormer, Copyright (c) 2022 Snap Inc.
 
 Modifications and timm support by / Copyright 2022, Ross Wightman
 """
-from typing import Dict
+from typing import Dict, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
-from timm.layers import DropPath, trunc_normal_, to_2tuple, Mlp
+from timm.layers import DropPath, trunc_normal_, to_2tuple, Mlp, ndgrid
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._manipulate import checkpoint_seq
 from ._registry import generate_default_cfgs, register_model
 
 __all__ = ['EfficientFormer']  # model_registry will add each entrypoint fn to this
 
 
 EfficientFormer_width = {
@@ -59,15 +60,15 @@
         self.val_attn_dim = self.val_dim * num_heads
         self.attn_ratio = attn_ratio
 
         self.qkv = nn.Linear(dim, self.key_attn_dim * 2 + self.val_attn_dim)
         self.proj = nn.Linear(self.val_attn_dim, dim)
 
         resolution = to_2tuple(resolution)
-        pos = torch.stack(torch.meshgrid(torch.arange(resolution[0]), torch.arange(resolution[1]))).flatten(1)
+        pos = torch.stack(ndgrid(torch.arange(resolution[0]), torch.arange(resolution[1]))).flatten(1)
         rel_pos = (pos[..., :, None] - pos[..., None, :]).abs()
         rel_pos = (rel_pos[0] * resolution[1]) + rel_pos[1]
         self.attention_biases = torch.nn.Parameter(torch.zeros(num_heads, resolution[0] * resolution[1]))
         self.register_buffer('attention_bias_idxs', rel_pos)
         self.attention_bias_cache = {}  # per-device attention_biases cache (data-parallel compat)
 
     @torch.no_grad()
@@ -378,36 +379,39 @@
         self.num_classes = num_classes
         self.global_pool = global_pool
 
         self.stem = Stem4(in_chans, embed_dims[0], norm_layer=norm_layer)
         prev_dim = embed_dims[0]
 
         # stochastic depth decay rule
+        self.num_stages = len(depths)
+        last_stage = self.num_stages - 1
         dpr = [x.tolist() for x in torch.linspace(0, drop_path_rate, sum(depths)).split(depths)]
-        downsamples = downsamples or (False,) + (True,) * (len(depths) - 1)
+        downsamples = downsamples or (False,) + (True,) * (self.num_stages - 1)
         stages = []
-        for i in range(len(depths)):
+        self.feature_info = []
+        for i in range(self.num_stages):
             stage = EfficientFormerStage(
                 prev_dim,
                 embed_dims[i],
                 depths[i],
                 downsample=downsamples[i],
-                num_vit=num_vit if i == 3 else 0,
+                num_vit=num_vit if i == last_stage else 0,
                 pool_size=pool_size,
                 mlp_ratio=mlp_ratios,
                 act_layer=act_layer,
                 norm_layer_cl=norm_layer_cl,
                 norm_layer=norm_layer,
                 proj_drop=proj_drop_rate,
                 drop_path=dpr[i],
                 layer_scale_init_value=layer_scale_init_value,
             )
             prev_dim = embed_dims[i]
             stages.append(stage)
-
+            self.feature_info += [dict(num_chs=embed_dims[i], reduction=2**(1+i), module=f'stages.{i}')]
         self.stages = nn.Sequential(*stages)
 
         # Classifier head
         self.num_features = embed_dims[-1]
         self.norm = norm_layer_cl(self.num_features)
         self.head_drop = nn.Dropout(drop_rate)
         self.head = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
@@ -441,25 +445,95 @@
         for s in self.stages:
             s.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head, self.head_dist
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             self.global_pool = global_pool
         self.head = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
         self.head_dist = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
 
     @torch.jit.ignore
     def set_distilled_training(self, enable=True):
         self.distilled_training = enable
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to compatible intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output shape must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.stages), indices)
+
+        # forward pass
+        x = self.stem(x)
+        B, C, H, W = x.shape
+
+        last_idx = self.num_stages - 1
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            stages = self.stages
+        else:
+            stages = self.stages[:max_index + 1]
+        feat_idx = 0
+        for feat_idx, stage in enumerate(stages):
+            x = stage(x)
+            if feat_idx < last_idx:
+                B, C, H, W = x.shape
+            if feat_idx in take_indices:
+                if feat_idx == last_idx:
+                    x_inter = self.norm(x) if norm else x
+                    intermediates.append(x_inter.reshape(B, H // 2, W // 2, -1).permute(0, 3, 1, 2))
+                else:
+                    intermediates.append(x)
+
+        if intermediates_only:
+            return intermediates
+
+        if feat_idx == last_idx:
+            x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.stages), indices)
+        self.stages = self.stages[:max_index + 1]  # truncate blocks w/ stem as idx 0
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.stem(x)
         x = self.stages(x)
         x = self.norm(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
@@ -530,21 +604,21 @@
     'efficientformer_l7.snap_dist_in1k': _cfg(
         hf_hub_id='timm/',
     ),
 })
 
 
 def _create_efficientformer(variant, pretrained=False, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError('features_only not implemented for EfficientFormer models.')
-
+    out_indices = kwargs.pop('out_indices', 4)
     model = build_model_with_cfg(
         EfficientFormer, variant, pretrained,
         pretrained_filter_fn=_checkpoint_filter_fn,
-        **kwargs)
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
+        **kwargs,
+    )
     return model
 
 
 @register_model
 def efficientformer_l1(pretrained=False, **kwargs) -> EfficientFormer:
     model_args = dict(
         depths=EfficientFormer_depth['l1'],
```

### Comparing `timm-0.9.9/timm/models/efficientformer_v2.py` & `timm-1.0.3/timm/models/efficientformer_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 Original code licensed Apache 2.0, Copyright (c) 2022 Snap Inc.
 
 Modifications and timm support by / Copyright 2023, Ross Wightman
 """
 import math
 from functools import partial
-from typing import Dict
+from typing import Dict, Optional
 
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import create_conv2d, create_norm_layer, get_act_layer, get_norm_layer, ConvNormAct
-from timm.layers import DropPath, trunc_normal_, to_2tuple, to_ntuple
+from timm.layers import DropPath, trunc_normal_, to_2tuple, to_ntuple, ndgrid
 from ._builder import build_model_with_cfg
 from ._manipulate import checkpoint_seq
 from ._registry import generate_default_cfgs, register_model
 
 
 EfficientFormer_width = {
     'L': (40, 80, 192, 384),  # 26m 83.3% 6attn
@@ -125,15 +125,15 @@
         self.v_local = ConvNorm(self.dh, self.dh, kernel_size=3, groups=self.dh)
         self.talking_head1 = nn.Conv2d(self.num_heads, self.num_heads, kernel_size=1)
         self.talking_head2 = nn.Conv2d(self.num_heads, self.num_heads, kernel_size=1)
 
         self.act = act_layer()
         self.proj = ConvNorm(self.dh, dim, 1)
 
-        pos = torch.stack(torch.meshgrid(torch.arange(self.resolution[0]), torch.arange(self.resolution[1]))).flatten(1)
+        pos = torch.stack(ndgrid(torch.arange(self.resolution[0]), torch.arange(self.resolution[1]))).flatten(1)
         rel_pos = (pos[..., :, None] - pos[..., None, :]).abs()
         rel_pos = (rel_pos[0] * self.resolution[1]) + rel_pos[1]
         self.attention_biases = torch.nn.Parameter(torch.zeros(num_heads, self.N))
         self.register_buffer('attention_bias_idxs', torch.LongTensor(rel_pos), persistent=False)
         self.attention_bias_cache = {}  # per-device attention_biases cache (data-parallel compat)
 
     @torch.no_grad()
@@ -227,20 +227,19 @@
         self.v = ConvNorm(dim, self.dh, 1)
         self.v_local = ConvNorm(self.dh, self.dh, kernel_size=3, stride=2, groups=self.dh)
 
         self.act = act_layer()
         self.proj = ConvNorm(self.dh, self.out_dim, 1)
 
         self.attention_biases = nn.Parameter(torch.zeros(num_heads, self.N))
-        k_pos = torch.stack(torch.meshgrid(torch.arange(
-            self.resolution[0]),
-            torch.arange(self.resolution[1]))).flatten(1)
-        q_pos = torch.stack(torch.meshgrid(
+        k_pos = torch.stack(ndgrid(torch.arange(self.resolution[0]), torch.arange(self.resolution[1]))).flatten(1)
+        q_pos = torch.stack(ndgrid(
             torch.arange(0, self.resolution[0], step=2),
-            torch.arange(0, self.resolution[1], step=2))).flatten(1)
+            torch.arange(0, self.resolution[1], step=2)
+        )).flatten(1)
         rel_pos = (q_pos[..., :, None] - k_pos[..., None, :]).abs()
         rel_pos = (rel_pos[0] * self.resolution[1]) + rel_pos[1]
         self.register_buffer('attention_bias_idxs', rel_pos, persistent=False)
         self.attention_bias_cache = {}  # per-device attention_biases cache (data-parallel compat)
 
     @torch.no_grad()
     def train(self, mode=True):
@@ -609,15 +608,15 @@
         for s in self.stages:
             s.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head, self.head_dist
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             self.global_pool = global_pool
         self.head = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
         self.head_dist = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
 
     @torch.jit.ignore
```

### Comparing `timm-0.9.9/timm/models/efficientnet.py` & `timm-1.0.3/timm/models/efficientnet.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,28 +32,28 @@
 The majority of the above models (EfficientNet*, MixNet, MnasNet) and original weights were made available
 by Mingxing Tan, Quoc Le, and other members of their Google Brain team. Thanks for consistently releasing
 the models and weights open source!
 
 Hacked together by / Copyright 2019, Ross Wightman
 """
 from functools import partial
-from typing import List
+from typing import List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils.checkpoint import checkpoint
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD, IMAGENET_INCEPTION_MEAN, IMAGENET_INCEPTION_STD
 from timm.layers import create_conv2d, create_classifier, get_norm_act_layer, GroupNormAct
 from ._builder import build_model_with_cfg, pretrained_cfg_for_features
 from ._efficientnet_blocks import SqueezeExcite
 from ._efficientnet_builder import EfficientNetBuilder, decode_arch_def, efficientnet_init_weights, \
     round_channels, resolve_bn_args, resolve_act_layer, BN_EPS_TF_DEFAULT
-from ._features import FeatureInfo, FeatureHooks
+from ._features import FeatureInfo, FeatureHooks, feature_take_indices
 from ._manipulate import checkpoint_seq
 from ._registry import generate_default_cfgs, register_model, register_model_deprecations
 
 __all__ = ['EfficientNet', 'EfficientNetFeatures']
 
 
 class EfficientNet(nn.Module):
@@ -114,14 +114,15 @@
             act_layer=act_layer,
             norm_layer=norm_layer,
             se_layer=se_layer,
             drop_path_rate=drop_path_rate,
         )
         self.blocks = nn.Sequential(*builder(stem_size, block_args))
         self.feature_info = builder.features
+        self.stage_ends = [f['stage'] for f in self.feature_info]
         head_chs = builder.in_chs
 
         # Head + Pooling
         self.conv_head = create_conv2d(head_chs, self.num_features, 1, padding=pad_type)
         self.bn2 = norm_act_layer(self.num_features, inplace=True)
         self.global_pool, self.classifier = create_classifier(
             self.num_features, self.num_classes, pool_type=global_pool)
@@ -154,14 +155,93 @@
         return self.classifier
 
     def reset_classifier(self, num_classes, global_pool='avg'):
         self.num_classes = num_classes
         self.global_pool, self.classifier = create_classifier(
             self.num_features, self.num_classes, pool_type=global_pool)
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+            extra_blocks: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to compatible intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+            extra_blocks: Include outputs of all blocks and head conv in output, does not align with feature_info
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output shape must be NCHW.'
+        intermediates = []
+        if extra_blocks:
+            take_indices, max_index = feature_take_indices(len(self.blocks) + 1, indices)
+        else:
+            take_indices, max_index = feature_take_indices(len(self.stage_ends), indices)
+            take_indices = [self.stage_ends[i] for i in take_indices]
+            max_index = self.stage_ends[max_index]
+        # forward pass
+        feat_idx = 0  # stem is index 0
+        x = self.conv_stem(x)
+        x = self.bn1(x)
+        if feat_idx in take_indices:
+            intermediates.append(x)
+
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            blocks = self.blocks
+        else:
+            blocks = self.blocks[:max_index]
+        for blk in blocks:
+            feat_idx += 1
+            x = blk(x)
+            if feat_idx in take_indices:
+                intermediates.append(x)
+
+        if intermediates_only:
+            return intermediates
+
+        if feat_idx == self.stage_ends[-1]:
+            x = self.conv_head(x)
+            x = self.bn2(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+            extra_blocks: bool = False,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        if extra_blocks:
+            take_indices, max_index = feature_take_indices(len(self.blocks) + 1, indices)
+        else:
+            take_indices, max_index = feature_take_indices(len(self.stage_ends), indices)
+            max_index = self.stage_ends[max_index]
+        self.blocks = self.blocks[:max_index]  # truncate blocks w/ stem as idx 0
+        if prune_norm or max_index < len(self.blocks):
+            self.conv_head = nn.Identity()
+            self.bn2 = nn.Identity()
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.conv_stem(x)
         x = self.bn1(x)
         if self.grad_checkpointing and not torch.jit.is_scripting():
             x = checkpoint_seq(self.blocks, x, flatten=True)
         else:
             x = self.blocks(x)
@@ -268,15 +348,15 @@
 
 
 def _create_effnet(variant, pretrained=False, **kwargs):
     features_mode = ''
     model_cls = EfficientNet
     kwargs_filter = None
     if kwargs.pop('features_only', False):
-        if 'feature_cfg' in kwargs:
+        if 'feature_cfg' in kwargs or 'feature_cls' in kwargs:
             features_mode = 'cfg'
         else:
             kwargs_filter = ('num_classes', 'num_features', 'head_conv', 'global_pool')
             model_cls = EfficientNetFeatures
             features_mode = 'cls'
 
     model = build_model_with_cfg(
@@ -1201,35 +1281,35 @@
     'tf_efficientnet_b7.aa_in1k': _cfg(
         url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-weights/tf_efficientnet_b7_aa-076e3472.pth',
         hf_hub_id='timm/',
         input_size=(3, 600, 600), pool_size=(19, 19), crop_pct=0.949),
 
     'tf_efficientnet_b0.in1k': _cfg(
         url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-weights/tf_efficientnet_b0-0af12548.pth',
-        #hf_hub_id='timm/',
+        hf_hub_id='timm/',
         input_size=(3, 224, 224)),
     'tf_efficientnet_b1.in1k': _cfg(
         url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-weights/tf_efficientnet_b1-5c1377c4.pth',
-        #hf_hub_id='timm/',
+        hf_hub_id='timm/',
         input_size=(3, 240, 240), pool_size=(8, 8), crop_pct=0.882),
     'tf_efficientnet_b2.in1k': _cfg(
         url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-weights/tf_efficientnet_b2-e393ef04.pth',
-        #hf_hub_id='timm/',
+        hf_hub_id='timm/',
         input_size=(3, 260, 260), pool_size=(9, 9), crop_pct=0.890),
     'tf_efficientnet_b3.in1k': _cfg(
         url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-weights/tf_efficientnet_b3-e3bd6955.pth',
-        #hf_hub_id='timm/',
+        hf_hub_id='timm/',
         input_size=(3, 300, 300), pool_size=(10, 10), crop_pct=0.904),
     'tf_efficientnet_b4.in1k': _cfg(
         url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-weights/tf_efficientnet_b4-74ee3bed.pth',
-        #hf_hub_id='timm/',
+        hf_hub_id='timm/',
         input_size=(3, 380, 380), pool_size=(12, 12), crop_pct=0.922),
     'tf_efficientnet_b5.in1k': _cfg(
         url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-weights/tf_efficientnet_b5-c6949ce9.pth',
-        #hf_hub_id='timm/',
+        hf_hub_id='timm/',
         input_size=(3, 456, 456), pool_size=(15, 15), crop_pct=0.934),
 
 
     'tf_efficientnet_es.in1k': _cfg(
         url='https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-weights/tf_efficientnet_es-ca1afbfe.pth',
         hf_hub_id='timm/',
         mean=(0.5, 0.5, 0.5), std=(0.5, 0.5, 0.5),
@@ -1438,20 +1518,14 @@
 def mnasnet_100(pretrained=False, **kwargs) -> EfficientNet:
     """ MNASNet B1, depth multiplier of 1.0. """
     model = _gen_mnasnet_b1('mnasnet_100', 1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
-def mnasnet_b1(pretrained=False, **kwargs) -> EfficientNet:
-    """ MNASNet B1, depth multiplier of 1.0. """
-    return mnasnet_100(pretrained, **kwargs)
-
-
-@register_model
 def mnasnet_140(pretrained=False, **kwargs) -> EfficientNet:
     """ MNASNet B1,  depth multiplier of 1.4 """
     model = _gen_mnasnet_b1('mnasnet_140', 1.4, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
@@ -1472,20 +1546,14 @@
 def semnasnet_100(pretrained=False, **kwargs) -> EfficientNet:
     """ MNASNet A1 (w/ SE), depth multiplier of 1.0. """
     model = _gen_mnasnet_a1('semnasnet_100', 1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
-def mnasnet_a1(pretrained=False, **kwargs) -> EfficientNet:
-    """ MNASNet A1 (w/ SE), depth multiplier of 1.0. """
-    return semnasnet_100(pretrained, **kwargs)
-
-
-@register_model
 def semnasnet_140(pretrained=False, **kwargs) -> EfficientNet:
     """ MNASNet A1 (w/ SE), depth multiplier of 1.4. """
     model = _gen_mnasnet_a1('semnasnet_140', 1.4, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
@@ -1547,15 +1615,15 @@
 
 
 @register_model
 def fbnetc_100(pretrained=False, **kwargs) -> EfficientNet:
     """ FBNet-C """
     if pretrained:
         # pretrained model trained with non-default BN epsilon
-        kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
+        kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
     model = _gen_fbnetc('fbnetc_100', 1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def spnasnet_100(pretrained=False, **kwargs) -> EfficientNet:
     """ Single-Path NAS Pixel1"""
@@ -1587,37 +1655,23 @@
     # NOTE for train, drop_rate should be 0.3, drop_path_rate should be 0.2
     model = _gen_efficientnet(
         'efficientnet_b2', channel_multiplier=1.1, depth_multiplier=1.2, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
-def efficientnet_b2a(pretrained=False, **kwargs) -> EfficientNet:
-    """ EfficientNet-B2 @ 288x288 w/ 1.0 test crop"""
-    # WARN this model def is deprecated, different train/test res + test crop handled by default_cfg now
-    return efficientnet_b2(pretrained=pretrained, **kwargs)
-
-
-@register_model
 def efficientnet_b3(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B3 """
     # NOTE for train, drop_rate should be 0.3, drop_path_rate should be 0.2
     model = _gen_efficientnet(
         'efficientnet_b3', channel_multiplier=1.2, depth_multiplier=1.4, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
-def efficientnet_b3a(pretrained=False, **kwargs) -> EfficientNet:
-    """ EfficientNet-B3 @ 320x320 w/ 1.0 test crop-pct """
-    # WARN this model def is deprecated, different train/test res + test crop handled by default_cfg now
-    return efficientnet_b3(pretrained=pretrained, **kwargs)
-
-
-@register_model
 def efficientnet_b4(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B4 """
     # NOTE for train, drop_rate should be 0.4, drop_path_rate should be 0.2
     model = _gen_efficientnet(
         'efficientnet_b4', channel_multiplier=1.4, depth_multiplier=1.8, pretrained=pretrained, **kwargs)
     return model
 
@@ -1824,38 +1878,38 @@
         'efficientnet_lite4', channel_multiplier=1.4, depth_multiplier=1.8, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def efficientnet_b1_pruned(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B1 Pruned. The pruning has been obtained using https://arxiv.org/pdf/2002.08258.pdf  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     variant = 'efficientnet_b1_pruned'
     model = _gen_efficientnet(
         variant, channel_multiplier=1.0, depth_multiplier=1.1, pruned=True, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def efficientnet_b2_pruned(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B2 Pruned. The pruning has been obtained using https://arxiv.org/pdf/2002.08258.pdf """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet(
         'efficientnet_b2_pruned', channel_multiplier=1.1, depth_multiplier=1.2, pruned=True,
         pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def efficientnet_b3_pruned(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B3 Pruned. The pruning has been obtained using https://arxiv.org/pdf/2002.08258.pdf """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet(
         'efficientnet_b3_pruned', channel_multiplier=1.2, depth_multiplier=1.4, pruned=True,
         pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
@@ -1922,306 +1976,306 @@
     model = _gen_efficientnetv2_xl('efficientnetv2_xl', pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_b0(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B0. Tensorflow compatible variant  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet(
         'tf_efficientnet_b0', channel_multiplier=1.0, depth_multiplier=1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_b1(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B1. Tensorflow compatible variant  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet(
         'tf_efficientnet_b1', channel_multiplier=1.0, depth_multiplier=1.1, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_b2(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B2. Tensorflow compatible variant  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet(
         'tf_efficientnet_b2', channel_multiplier=1.1, depth_multiplier=1.2, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_b3(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B3. Tensorflow compatible variant """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet(
         'tf_efficientnet_b3', channel_multiplier=1.2, depth_multiplier=1.4, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_b4(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B4. Tensorflow compatible variant """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet(
         'tf_efficientnet_b4', channel_multiplier=1.4, depth_multiplier=1.8, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_b5(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B5. Tensorflow compatible variant """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet(
         'tf_efficientnet_b5', channel_multiplier=1.6, depth_multiplier=2.2, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_b6(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B6. Tensorflow compatible variant """
     # NOTE for train, drop_rate should be 0.5
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet(
         'tf_efficientnet_b6', channel_multiplier=1.8, depth_multiplier=2.6, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_b7(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B7. Tensorflow compatible variant """
     # NOTE for train, drop_rate should be 0.5
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet(
         'tf_efficientnet_b7', channel_multiplier=2.0, depth_multiplier=3.1, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_b8(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-B8. Tensorflow compatible variant """
     # NOTE for train, drop_rate should be 0.5
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet(
         'tf_efficientnet_b8', channel_multiplier=2.2, depth_multiplier=3.6, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_l2(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-L2 NoisyStudent. Tensorflow compatible variant """
     # NOTE for train, drop_rate should be 0.5
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet(
         'tf_efficientnet_l2', channel_multiplier=4.3, depth_multiplier=5.3, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_es(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-Edge Small. Tensorflow compatible variant  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet_edge(
         'tf_efficientnet_es', channel_multiplier=1.0, depth_multiplier=1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_em(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-Edge-Medium. Tensorflow compatible variant  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet_edge(
         'tf_efficientnet_em', channel_multiplier=1.0, depth_multiplier=1.1, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_el(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-Edge-Large. Tensorflow compatible variant  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet_edge(
         'tf_efficientnet_el', channel_multiplier=1.2, depth_multiplier=1.4, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_cc_b0_4e(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-CondConv-B0 w/ 4 Experts. Tensorflow compatible variant """
     # NOTE for train, drop_rate should be 0.2, drop_path_rate should be 0.2
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet_condconv(
         'tf_efficientnet_cc_b0_4e', channel_multiplier=1.0, depth_multiplier=1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_cc_b0_8e(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-CondConv-B0 w/ 8 Experts. Tensorflow compatible variant """
     # NOTE for train, drop_rate should be 0.2, drop_path_rate should be 0.2
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet_condconv(
         'tf_efficientnet_cc_b0_8e', channel_multiplier=1.0, depth_multiplier=1.0, experts_multiplier=2,
         pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_cc_b1_8e(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-CondConv-B1 w/ 8 Experts. Tensorflow compatible variant """
     # NOTE for train, drop_rate should be 0.2, drop_path_rate should be 0.2
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet_condconv(
         'tf_efficientnet_cc_b1_8e', channel_multiplier=1.0, depth_multiplier=1.1, experts_multiplier=2,
         pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_lite0(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-Lite0 """
     # NOTE for train, drop_rate should be 0.2, drop_path_rate should be 0.2
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet_lite(
         'tf_efficientnet_lite0', channel_multiplier=1.0, depth_multiplier=1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_lite1(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-Lite1 """
     # NOTE for train, drop_rate should be 0.2, drop_path_rate should be 0.2
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet_lite(
         'tf_efficientnet_lite1', channel_multiplier=1.0, depth_multiplier=1.1, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_lite2(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-Lite2 """
     # NOTE for train, drop_rate should be 0.3, drop_path_rate should be 0.2
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet_lite(
         'tf_efficientnet_lite2', channel_multiplier=1.1, depth_multiplier=1.2, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_lite3(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-Lite3 """
     # NOTE for train, drop_rate should be 0.3, drop_path_rate should be 0.2
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet_lite(
         'tf_efficientnet_lite3', channel_multiplier=1.2, depth_multiplier=1.4, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnet_lite4(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-Lite4 """
     # NOTE for train, drop_rate should be 0.4, drop_path_rate should be 0.2
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnet_lite(
         'tf_efficientnet_lite4', channel_multiplier=1.4, depth_multiplier=1.8, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnetv2_s(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-V2 Small. Tensorflow compatible variant  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnetv2_s('tf_efficientnetv2_s', pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnetv2_m(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-V2 Medium. Tensorflow compatible variant  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnetv2_m('tf_efficientnetv2_m', pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnetv2_l(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-V2 Large. Tensorflow compatible variant  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnetv2_l('tf_efficientnetv2_l', pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnetv2_xl(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-V2 Xtra-Large. Tensorflow compatible variant
     """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnetv2_xl('tf_efficientnetv2_xl', pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnetv2_b0(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-V2-B0. Tensorflow compatible variant  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnetv2_base('tf_efficientnetv2_b0', pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnetv2_b1(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-V2-B1. Tensorflow compatible variant  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnetv2_base(
         'tf_efficientnetv2_b1', channel_multiplier=1.0, depth_multiplier=1.1, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnetv2_b2(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-V2-B2. Tensorflow compatible variant  """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnetv2_base(
         'tf_efficientnetv2_b2', channel_multiplier=1.1, depth_multiplier=1.2, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_efficientnetv2_b3(pretrained=False, **kwargs) -> EfficientNet:
     """ EfficientNet-V2-B3. Tensorflow compatible variant """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_efficientnetv2_base(
         'tf_efficientnetv2_b3', channel_multiplier=1.2, depth_multiplier=1.4, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def mixnet_s(pretrained=False, **kwargs) -> EfficientNet:
@@ -2270,38 +2324,38 @@
     return model
 
 
 @register_model
 def tf_mixnet_s(pretrained=False, **kwargs) -> EfficientNet:
     """Creates a MixNet Small model. Tensorflow compatible variant
     """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_mixnet_s(
         'tf_mixnet_s', channel_multiplier=1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_mixnet_m(pretrained=False, **kwargs) -> EfficientNet:
     """Creates a MixNet Medium model. Tensorflow compatible variant
     """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_mixnet_m(
         'tf_mixnet_m', channel_multiplier=1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_mixnet_l(pretrained=False, **kwargs) -> EfficientNet:
     """Creates a MixNet Large model. Tensorflow compatible variant
     """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_mixnet_m(
         'tf_mixnet_l', channel_multiplier=1.3, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tinynet_a(pretrained=False, **kwargs) -> EfficientNet:
@@ -2357,8 +2411,12 @@
     'tf_efficientnetv2_m_in21ft1k': 'tf_efficientnetv2_m.in21k_ft_in1k',
     'tf_efficientnetv2_l_in21ft1k': 'tf_efficientnetv2_l.in21k_ft_in1k',
     'tf_efficientnetv2_xl_in21ft1k': 'tf_efficientnetv2_xl.in21k_ft_in1k',
     'tf_efficientnetv2_s_in21k': 'tf_efficientnetv2_s.in21k',
     'tf_efficientnetv2_m_in21k': 'tf_efficientnetv2_m.in21k',
     'tf_efficientnetv2_l_in21k': 'tf_efficientnetv2_l.in21k',
     'tf_efficientnetv2_xl_in21k': 'tf_efficientnetv2_xl.in21k',
+    'efficientnet_b2a': 'efficientnet_b2',
+    'efficientnet_b3a': 'efficientnet_b3',
+    'mnasnet_a1': 'semnasnet_100',
+    'mnasnet_b1': 'mnasnet_100',
 })
```

### Comparing `timm-0.9.9/timm/models/efficientvit_mit.py` & `timm-1.0.3/timm/models/efficientvit_mit.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,21 +4,22 @@
     - https://arxiv.org/abs/2205.14756
 
 Adapted from official impl at https://github.com/mit-han-lab/efficientvit
 """
 
 __all__ = ['EfficientVit']
 from typing import Optional
+from functools import partial
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
-from timm.layers import SelectAdaptivePool2d, create_conv2d
+from timm.layers import SelectAdaptivePool2d, create_conv2d, GELUTanh
 from ._builder import build_model_with_cfg
 from ._features_fx import register_notrace_module
 from ._manipulate import checkpoint_seq
 from ._registry import register_model, generate_default_cfgs
 
 
 def val2list(x: list or tuple or any, repeat_time=1):
@@ -66,15 +67,15 @@
             kernel_size=kernel_size,
             stride=stride,
             dilation=dilation,
             groups=groups,
             bias=bias,
         )
         self.norm = norm_layer(num_features=out_channels) if norm_layer else nn.Identity()
-        self.act = act_layer(inplace=True) if act_layer else nn.Identity()
+        self.act = act_layer(inplace=True) if act_layer is not None else nn.Identity()
 
     def forward(self, x):
         x = self.dropout(x)
         x = self.conv(x)
         x = self.norm(x)
         x = self.act(x)
         return x
@@ -117,14 +118,58 @@
 
     def forward(self, x):
         x = self.depth_conv(x)
         x = self.point_conv(x)
         return x
 
 
+class ConvBlock(nn.Module):
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+        kernel_size=3,
+        stride=1,
+        mid_channels=None,
+        expand_ratio=1,
+        use_bias=False,
+        norm_layer=(nn.BatchNorm2d, nn.BatchNorm2d),
+        act_layer=(nn.ReLU6, None),
+    ):
+        super(ConvBlock, self).__init__()
+        use_bias = val2tuple(use_bias, 2)
+        norm_layer = val2tuple(norm_layer, 2)
+        act_layer = val2tuple(act_layer, 2)
+        mid_channels = mid_channels or round(in_channels * expand_ratio)
+
+        self.conv1 = ConvNormAct(
+            in_channels,
+            mid_channels,
+            kernel_size,
+            stride,
+            norm_layer=norm_layer[0],
+            act_layer=act_layer[0],
+            bias=use_bias[0],
+        )
+        self.conv2 = ConvNormAct(
+            mid_channels,
+            out_channels,
+            kernel_size,
+            1,
+            norm_layer=norm_layer[1],
+            act_layer=act_layer[1],
+            bias=use_bias[1],
+        )
+
+    def forward(self, x):
+        x = self.conv1(x)
+        x = self.conv2(x)
+        return x
+
+
 class MBConv(nn.Module):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         kernel_size=3,
         stride=1,
@@ -171,16 +216,61 @@
     def forward(self, x):
         x = self.inverted_conv(x)
         x = self.depth_conv(x)
         x = self.point_conv(x)
         return x
 
 
-class LiteMSA(nn.Module):
-    """Lightweight multi-scale attention"""
+class FusedMBConv(nn.Module):
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+        kernel_size=3,
+        stride=1,
+        mid_channels=None,
+        expand_ratio=6,
+        groups=1,
+        use_bias=False,
+        norm_layer=(nn.BatchNorm2d, nn.BatchNorm2d),
+        act_layer=(nn.ReLU6, None),
+    ):
+        super(FusedMBConv, self).__init__()
+        use_bias = val2tuple(use_bias, 2)
+        norm_layer = val2tuple(norm_layer, 2)
+        act_layer = val2tuple(act_layer, 2)
+        mid_channels = mid_channels or round(in_channels * expand_ratio)
+
+        self.spatial_conv = ConvNormAct(
+            in_channels,
+            mid_channels,
+            kernel_size,
+            stride=stride,
+            groups=groups,
+            norm_layer=norm_layer[0],
+            act_layer=act_layer[0],
+            bias=use_bias[0],
+        )
+        self.point_conv = ConvNormAct(
+            mid_channels,
+            out_channels,
+            1,
+            norm_layer=norm_layer[1],
+            act_layer=act_layer[1],
+            bias=use_bias[1],
+        )
+
+    def forward(self, x):
+        x = self.spatial_conv(x)
+        x = self.point_conv(x)
+        return x
+
+
+class LiteMLA(nn.Module):
+    """Lightweight multi-scale linear attention"""
 
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         heads: int or None = None,
         heads_ratio: float = 1.0,
@@ -188,15 +278,15 @@
         use_bias=False,
         norm_layer=(None, nn.BatchNorm2d),
         act_layer=(None, None),
         kernel_func=nn.ReLU,
         scales=(5,),
         eps=1e-5,
     ):
-        super(LiteMSA, self).__init__()
+        super(LiteMLA, self).__init__()
         self.eps = eps
         heads = heads or int(in_channels // dim * heads_ratio)
         total_dim = heads * dim
         use_bias = val2tuple(use_bias, 2)
         norm_layer = val2tuple(norm_layer, 2)
         act_layer = val2tuple(act_layer, 2)
 
@@ -267,30 +357,30 @@
 
         # final projection
         out = out.transpose(-1, -2).reshape(B, -1, H, W)
         out = self.proj(out)
         return out
 
 
-register_notrace_module(LiteMSA)
+register_notrace_module(LiteMLA)
 
 
 class EfficientVitBlock(nn.Module):
     def __init__(
         self,
         in_channels,
         heads_ratio=1.0,
         head_dim=32,
         expand_ratio=4,
         norm_layer=nn.BatchNorm2d,
         act_layer=nn.Hardswish,
     ):
         super(EfficientVitBlock, self).__init__()
         self.context_module = ResidualBlock(
-            LiteMSA(
+            LiteMLA(
                 in_channels=in_channels,
                 out_channels=in_channels,
                 heads_ratio=heads_ratio,
                 dim=head_dim,
                 norm_layer=(None, norm_layer),
             ),
             nn.Identity(),
@@ -336,39 +426,62 @@
         in_channels: int,
         out_channels: int,
         stride: int,
         expand_ratio: float,
         norm_layer: str,
         act_layer: str,
         fewer_norm: bool = False,
+        block_type: str = "default",
 ):
+    assert block_type in ["default", "large", "fused"]
     if expand_ratio == 1:
-        block = DSConv(
-            in_channels=in_channels,
-            out_channels=out_channels,
-            stride=stride,
-            use_bias=(True, False) if fewer_norm else False,
-            norm_layer=(None, norm_layer) if fewer_norm else norm_layer,
-            act_layer=(act_layer, None),
-        )
+        if block_type == "default":
+            block = DSConv(
+                in_channels=in_channels,
+                out_channels=out_channels,
+                stride=stride,
+                use_bias=(True, False) if fewer_norm else False,
+                norm_layer=(None, norm_layer) if fewer_norm else norm_layer,
+                act_layer=(act_layer, None),
+            )
+        else:
+            block = ConvBlock(
+                in_channels=in_channels,
+                out_channels=out_channels,
+                stride=stride,
+                use_bias=(True, False) if fewer_norm else False,
+                norm_layer=(None, norm_layer) if fewer_norm else norm_layer,
+                act_layer=(act_layer, None),
+            )
     else:
-        block = MBConv(
-            in_channels=in_channels,
-            out_channels=out_channels,
-            stride=stride,
-            expand_ratio=expand_ratio,
-            use_bias=(True, True, False) if fewer_norm else False,
-            norm_layer=(None, None, norm_layer) if fewer_norm else norm_layer,
-            act_layer=(act_layer, act_layer, None),
-        )
+        if block_type == "default":
+            block = MBConv(
+                in_channels=in_channels,
+                out_channels=out_channels,
+                stride=stride,
+                expand_ratio=expand_ratio,
+                use_bias=(True, True, False) if fewer_norm else False,
+                norm_layer=(None, None, norm_layer) if fewer_norm else norm_layer,
+                act_layer=(act_layer, act_layer, None),
+            )
+        else:
+            block = FusedMBConv(
+                in_channels=in_channels,
+                out_channels=out_channels,
+                stride=stride,
+                expand_ratio=expand_ratio,
+                use_bias=(True, False) if fewer_norm else False,
+                norm_layer=(None, norm_layer) if fewer_norm else norm_layer,
+                act_layer=(act_layer, None),
+            )
     return block
 
 
 class Stem(nn.Sequential):
-    def __init__(self, in_chs, out_chs, depth, norm_layer, act_layer):
+    def __init__(self, in_chs, out_chs, depth, norm_layer, act_layer, block_type='default'):
         super().__init__()
         self.stride = 2
 
         self.add_module(
             'in_conv',
             ConvNormAct(
                 in_chs, out_chs,
@@ -381,14 +494,15 @@
                 build_local_block(
                     in_channels=out_chs,
                     out_channels=out_chs,
                     stride=1,
                     expand_ratio=1,
                     norm_layer=norm_layer,
                     act_layer=act_layer,
+                    block_type=block_type,
                 ),
                 nn.Identity(),
             ))
             stem_block += 1
 
 
 class EfficientVitStage(nn.Module):
@@ -447,32 +561,96 @@
 
         self.blocks = nn.Sequential(*blocks)
 
     def forward(self, x):
         return self.blocks(x)
 
 
+class EfficientVitLargeStage(nn.Module):
+    def __init__(
+            self,
+            in_chs,
+            out_chs,
+            depth,
+            norm_layer,
+            act_layer,
+            head_dim,
+            vit_stage=False,
+            fewer_norm=False,
+    ):
+        super(EfficientVitLargeStage, self).__init__()
+        blocks = [ResidualBlock(
+            build_local_block(
+                in_channels=in_chs,
+                out_channels=out_chs,
+                stride=2,
+                expand_ratio=24 if vit_stage else 16,
+                norm_layer=norm_layer,
+                act_layer=act_layer,
+                fewer_norm=vit_stage or fewer_norm,
+                block_type='default' if fewer_norm else 'fused',
+            ),
+            None,
+        )]
+        in_chs = out_chs
+
+        if vit_stage:
+            # for stage 4
+            for _ in range(depth):
+                blocks.append(
+                    EfficientVitBlock(
+                        in_channels=in_chs,
+                        head_dim=head_dim,
+                        expand_ratio=6,
+                        norm_layer=norm_layer,
+                        act_layer=act_layer,
+                    )
+                )
+        else:
+            # for stage 1, 2, 3
+            for i in range(depth):
+                blocks.append(ResidualBlock(
+                    build_local_block(
+                        in_channels=in_chs,
+                        out_channels=out_chs,
+                        stride=1,
+                        expand_ratio=4,
+                        norm_layer=norm_layer,
+                        act_layer=act_layer,
+                        fewer_norm=fewer_norm,
+                        block_type='default' if fewer_norm else 'fused',
+                    ),
+                    nn.Identity(),
+                ))
+
+        self.blocks = nn.Sequential(*blocks)
+
+    def forward(self, x):
+        return self.blocks(x)
+
+
 class ClassifierHead(nn.Module):
     def __init__(
         self,
         in_channels,
         widths,
         n_classes=1000,
         dropout=0.,
         norm_layer=nn.BatchNorm2d,
         act_layer=nn.Hardswish,
         global_pool='avg',
+        norm_eps=1e-5,
     ):
         super(ClassifierHead, self).__init__()
         self.in_conv = ConvNormAct(in_channels, widths[0], 1, norm_layer=norm_layer, act_layer=act_layer)
         self.global_pool = SelectAdaptivePool2d(pool_type=global_pool, flatten=True, input_fmt='NCHW')
         self.classifier = nn.Sequential(
             nn.Linear(widths[0], widths[1], bias=False),
-            nn.LayerNorm(widths[1]),
-            act_layer(inplace=True),
+            nn.LayerNorm(widths[1], eps=norm_eps),
+            act_layer(inplace=True) if act_layer is not None else nn.Identity(),
             nn.Dropout(dropout, inplace=False),
             nn.Linear(widths[1], n_classes, bias=True),
         )
 
     def forward(self, x, pre_logits: bool = False):
         x = self.in_conv(x)
         x = self.global_pool(x)
@@ -557,25 +735,144 @@
     def set_grad_checkpointing(self, enable=True):
         self.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.classifier[-1]
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
+        self.num_classes = num_classes
+        if global_pool is not None:
+            self.global_pool = global_pool
+        if num_classes > 0:
+            self.head = ClassifierHead(
+                self.num_features,
+                self.head_widths,
+                n_classes=num_classes,
+                dropout=self.head_dropout,
+                global_pool=self.global_pool,
+            )
+        else:
+            if self.global_pool == 'avg':
+                self.head = SelectAdaptivePool2d(pool_type=self.global_pool, flatten=True)
+            else:
+                self.head = nn.Identity()
+
+    def forward_features(self, x):
+        x = self.stem(x)
+        if self.grad_checkpointing and not torch.jit.is_scripting():
+            x = checkpoint_seq(self.stages, x)
+        else:
+            x = self.stages(x)
+        return x
+
+    def forward_head(self, x, pre_logits: bool = False):
+        return self.head(x, pre_logits=pre_logits) if pre_logits else self.head(x)
+
+    def forward(self, x):
+        x = self.forward_features(x)
+        x = self.forward_head(x)
+        return x
+
+
+class EfficientVitLarge(nn.Module):
+    def __init__(
+        self,
+        in_chans=3,
+        widths=(),
+        depths=(),
+        head_dim=32,
+        norm_layer=nn.BatchNorm2d,
+        act_layer=GELUTanh,
+        global_pool='avg',
+        head_widths=(),
+        drop_rate=0.0,
+        num_classes=1000,
+        norm_eps=1e-7,
+    ):
+        super(EfficientVitLarge, self).__init__()
+        self.grad_checkpointing = False
+        self.global_pool = global_pool
+        self.num_classes = num_classes
+        self.norm_eps = norm_eps
+        norm_layer = partial(norm_layer, eps=self.norm_eps)
+
+        # input stem
+        self.stem = Stem(in_chans, widths[0], depths[0], norm_layer, act_layer, block_type='large')
+        stride = self.stem.stride
+
+        # stages
+        self.feature_info = []
+        self.stages = nn.Sequential()
+        in_channels = widths[0]
+        for i, (w, d) in enumerate(zip(widths[1:], depths[1:])):
+            self.stages.append(EfficientVitLargeStage(
+                in_channels,
+                w,
+                depth=d,
+                norm_layer=norm_layer,
+                act_layer=act_layer,
+                head_dim=head_dim,
+                vit_stage=i >= 3,
+                fewer_norm=i >= 2,
+            ))
+            stride *= 2
+            in_channels = w
+            self.feature_info += [dict(num_chs=in_channels, reduction=stride, module=f'stages.{i}')]
+
+        self.num_features = in_channels
+        self.head_widths = head_widths
+        self.head_dropout = drop_rate
+        if num_classes > 0:
+            self.head = ClassifierHead(
+                self.num_features,
+                self.head_widths,
+                n_classes=num_classes,
+                dropout=self.head_dropout,
+                global_pool=self.global_pool,
+                act_layer=act_layer,
+                norm_eps=self.norm_eps,
+            )
+        else:
+            if self.global_pool == 'avg':
+                self.head = SelectAdaptivePool2d(pool_type=global_pool, flatten=True)
+            else:
+                self.head = nn.Identity()
+
+    @torch.jit.ignore
+    def group_matcher(self, coarse=False):
+        matcher = dict(
+            stem=r'^stem',
+            blocks=r'^stages\.(\d+)' if coarse else [
+                (r'^stages\.(\d+).downsample', (0,)),
+                (r'^stages\.(\d+)\.\w+\.(\d+)', None),
+            ]
+        )
+        return matcher
+
+    @torch.jit.ignore
+    def set_grad_checkpointing(self, enable=True):
+        self.grad_checkpointing = enable
+
+    @torch.jit.ignore
+    def get_classifier(self):
+        return self.head.classifier[-1]
+
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             self.global_pool = global_pool
         if num_classes > 0:
             self.head = ClassifierHead(
                 self.num_features,
                 self.head_widths,
                 n_classes=num_classes,
                 dropout=self.head_dropout,
                 global_pool=self.global_pool,
+                norm_eps=self.norm_eps
             )
         else:
             if self.global_pool == 'avg':
                 self.head = SelectAdaptivePool2d(pool_type=self.global_pool, flatten=True)
             else:
                 self.head = nn.Identity()
 
@@ -644,14 +941,65 @@
         hf_hub_id='timm/',
         input_size=(3, 256, 256), pool_size=(8, 8), crop_pct=1.0,
     ),
     'efficientvit_b3.r288_in1k': _cfg(
         hf_hub_id='timm/',
         input_size=(3, 288, 288), pool_size=(9, 9), crop_pct=1.0,
     ),
+    'efficientvit_l1.r224_in1k': _cfg(
+        hf_hub_id='timm/',
+        crop_pct=1.0,
+    ),
+    'efficientvit_l2.r224_in1k': _cfg(
+        hf_hub_id='timm/',
+        crop_pct=1.0,
+    ),
+    'efficientvit_l2.r256_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), pool_size=(8, 8), crop_pct=1.0,
+    ),
+    'efficientvit_l2.r288_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 288, 288), pool_size=(9, 9), crop_pct=1.0,
+    ),
+    'efficientvit_l2.r384_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 384, 384), pool_size=(12, 12), crop_pct=1.0,
+    ),
+    'efficientvit_l3.r224_in1k': _cfg(
+        hf_hub_id='timm/',
+        crop_pct=1.0,
+    ),
+    'efficientvit_l3.r256_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), pool_size=(8, 8), crop_pct=1.0,
+    ),
+    'efficientvit_l3.r320_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 320, 320), pool_size=(10, 10), crop_pct=1.0,
+    ),
+    'efficientvit_l3.r384_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 384, 384), pool_size=(12, 12), crop_pct=1.0,
+    ),
+    # 'efficientvit_l0_sam.sam': _cfg(
+    #     # hf_hub_id='timm/',
+    #     input_size=(3, 512, 512), crop_pct=1.0,
+    #     num_classes=0,
+    # ),
+    # 'efficientvit_l1_sam.sam': _cfg(
+    #     # hf_hub_id='timm/',
+    #     input_size=(3, 512, 512), crop_pct=1.0,
+    #     num_classes=0,
+    # ),
+    # 'efficientvit_l2_sam.sam': _cfg(
+    #     # hf_hub_id='timm/',f
+    #     input_size=(3, 512, 512), crop_pct=1.0,
+    #     num_classes=0,
+    # ),
 })
 
 
 def _create_efficientvit(variant, pretrained=False, **kwargs):
     out_indices = kwargs.pop('out_indices', (0, 1, 2, 3))
     model = build_model_with_cfg(
         EfficientVit,
@@ -659,14 +1007,26 @@
         pretrained,
         feature_cfg=dict(flatten_sequential=True, out_indices=out_indices),
         **kwargs
     )
     return model
 
 
+def _create_efficientvit_large(variant, pretrained=False, **kwargs):
+    out_indices = kwargs.pop('out_indices', (0, 1, 2, 3))
+    model = build_model_with_cfg(
+        EfficientVitLarge,
+        variant,
+        pretrained,
+        feature_cfg=dict(flatten_sequential=True, out_indices=out_indices),
+        **kwargs
+    )
+    return model
+
+
 @register_model
 def efficientvit_b0(pretrained=False, **kwargs):
     model_args = dict(
         widths=(8, 16, 32, 64, 128), depths=(1, 2, 2, 2, 2), head_dim=16, head_widths=(1024, 1280))
     return _create_efficientvit('efficientvit_b0', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
@@ -685,7 +1045,53 @@
 
 
 @register_model
 def efficientvit_b3(pretrained=False, **kwargs):
     model_args = dict(
         widths=(32, 64, 128, 256, 512), depths=(1, 4, 6, 6, 9), head_dim=32, head_widths=(2304, 2560))
     return _create_efficientvit('efficientvit_b3', pretrained=pretrained, **dict(model_args, **kwargs))
+
+
+@register_model
+def efficientvit_l1(pretrained=False, **kwargs):
+    model_args = dict(
+        widths=(32, 64, 128, 256, 512), depths=(1, 1, 1, 6, 6), head_dim=32, head_widths=(3072, 3200))
+    return _create_efficientvit_large('efficientvit_l1', pretrained=pretrained, **dict(model_args, **kwargs))
+
+
+@register_model
+def efficientvit_l2(pretrained=False, **kwargs):
+    model_args = dict(
+        widths=(32, 64, 128, 256, 512), depths=(1, 2, 2, 8, 8), head_dim=32, head_widths=(3072, 3200))
+    return _create_efficientvit_large('efficientvit_l2', pretrained=pretrained, **dict(model_args, **kwargs))
+
+
+@register_model
+def efficientvit_l3(pretrained=False, **kwargs):
+    model_args = dict(
+        widths=(64, 128, 256, 512, 1024), depths=(1, 2, 2, 8, 8), head_dim=32, head_widths=(6144, 6400))
+    return _create_efficientvit_large('efficientvit_l3', pretrained=pretrained, **dict(model_args, **kwargs))
+
+
+# FIXME will wait for v2 SAM models which are pending
+# @register_model
+# def efficientvit_l0_sam(pretrained=False, **kwargs):
+#     # only backbone for segment-anything-model weights
+#     model_args = dict(
+#         widths=(32, 64, 128, 256, 512), depths=(1, 1, 1, 4, 4), head_dim=32, num_classes=0, norm_eps=1e-6)
+#     return _create_efficientvit_large('efficientvit_l0_sam', pretrained=pretrained, **dict(model_args, **kwargs))
+#
+#
+# @register_model
+# def efficientvit_l1_sam(pretrained=False, **kwargs):
+#     # only backbone for segment-anything-model weights
+#     model_args = dict(
+#         widths=(32, 64, 128, 256, 512), depths=(1, 1, 1, 6, 6), head_dim=32, num_classes=0, norm_eps=1e-6)
+#     return _create_efficientvit_large('efficientvit_l1_sam', pretrained=pretrained, **dict(model_args, **kwargs))
+#
+#
+# @register_model
+# def efficientvit_l2_sam(pretrained=False, **kwargs):
+#     # only backbone for segment-anything-model weights
+#     model_args = dict(
+#         widths=(32, 64, 128, 256, 512), depths=(1, 2, 2, 8, 8), head_dim=32, num_classes=0, norm_eps=1e-6)
+#     return _create_efficientvit_large('efficientvit_l2_sam', pretrained=pretrained, **dict(model_args, **kwargs))
```

### Comparing `timm-0.9.9/timm/models/efficientvit_msra.py` & `timm-1.0.3/timm/models/efficientvit_msra.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 Adapted from official impl at https://github.com/microsoft/Cream/tree/main/EfficientViT
 """
 
 __all__ = ['EfficientVitMsra']
 import itertools
 from collections import OrderedDict
-from typing import Dict
+from typing import Dict, Optional
 
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import SqueezeExcite, SelectAdaptivePool2d, trunc_normal_, _assert
 from ._builder import build_model_with_cfg
@@ -460,15 +460,15 @@
     def set_grad_checkpointing(self, enable=True):
         self.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.linear
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             if global_pool == 'avg':
                 self.global_pool = SelectAdaptivePool2d(pool_type=global_pool, flatten=True)
             else:
                 assert num_classes == 0
                 self.global_pool = nn.Identity()
```

### Comparing `timm-0.9.9/timm/models/eva.py` & `timm-1.0.3/timm/models/eva.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,43 +20,44 @@
 
 This file contains EVA & EVA02 model implementations evolved from BEiT, additional models in vision_transformer.py.
 
 Modifications by / Copyright 2023 Ross Wightman, original copyrights below
 """
 # EVA models Copyright (c) 2022 BAAI-Vision
 # EVA02 models Copyright (c) 2023 BAAI-Vision
-
 import math
-from typing import Callable, Optional, Tuple, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils.checkpoint import checkpoint
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD, OPENAI_CLIP_MEAN, OPENAI_CLIP_STD
 from timm.layers import PatchEmbed, Mlp, GluMlp, SwiGLU, LayerNorm, DropPath, PatchDropout, RotaryEmbeddingCat, \
     apply_rot_embed_cat, apply_keep_indices_nlc, trunc_normal_, resample_patch_embed, resample_abs_pos_embed, \
     to_2tuple, use_fused_attn
 
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._registry import generate_default_cfgs, register_model
 
 __all__ = ['Eva']
 
 
 class EvaAttention(nn.Module):
     fused_attn: torch.jit.Final[bool]
 
     def __init__(
             self,
             dim: int,
             num_heads: int = 8,
             qkv_bias: bool = True,
             qkv_fused: bool = True,
+            num_prefix_tokens: int = 1,
             attn_drop: float = 0.,
             proj_drop: float = 0.,
             attn_head_dim: Optional[int] = None,
             norm_layer: Optional[Callable] = None,
     ):
         """
 
@@ -73,14 +74,15 @@
         super().__init__()
         self.num_heads = num_heads
         head_dim = dim // num_heads
         if attn_head_dim is not None:
             head_dim = attn_head_dim
         all_head_dim = head_dim * self.num_heads
         self.scale = head_dim ** -0.5
+        self.num_prefix_tokens = num_prefix_tokens
         self.fused_attn = use_fused_attn()
 
         if qkv_fused:
             self.qkv = nn.Linear(dim, all_head_dim * 3, bias=False)
             self.q_proj = self.k_proj = self.v_proj = None
             if qkv_bias:
                 self.q_bias = nn.Parameter(torch.zeros(all_head_dim))
@@ -115,16 +117,17 @@
             q, k, v = qkv.unbind(0)  # B, num_heads, N, head_dim
         else:
             q = self.q_proj(x).reshape(B, N, self.num_heads, -1).transpose(1, 2)  # B, num_heads, N, C
             k = self.k_proj(x).reshape(B, N, self.num_heads, -1).transpose(1, 2)
             v = self.v_proj(x).reshape(B, N, self.num_heads, -1).transpose(1, 2)
 
         if rope is not None:
-            q = torch.cat([q[:, :, :1, :], apply_rot_embed_cat(q[:, :, 1:, :], rope)], 2).type_as(v)
-            k = torch.cat([k[:, :, :1, :], apply_rot_embed_cat(k[:, :, 1:, :], rope)], 2).type_as(v)
+            npt = self.num_prefix_tokens
+            q = torch.cat([q[:, :, :npt, :], apply_rot_embed_cat(q[:, :, npt:, :], rope)], dim=2).type_as(v)
+            k = torch.cat([k[:, :, :npt, :], apply_rot_embed_cat(k[:, :, npt:, :], rope)], dim=2).type_as(v)
 
         if self.fused_attn:
             x = F.scaled_dot_product_attention(
                 q, k, v,
                 attn_mask=attn_mask,
                 dropout_p=self.attn_drop.p if self.training else 0.,
             )
@@ -153,14 +156,15 @@
             num_heads: int,
             qkv_bias: bool = True,
             qkv_fused: bool = True,
             mlp_ratio: float = 4.,
             swiglu_mlp: bool = False,
             scale_mlp: bool = False,
             scale_attn_inner: bool = False,
+            num_prefix_tokens: int = 1,
             proj_drop: float = 0.,
             attn_drop: float = 0.,
             drop_path: float = 0.,
             init_values: Optional[float] = None,
             act_layer: Callable = nn.GELU,
             norm_layer: Callable = LayerNorm,
             attn_head_dim: Optional[int] = None,
@@ -187,14 +191,15 @@
         super().__init__()
         self.norm1 = norm_layer(dim)
         self.attn = EvaAttention(
             dim,
             num_heads=num_heads,
             qkv_bias=qkv_bias,
             qkv_fused=qkv_fused,
+            num_prefix_tokens=num_prefix_tokens,
             attn_drop=attn_drop,
             proj_drop=proj_drop,
             attn_head_dim=attn_head_dim,
             norm_layer=norm_layer if scale_attn_inner else None,
         )
         self.gamma_1 = nn.Parameter(init_values * torch.ones(dim)) if init_values is not None else None
         self.drop_path1 = DropPath(drop_path) if drop_path > 0. else nn.Identity()
@@ -249,14 +254,15 @@
             num_heads: int,
             qkv_bias: bool = True,
             qkv_fused: bool = True,
             mlp_ratio: float = 4.,
             swiglu_mlp: bool = False,
             scale_mlp: bool = False,
             scale_attn_inner: bool = False,
+            num_prefix_tokens: int = 1,
             proj_drop: float = 0.,
             attn_drop: float = 0.,
             drop_path: float = 0.,
             init_values: Optional[float] = None,  # ignore for post-norm
             act_layer: Callable = nn.GELU,
             norm_layer: Callable = nn.LayerNorm,
             attn_head_dim: Optional[int] = None,
@@ -282,14 +288,15 @@
         """
         super().__init__()
         self.attn = EvaAttention(
             dim,
             num_heads=num_heads,
             qkv_bias=qkv_bias,
             qkv_fused=qkv_fused,
+            num_prefix_tokens=num_prefix_tokens,
             attn_drop=attn_drop,
             proj_drop=proj_drop,
             attn_head_dim=attn_head_dim,
             norm_layer=norm_layer if scale_attn_inner else None,
         )
         self.norm1 = norm_layer(dim)
         self.drop_path1 = DropPath(drop_path) if drop_path > 0. else nn.Identity()
@@ -360,14 +367,15 @@
             patch_drop_rate: float = 0.,
             proj_drop_rate: float = 0.,
             attn_drop_rate: float = 0.,
             drop_path_rate: float = 0.,
             norm_layer: Callable = LayerNorm,
             init_values: Optional[float] = None,
             class_token: bool = True,
+            num_reg_tokens: int = 0,
             use_abs_pos_emb: bool = True,
             use_rot_pos_emb: bool = False,
             use_post_norm: bool = False,
             dynamic_img_size: bool = False,
             dynamic_img_pad: bool = False,
             ref_feat_shape: Optional[Union[Tuple[int, int], int]] = None,
             head_init_scale: float = 0.001,
@@ -403,15 +411,15 @@
             ref_feat_shape:
             head_init_scale:
         """
         super().__init__()
         self.num_classes = num_classes
         self.global_pool = global_pool
         self.num_features = self.embed_dim = embed_dim  # num_features for consistency with other models
-        self.num_prefix_tokens = 1 if class_token else 0
+        self.num_prefix_tokens = (1 if class_token else 0) + num_reg_tokens
         self.dynamic_img_size = dynamic_img_size
         self.grad_checkpointing = False
 
         embed_args = {}
         if dynamic_img_size:
             # flatten deferred until after pos embed
             embed_args.update(dict(strict_img_size=False, output_fmt='NHWC'))
@@ -420,16 +428,19 @@
             patch_size=patch_size,
             in_chans=in_chans,
             embed_dim=embed_dim,
             dynamic_img_pad=dynamic_img_pad,
             **embed_args,
         )
         num_patches = self.patch_embed.num_patches
+        r = self.patch_embed.feat_ratio() if hasattr(self.patch_embed, 'feat_ratio') else patch_size
 
         self.cls_token = nn.Parameter(torch.zeros(1, 1, embed_dim)) if class_token else None
+        self.reg_token = nn.Parameter(torch.zeros(1, num_reg_tokens, embed_dim)) if num_reg_tokens else None
+        self.cls_embed = class_token and self.reg_token is None
 
         self.pos_embed = nn.Parameter(
             torch.zeros(1, num_patches + self.num_prefix_tokens, embed_dim)) if use_abs_pos_emb else None
         self.pos_drop = nn.Dropout(p=pos_drop_rate)
         if patch_drop_rate > 0:
             self.patch_drop = PatchDropout(
                 patch_drop_rate,
@@ -458,32 +469,38 @@
                 num_heads=num_heads,
                 qkv_bias=qkv_bias,
                 qkv_fused=qkv_fused,
                 mlp_ratio=mlp_ratio,
                 swiglu_mlp=swiglu_mlp,
                 scale_mlp=scale_mlp,
                 scale_attn_inner=scale_attn_inner,
+                num_prefix_tokens=self.num_prefix_tokens,
                 proj_drop=proj_drop_rate,
                 attn_drop=attn_drop_rate,
                 drop_path=dpr[i],
                 norm_layer=norm_layer,
                 init_values=init_values,
             )
             for i in range(depth)])
+        self.feature_info = [
+            dict(module=f'blocks.{i}', num_chs=embed_dim, reduction=r) for i in range(depth)]
 
         use_fc_norm = self.global_pool == 'avg'
         self.norm = nn.Identity() if use_fc_norm else norm_layer(embed_dim)
         self.fc_norm = norm_layer(embed_dim) if use_fc_norm else nn.Identity()
         self.head_drop = nn.Dropout(drop_rate)
         self.head = nn.Linear(embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
         self.apply(self._init_weights)
         if self.pos_embed is not None:
             trunc_normal_(self.pos_embed, std=.02)
-        trunc_normal_(self.cls_token, std=.02)
+        if self.cls_token is not None:
+            trunc_normal_(self.cls_token, std=.02)
+        if self.reg_token is not None:
+            trunc_normal_(self.reg_token, std=.02)
 
         self.fix_init_weight()
         if isinstance(self.head, nn.Linear):
             trunc_normal_(self.head.weight, std=.02)
             self.head.weight.data.mul_(head_init_scale)
             self.head.bias.data.mul_(head_init_scale)
 
@@ -518,15 +535,15 @@
         )
         return matcher
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             self.global_pool = global_pool
         self.head = nn.Linear(self.embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
     def _pos_embed(self, x) -> Tuple[torch.Tensor, Optional[torch.Tensor]]:
         if self.dynamic_img_size:
@@ -543,25 +560,109 @@
             rot_pos_embed = self.rope.get_embed(shape=(H, W)) if self.rope is not None else None
         else:
             pos_embed = self.pos_embed
             rot_pos_embed = self.rope.get_embed() if self.rope is not None else None
 
         if self.cls_token is not None:
             x = torch.cat((self.cls_token.expand(x.shape[0], -1, -1), x), dim=1)
+
         if pos_embed is not None:
             x = x + pos_embed
+
+        if self.reg_token is not None:
+            to_cat = []
+            if self.cls_token is not None:
+                to_cat.append(self.cls_token.expand(x.shape[0], -1, -1))
+            to_cat.append(self.reg_token.expand(x.shape[0], -1, -1))
+            x = torch.cat(to_cat + [x], dim=1)
+
         x = self.pos_drop(x)
 
         # obtain shared rotary position embedding and apply patch dropout
         if self.patch_drop is not None:
             x, keep_indices = self.patch_drop(x)
             if rot_pos_embed is not None and keep_indices is not None:
                 rot_pos_embed = apply_keep_indices_nlc(x, rot_pos_embed, keep_indices)
         return x, rot_pos_embed
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            return_prefix_tokens: bool = False,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if an int, if is a sequence, select by matching indices
+            return_prefix_tokens: Return both prefix and spatial intermediate tokens
+            norm: Apply norm layer to all intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        """
+        assert output_fmt in ('NCHW', 'NLC'), 'Output format for EVA-ViT features must be one of NCHW or NLC.'
+        reshape = output_fmt == 'NCHW'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+
+        # forward pass
+        B, _, height, width = x.shape
+        x = self.patch_embed(x)
+        x, rot_pos_embed = self._pos_embed(x)
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            blocks = self.blocks
+        else:
+            blocks = self.blocks[:max_index + 1]
+        for i, blk in enumerate(blocks):
+            x = blk(x, rope=rot_pos_embed)
+            if i in take_indices:
+                intermediates.append(self.norm(x) if norm else x)
+
+        # process intermediates
+        if self.num_prefix_tokens:
+            # split prefix (e.g. class, distill) and spatial feature tokens
+            prefix_tokens = [y[:, 0:self.num_prefix_tokens] for y in intermediates]
+            intermediates = [y[:, self.num_prefix_tokens:] for y in intermediates]
+        if reshape:
+            # reshape to BCHW output format
+            H, W = self.patch_embed.dynamic_feat_size((height, width))
+            intermediates = [y.reshape(B, H, W, -1).permute(0, 3, 1, 2).contiguous() for y in intermediates]
+        if not torch.jit.is_scripting() and return_prefix_tokens:
+            # return_prefix not support in torchscript due to poor type handling
+            intermediates = list(zip(intermediates, prefix_tokens))
+
+        if intermediates_only:
+            return intermediates
+
+        x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+        self.blocks = self.blocks[:max_index + 1]  # truncate blocks
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.fc_norm = nn.Identity()
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.patch_embed(x)
         x, rot_pos_embed = self._pos_embed(x)
         for blk in self.blocks:
             if self.grad_checkpointing and not torch.jit.is_scripting():
                 x = checkpoint(blk, x, rope=rot_pos_embed)
             else:
@@ -658,21 +759,21 @@
 
         out_dict[k] = v
 
     return out_dict
 
 
 def _create_eva(variant, pretrained=False, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError('features_only not implemented for Eva models.')
-
+    out_indices = kwargs.pop('out_indices', 3)
     model = build_model_with_cfg(
         Eva, variant, pretrained,
         pretrained_filter_fn=checkpoint_filter_fn,
-        **kwargs)
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
+        **kwargs,
+    )
     return model
 
 
 def _cfg(url='', **kwargs):
     return {
         'url': url,
         'num_classes': 1000, 'input_size': (3, 224, 224), 'pool_size': None,
@@ -840,14 +941,33 @@
         num_classes=1024,
     ),
     'eva02_enormous_patch14_clip_224.pretrain': _cfg(
         # hf_hub_id='QuanSun/EVA-CLIP', hf_hub_filename='EVA02_E_psz14.pt',
         num_classes=0,
     ),
 
+    'vit_medium_patch16_rope_reg1_gap_256.sbb_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95,
+        mean=(0.5, 0.5, 0.5), std=(0.5, 0.5, 0.5)
+    ),
+    'vit_mediumd_patch16_rope_reg1_gap_256.sbb_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95,
+        mean=(0.5, 0.5, 0.5), std=(0.5, 0.5, 0.5)
+    ),
+    'vit_betwixt_patch16_rope_reg4_gap_256.sbb_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95,
+    ),
+    'vit_base_patch16_rope_reg1_gap_256.sbb_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95,
+        mean=(0.5, 0.5, 0.5), std=(0.5, 0.5, 0.5)
+    ),
 })
 
 
 @register_model
 def eva_giant_patch14_224(pretrained=False, **kwargs) -> Eva:
     """ EVA-g model https://arxiv.org/abs/2211.07636 """
     model_args = dict(patch_size=14, embed_dim=1408, depth=40, num_heads=16, mlp_ratio=6144 / 1408)
@@ -1102,7 +1222,91 @@
         num_heads=16,
         mlp_ratio=15360 / 1792,
         use_post_norm=True,
         global_pool=kwargs.pop('global_pool', 'token'),
     )
     model = _create_eva('eva02_enormous_patch14_clip_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
+
+
+@register_model
+def vit_medium_patch16_rope_reg1_gap_256(pretrained=False, **kwargs) -> Eva:
+    model_args = dict(
+        img_size=256,
+        patch_size=16,
+        embed_dim=512,
+        depth=12,
+        num_heads=8,
+        qkv_fused=True,
+        qkv_bias=True,
+        init_values=1e-5,
+        class_token=False,
+        num_reg_tokens=1,
+        use_rot_pos_emb=True,
+        use_abs_pos_emb=False,
+        ref_feat_shape=(16, 16),  # 224/14
+    )
+    model = _create_eva('vit_medium_patch16_rope_reg1_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_mediumd_patch16_rope_reg1_gap_256(pretrained=False, **kwargs) -> Eva:
+    model_args = dict(
+        img_size=256,
+        patch_size=16,
+        embed_dim=512,
+        depth=20,
+        num_heads=8,
+        qkv_fused=True,
+        qkv_bias=False,
+        init_values=1e-5,
+        class_token=False,
+        num_reg_tokens=1,
+        use_rot_pos_emb=True,
+        use_abs_pos_emb=False,
+        ref_feat_shape=(16, 16),  # 224/14
+    )
+    model = _create_eva('vit_mediumd_patch16_rope_reg1_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_betwixt_patch16_rope_reg4_gap_256(pretrained=False, **kwargs) -> Eva:
+    model_args = dict(
+        img_size=256,
+        patch_size=16,
+        embed_dim=640,
+        depth=12,
+        num_heads=10,
+        qkv_fused=True,
+        qkv_bias=True,
+        init_values=1e-5,
+        class_token=False,
+        num_reg_tokens=4,
+        use_rot_pos_emb=True,
+        use_abs_pos_emb=False,
+        ref_feat_shape=(16, 16),  # 224/14
+    )
+    model = _create_eva('vit_betwixt_patch16_rope_reg4_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_base_patch16_rope_reg1_gap_256(pretrained=False, **kwargs) -> Eva:
+    model_args = dict(
+        img_size=256,
+        patch_size=16,
+        embed_dim=768,
+        depth=12,
+        num_heads=12,
+        qkv_fused=True,
+        qkv_bias=True,
+        init_values=1e-5,
+        class_token=False,
+        num_reg_tokens=1,
+        use_rot_pos_emb=True,
+        use_abs_pos_emb=False,
+        ref_feat_shape=(16, 16),  # 224/14
+    )
+    model = _create_eva('vit_base_patch16_rope_reg1_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
```

### Comparing `timm-0.9.9/timm/models/fastvit.py` & `timm-1.0.3/timm/models/fastvit.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,15 +392,15 @@
         self.reparam_conv.bias.data = eq_b
         self.__delattr__("large_conv")
         if hasattr(self, "small_conv"):
             self.__delattr__("small_conv")
 
     @staticmethod
     def _fuse_bn(
-        conv: torch.Tensor, bn: nn.BatchNorm2d
+        conv: nn.Conv2d, bn: nn.BatchNorm2d
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Method to fuse batchnorm layer with conv layer.
 
         Args:
             conv: Convolutional kernel weights.
             bn: Batchnorm 2d layer.
 
@@ -1160,16 +1160,18 @@
                 scale *= 2
             self.feature_info += [dict(num_chs=prev_dim, reduction=4 * scale, module=f'stages.{i}')]
         self.stages = nn.Sequential(*stages)
         self.num_features = prev_dim
 
         # For segmentation and detection, extract intermediate output
         if self.fork_feat:
-            # add a norm layer for each output
-            self.out_indices = [0, 2, 4, 6]
+            # Add a norm layer for each output. self.stages is slightly different than self.network
+            # in the original code, the PatchEmbed layer is part of self.stages in this code where
+            # it was part of self.network in the original code. So we do not need to skip out indices.
+            self.out_indices = [0, 1, 2, 3]
             for i_emb, i_layer in enumerate(self.out_indices):
                 if i_emb == 0 and os.environ.get("FORK_LAST3", None):
                     """For RetinaNet, `start_level=1`. The first norm layer will not used.
                     cmd: `FORK_LAST3=1 python -m torch.distributed.launch ...`
                     """
                     layer = nn.Identity()
                 else:
@@ -1226,15 +1228,15 @@
         for s in self.stages:
             s.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         self.head.reset(num_classes, global_pool)
 
     def forward_features(self, x: torch.Tensor) -> torch.Tensor:
         # input embedding
         x = self.stem(x)
         outs = []
@@ -1412,8 +1414,8 @@
     model_args = dict(
         layers=(6, 6, 18, 6),
         embed_dims=(76, 152, 304, 608),
         mlp_ratios=(4, 4, 4, 4),
         pos_embs=(None, None, None, partial(RepConditionalPosEnc, spatial_shape=(7, 7))),
         token_mixers=("repmixer", "repmixer", "repmixer", "attention")
     )
-    return _create_fastvit('fastvit_ma36', pretrained=pretrained, **dict(model_args, **kwargs))
+    return _create_fastvit('fastvit_ma36', pretrained=pretrained, **dict(model_args, **kwargs))
```

### Comparing `timm-0.9.9/timm/models/focalnet.py` & `timm-1.0.3/timm/models/focalnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,25 +450,25 @@
         for l in self.layers:
             l.set_grad_checkpointing(enable=enable)
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.head.reset(num_classes, pool_type=global_pool)
 
     def forward_features(self, x):
         x = self.stem(x)
         x = self.layers(x)
         x = self.norm(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
-        return self.head(x, pre_logits=pre_logits)
+        return self.head(x, pre_logits=pre_logits) if pre_logits else self.head(x)
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
```

### Comparing `timm-0.9.9/timm/models/gcvit.py` & `timm-1.0.3/timm/models/gcvit.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,27 +485,27 @@
         for s in self.stages:
             s.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is None:
             global_pool = self.head.global_pool.pool_type
         self.head = ClassifierHead(self.num_features, num_classes, pool_type=global_pool, drop_rate=self.drop_rate)
 
     def forward_features(self, x: torch.Tensor) -> torch.Tensor:
         x = self.stem(x)
         x = self.stages(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
-        return self.head(x, pre_logits=pre_logits)
+        return self.head(x, pre_logits=pre_logits) if pre_logits else self.head(x)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
```

### Comparing `timm-0.9.9/timm/models/ghostnet.py` & `timm-1.0.3/timm/models/ghostnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/hardcorenas.py` & `timm-1.0.3/timm/models/hardcorenas.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/hrnet.py` & `timm-1.0.3/timm/models/hrnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -858,20 +858,25 @@
     features_only = False
     kwargs_filter = None
     if model_kwargs.pop('features_only', False):
         model_cls = HighResolutionNetFeatures
         kwargs_filter = ('num_classes', 'global_pool')
         features_only = True
     cfg_variant = cfg_variant or variant
+
+    pretrained_strict = model_kwargs.pop(
+        'pretrained_strict',
+        not features_only and model_kwargs.get('head', 'classification') == 'classification'
+    )
     model = build_model_with_cfg(
         model_cls,
         variant,
         pretrained,
         model_cfg=cfg_cls[cfg_variant],
-        pretrained_strict=not features_only,
+        pretrained_strict=pretrained_strict,
         kwargs_filter=kwargs_filter,
         **model_kwargs,
     )
     if features_only:
         model.pretrained_cfg = pretrained_cfg_for_features(model.default_cfg)
         model.default_cfg = model.pretrained_cfg  # backwards compat
     return model
```

### Comparing `timm-0.9.9/timm/models/inception_next.py` & `timm-1.0.3/timm/models/inception_next.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/inception_resnet_v2.py` & `timm-1.0.3/timm/models/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/inception_v3.py` & `timm-1.0.3/timm/models/inception_v3.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/inception_v4.py` & `timm-1.0.3/timm/models/inception_v4.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/layers/__init__.py` & `timm-1.0.3/timm/models/layers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from timm.layers.norm_act import BatchNormAct2d, GroupNormAct, convert_sync_batchnorm
 from timm.layers.padding import get_padding, get_same_padding, pad_same
 from timm.layers.patch_embed import PatchEmbed
 from timm.layers.pool2d_same import AvgPool2dSame, create_pool2d
 from timm.layers.squeeze_excite import SEModule, SqueezeExcite, EffectiveSEModule, EffectiveSqueezeExcite
 from timm.layers.selective_kernel import SelectiveKernel
 from timm.layers.separable_conv import SeparableConv2d, SeparableConvNormAct
-from timm.layers.space_to_depth import SpaceToDepthModule
 from timm.layers.split_attn import SplitAttn
 from timm.layers.split_batchnorm import SplitBatchNorm2d, convert_splitbn_model
 from timm.layers.std_conv import StdConv2d, StdConv2dSame, ScaledStdConv2d, ScaledStdConv2dSame
 from timm.layers.test_time_pool import TestTimePoolHead, apply_test_time_pool
 from timm.layers.trace_utils import _assert, _float_to_int
 from timm.layers.weight_init import trunc_normal_, trunc_normal_tf_, variance_scaling_, lecun_normal_
```

### Comparing `timm-0.9.9/timm/models/levit.py` & `timm-1.0.3/timm/models/levit.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 # All rights reserved.
 
 # Modified from
 # https://github.com/rwightman/pytorch-image-models/blob/master/timm/models/vision_transformer.py
 # Copyright 2020 Ross Wightman, Apache-2.0 License
 from collections import OrderedDict
 from functools import partial
-from typing import Dict
+from typing import Dict, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_STD, IMAGENET_DEFAULT_MEAN
-from timm.layers import to_ntuple, to_2tuple, get_act_layer, DropPath, trunc_normal_
+from timm.layers import to_ntuple, to_2tuple, get_act_layer, DropPath, trunc_normal_, ndgrid
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._manipulate import checkpoint_seq
 from ._registry import generate_default_cfgs, register_model
 
 __all__ = ['Levit']
 
 
 class ConvNorm(nn.Module):
@@ -190,15 +191,15 @@
         self.qkv = ln_layer(dim, self.val_attn_dim + self.key_attn_dim * 2)
         self.proj = nn.Sequential(OrderedDict([
             ('act', act_layer()),
             ('ln', ln_layer(self.val_attn_dim, dim, bn_weight_init=0))
         ]))
 
         self.attention_biases = nn.Parameter(torch.zeros(num_heads, resolution[0] * resolution[1]))
-        pos = torch.stack(torch.meshgrid(torch.arange(resolution[0]), torch.arange(resolution[1]))).flatten(1)
+        pos = torch.stack(ndgrid(torch.arange(resolution[0]), torch.arange(resolution[1]))).flatten(1)
         rel_pos = (pos[..., :, None] - pos[..., None, :]).abs()
         rel_pos = (rel_pos[0] * resolution[1]) + rel_pos[1]
         self.register_buffer('attention_bias_idxs', rel_pos, persistent=False)
         self.attention_bias_cache = {}
 
     @torch.no_grad()
     def train(self, mode=True):
@@ -286,18 +287,19 @@
         ]))
         self.proj = nn.Sequential(OrderedDict([
             ('act', act_layer()),
             ('ln', ln_layer(self.val_attn_dim, out_dim))
         ]))
 
         self.attention_biases = nn.Parameter(torch.zeros(num_heads, resolution[0] * resolution[1]))
-        k_pos = torch.stack(torch.meshgrid(torch.arange(resolution[0]), torch.arange(resolution[1]))).flatten(1)
-        q_pos = torch.stack(torch.meshgrid(
+        k_pos = torch.stack(ndgrid(torch.arange(resolution[0]), torch.arange(resolution[1]))).flatten(1)
+        q_pos = torch.stack(ndgrid(
             torch.arange(0, resolution[0], step=stride),
-            torch.arange(0, resolution[1], step=stride))).flatten(1)
+            torch.arange(0, resolution[1], step=stride)
+        )).flatten(1)
         rel_pos = (q_pos[..., :, None] - k_pos[..., None, :]).abs()
         rel_pos = (rel_pos[0] * resolution[1]) + rel_pos[1]
         self.register_buffer('attention_bias_idxs', rel_pos, persistent=False)
 
         self.attention_bias_cache = {}  # per-device attention_biases cache
 
     @torch.no_grad()
@@ -622,21 +624,85 @@
     def set_grad_checkpointing(self, enable=True):
         self.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None, distillation=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None, distillation=None):
         self.num_classes = num_classes
         if global_pool is not None:
             self.global_pool = global_pool
         self.head = NormLinear(
             self.embed_dim[-1], num_classes, drop=self.drop_rate) if num_classes > 0 else nn.Identity()
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to compatible intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output shape must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.stages), indices)
+
+        # forward pass
+        x = self.stem(x)
+        B, C, H, W = x.shape
+        if not self.use_conv:
+            x = x.flatten(2).transpose(1, 2)
+
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            stages = self.stages
+        else:
+            stages = self.stages[:max_index + 1]
+        for feat_idx, stage in enumerate(stages):
+            x = stage(x)
+            if feat_idx in take_indices:
+                if self.use_conv:
+                    intermediates.append(x)
+                else:
+                    intermediates.append(x.reshape(B, H, W, -1).permute(0, 3, 1, 2))
+            H = (H + 2 - 1) // 2
+            W = (W + 2 - 1) // 2
+
+        if intermediates_only:
+            return intermediates
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.stages), indices)
+        self.stages = self.stages[:max_index + 1]  # truncate blocks w/ stem as idx 0
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.stem(x)
         if not self.use_conv:
             x = x.flatten(2).transpose(1, 2)
         if self.grad_checkpointing and not torch.jit.is_scripting():
             x = checkpoint_seq(self.stages, x)
         else:
@@ -660,15 +726,15 @@
         self.head_dist = NormLinear(self.num_features, self.num_classes) if self.num_classes > 0 else nn.Identity()
         self.distilled_training = False  # must set this True to train w/ distillation token
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head, self.head_dist
 
-    def reset_classifier(self, num_classes, global_pool=None, distillation=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None, distillation=None):
         self.num_classes = num_classes
         if global_pool is not None:
             self.global_pool = global_pool
         self.head = NormLinear(
             self.num_features, num_classes, drop=self.drop_rate) if num_classes > 0 else nn.Identity()
         self.head_dist = NormLinear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
 
@@ -741,17 +807,16 @@
         embed_dim=(512, 640, 768), key_dim=64, num_heads=(8, 10, 12), depth=(4, 8, 6), act_layer='silu'),
 )
 
 
 def create_levit(variant, cfg_variant=None, pretrained=False, distilled=True, **kwargs):
     is_conv = '_conv' in variant
     out_indices = kwargs.pop('out_indices', (0, 1, 2))
-    if kwargs.get('features_only', None):
-        if not is_conv:
-            raise RuntimeError('features_only not implemented for LeVit in non-convolutional mode.')
+    if kwargs.get('features_only', False) and not is_conv:
+        kwargs.setdefault('feature_cls', 'getter')
     if cfg_variant is None:
         if variant in model_cfgs:
             cfg_variant = variant
         elif is_conv:
             cfg_variant = variant.replace('_conv', '')
 
     model_cfg = dict(model_cfgs[cfg_variant], **kwargs)
```

### Comparing `timm-0.9.9/timm/models/maxxvit.py` & `timm-1.0.3/timm/models/maxxvit.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import Mlp, ConvMlp, DropPath, LayerNorm, ClassifierHead, NormMlpClassifierHead
 from timm.layers import create_attn, get_act_layer, get_norm_layer, get_norm_act_layer, create_conv2d, create_pool2d
 from timm.layers import trunc_normal_tf_, to_2tuple, extend_tuple, make_divisible, _assert
 from timm.layers import RelPosMlp, RelPosBias, RelPosBiasTf, use_fused_attn, resize_rel_pos_bias_table
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._features_fx import register_notrace_function
 from ._manipulate import named_apply, checkpoint_seq
 from ._registry import generate_default_cfgs, register_model
 
 __all__ = ['MaxxVitCfg', 'MaxxVitConvCfg', 'MaxxVitTransformerCfg', 'MaxxVit']
 
 
@@ -628,15 +629,15 @@
         x = self.drop_path(x) + shortcut
         return x
 
 
 def window_partition(x, window_size: List[int]):
     B, H, W, C = x.shape
     _assert(H % window_size[0] == 0, f'height ({H}) must be divisible by window ({window_size[0]})')
-    _assert(W % window_size[1] == 0, '')
+    _assert(W % window_size[1] == 0, f'width ({W}) must be divisible by window ({window_size[1]})')
     x = x.view(B, H // window_size[0], window_size[0], W // window_size[1], window_size[1], C)
     windows = x.permute(0, 1, 3, 2, 4, 5).contiguous().view(-1, window_size[0], window_size[1], C)
     return windows
 
 
 @register_notrace_function  # reason: int argument is a Proxy
 def window_reverse(windows, window_size: List[int], img_size: List[int]):
@@ -646,15 +647,15 @@
     x = x.permute(0, 1, 3, 2, 4, 5).contiguous().view(-1, H, W, C)
     return x
 
 
 def grid_partition(x, grid_size: List[int]):
     B, H, W, C = x.shape
     _assert(H % grid_size[0] == 0, f'height {H} must be divisible by grid {grid_size[0]}')
-    _assert(W % grid_size[1] == 0, '')
+    _assert(W % grid_size[1] == 0, f'width {W} must be divisible by grid {grid_size[1]}')
     x = x.view(B, grid_size[0], H // grid_size[0], grid_size[1], W // grid_size[1], C)
     windows = x.permute(0, 2, 4, 1, 3, 5).contiguous().view(-1, grid_size[0], grid_size[1], C)
     return windows
 
 
 @register_notrace_function  # reason: int argument is a Proxy
 def grid_reverse(windows, grid_size: List[int], img_size: List[int]):
@@ -812,15 +813,15 @@
         x = x + self.drop_path2(self.ls2(self.mlp(self.norm2(x))))
         return x
 
 
 def window_partition_nchw(x, window_size: List[int]):
     B, C, H, W = x.shape
     _assert(H % window_size[0] == 0, f'height ({H}) must be divisible by window ({window_size[0]})')
-    _assert(W % window_size[1] == 0, '')
+    _assert(W % window_size[1] == 0, f'width ({W}) must be divisible by window ({window_size[1]})')
     x = x.view(B, C, H // window_size[0], window_size[0], W // window_size[1], window_size[1])
     windows = x.permute(0, 2, 4, 1, 3, 5).contiguous().view(-1, C, window_size[0], window_size[1])
     return windows
 
 
 @register_notrace_function  # reason: int argument is a Proxy
 def window_reverse_nchw(windows, window_size: List[int], img_size: List[int]):
@@ -830,15 +831,15 @@
     x = x.permute(0, 3, 1, 4, 2, 5).contiguous().view(-1, C, H, W)
     return x
 
 
 def grid_partition_nchw(x, grid_size: List[int]):
     B, C, H, W = x.shape
     _assert(H % grid_size[0] == 0, f'height {H} must be divisible by grid {grid_size[0]}')
-    _assert(W % grid_size[1] == 0, '')
+    _assert(W % grid_size[1] == 0, f'width {W} must be divisible by grid {grid_size[1]}')
     x = x.view(B, C, grid_size[0], H // grid_size[0], grid_size[1], W // grid_size[1])
     windows = x.permute(0, 3, 5, 1, 2, 4).contiguous().view(-1, C, grid_size[0], grid_size[1])
     return windows
 
 
 @register_notrace_function  # reason: int argument is a Proxy
 def grid_reverse_nchw(windows, grid_size: List[int], img_size: List[int]):
@@ -1243,26 +1244,95 @@
         for s in self.stages:
             s.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         self.head.reset(num_classes, global_pool)
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to compatible intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output shape must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.stages) + 1, indices)
+
+        # forward pass
+        feat_idx = 0  # stem is index 0
+        x = self.stem(x)
+        if feat_idx in take_indices:
+            intermediates.append(x)
+
+        last_idx = len(self.stages)
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            stages = self.stages
+        else:
+            stages = self.stages[:max_index]
+        for stage in stages:
+            feat_idx += 1
+            x = stage(x)
+            if feat_idx in take_indices:
+                if norm and feat_idx == last_idx:
+                    x_inter = self.norm(x)  # applying final norm to last intermediate
+                else:
+                    x_inter = x
+                intermediates.append(x_inter)
+
+        if intermediates_only:
+            return intermediates
+
+        x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.stages) + 1, indices)
+        self.stages = self.stages[:max_index]  # truncate blocks w/ stem as idx 0
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.head = self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.stem(x)
         x = self.stages(x)
         x = self.norm(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
-        return self.head(x, pre_logits=pre_logits)
+        return self.head(x, pre_logits=pre_logits) if pre_logits else self.head(x)
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
```

### Comparing `timm-0.9.9/timm/models/metaformer.py` & `timm-1.0.3/timm/models/metaformer.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/mlp_mixer.py` & `timm-1.0.3/timm/models/mlp_mixer.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,21 +36,23 @@
 
 A thank you to paper authors for releasing code and weights.
 
 Hacked together by / Copyright 2021 Ross Wightman
 """
 import math
 from functools import partial
+from typing import List, Optional, Union, Tuple
 
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import PatchEmbed, Mlp, GluMlp, GatedMlp, DropPath, lecun_normal_, to_2tuple
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._manipulate import named_apply, checkpoint_seq
 from ._registry import generate_default_cfgs, register_model, register_model_deprecations
 
 __all__ = ['MixerBlock', 'MlpMixer']  # model_registry will add each entrypoint fn to this
 
 
 class MixerBlock(nn.Module):
@@ -207,27 +209,30 @@
         self.stem = PatchEmbed(
             img_size=img_size,
             patch_size=patch_size,
             in_chans=in_chans,
             embed_dim=embed_dim,
             norm_layer=norm_layer if stem_norm else None,
         )
+        reduction = self.stem.feat_ratio() if hasattr(self.stem, 'feat_ratio') else patch_size
         # FIXME drop_path (stochastic depth scaling rule or all the same?)
         self.blocks = nn.Sequential(*[
             block_layer(
                 embed_dim,
                 self.stem.num_patches,
                 mlp_ratio,
                 mlp_layer=mlp_layer,
                 norm_layer=norm_layer,
                 act_layer=act_layer,
                 drop=proj_drop_rate,
                 drop_path=drop_path_rate,
             )
             for _ in range(num_blocks)])
+        self.feature_info = [
+            dict(module=f'blocks.{i}', num_chs=embed_dim, reduction=reduction) for i in range(num_blocks)]
         self.norm = norm_layer(embed_dim)
         self.head_drop = nn.Dropout(drop_rate)
         self.head = nn.Linear(embed_dim, self.num_classes) if num_classes > 0 else nn.Identity()
 
         self.init_weights(nlhb=nlhb)
 
     @torch.jit.ignore
@@ -246,21 +251,91 @@
     def set_grad_checkpointing(self, enable=True):
         self.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             assert global_pool in ('', 'avg')
             self.global_pool = global_pool
         self.head = nn.Linear(self.embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            return_prefix_tokens: Return both prefix and spatial intermediate tokens
+            norm: Apply norm layer to all intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW', 'NLC'), 'Output format must be one of NCHW or NLC.'
+        reshape = output_fmt == 'NCHW'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+
+        # forward pass
+        B, _, height, width = x.shape
+        x = self.stem(x)
+
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            blocks = self.blocks
+        else:
+            blocks = self.blocks[:max_index + 1]
+        for i, blk in enumerate(blocks):
+            x = blk(x)
+            if i in take_indices:
+                # normalize intermediates with final norm layer if enabled
+                intermediates.append(self.norm(x) if norm else x)
+
+        # process intermediates
+        if reshape:
+            # reshape to BCHW output format
+            H, W = self.stem.dynamic_feat_size((height, width))
+            intermediates = [y.reshape(B, H, W, -1).permute(0, 3, 1, 2).contiguous() for y in intermediates]
+
+        if intermediates_only:
+            return intermediates
+
+        x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+        self.blocks = self.blocks[:max_index + 1]  # truncate blocks
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.stem(x)
         if self.grad_checkpointing and not torch.jit.is_scripting():
             x = checkpoint_seq(self.blocks, x)
         else:
             x = self.blocks(x)
         x = self.norm(x)
@@ -326,22 +401,21 @@
                 v = v.reshape(1, 1, -1)
             out_dict[k] = v
         return out_dict
     return state_dict
 
 
 def _create_mixer(variant, pretrained=False, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError('features_only not implemented for MLP-Mixer models.')
-
+    out_indices = kwargs.pop('out_indices', 3)
     model = build_model_with_cfg(
         MlpMixer,
         variant,
         pretrained,
         pretrained_filter_fn=checkpoint_filter_fn,
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
         **kwargs,
     )
     return model
 
 
 def _cfg(url='', **kwargs):
     return {
```

### Comparing `timm-0.9.9/timm/models/mobilenetv3.py` & `timm-1.0.3/timm/models/mobilenetv3.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 A PyTorch impl of MobileNet-V3, compatible with TF weights from official impl.
 
 Paper: Searching for MobileNetV3 - https://arxiv.org/abs/1905.02244
 
 Hacked together by / Copyright 2019, Ross Wightman
 """
 from functools import partial
-from typing import Callable, List, Optional, Tuple
+from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils.checkpoint import checkpoint
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD, IMAGENET_INCEPTION_MEAN, IMAGENET_INCEPTION_STD
 from timm.layers import SelectAdaptivePool2d, Linear, LayerType, PadType, create_conv2d, get_norm_act_layer
 from ._builder import build_model_with_cfg, pretrained_cfg_for_features
 from ._efficientnet_blocks import SqueezeExcite
 from ._efficientnet_builder import BlockArgs, EfficientNetBuilder, decode_arch_def, efficientnet_init_weights, \
     round_channels, resolve_bn_args, resolve_act_layer, BN_EPS_TF_DEFAULT
-from ._features import FeatureInfo, FeatureHooks
+from ._features import FeatureInfo, FeatureHooks, feature_take_indices
 from ._manipulate import checkpoint_seq
 from ._registry import generate_default_cfgs, register_model, register_model_deprecations
 
 __all__ = ['MobileNetV3', 'MobileNetV3Features']
 
 
 class MobileNetV3(nn.Module):
@@ -105,14 +105,15 @@
             act_layer=act_layer,
             norm_layer=norm_layer,
             se_layer=se_layer,
             drop_path_rate=drop_path_rate,
         )
         self.blocks = nn.Sequential(*builder(stem_size, block_args))
         self.feature_info = builder.features
+        self.stage_ends = [f['stage'] for f in self.feature_info]
         head_chs = builder.in_chs
 
         # Head + Pooling
         self.global_pool = SelectAdaptivePool2d(pool_type=global_pool)
         num_pooled_chs = head_chs * self.global_pool.feat_mult()
         self.conv_head = create_conv2d(num_pooled_chs, self.num_features, 1, padding=pad_type, bias=head_bias)
         self.act2 = act_layer(inplace=True)
@@ -146,14 +147,92 @@
     def reset_classifier(self, num_classes: int, global_pool: str = 'avg'):
         self.num_classes = num_classes
         # cannot meaningfully change pooling of efficient head after creation
         self.global_pool = SelectAdaptivePool2d(pool_type=global_pool)
         self.flatten = nn.Flatten(1) if global_pool else nn.Identity()  # don't flatten if pooling disabled
         self.classifier = Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+            extra_blocks: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to compatible intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+            extra_blocks: Include outputs of all blocks and head conv in output, does not align with feature_info
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output shape must be NCHW.'
+        if stop_early:
+            assert intermediates_only, 'Must use intermediates_only for early stopping.'
+        intermediates = []
+        if extra_blocks:
+            take_indices, max_index = feature_take_indices(len(self.blocks) + 1, indices)
+        else:
+            take_indices, max_index = feature_take_indices(len(self.stage_ends), indices)
+            take_indices = [self.stage_ends[i] for i in take_indices]
+            max_index = self.stage_ends[max_index]
+
+        # forward pass
+        feat_idx = 0  # stem is index 0
+        x = self.conv_stem(x)
+        x = self.bn1(x)
+        if feat_idx in take_indices:
+            intermediates.append(x)
+
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            blocks = self.blocks
+        else:
+            blocks = self.blocks[:max_index]
+        for blk in blocks:
+            feat_idx += 1
+            x = blk(x)
+            if feat_idx in take_indices:
+                intermediates.append(x)
+
+        if intermediates_only:
+            return intermediates
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+            extra_blocks: bool = False,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        if extra_blocks:
+            take_indices, max_index = feature_take_indices(len(self.blocks) + 1, indices)
+        else:
+            take_indices, max_index = feature_take_indices(len(self.stage_ends), indices)
+            max_index = self.stage_ends[max_index]
+        self.blocks = self.blocks[:max_index]  # truncate blocks w/ stem as idx 0
+        if max_index < len(self.blocks):
+            self.conv_head = nn.Identity()
+        if prune_head:
+            self.conv_head = nn.Identity()
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x: torch.Tensor) -> torch.Tensor:
         x = self.conv_stem(x)
         x = self.bn1(x)
         if self.grad_checkpointing and not torch.jit.is_scripting():
             x = checkpoint_seq(self.blocks, x, flatten=True)
         else:
             x = self.blocks(x)
@@ -284,15 +363,15 @@
 
 
 def _create_mnv3(variant: str, pretrained: bool = False, **kwargs) -> MobileNetV3:
     features_mode = ''
     model_cls = MobileNetV3
     kwargs_filter = None
     if kwargs.pop('features_only', False):
-        if 'feature_cfg' in kwargs:
+        if 'feature_cfg' in kwargs or 'feature_cls' in kwargs:
             features_mode = 'cfg'
         else:
             kwargs_filter = ('num_classes', 'num_features', 'head_conv', 'head_bias', 'global_pool')
             model_cls = MobileNetV3Features
             features_mode = 'cls'
 
     model = build_model_with_cfg(
@@ -539,51 +618,14 @@
         num_features=1280,
         **kwargs,
     )
     model = _create_mnv3(variant, pretrained, **model_kwargs)
     return model
 
 
-def _gen_lcnet(variant: str, channel_multiplier: float = 1.0, pretrained: bool = False, **kwargs):
-    """ LCNet
-    Essentially a MobileNet-V3 crossed with a MobileNet-V1
-
-    Paper: `PP-LCNet: A Lightweight CPU Convolutional Neural Network` - https://arxiv.org/abs/2109.15099
-
-    Args:
-      channel_multiplier: multiplier to number of channels per layer.
-    """
-    arch_def = [
-        # stage 0, 112x112 in
-        ['dsa_r1_k3_s1_c32'],
-        # stage 1, 112x112 in
-        ['dsa_r2_k3_s2_c64'],
-        # stage 2, 56x56 in
-        ['dsa_r2_k3_s2_c128'],
-        # stage 3, 28x28 in
-        ['dsa_r1_k3_s2_c256', 'dsa_r1_k5_s1_c256'],
-        # stage 4, 14x14in
-        ['dsa_r4_k5_s1_c256'],
-        # stage 5, 14x14in
-        ['dsa_r2_k5_s2_c512_se0.25'],
-        # 7x7
-    ]
-    model_kwargs = dict(
-        block_args=decode_arch_def(arch_def),
-        stem_size=16,
-        round_chs_fn=partial(round_channels, multiplier=channel_multiplier),
-        norm_layer=partial(nn.BatchNorm2d, **resolve_bn_args(kwargs)),
-        act_layer=resolve_act_layer(kwargs, 'hard_swish'),
-        se_layer=partial(SqueezeExcite, gate_layer='hard_sigmoid', force_act_layer=nn.ReLU),
-        num_features=1280,
-        **kwargs,
-    )
-    model = _create_mnv3(variant, pretrained, **model_kwargs)
-    return model
-
 
 def _cfg(url: str = '', **kwargs):
     return {
         'url': url, 'num_classes': 1000, 'input_size': (3, 224, 224), 'pool_size': (7, 7),
         'crop_pct': 0.875, 'interpolation': 'bilinear',
         'mean': IMAGENET_DEFAULT_MEAN, 'std': IMAGENET_DEFAULT_STD,
         'first_conv': 'conv_stem', 'classifier': 'classifier',
@@ -621,14 +663,15 @@
     'mobilenetv3_small_100.lamb_in1k': _cfg(
         url='https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-weights/mobilenetv3_small_100_lamb-266a294c.pth',
         hf_hub_id='timm/',
         interpolation='bicubic'),
 
     'mobilenetv3_rw.rmsp_in1k': _cfg(
         url='https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-weights/mobilenetv3_100-35495452.pth',
+        hf_hub_id='timm/',
         interpolation='bicubic'),
 
     'tf_mobilenetv3_large_075.in1k': _cfg(
         url='https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-weights/tf_mobilenetv3_large_075-150ee8b0.pth',
         hf_hub_id='timm/',
         mean=IMAGENET_INCEPTION_MEAN, std=IMAGENET_INCEPTION_STD),
     'tf_mobilenetv3_large_100.in1k': _cfg(
@@ -719,71 +762,69 @@
     model = _gen_mobilenet_v3('mobilenetv3_small_100', 1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def mobilenetv3_rw(pretrained: bool = False, **kwargs) -> MobileNetV3:
     """ MobileNet V3 """
-    if pretrained:
-        # pretrained model trained with non-default BN epsilon
-        kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
     model = _gen_mobilenet_v3_rw('mobilenetv3_rw', 1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_mobilenetv3_large_075(pretrained: bool = False, **kwargs) -> MobileNetV3:
     """ MobileNet V3 """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_mobilenet_v3('tf_mobilenetv3_large_075', 0.75, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_mobilenetv3_large_100(pretrained: bool = False, **kwargs) -> MobileNetV3:
     """ MobileNet V3 """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_mobilenet_v3('tf_mobilenetv3_large_100', 1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_mobilenetv3_large_minimal_100(pretrained: bool = False, **kwargs) -> MobileNetV3:
     """ MobileNet V3 """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_mobilenet_v3('tf_mobilenetv3_large_minimal_100', 1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_mobilenetv3_small_075(pretrained: bool = False, **kwargs) -> MobileNetV3:
     """ MobileNet V3 """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_mobilenet_v3('tf_mobilenetv3_small_075', 0.75, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_mobilenetv3_small_100(pretrained: bool = False, **kwargs) -> MobileNetV3:
     """ MobileNet V3 """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_mobilenet_v3('tf_mobilenetv3_small_100', 1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def tf_mobilenetv3_small_minimal_100(pretrained: bool = False, **kwargs) -> MobileNetV3:
     """ MobileNet V3 """
-    kwargs['bn_eps'] = BN_EPS_TF_DEFAULT
-    kwargs['pad_type'] = 'same'
+    kwargs.setdefault('bn_eps', BN_EPS_TF_DEFAULT)
+    kwargs.setdefault('pad_type', 'same')
     model = _gen_mobilenet_v3('tf_mobilenetv3_small_minimal_100', 1.0, pretrained=pretrained, **kwargs)
     return model
 
 
 @register_model
 def fbnetv3_b(pretrained: bool = False, **kwargs) -> MobileNetV3:
     """ FBNetV3-B """
```

### Comparing `timm-0.9.9/timm/models/mobilevit.py` & `timm-1.0.3/timm/models/mobilevit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/mvitv2.py` & `timm-1.0.3/timm/models/mvitv2.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import torch
 import torch.utils.checkpoint as checkpoint
 from torch import nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import Mlp, DropPath, trunc_normal_tf_, get_norm_layer, to_2tuple
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._features_fx import register_notrace_function
 from ._registry import register_model, register_model_deprecations, generate_default_cfgs
 
 __all__ = ['MultiScaleVit', 'MultiScaleVitCfg']  # model_registry will add each entrypoint fn to this
 
 
 @dataclass
@@ -743,16 +744,18 @@
         if cfg.use_abs_pos:
             self.pos_embed = nn.Parameter(torch.zeros(1, pos_embed_dim, embed_dim))
         else:
             self.pos_embed = None
 
         num_stages = len(cfg.embed_dim)
         feat_size = patch_dims
+        curr_stride = max(cfg.patch_stride)
         dpr = [x.tolist() for x in torch.linspace(0, drop_path_rate, sum(cfg.depths)).split(cfg.depths)]
         self.stages = nn.ModuleList()
+        self.feature_info = []
         for i in range(num_stages):
             if cfg.expand_attn:
                 dim_out = cfg.embed_dim[i]
             else:
                 dim_out = cfg.embed_dim[min(i + 1, num_stages - 1)]
             stage = MultiScaleVitStage(
                 dim=embed_dim,
@@ -771,14 +774,16 @@
                 stride_kv=cfg.stride_kv[i],
                 has_cls_token=cfg.use_cls_token,
                 rel_pos_type=cfg.rel_pos_type,
                 residual_pooling=cfg.residual_pooling,
                 norm_layer=norm_layer,
                 drop_path=dpr[i],
             )
+            curr_stride *= max(cfg.stride_q[i])
+            self.feature_info += [dict(module=f'block.{i}', num_chs=dim_out, reduction=curr_stride)]
             embed_dim = dim_out
             feat_size = stage.feat_size
             self.stages.append(stage)
 
         self.num_features = embed_dim
         self.norm = norm_layer(embed_dim)
         self.head = nn.Sequential(OrderedDict([
@@ -816,23 +821,97 @@
         for s in self.stages:
             s.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             self.global_pool = global_pool
         self.head = nn.Sequential(OrderedDict([
             ('drop', nn.Dropout(self.drop_rate)),
             ('fc', nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity())
         ]))
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to all intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW', 'NLC'), 'Output shape must be NCHW or NLC.'
+        reshape = output_fmt == 'NCHW'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.stages), indices)
+
+        # FIXME slice block/pos_block if < max
+        # forward pass
+        x, feat_size = self.patch_embed(x)
+        B = x.shape[0]
+        if self.cls_token is not None:
+            cls_tokens = self.cls_token.expand(B, -1, -1)
+            x = torch.cat((cls_tokens, x), dim=1)
+        if self.pos_embed is not None:
+            x = x + self.pos_embed
+
+        for i, stage in enumerate(self.stages):
+            x, feat_size = stage(x, feat_size)
+            if i in take_indices:
+                if norm and i == (len(self.stages) - 1):
+                    x_inter = self.norm(x)  # applying final norm last intermediate
+                else:
+                    x_inter = x
+                if reshape:
+                    if self.cls_token is not None:
+                        # possible to allow return of class tokens, TBD
+                        x_inter = x_inter[:, 1:]
+                    x_inter = x_inter.reshape(B, feat_size[0], feat_size[1], -1).permute(0, 3, 1, 2)
+                intermediates.append(x_inter)
+
+        if intermediates_only:
+            return intermediates
+
+        x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.stages), indices)
+        # FIXME add stage pruning
+        # self.stages = self.stages[:max_index]  # truncate blocks w/ stem as idx 0
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x, feat_size = self.patch_embed(x)
         B, N, C = x.shape
 
         if self.cls_token is not None:
             cls_tokens = self.cls_token.expand(B, -1, -1)
             x = torch.cat((cls_tokens, x), dim=1)
@@ -858,14 +937,26 @@
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
 def checkpoint_filter_fn(state_dict, model):
     if 'stages.0.blocks.0.norm1.weight' in state_dict:
+        # native checkpoint, look for rel_pos interpolations
+        for k in state_dict.keys():
+            if 'rel_pos' in k:
+                rel_pos = state_dict[k]
+                dest_rel_pos_shape = model.state_dict()[k].shape
+                if rel_pos.shape[0] != dest_rel_pos_shape[0]:
+                    rel_pos_resized = torch.nn.functional.interpolate(
+                        rel_pos.reshape(1, rel_pos.shape[0], -1).permute(0, 2, 1),
+                        size=dest_rel_pos_shape[0],
+                        mode="linear",
+                    )
+                    state_dict[k] = rel_pos_resized.reshape(-1, dest_rel_pos_shape[0]).permute(1, 0)
         return state_dict
 
     import re
     if 'model_state' in state_dict:
         state_dict = state_dict['model_state']
 
     depths = getattr(model, 'depths', None)
@@ -888,24 +979,14 @@
             k = re.sub(r'stages\.(\d+).blocks\.(\d+).proj', f'stages.\\1.blocks.\\2.shortcut_proj_attn', k)
         else:
             k = re.sub(r'stages\.(\d+).blocks\.(\d+).proj', f'stages.\\1.blocks.\\2.shortcut_proj_mlp', k)
         if 'head' in k:
             k = k.replace('head.projection', 'head.fc')
         out_dict[k] = v
 
-    # for k, v in state_dict.items():
-    #     if model.pos_embed is not None and k == 'pos_embed' and v.shape[1] != model.pos_embed.shape[1]:
-    #         # To resize pos embedding when using model at different size from pretrained weights
-    #         v = resize_pos_embed(
-    #             v,
-    #             model.pos_embed,
-    #             0 if getattr(model, 'no_embed_class') else getattr(model, 'num_prefix_tokens', 1),
-    #             model.patch_embed.grid_size
-    #         )
-
     return out_dict
 
 
 model_cfgs = dict(
     mvitv2_tiny=MultiScaleVitCfg(
         depths=(1, 2, 5, 2),
     ),
@@ -944,24 +1025,22 @@
         use_cls_token=True,
         expand_attn=True,
     ),
 )
 
 
 def _create_mvitv2(variant, cfg_variant=None, pretrained=False, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError('features_only not implemented for Multiscale Vision Transformer models.')
-
+    out_indices = kwargs.pop('out_indices', 4)
     return build_model_with_cfg(
         MultiScaleVit,
         variant,
         pretrained,
         model_cfg=model_cfgs[variant] if not cfg_variant else model_cfgs[cfg_variant],
         pretrained_filter_fn=checkpoint_filter_fn,
-        feature_cfg=dict(flatten_sequential=True),
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
         **kwargs,
     )
 
 
 def _cfg(url='', **kwargs):
     return {
         'url': url,
@@ -971,28 +1050,36 @@
         'first_conv': 'patch_embed.proj', 'classifier': 'head.fc',
         'fixed_input_size': True,
         **kwargs
     }
 
 
 default_cfgs = generate_default_cfgs({
-    'mvitv2_tiny.fb_in1k': _cfg(url='https://dl.fbaipublicfiles.com/mvit/mvitv2_models/MViTv2_T_in1k.pyth'),
-    'mvitv2_small.fb_in1k': _cfg(url='https://dl.fbaipublicfiles.com/mvit/mvitv2_models/MViTv2_S_in1k.pyth'),
-    'mvitv2_base.fb_in1k': _cfg(url='https://dl.fbaipublicfiles.com/mvit/mvitv2_models/MViTv2_B_in1k.pyth'),
-    'mvitv2_large.fb_in1k': _cfg(url='https://dl.fbaipublicfiles.com/mvit/mvitv2_models/MViTv2_L_in1k.pyth'),
+    'mvitv2_tiny.fb_in1k': _cfg(
+        url='https://dl.fbaipublicfiles.com/mvit/mvitv2_models/MViTv2_T_in1k.pyth',
+        hf_hub_id='timm/'),
+    'mvitv2_small.fb_in1k': _cfg(url='https://dl.fbaipublicfiles.com/mvit/mvitv2_models/MViTv2_S_in1k.pyth',
+        hf_hub_id='timm/'),
+    'mvitv2_base.fb_in1k': _cfg(url='https://dl.fbaipublicfiles.com/mvit/mvitv2_models/MViTv2_B_in1k.pyth',
+        hf_hub_id='timm/'),
+    'mvitv2_large.fb_in1k': _cfg(url='https://dl.fbaipublicfiles.com/mvit/mvitv2_models/MViTv2_L_in1k.pyth',
+        hf_hub_id='timm/'),
 
     'mvitv2_small_cls': _cfg(url=''),
     'mvitv2_base_cls.fb_inw21k': _cfg(
         url='https://dl.fbaipublicfiles.com/mvit/mvitv2_models/MViTv2_B_in21k.pyth',
+        hf_hub_id='timm/',
         num_classes=19168),
     'mvitv2_large_cls.fb_inw21k': _cfg(
         url='https://dl.fbaipublicfiles.com/mvit/mvitv2_models/MViTv2_L_in21k.pyth',
+        hf_hub_id='timm/',
         num_classes=19168),
     'mvitv2_huge_cls.fb_inw21k': _cfg(
         url='https://dl.fbaipublicfiles.com/mvit/mvitv2_models/MViTv2_H_in21k.pyth',
+        hf_hub_id='timm/',
         num_classes=19168),
 })
 
 
 @register_model
 def mvitv2_tiny(pretrained=False, **kwargs) -> MultiScaleVit:
     return _create_mvitv2('mvitv2_tiny', pretrained=pretrained, **kwargs)
```

### Comparing `timm-0.9.9/timm/models/nasnet.py` & `timm-1.0.3/timm/models/nasnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/nest.py` & `timm-1.0.3/timm/models/nest.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/nfnet.py` & `timm-1.0.3/timm/models/nfnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/pit.py` & `timm-1.0.3/timm/models/pit.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 # PiT
 # Copyright 2021-present NAVER Corp.
 # Apache License v2.0
 
 import math
 import re
 from functools import partial
-from typing import Sequence, Tuple
+from typing import Optional, Sequence, Tuple
 
 import torch
 from torch import nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
-from timm.layers import trunc_normal_, to_2tuple, LayerNorm
+from timm.layers import trunc_normal_, to_2tuple
 from ._builder import build_model_with_cfg
 from ._registry import register_model, generate_default_cfgs
 from .vision_transformer import Block
 
 
 __all__ = ['PoolingVisionTransformer']  # model_registry will add each entrypoint fn to this
 
@@ -242,15 +242,15 @@
 
     def get_classifier(self):
         if self.head_dist is not None:
             return self.head, self.head_dist
         else:
             return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         self.head = nn.Linear(self.embed_dim, num_classes) if num_classes > 0 else nn.Identity()
         if self.head_dist is not None:
             self.head_dist = nn.Linear(self.embed_dim, self.num_classes) if num_classes > 0 else nn.Identity()
 
     def forward_features(self, x):
         x = self.patch_embed(x)
```

### Comparing `timm-0.9.9/timm/models/pnasnet.py` & `timm-1.0.3/timm/models/pnasnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/pvt_v2.py` & `timm-1.0.3/timm/models/pvt_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Based on Apache 2.0 licensed code at https://github.com/whai362/PVT
 
 Modifications and timm support by / Copyright 2022, Ross Wightman
 """
 
 import math
-from typing import Tuple, List, Callable, Union
+from typing import Callable, List, Optional, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.checkpoint as checkpoint
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
@@ -375,15 +375,15 @@
     def set_grad_checkpointing(self, enable=True):
         for s in self.stages:
             s.grad_checkpointing = enable
 
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             assert global_pool in ('avg', '')
             self.global_pool = global_pool
         self.head = nn.Linear(self.embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
     def forward_features(self, x):
```

### Comparing `timm-0.9.9/timm/models/regnet.py` & `timm-1.0.3/timm/models/regnet.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,24 +22,25 @@
 * only known RegNet-Z model definitions with pretrained weights
 
 Hacked together by / Copyright 2020 Ross Wightman
 """
 import math
 from dataclasses import dataclass, replace
 from functools import partial
-from typing import Optional, Union, Callable
+from typing import Callable, List, Optional, Union, Tuple
 
 import numpy as np
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import ClassifierHead, AvgPool2dSame, ConvNormAct, SEModule, DropPath, GroupNormAct
 from timm.layers import get_act_layer, get_norm_act_layer, create_conv2d, make_divisible
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._manipulate import checkpoint_seq, named_apply
 from ._registry import generate_default_cfgs, register_model, register_model_deprecations
 
 __all__ = ['RegNet', 'RegNetCfg']  # model_registry will add each entrypoint fn to this
 
 
 @dataclass
@@ -511,25 +512,92 @@
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
     def reset_classifier(self, num_classes, global_pool='avg'):
         self.head.reset(num_classes, pool_type=global_pool)
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to compatible intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output shape must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(5, indices)
+
+        # forward pass
+        feat_idx = 0
+        x = self.stem(x)
+        if feat_idx in take_indices:
+            intermediates.append(x)
+
+        layer_names = ('s1', 's2', 's3', 's4')
+        if stop_early:
+            layer_names = layer_names[:max_index]
+        for n in layer_names:
+            feat_idx += 1
+            x = getattr(self, n)(x)  # won't work with torchscript, but keeps code reasonable, FML
+            if feat_idx in take_indices:
+                intermediates.append(x)
+
+        if intermediates_only:
+            return intermediates
+
+        if feat_idx == 4:
+            x = self.final_conv(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(5, indices)
+        layer_names = ('s1', 's2', 's3', 's4')
+        layer_names = layer_names[max_index:]
+        for n in layer_names:
+            setattr(self, n, nn.Identity())
+        if max_index < 4:
+            self.final_conv = nn.Identity()
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.stem(x)
         x = self.s1(x)
         x = self.s2(x)
         x = self.s3(x)
         x = self.s4(x)
         x = self.final_conv(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
-        return self.head(x, pre_logits=pre_logits)
+        return self.head(x, pre_logits=pre_logits) if pre_logits else self.head(x)
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
```

### Comparing `timm-0.9.9/timm/models/repghost.py` & `timm-1.0.3/timm/models/repghost.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/repvit.py` & `timm-1.0.3/timm/models/repvit.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,23 +12,24 @@
       primaryClass={cs.CV}
 }
 
 Adapted from official impl at https://github.com/jameslahm/RepViT
 """
 
 __all__ = ['RepVit']
+from typing import Optional
 
+import torch
 import torch.nn as nn
+
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
-from ._registry import register_model, generate_default_cfgs
-from ._builder import build_model_with_cfg
 from timm.layers import SqueezeExcite, trunc_normal_, to_ntuple, to_2tuple
+from ._builder import build_model_with_cfg
 from ._manipulate import checkpoint_seq
-
-import torch
+from ._registry import register_model, generate_default_cfgs
 
 
 class ConvNorm(nn.Sequential):
     def __init__(self, in_dim, out_dim, ks=1, stride=1, pad=0, dilation=1, groups=1, bn_weight_init=1):
         super().__init__()
         self.add_module('c', nn.Conv2d(in_dim, out_dim, ks, stride, pad, dilation, groups, bias=False))
         self.add_module('bn', nn.BatchNorm2d(out_dim))
@@ -318,15 +319,15 @@
     def set_grad_checkpointing(self, enable=True):
         self.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None, distillation=False):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None, distillation=False):
         self.num_classes = num_classes
         if global_pool is not None:
             self.global_pool = global_pool
         self.head = (
             RepVitClassifier(self.embed_dim[-1], num_classes, distillation) if num_classes > 0 else nn.Identity()
         )
```

### Comparing `timm-0.9.9/timm/models/res2net.py` & `timm-1.0.3/timm/models/res2net.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/resnest.py` & `timm-1.0.3/timm/models/resnest.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/resnet.py` & `timm-1.0.3/timm/models/resnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import torch.nn as nn
 import torch.nn.functional as F
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import DropBlock2d, DropPath, AvgPool2dSame, BlurPool2d, GroupNorm, LayerType, create_attn, \
     get_attn, get_act_layer, get_norm_layer, create_classifier
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._manipulate import checkpoint_seq
 from ._registry import register_model, generate_default_cfgs, register_model_deprecations
 
 __all__ = ['ResNet', 'BasicBlock', 'Bottleneck']  # model_registry will add each entrypoint fn to this
 
 
 def get_padding(kernel_size: int, stride: int, dilation: int = 1) -> int:
@@ -291,16 +292,16 @@
         None, None,
         partial(DropBlock2d, drop_prob=drop_prob, block_size=5, gamma_scale=0.25) if drop_prob else None,
         partial(DropBlock2d, drop_prob=drop_prob, block_size=3, gamma_scale=1.00) if drop_prob else None]
 
 
 def make_blocks(
         block_fn: Union[BasicBlock, Bottleneck],
-        channels: List[int],
-        block_repeats: List[int],
+        channels: Tuple[int, ...],
+        block_repeats: Tuple[int, ...],
         inplanes: int,
         reduce_first: int = 1,
         output_stride: int = 32,
         down_kernel_size: int = 1,
         avg_down: bool = False,
         drop_block_rate: float = 0.,
         drop_path_rate: float = 0.,
@@ -390,15 +391,15 @@
     SENet-154 - 3 layer deep 3x3 stem (same as v1c-v1s), stem_width = 64, cardinality=64,
         reduction by 2 on width of first bottleneck convolution, 3x3 downsample convs after first block
     """
 
     def __init__(
             self,
             block: Union[BasicBlock, Bottleneck],
-            layers: List[int],
+            layers: Tuple[int, ...],
             num_classes: int = 1000,
             in_chans: int = 3,
             output_stride: int = 32,
             global_pool: str = 'avg',
             cardinality: int = 1,
             base_width: int = 64,
             stem_width: int = 64,
@@ -493,15 +494,15 @@
                     self.maxpool = nn.Sequential(*[
                         nn.MaxPool2d(kernel_size=3, stride=1, padding=1),
                         aa_layer(channels=inplanes, stride=2)])
             else:
                 self.maxpool = nn.MaxPool2d(kernel_size=3, stride=2, padding=1)
 
         # Feature Blocks
-        channels = [64, 128, 256, 512]
+        channels = (64, 128, 256, 512)
         stage_modules, stage_feature_info = make_blocks(
             block,
             channels,
             layers,
             inplanes,
             cardinality=cardinality,
             base_width=base_width,
@@ -549,14 +550,79 @@
     def get_classifier(self, name_only: bool = False):
         return 'fc' if name_only else self.fc
 
     def reset_classifier(self, num_classes, global_pool='avg'):
         self.num_classes = num_classes
         self.global_pool, self.fc = create_classifier(self.num_features, self.num_classes, pool_type=global_pool)
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to compatible intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output shape must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(5, indices)
+
+        # forward pass
+        feat_idx = 0
+        x = self.conv1(x)
+        x = self.bn1(x)
+        x = self.act1(x)
+        if feat_idx in take_indices:
+            intermediates.append(x)
+        x = self.maxpool(x)
+
+        layer_names = ('layer1', 'layer2', 'layer3', 'layer4')
+        if stop_early:
+            layer_names = layer_names[:max_index]
+        for n in layer_names:
+            feat_idx += 1
+            x = getattr(self, n)(x)  # won't work with torchscript, but keeps code reasonable, FML
+            if feat_idx in take_indices:
+                intermediates.append(x)
+
+        if intermediates_only:
+            return intermediates
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(5, indices)
+        layer_names = ('layer1', 'layer2', 'layer3', 'layer4')
+        layer_names = layer_names[max_index:]
+        for n in layer_names:
+            setattr(self, n, nn.Identity())
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x: torch.Tensor) -> torch.Tensor:
         x = self.conv1(x)
         x = self.bn1(x)
         x = self.act1(x)
         x = self.maxpool(x)
 
         if self.grad_checkpointing and not torch.jit.is_scripting():
@@ -727,14 +793,15 @@
         url='https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-weights/resnet50d_ra2-464e36ba.pth',
         first_conv='conv1.0'),
     'resnet50d.a1_in1k': _rcfg(
         hf_hub_id='timm/',
         url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-rsb-weights/resnet50d_a1_0-e20cff14.pth',
         first_conv='conv1.0'),
     'resnet50d.a2_in1k': _rcfg(
+        hf_hub_id='timm/',
         url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-rsb-weights/resnet50d_a2_0-a3adc64d.pth',
         first_conv='conv1.0'),
     'resnet50d.a3_in1k': _r3cfg(
         hf_hub_id='timm/',
         url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-rsb-weights/resnet50d_a3_0-403fdfad.pth',
         first_conv='conv1.0'),
     'resnet50t.untrained': _ttcfg(first_conv='conv1.0'),
@@ -1112,14 +1179,15 @@
 
     'resnetblur18.untrained': _ttcfg(),
     'resnetblur50.bt_in1k': _ttcfg(
         hf_hub_id='timm/',
         url='https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-weights/resnetblur50-84f4748f.pth'),
     'resnetblur50d.untrained': _ttcfg(first_conv='conv1.0'),
     'resnetblur101d.untrained': _ttcfg(first_conv='conv1.0'),
+    'resnetaa34d.untrained': _ttcfg(first_conv='conv1.0'),
     'resnetaa50.a1h_in1k': _rcfg(
         hf_hub_id='timm/',
         url='https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-rsb-weights/resnetaa50_a1h-4cf422b3.pth'),
 
     'seresnetaa50d.untrained': _ttcfg(first_conv='conv1.0'),
     'seresnextaa101d_32x8d.ah_in1k': _rcfg(
         hf_hub_id='timm/',
@@ -1240,751 +1308,742 @@
 })
 
 
 @register_model
 def resnet10t(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-10-T model.
     """
-    model_args = dict(block=BasicBlock, layers=[1, 1, 1, 1], stem_width=32, stem_type='deep_tiered', avg_down=True)
+    model_args = dict(block=BasicBlock, layers=(1, 1, 1, 1), stem_width=32, stem_type='deep_tiered', avg_down=True)
     return _create_resnet('resnet10t', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet14t(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-14-T model.
     """
-    model_args = dict(block=Bottleneck, layers=[1, 1, 1, 1], stem_width=32, stem_type='deep_tiered', avg_down=True)
+    model_args = dict(block=Bottleneck, layers=(1, 1, 1, 1), stem_width=32, stem_type='deep_tiered', avg_down=True)
     return _create_resnet('resnet14t', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet18(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-18 model.
     """
-    model_args = dict(block=BasicBlock, layers=[2, 2, 2, 2])
+    model_args = dict(block=BasicBlock, layers=(2, 2, 2, 2))
     return _create_resnet('resnet18', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet18d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-18-D model.
     """
-    model_args = dict(block=BasicBlock, layers=[2, 2, 2, 2], stem_width=32, stem_type='deep', avg_down=True)
+    model_args = dict(block=BasicBlock, layers=(2, 2, 2, 2), stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnet18d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet34(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-34 model.
     """
-    model_args = dict(block=BasicBlock, layers=[3, 4, 6, 3])
+    model_args = dict(block=BasicBlock, layers=(3, 4, 6, 3))
     return _create_resnet('resnet34', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet34d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-34-D model.
     """
-    model_args = dict(block=BasicBlock, layers=[3, 4, 6, 3], stem_width=32, stem_type='deep', avg_down=True)
+    model_args = dict(block=BasicBlock, layers=(3, 4, 6, 3), stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnet34d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet26(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-26 model.
     """
-    model_args = dict(block=Bottleneck, layers=[2, 2, 2, 2])
+    model_args = dict(block=Bottleneck, layers=(2, 2, 2, 2))
     return _create_resnet('resnet26', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet26t(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-26-T model.
     """
-    model_args = dict(block=Bottleneck, layers=[2, 2, 2, 2], stem_width=32, stem_type='deep_tiered', avg_down=True)
+    model_args = dict(block=Bottleneck, layers=(2, 2, 2, 2), stem_width=32, stem_type='deep_tiered', avg_down=True)
     return _create_resnet('resnet26t', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet26d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-26-D model.
     """
-    model_args = dict(block=Bottleneck, layers=[2, 2, 2, 2], stem_width=32, stem_type='deep', avg_down=True)
+    model_args = dict(block=Bottleneck, layers=(2, 2, 2, 2), stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnet26d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet50(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50 model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3],  **kwargs)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 6, 3))
     return _create_resnet('resnet50', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet50c(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50-C model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3], stem_width=32, stem_type='deep')
+    model_args = dict(block=Bottleneck, layers=(3, 4, 6, 3), stem_width=32, stem_type='deep')
     return _create_resnet('resnet50c', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet50d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50-D model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3], stem_width=32, stem_type='deep', avg_down=True)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 6, 3), stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnet50d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet50s(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50-S model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3], stem_width=64, stem_type='deep')
+    model_args = dict(block=Bottleneck, layers=(3, 4, 6, 3), stem_width=64, stem_type='deep')
     return _create_resnet('resnet50s', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet50t(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50-T model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3], stem_width=32, stem_type='deep_tiered', avg_down=True)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 6, 3), stem_width=32, stem_type='deep_tiered', avg_down=True)
     return _create_resnet('resnet50t', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet101(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-101 model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3])
+    model_args = dict(block=Bottleneck, layers=(3, 4, 23, 3))
     return _create_resnet('resnet101', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet101c(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-101-C model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], stem_width=32, stem_type='deep')
+    model_args = dict(block=Bottleneck, layers=(3, 4, 23, 3), stem_width=32, stem_type='deep')
     return _create_resnet('resnet101c', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet101d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-101-D model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], stem_width=32, stem_type='deep', avg_down=True)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 23, 3), stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnet101d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet101s(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-101-S model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], stem_width=64, stem_type='deep')
+    model_args = dict(block=Bottleneck, layers=(3, 4, 23, 3), stem_width=64, stem_type='deep')
     return _create_resnet('resnet101s', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet152(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-152 model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 8, 36, 3])
+    model_args = dict(block=Bottleneck, layers=(3, 8, 36, 3))
     return _create_resnet('resnet152', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet152c(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-152-C model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 8, 36, 3], stem_width=32, stem_type='deep')
+    model_args = dict(block=Bottleneck, layers=(3, 8, 36, 3), stem_width=32, stem_type='deep')
     return _create_resnet('resnet152c', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet152d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-152-D model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 8, 36, 3], stem_width=32, stem_type='deep', avg_down=True)
+    model_args = dict(block=Bottleneck, layers=(3, 8, 36, 3), stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnet152d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet152s(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-152-S model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 8, 36, 3], stem_width=64, stem_type='deep')
+    model_args = dict(block=Bottleneck, layers=(3, 8, 36, 3), stem_width=64, stem_type='deep')
     return _create_resnet('resnet152s', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet200(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-200 model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 24, 36, 3])
+    model_args = dict(block=Bottleneck, layers=(3, 24, 36, 3))
     return _create_resnet('resnet200', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet200d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-200-D model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 24, 36, 3], stem_width=32, stem_type='deep', avg_down=True)
+    model_args = dict(block=Bottleneck, layers=(3, 24, 36, 3), stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnet200d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def wide_resnet50_2(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a Wide ResNet-50-2 model.
     The model is the same as ResNet except for the bottleneck number of channels
     which is twice larger in every block. The number of channels in outer 1x1
     convolutions is the same, e.g. last block in ResNet-50 has 2048-512-2048
     channels, and in Wide ResNet-50-2 has 2048-1024-2048.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3], base_width=128)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 6, 3), base_width=128)
     return _create_resnet('wide_resnet50_2', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def wide_resnet101_2(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a Wide ResNet-101-2 model.
     The model is the same as ResNet except for the bottleneck number of channels
     which is twice larger in every block. The number of channels in outer 1x1
     convolutions is the same.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], base_width=128)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 23, 3), base_width=128)
     return _create_resnet('wide_resnet101_2', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnet50_gn(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50 model w/ GroupNorm
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3],  **kwargs)
-    return _create_resnet('resnet50_gn', pretrained, norm_layer=GroupNorm, **model_args)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 6, 3), norm_layer='groupnorm')
+    return _create_resnet('resnet50_gn', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnext50_32x4d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNeXt50-32x4d model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3], cardinality=32, base_width=4)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 6, 3), cardinality=32, base_width=4)
     return _create_resnet('resnext50_32x4d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnext50d_32x4d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNeXt50d-32x4d model. ResNext50 w/ deep stem & avg pool downsample
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 6, 3],  cardinality=32, base_width=4,
+        block=Bottleneck, layers=(3, 4, 6, 3),  cardinality=32, base_width=4,
         stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnext50d_32x4d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnext101_32x4d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNeXt-101 32x4d model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], cardinality=32, base_width=4)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 23, 3), cardinality=32, base_width=4)
     return _create_resnet('resnext101_32x4d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnext101_32x8d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNeXt-101 32x8d model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], cardinality=32, base_width=8)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 23, 3), cardinality=32, base_width=8)
     return _create_resnet('resnext101_32x8d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnext101_32x16d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNeXt-101 32x16d model
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], cardinality=32, base_width=16)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 23, 3), cardinality=32, base_width=16)
     return _create_resnet('resnext101_32x16d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnext101_32x32d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNeXt-101 32x32d model
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], cardinality=32, base_width=32)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 23, 3), cardinality=32, base_width=32)
     return _create_resnet('resnext101_32x32d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnext101_64x4d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNeXt101-64x4d model.
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], cardinality=64, base_width=4)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 23, 3), cardinality=64, base_width=4)
     return _create_resnet('resnext101_64x4d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def ecaresnet26t(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs an ECA-ResNeXt-26-T model.
     This is technically a 28 layer ResNet, like a 'D' bag-of-tricks model but with tiered 24, 32, 64 channels
     in the deep stem and ECA attn.
     """
     model_args = dict(
-        block=Bottleneck, layers=[2, 2, 2, 2], stem_width=32,
+        block=Bottleneck, layers=(2, 2, 2, 2), stem_width=32,
         stem_type='deep_tiered', avg_down=True, block_args=dict(attn_layer='eca'))
     return _create_resnet('ecaresnet26t', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def ecaresnet50d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50-D model with eca.
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 6, 3], stem_width=32, stem_type='deep', avg_down=True,
+        block=Bottleneck, layers=(3, 4, 6, 3), stem_width=32, stem_type='deep', avg_down=True,
         block_args=dict(attn_layer='eca'))
     return _create_resnet('ecaresnet50d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def ecaresnet50d_pruned(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50-D model pruned with eca.
         The pruning has been obtained using https://arxiv.org/pdf/2002.08258.pdf
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 6, 3], stem_width=32, stem_type='deep', avg_down=True,
+        block=Bottleneck, layers=(3, 4, 6, 3), stem_width=32, stem_type='deep', avg_down=True,
         block_args=dict(attn_layer='eca'))
     return _create_resnet('ecaresnet50d_pruned', pretrained, pruned=True, **dict(model_args, **kwargs))
 
 
 @register_model
 def ecaresnet50t(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs an ECA-ResNet-50-T model.
     Like a 'D' bag-of-tricks model but with tiered 24, 32, 64 channels in the deep stem and ECA attn.
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 6, 3], stem_width=32,
+        block=Bottleneck, layers=(3, 4, 6, 3), stem_width=32,
         stem_type='deep_tiered', avg_down=True, block_args=dict(attn_layer='eca'))
     return _create_resnet('ecaresnet50t', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def ecaresnetlight(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50-D light model with eca.
     """
     model_args = dict(
-        block=Bottleneck, layers=[1, 1, 11, 3], stem_width=32, avg_down=True,
+        block=Bottleneck, layers=(1, 1, 11, 3), stem_width=32, avg_down=True,
         block_args=dict(attn_layer='eca'))
     return _create_resnet('ecaresnetlight', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def ecaresnet101d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-101-D model with eca.
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 23, 3], stem_width=32, stem_type='deep', avg_down=True,
+        block=Bottleneck, layers=(3, 4, 23, 3), stem_width=32, stem_type='deep', avg_down=True,
         block_args=dict(attn_layer='eca'))
     return _create_resnet('ecaresnet101d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def ecaresnet101d_pruned(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-101-D model pruned with eca.
        The pruning has been obtained using https://arxiv.org/pdf/2002.08258.pdf
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 23, 3], stem_width=32, stem_type='deep', avg_down=True,
+        block=Bottleneck, layers=(3, 4, 23, 3), stem_width=32, stem_type='deep', avg_down=True,
         block_args=dict(attn_layer='eca'))
     return _create_resnet('ecaresnet101d_pruned', pretrained, pruned=True, **dict(model_args, **kwargs))
 
 
 @register_model
 def ecaresnet200d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-200-D model with ECA.
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 24, 36, 3], stem_width=32, stem_type='deep', avg_down=True,
+        block=Bottleneck, layers=(3, 24, 36, 3), stem_width=32, stem_type='deep', avg_down=True,
         block_args=dict(attn_layer='eca'))
     return _create_resnet('ecaresnet200d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def ecaresnet269d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-269-D model with ECA.
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 30, 48, 8], stem_width=32, stem_type='deep', avg_down=True,
+        block=Bottleneck, layers=(3, 30, 48, 8), stem_width=32, stem_type='deep', avg_down=True,
         block_args=dict(attn_layer='eca'))
     return _create_resnet('ecaresnet269d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def ecaresnext26t_32x4d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs an ECA-ResNeXt-26-T model.
     This is technically a 28 layer ResNet, like a 'D' bag-of-tricks model but with tiered 24, 32, 64 channels
     in the deep stem. This model replaces SE module with the ECA module
     """
     model_args = dict(
-        block=Bottleneck, layers=[2, 2, 2, 2], cardinality=32, base_width=4, stem_width=32,
+        block=Bottleneck, layers=(2, 2, 2, 2), cardinality=32, base_width=4, stem_width=32,
         stem_type='deep_tiered', avg_down=True, block_args=dict(attn_layer='eca'))
     return _create_resnet('ecaresnext26t_32x4d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def ecaresnext50t_32x4d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs an ECA-ResNeXt-50-T model.
     This is technically a 28 layer ResNet, like a 'D' bag-of-tricks model but with tiered 24, 32, 64 channels
     in the deep stem. This model replaces SE module with the ECA module
     """
     model_args = dict(
-        block=Bottleneck, layers=[2, 2, 2, 2], cardinality=32, base_width=4, stem_width=32,
+        block=Bottleneck, layers=(2, 2, 2, 2), cardinality=32, base_width=4, stem_width=32,
         stem_type='deep_tiered', avg_down=True, block_args=dict(attn_layer='eca'))
     return _create_resnet('ecaresnext50t_32x4d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnet18(pretrained: bool = False, **kwargs) -> ResNet:
-    model_args = dict(block=BasicBlock, layers=[2, 2, 2, 2], block_args=dict(attn_layer='se'))
+    model_args = dict(block=BasicBlock, layers=(2, 2, 2, 2), block_args=dict(attn_layer='se'))
     return _create_resnet('seresnet18', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnet34(pretrained: bool = False, **kwargs) -> ResNet:
-    model_args = dict(block=BasicBlock, layers=[3, 4, 6, 3], block_args=dict(attn_layer='se'))
+    model_args = dict(block=BasicBlock, layers=(3, 4, 6, 3), block_args=dict(attn_layer='se'))
     return _create_resnet('seresnet34', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnet50(pretrained: bool = False, **kwargs) -> ResNet:
-    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3], block_args=dict(attn_layer='se'))
+    model_args = dict(block=Bottleneck, layers=(3, 4, 6, 3), block_args=dict(attn_layer='se'))
     return _create_resnet('seresnet50', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnet50t(pretrained: bool = False, **kwargs) -> ResNet:
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 6, 3],  stem_width=32, stem_type='deep_tiered',
+        block=Bottleneck, layers=(3, 4, 6, 3),  stem_width=32, stem_type='deep_tiered',
         avg_down=True, block_args=dict(attn_layer='se'))
     return _create_resnet('seresnet50t', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnet101(pretrained: bool = False, **kwargs) -> ResNet:
-    model_args = dict(block=Bottleneck, layers=[3, 4, 23, 3], block_args=dict(attn_layer='se'))
+    model_args = dict(block=Bottleneck, layers=(3, 4, 23, 3), block_args=dict(attn_layer='se'))
     return _create_resnet('seresnet101', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnet152(pretrained: bool = False, **kwargs) -> ResNet:
-    model_args = dict(block=Bottleneck, layers=[3, 8, 36, 3], block_args=dict(attn_layer='se'))
+    model_args = dict(block=Bottleneck, layers=(3, 8, 36, 3), block_args=dict(attn_layer='se'))
     return _create_resnet('seresnet152', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnet152d(pretrained: bool = False, **kwargs) -> ResNet:
     model_args = dict(
-        block=Bottleneck, layers=[3, 8, 36, 3], stem_width=32, stem_type='deep',
+        block=Bottleneck, layers=(3, 8, 36, 3), stem_width=32, stem_type='deep',
         avg_down=True, block_args=dict(attn_layer='se'))
     return _create_resnet('seresnet152d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnet200d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-200-D model with SE attn.
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 24, 36, 3], stem_width=32, stem_type='deep',
+        block=Bottleneck, layers=(3, 24, 36, 3), stem_width=32, stem_type='deep',
         avg_down=True, block_args=dict(attn_layer='se'))
     return _create_resnet('seresnet200d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnet269d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-269-D model with SE attn.
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 30, 48, 8], stem_width=32, stem_type='deep',
+        block=Bottleneck, layers=(3, 30, 48, 8), stem_width=32, stem_type='deep',
         avg_down=True, block_args=dict(attn_layer='se'))
     return _create_resnet('seresnet269d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnext26d_32x4d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a SE-ResNeXt-26-D model.`
     This is technically a 28 layer ResNet, using the 'D' modifier from Gluon / bag-of-tricks for
     combination of deep stem and avg_pool in downsample.
     """
     model_args = dict(
-        block=Bottleneck, layers=[2, 2, 2, 2], cardinality=32, base_width=4, stem_width=32,
+        block=Bottleneck, layers=(2, 2, 2, 2), cardinality=32, base_width=4, stem_width=32,
         stem_type='deep', avg_down=True, block_args=dict(attn_layer='se'))
     return _create_resnet('seresnext26d_32x4d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnext26t_32x4d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a SE-ResNet-26-T model.
     This is technically a 28 layer ResNet, like a 'D' bag-of-tricks model but with tiered 24, 32, 64 channels
     in the deep stem.
     """
     model_args = dict(
-        block=Bottleneck, layers=[2, 2, 2, 2], cardinality=32, base_width=4, stem_width=32,
+        block=Bottleneck, layers=(2, 2, 2, 2), cardinality=32, base_width=4, stem_width=32,
         stem_type='deep_tiered', avg_down=True, block_args=dict(attn_layer='se'))
     return _create_resnet('seresnext26t_32x4d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
-def seresnext26tn_32x4d(pretrained: bool = False, **kwargs) -> ResNet:
-    """Constructs a SE-ResNeXt-26-T model.
-    NOTE I deprecated previous 't' model defs and replaced 't' with 'tn', this was the only tn model of note
-    so keeping this def for backwards compat with any uses out there. Old 't' model is lost.
-    """
-    return seresnext26t_32x4d(pretrained=pretrained, **kwargs)
-
-
-@register_model
 def seresnext50_32x4d(pretrained: bool = False, **kwargs) -> ResNet:
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 6, 3], cardinality=32, base_width=4,
+        block=Bottleneck, layers=(3, 4, 6, 3), cardinality=32, base_width=4,
         block_args=dict(attn_layer='se'))
     return _create_resnet('seresnext50_32x4d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnext101_32x4d(pretrained: bool = False, **kwargs) -> ResNet:
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 23, 3], cardinality=32, base_width=4,
+        block=Bottleneck, layers=(3, 4, 23, 3), cardinality=32, base_width=4,
         block_args=dict(attn_layer='se'))
     return _create_resnet('seresnext101_32x4d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnext101_32x8d(pretrained: bool = False, **kwargs) -> ResNet:
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 23, 3], cardinality=32, base_width=8,
+        block=Bottleneck, layers=(3, 4, 23, 3), cardinality=32, base_width=8,
         block_args=dict(attn_layer='se'))
     return _create_resnet('seresnext101_32x8d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnext101d_32x8d(pretrained: bool = False, **kwargs) -> ResNet:
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 23, 3], cardinality=32, base_width=8,
+        block=Bottleneck, layers=(3, 4, 23, 3), cardinality=32, base_width=8,
         stem_width=32, stem_type='deep', avg_down=True,
         block_args=dict(attn_layer='se'))
     return _create_resnet('seresnext101d_32x8d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnext101_64x4d(pretrained: bool = False, **kwargs) -> ResNet:
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 23, 3], cardinality=64, base_width=4,
+        block=Bottleneck, layers=(3, 4, 23, 3), cardinality=64, base_width=4,
         block_args=dict(attn_layer='se'))
     return _create_resnet('seresnext101_64x4d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def senet154(pretrained: bool = False, **kwargs) -> ResNet:
     model_args = dict(
-        block=Bottleneck, layers=[3, 8, 36, 3], cardinality=64, base_width=4, stem_type='deep',
+        block=Bottleneck, layers=(3, 8, 36, 3), cardinality=64, base_width=4, stem_type='deep',
         down_kernel_size=3, block_reduce_first=2, block_args=dict(attn_layer='se'))
     return _create_resnet('senet154', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetblur18(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-18 model with blur anti-aliasing
     """
-    model_args = dict(block=BasicBlock, layers=[2, 2, 2, 2], aa_layer=BlurPool2d)
+    model_args = dict(block=BasicBlock, layers=(2, 2, 2, 2), aa_layer=BlurPool2d)
     return _create_resnet('resnetblur18', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetblur50(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50 model with blur anti-aliasing
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3], aa_layer=BlurPool2d)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 6, 3), aa_layer=BlurPool2d)
     return _create_resnet('resnetblur50', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetblur50d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50-D model with blur anti-aliasing
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 6, 3], aa_layer=BlurPool2d,
+        block=Bottleneck, layers=(3, 4, 6, 3), aa_layer=BlurPool2d,
         stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnetblur50d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetblur101d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-101-D model with blur anti-aliasing
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 23, 3], aa_layer=BlurPool2d,
+        block=Bottleneck, layers=(3, 4, 23, 3), aa_layer=BlurPool2d,
         stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnetblur101d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetaa34d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-34-D model w/ avgpool anti-aliasing
     """
     model_args = dict(
-        block=BasicBlock, layers=[3, 4, 6, 3],  aa_layer=nn.AvgPool2d, stem_width=32, stem_type='deep', avg_down=True)
+        block=BasicBlock, layers=(3, 4, 6, 3),  aa_layer=nn.AvgPool2d, stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnetaa34d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetaa50(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50 model with avgpool anti-aliasing
     """
-    model_args = dict(block=Bottleneck, layers=[3, 4, 6, 3], aa_layer=nn.AvgPool2d)
+    model_args = dict(block=Bottleneck, layers=(3, 4, 6, 3), aa_layer=nn.AvgPool2d)
     return _create_resnet('resnetaa50', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetaa50d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-50-D model with avgpool anti-aliasing
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 6, 3], aa_layer=nn.AvgPool2d,
+        block=Bottleneck, layers=(3, 4, 6, 3), aa_layer=nn.AvgPool2d,
         stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnetaa50d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetaa101d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-101-D model with avgpool anti-aliasing
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 23, 3], aa_layer=nn.AvgPool2d,
+        block=Bottleneck, layers=(3, 4, 23, 3), aa_layer=nn.AvgPool2d,
         stem_width=32, stem_type='deep', avg_down=True)
     return _create_resnet('resnetaa101d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnetaa50d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a SE=ResNet-50-D model with avgpool anti-aliasing
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 6, 3], aa_layer=nn.AvgPool2d,
+        block=Bottleneck, layers=(3, 4, 6, 3), aa_layer=nn.AvgPool2d,
         stem_width=32, stem_type='deep', avg_down=True, block_args=dict(attn_layer='se'))
     return _create_resnet('seresnetaa50d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnextaa101d_32x8d(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a SE=ResNeXt-101-D 32x8d model with avgpool anti-aliasing
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 23, 3], cardinality=32, base_width=8,
+        block=Bottleneck, layers=(3, 4, 23, 3), cardinality=32, base_width=8,
         stem_width=32, stem_type='deep', avg_down=True, aa_layer=nn.AvgPool2d,
         block_args=dict(attn_layer='se'))
     return _create_resnet('seresnextaa101d_32x8d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def seresnextaa201d_32x8d(pretrained: bool = False, **kwargs):
     """Constructs a SE=ResNeXt-101-D 32x8d model with avgpool anti-aliasing
     """
     model_args = dict(
-        block=Bottleneck, layers=[3, 24, 36, 4], cardinality=32, base_width=8,
+        block=Bottleneck, layers=(3, 24, 36, 4), cardinality=32, base_width=8,
         stem_width=64, stem_type='deep', avg_down=True, aa_layer=nn.AvgPool2d,
         block_args=dict(attn_layer='se'))
     return _create_resnet('seresnextaa201d_32x8d', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetrs50(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-RS-50 model.
     Paper: Revisiting ResNets - https://arxiv.org/abs/2103.07579
     Pretrained weights from https://github.com/tensorflow/tpu/tree/bee9c4f6/models/official/resnet/resnet_rs
     """
     attn_layer = partial(get_attn('se'), rd_ratio=0.25)
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 6, 3], stem_width=32, stem_type='deep', replace_stem_pool=True,
+        block=Bottleneck, layers=(3, 4, 6, 3), stem_width=32, stem_type='deep', replace_stem_pool=True,
         avg_down=True,  block_args=dict(attn_layer=attn_layer))
     return _create_resnet('resnetrs50', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetrs101(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-RS-101 model.
     Paper: Revisiting ResNets - https://arxiv.org/abs/2103.07579
     Pretrained weights from https://github.com/tensorflow/tpu/tree/bee9c4f6/models/official/resnet/resnet_rs
     """
     attn_layer = partial(get_attn('se'), rd_ratio=0.25)
     model_args = dict(
-        block=Bottleneck, layers=[3, 4, 23, 3], stem_width=32, stem_type='deep', replace_stem_pool=True,
+        block=Bottleneck, layers=(3, 4, 23, 3), stem_width=32, stem_type='deep', replace_stem_pool=True,
         avg_down=True,  block_args=dict(attn_layer=attn_layer))
     return _create_resnet('resnetrs101', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetrs152(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-RS-152 model.
     Paper: Revisiting ResNets - https://arxiv.org/abs/2103.07579
     Pretrained weights from https://github.com/tensorflow/tpu/tree/bee9c4f6/models/official/resnet/resnet_rs
     """
     attn_layer = partial(get_attn('se'), rd_ratio=0.25)
     model_args = dict(
-        block=Bottleneck, layers=[3, 8, 36, 3], stem_width=32, stem_type='deep', replace_stem_pool=True,
+        block=Bottleneck, layers=(3, 8, 36, 3), stem_width=32, stem_type='deep', replace_stem_pool=True,
         avg_down=True,  block_args=dict(attn_layer=attn_layer))
     return _create_resnet('resnetrs152', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetrs200(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-RS-200 model.
     Paper: Revisiting ResNets - https://arxiv.org/abs/2103.07579
     Pretrained weights from https://github.com/tensorflow/tpu/tree/bee9c4f6/models/official/resnet/resnet_rs
     """
     attn_layer = partial(get_attn('se'), rd_ratio=0.25)
     model_args = dict(
-        block=Bottleneck, layers=[3, 24, 36, 3], stem_width=32, stem_type='deep', replace_stem_pool=True,
+        block=Bottleneck, layers=(3, 24, 36, 3), stem_width=32, stem_type='deep', replace_stem_pool=True,
         avg_down=True,  block_args=dict(attn_layer=attn_layer))
     return _create_resnet('resnetrs200', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetrs270(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-RS-270 model.
     Paper: Revisiting ResNets - https://arxiv.org/abs/2103.07579
     Pretrained weights from https://github.com/tensorflow/tpu/tree/bee9c4f6/models/official/resnet/resnet_rs
     """
     attn_layer = partial(get_attn('se'), rd_ratio=0.25)
     model_args = dict(
-        block=Bottleneck, layers=[4, 29, 53, 4], stem_width=32, stem_type='deep', replace_stem_pool=True,
+        block=Bottleneck, layers=(4, 29, 53, 4), stem_width=32, stem_type='deep', replace_stem_pool=True,
         avg_down=True,  block_args=dict(attn_layer=attn_layer))
     return _create_resnet('resnetrs270', pretrained, **dict(model_args, **kwargs))
 
 
 
 @register_model
 def resnetrs350(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-RS-350 model.
     Paper: Revisiting ResNets - https://arxiv.org/abs/2103.07579
     Pretrained weights from https://github.com/tensorflow/tpu/tree/bee9c4f6/models/official/resnet/resnet_rs
     """
     attn_layer = partial(get_attn('se'), rd_ratio=0.25)
     model_args = dict(
-        block=Bottleneck, layers=[4, 36, 72, 4], stem_width=32, stem_type='deep', replace_stem_pool=True,
+        block=Bottleneck, layers=(4, 36, 72, 4), stem_width=32, stem_type='deep', replace_stem_pool=True,
         avg_down=True,  block_args=dict(attn_layer=attn_layer))
     return _create_resnet('resnetrs350', pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def resnetrs420(pretrained: bool = False, **kwargs) -> ResNet:
     """Constructs a ResNet-RS-420 model
     Paper: Revisiting ResNets - https://arxiv.org/abs/2103.07579
     Pretrained weights from https://github.com/tensorflow/tpu/tree/bee9c4f6/models/official/resnet/resnet_rs
     """
     attn_layer = partial(get_attn('se'), rd_ratio=0.25)
     model_args = dict(
-        block=Bottleneck, layers=[4, 44, 87, 4], stem_width=32, stem_type='deep', replace_stem_pool=True,
+        block=Bottleneck, layers=(4, 44, 87, 4), stem_width=32, stem_type='deep', replace_stem_pool=True,
         avg_down=True,  block_args=dict(attn_layer=attn_layer))
     return _create_resnet('resnetrs420', pretrained, **dict(model_args, **kwargs))
 
 
 register_model_deprecations(__name__, {
     'tv_resnet34': 'resnet34.tv_in1k',
     'tv_resnet50': 'resnet50.tv_in1k',
@@ -2024,8 +2083,9 @@
     'gluon_resnext50_32x4d': 'resnext50_32x4d.gluon_in1k',
     'gluon_resnext101_32x4d': 'resnext101_32x4d.gluon_in1k',
     'gluon_resnext101_64x4d': 'resnext101_64x4d.gluon_in1k',
     'gluon_seresnext50_32x4d': 'seresnext50_32x4d.gluon_in1k',
     'gluon_seresnext101_32x4d': 'seresnext101_32x4d.gluon_in1k',
     'gluon_seresnext101_64x4d': 'seresnext101_64x4d.gluon_in1k',
     'gluon_senet154': 'senet154.gluon_in1k',
+    'seresnext26tn_32x4d': 'seresnext26t_32x4d',
 })
```

### Comparing `timm-0.9.9/timm/models/resnetv2.py` & `timm-1.0.3/timm/models/resnetv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,15 @@
             x = checkpoint_seq(self.stages, x, flatten=True)
         else:
             x = self.stages(x)
         x = self.norm(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
-        return self.head(x, pre_logits=pre_logits)
+        return self.head(x, pre_logits=pre_logits) if pre_logits else self.head(x)
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
```

### Comparing `timm-0.9.9/timm/models/rexnet.py` & `timm-1.0.3/timm/models/rexnet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/selecsls.py` & `timm-1.0.3/timm/models/selecsls.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/senet.py` & `timm-1.0.3/timm/models/senet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/sequencer.py` & `timm-1.0.3/timm/models/sequencer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 #  Copyright (c) 2022. Yuki Tatsunami
 #  Licensed under the Apache License, Version 2.0 (the "License");
 
 import math
 from functools import partial
 from itertools import accumulate
-from typing import Tuple
+from typing import Optional, Tuple
 
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD, DEFAULT_CROP_PCT
 from timm.layers import lecun_normal_, DropPath, Mlp, PatchEmbed, ClassifierHead
 from ._builder import build_model_with_cfg
@@ -415,15 +415,15 @@
     def set_grad_checkpointing(self, enable=True):
         assert not enable, 'gradient checkpointing not supported'
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         self.head.reset(num_classes, pool_type=global_pool)
 
     def forward_features(self, x):
         x = self.stem(x)
         x = self.stages(x)
         x = self.norm(x)
```

### Comparing `timm-0.9.9/timm/models/sknet.py` & `timm-1.0.3/timm/models/sknet.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/swin_transformer.py` & `timm-1.0.3/timm/models/swin_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import PatchEmbed, Mlp, DropPath, ClassifierHead, to_2tuple, to_ntuple, trunc_normal_, \
-    _assert, use_fused_attn, resize_rel_pos_bias_table, resample_patch_embed
+    _assert, use_fused_attn, resize_rel_pos_bias_table, resample_patch_embed, ndgrid
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._features_fx import register_notrace_function
 from ._manipulate import checkpoint_seq, named_apply
 from ._registry import generate_default_cfgs, register_model, register_model_deprecations
 from .vision_transformer import get_init_weights_vit
 
 __all__ = ['SwinTransformer']  # model_registry will add each entrypoint fn to this
 
@@ -74,15 +75,15 @@
     x = windows.view(-1, H // window_size[0], W // window_size[1], window_size[0], window_size[1], C)
     x = x.permute(0, 1, 3, 2, 4, 5).contiguous().view(-1, H, W, C)
     return x
 
 
 def get_relative_position_index(win_h: int, win_w: int):
     # get pair-wise relative position index for each token inside the window
-    coords = torch.stack(torch.meshgrid([torch.arange(win_h), torch.arange(win_w)]))  # 2, Wh, Ww
+    coords = torch.stack(ndgrid(torch.arange(win_h), torch.arange(win_w)))  # 2, Wh, Ww
     coords_flatten = torch.flatten(coords, 1)  # 2, Wh*Ww
     relative_coords = coords_flatten[:, :, None] - coords_flatten[:, None, :]  # 2, Wh*Ww, Wh*Ww
     relative_coords = relative_coords.permute(1, 2, 0).contiguous()  # Wh*Ww, Wh*Ww, 2
     relative_coords[:, :, 0] += win_h - 1  # shift to start from 0
     relative_coords[:, :, 1] += win_w - 1
     relative_coords[:, :, 0] *= 2 * win_w - 1
     return relative_coords.sum(-1)  # Wh*Ww, Wh*Ww
@@ -379,14 +380,15 @@
             attn_drop: float = 0.,
             drop_path: Union[List[float], float] = 0.,
             norm_layer: Callable = nn.LayerNorm,
     ):
         """
         Args:
             dim: Number of input channels.
+            out_dim: Number of output channels.
             input_resolution: Input resolution.
             depth: Number of blocks.
             downsample: Downsample layer at the end of the layer.
             num_heads: Number of attention heads.
             head_dim: Channels per head (dim // num_heads if not set)
             window_size: Local window size.
             mlp_ratio: Ratio of mlp hidden dim to embedding dim.
@@ -598,18 +600,84 @@
         for l in self.layers:
             l.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         self.head.reset(num_classes, pool_type=global_pool)
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to compatible intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output shape must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.layers), indices)
+
+        # forward pass
+        x = self.patch_embed(x)
+
+        num_stages = len(self.layers)
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            stages = self.layers
+        else:
+            stages = self.layers[:max_index + 1]
+        for i, stage in enumerate(stages):
+            x = stage(x)
+            if i in take_indices:
+                if norm and i == num_stages - 1:
+                    x_inter = self.norm(x)  # applying final norm last intermediate
+                else:
+                    x_inter = x
+                x_inter = x_inter.permute(0, 3, 1, 2).contiguous()
+                intermediates.append(x_inter)
+
+        if intermediates_only:
+            return intermediates
+
+        x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.layers), indices)
+        self.layers = self.layers[:max_index + 1]  # truncate blocks
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.patch_embed(x)
         x = self.layers(x)
         x = self.norm(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
```

### Comparing `timm-0.9.9/timm/models/swin_transformer_v2.py` & `timm-1.0.3/timm/models/swin_transformer_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,34 +9,35 @@
 # --------------------------------------------------------
 # Swin Transformer V2
 # Copyright (c) 2022 Microsoft
 # Licensed under The MIT License [see LICENSE for details]
 # Written by Ze Liu
 # --------------------------------------------------------
 import math
-from typing import Callable, Optional, Tuple, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.checkpoint as checkpoint
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import PatchEmbed, Mlp, DropPath, to_2tuple, trunc_normal_, _assert, ClassifierHead,\
-    resample_patch_embed
+    resample_patch_embed, ndgrid, get_act_layer, LayerType
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._features_fx import register_notrace_function
 from ._registry import generate_default_cfgs, register_model, register_model_deprecations
 
 __all__ = ['SwinTransformerV2']  # model_registry will add each entrypoint fn to this
 
 _int_or_tuple_2_t = Union[int, Tuple[int, int]]
 
 
-def window_partition(x, window_size: Tuple[int, int]):
+def window_partition(x: torch.Tensor, window_size: Tuple[int, int]) -> torch.Tensor:
     """
     Args:
         x: (B, H, W, C)
         window_size (int): window size
 
     Returns:
         windows: (num_windows*B, window_size, window_size, C)
@@ -44,15 +45,15 @@
     B, H, W, C = x.shape
     x = x.view(B, H // window_size[0], window_size[0], W // window_size[1], window_size[1], C)
     windows = x.permute(0, 1, 3, 2, 4, 5).contiguous().view(-1, window_size[0], window_size[1], C)
     return windows
 
 
 @register_notrace_function  # reason: int argument is a Proxy
-def window_reverse(windows, window_size: Tuple[int, int], img_size: Tuple[int, int]):
+def window_reverse(windows: torch.Tensor, window_size: Tuple[int, int], img_size: Tuple[int, int]) -> torch.Tensor:
     """
     Args:
         windows: (num_windows * B, window_size[0], window_size[1], C)
         window_size (Tuple[int, int]): Window size
         img_size (Tuple[int, int]): Image size
 
     Returns:
@@ -77,22 +78,22 @@
         attn_drop (float, optional): Dropout ratio of attention weight. Default: 0.0
         proj_drop (float, optional): Dropout ratio of output. Default: 0.0
         pretrained_window_size (tuple[int]): The height and width of the window in pre-training.
     """
 
     def __init__(
             self,
-            dim,
-            window_size,
-            num_heads,
-            qkv_bias=True,
-            attn_drop=0.,
-            proj_drop=0.,
-            pretrained_window_size=[0, 0],
-    ):
+            dim: int,
+            window_size: Tuple[int, int],
+            num_heads: int,
+            qkv_bias: bool = True,
+            attn_drop: float = 0.,
+            proj_drop: float = 0.,
+            pretrained_window_size: Tuple[int, int] = (0, 0),
+    ) -> None:
         super().__init__()
         self.dim = dim
         self.window_size = window_size  # Wh, Ww
         self.pretrained_window_size = pretrained_window_size
         self.num_heads = num_heads
 
         self.logit_scale = nn.Parameter(torch.log(10 * torch.ones((num_heads, 1, 1))))
@@ -101,19 +102,18 @@
         self.cpb_mlp = nn.Sequential(
             nn.Linear(2, 512, bias=True),
             nn.ReLU(inplace=True),
             nn.Linear(512, num_heads, bias=False)
         )
 
         # get relative_coords_table
-        relative_coords_h = torch.arange(-(self.window_size[0] - 1), self.window_size[0], dtype=torch.float32)
-        relative_coords_w = torch.arange(-(self.window_size[1] - 1), self.window_size[1], dtype=torch.float32)
-        relative_coords_table = torch.stack(torch.meshgrid([
-            relative_coords_h,
-            relative_coords_w])).permute(1, 2, 0).contiguous().unsqueeze(0)  # 1, 2*Wh-1, 2*Ww-1, 2
+        relative_coords_h = torch.arange(-(self.window_size[0] - 1), self.window_size[0]).to(torch.float32)
+        relative_coords_w = torch.arange(-(self.window_size[1] - 1), self.window_size[1]).to(torch.float32)
+        relative_coords_table = torch.stack(ndgrid(relative_coords_h, relative_coords_w))
+        relative_coords_table = relative_coords_table.permute(1, 2, 0).contiguous().unsqueeze(0)  # 1, 2*Wh-1, 2*Ww-1, 2
         if pretrained_window_size[0] > 0:
             relative_coords_table[:, :, :, 0] /= (pretrained_window_size[0] - 1)
             relative_coords_table[:, :, :, 1] /= (pretrained_window_size[1] - 1)
         else:
             relative_coords_table[:, :, :, 0] /= (self.window_size[0] - 1)
             relative_coords_table[:, :, :, 1] /= (self.window_size[1] - 1)
         relative_coords_table *= 8  # normalize to -8, 8
@@ -121,15 +121,15 @@
             torch.abs(relative_coords_table) + 1.0) / math.log2(8)
 
         self.register_buffer("relative_coords_table", relative_coords_table, persistent=False)
 
         # get pair-wise relative position index for each token inside the window
         coords_h = torch.arange(self.window_size[0])
         coords_w = torch.arange(self.window_size[1])
-        coords = torch.stack(torch.meshgrid([coords_h, coords_w]))  # 2, Wh, Ww
+        coords = torch.stack(ndgrid(coords_h, coords_w))  # 2, Wh, Ww
         coords_flatten = torch.flatten(coords, 1)  # 2, Wh*Ww
         relative_coords = coords_flatten[:, :, None] - coords_flatten[:, None, :]  # 2, Wh*Ww, Wh*Ww
         relative_coords = relative_coords.permute(1, 2, 0).contiguous()  # Wh*Ww, Wh*Ww, 2
         relative_coords[:, :, 0] += self.window_size[0] - 1  # shift to start from 0
         relative_coords[:, :, 1] += self.window_size[1] - 1
         relative_coords[:, :, 0] *= 2 * self.window_size[1] - 1
         relative_position_index = relative_coords.sum(-1)  # Wh*Ww, Wh*Ww
@@ -145,15 +145,15 @@
             self.k_bias = None
             self.v_bias = None
         self.attn_drop = nn.Dropout(attn_drop)
         self.proj = nn.Linear(dim, dim)
         self.proj_drop = nn.Dropout(proj_drop)
         self.softmax = nn.Softmax(dim=-1)
 
-    def forward(self, x, mask: Optional[torch.Tensor] = None):
+    def forward(self, x: torch.Tensor, mask: Optional[torch.Tensor] = None) -> torch.Tensor:
         """
         Args:
             x: input features with shape of (num_windows*B, N, C)
             mask: (0/-inf) mask with shape of (num_windows, Wh*Ww, Wh*Ww) or None
         """
         B_, N, C = x.shape
         qkv_bias = None
@@ -193,28 +193,28 @@
 
 class SwinTransformerV2Block(nn.Module):
     """ Swin Transformer Block.
     """
 
     def __init__(
             self,
-            dim,
-            input_resolution,
-            num_heads,
-            window_size=7,
-            shift_size=0,
-            mlp_ratio=4.,
-            qkv_bias=True,
-            proj_drop=0.,
-            attn_drop=0.,
-            drop_path=0.,
-            act_layer=nn.GELU,
-            norm_layer=nn.LayerNorm,
-            pretrained_window_size=0,
-    ):
+            dim: int,
+            input_resolution: _int_or_tuple_2_t,
+            num_heads: int,
+            window_size: _int_or_tuple_2_t = 7,
+            shift_size: _int_or_tuple_2_t = 0,
+            mlp_ratio: float = 4.,
+            qkv_bias: bool = True,
+            proj_drop: float = 0.,
+            attn_drop: float = 0.,
+            drop_path: float = 0.,
+            act_layer: LayerType = "gelu",
+            norm_layer: nn.Module = nn.LayerNorm,
+            pretrained_window_size: _int_or_tuple_2_t = 0,
+    ) -> None:
         """
         Args:
             dim: Number of input channels.
             input_resolution: Input resolution.
             num_heads: Number of attention heads.
             window_size: Window size.
             shift_size: Shift size for SW-MSA.
@@ -232,14 +232,15 @@
         self.input_resolution = to_2tuple(input_resolution)
         self.num_heads = num_heads
         ws, ss = self._calc_window_shift(window_size, shift_size)
         self.window_size: Tuple[int, int] = ws
         self.shift_size: Tuple[int, int] = ss
         self.window_area = self.window_size[0] * self.window_size[1]
         self.mlp_ratio = mlp_ratio
+        act_layer = get_act_layer(act_layer)
 
         self.attn = WindowAttention(
             dim,
             window_size=to_2tuple(self.window_size),
             num_heads=num_heads,
             qkv_bias=qkv_bias,
             attn_drop=attn_drop,
@@ -278,22 +279,24 @@
             attn_mask = mask_windows.unsqueeze(1) - mask_windows.unsqueeze(2)
             attn_mask = attn_mask.masked_fill(attn_mask != 0, float(-100.0)).masked_fill(attn_mask == 0, float(0.0))
         else:
             attn_mask = None
 
         self.register_buffer("attn_mask", attn_mask, persistent=False)
 
-    def _calc_window_shift(self, target_window_size, target_shift_size) -> Tuple[Tuple[int, int], Tuple[int, int]]:
+    def _calc_window_shift(self,
+                           target_window_size: _int_or_tuple_2_t,
+                           target_shift_size: _int_or_tuple_2_t) -> Tuple[Tuple[int, int], Tuple[int, int]]:
         target_window_size = to_2tuple(target_window_size)
         target_shift_size = to_2tuple(target_shift_size)
         window_size = [r if r <= w else w for r, w in zip(self.input_resolution, target_window_size)]
         shift_size = [0 if r <= w else s for r, w, s in zip(self.input_resolution, window_size, target_shift_size)]
         return tuple(window_size), tuple(shift_size)
 
-    def _attn(self, x):
+    def _attn(self, x: torch.Tensor) -> torch.Tensor:
         B, H, W, C = x.shape
 
         # cyclic shift
         has_shift = any(self.shift_size)
         if has_shift:
             shifted_x = torch.roll(x, shifts=(-self.shift_size[0], -self.shift_size[1]), dims=(1, 2))
         else:
@@ -313,41 +316,41 @@
         # reverse cyclic shift
         if has_shift:
             x = torch.roll(shifted_x, shifts=self.shift_size, dims=(1, 2))
         else:
             x = shifted_x
         return x
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         B, H, W, C = x.shape
         x = x + self.drop_path1(self.norm1(self._attn(x)))
         x = x.reshape(B, -1, C)
         x = x + self.drop_path2(self.norm2(self.mlp(x)))
         x = x.reshape(B, H, W, C)
         return x
 
 
 class PatchMerging(nn.Module):
     """ Patch Merging Layer.
     """
 
-    def __init__(self, dim, out_dim=None, norm_layer=nn.LayerNorm):
+    def __init__(self, dim: int, out_dim: Optional[int] = None, norm_layer: nn.Module = nn.LayerNorm) -> None:
         """
         Args:
             dim (int): Number of input channels.
             out_dim (int): Number of output channels (or 2 * dim if None)
             norm_layer (nn.Module, optional): Normalization layer.  Default: nn.LayerNorm
         """
         super().__init__()
         self.dim = dim
         self.out_dim = out_dim or 2 * dim
         self.reduction = nn.Linear(4 * dim, self.out_dim, bias=False)
         self.norm = norm_layer(self.out_dim)
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         B, H, W, C = x.shape
         _assert(H % 2 == 0, f"x height ({H}) is not even.")
         _assert(W % 2 == 0, f"x width ({W}) is not even.")
         x = x.reshape(B, H // 2, 2, W // 2, 2, C).permute(0, 1, 3, 4, 2, 5).flatten(3)
         x = self.reduction(x)
         x = self.norm(x)
         return x
@@ -355,43 +358,46 @@
 
 class SwinTransformerV2Stage(nn.Module):
     """ A Swin Transformer V2 Stage.
     """
 
     def __init__(
             self,
-            dim,
-            out_dim,
-            input_resolution,
-            depth,
-            num_heads,
-            window_size,
-            downsample=False,
-            mlp_ratio=4.,
-            qkv_bias=True,
-            proj_drop=0.,
-            attn_drop=0.,
-            drop_path=0.,
-            norm_layer=nn.LayerNorm,
-            pretrained_window_size=0,
-            output_nchw=False,
-    ):
+            dim: int,
+            out_dim: int,
+            input_resolution: _int_or_tuple_2_t,
+            depth: int,
+            num_heads: int,
+            window_size: _int_or_tuple_2_t,
+            downsample: bool = False,
+            mlp_ratio: float = 4.,
+            qkv_bias: bool = True,
+            proj_drop: float = 0.,
+            attn_drop: float = 0.,
+            drop_path: float = 0.,
+            act_layer: Union[str, Callable] = 'gelu',
+            norm_layer: nn.Module = nn.LayerNorm,
+            pretrained_window_size: _int_or_tuple_2_t = 0,
+            output_nchw: bool = False,
+    ) -> None:
         """
         Args:
             dim: Number of input channels.
+            out_dim: Number of output channels.
             input_resolution: Input resolution.
             depth: Number of blocks.
             num_heads: Number of attention heads.
             window_size: Local window size.
             downsample: Use downsample layer at start of the block.
             mlp_ratio: Ratio of mlp hidden dim to embedding dim.
             qkv_bias: If True, add a learnable bias to query, key, value.
             proj_drop: Projection dropout rate
             attn_drop: Attention dropout rate.
             drop_path: Stochastic depth rate.
+            act_layer: Activation layer type.
             norm_layer: Normalization layer.
             pretrained_window_size: Local window size in pretraining.
             output_nchw: Output tensors on NCHW format instead of NHWC.
         """
         super().__init__()
         self.dim = dim
         self.input_resolution = input_resolution
@@ -418,30 +424,31 @@
                 window_size=window_size,
                 shift_size=0 if (i % 2 == 0) else shift_size,
                 mlp_ratio=mlp_ratio,
                 qkv_bias=qkv_bias,
                 proj_drop=proj_drop,
                 attn_drop=attn_drop,
                 drop_path=drop_path[i] if isinstance(drop_path, list) else drop_path,
+                act_layer=act_layer,
                 norm_layer=norm_layer,
                 pretrained_window_size=pretrained_window_size,
             )
             for i in range(depth)])
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         x = self.downsample(x)
 
         for blk in self.blocks:
             if self.grad_checkpointing and not torch.jit.is_scripting():
                 x = checkpoint.checkpoint(blk, x)
             else:
                 x = blk(x)
         return x
 
-    def _init_respostnorm(self):
+    def _init_respostnorm(self) -> None:
         for blk in self.blocks:
             nn.init.constant_(blk.norm1.bias, 0)
             nn.init.constant_(blk.norm1.weight, 0)
             nn.init.constant_(blk.norm2.bias, 0)
             nn.init.constant_(blk.norm2.weight, 0)
 
 
@@ -465,14 +472,15 @@
             window_size: _int_or_tuple_2_t = 7,
             mlp_ratio: float = 4.,
             qkv_bias: bool = True,
             drop_rate: float = 0.,
             proj_drop_rate: float = 0.,
             attn_drop_rate: float = 0.,
             drop_path_rate: float = 0.1,
+            act_layer: Union[str, Callable] = 'gelu',
             norm_layer: Callable = nn.LayerNorm,
             pretrained_window_sizes: Tuple[int, ...] = (0, 0, 0, 0),
             **kwargs,
     ):
         """
         Args:
             img_size: Input image size.
@@ -486,14 +494,15 @@
             mlp_ratio: Ratio of mlp hidden dim to embedding dim.
             qkv_bias: If True, add a learnable bias to query, key, value.
             drop_rate: Head dropout rate.
             proj_drop_rate: Projection dropout rate.
             attn_drop_rate: Attention dropout rate.
             drop_path_rate: Stochastic depth rate.
             norm_layer: Normalization layer.
+            act_layer: Activation layer type.
             patch_norm: If True, add normalization after patch embedding.
             pretrained_window_sizes: Pretrained window sizes of each layer.
             output_fmt: Output tensor format if not None, otherwise output 'NHWC' by default.
         """
         super().__init__()
 
         self.num_classes = num_classes
@@ -535,14 +544,15 @@
                 num_heads=num_heads[i],
                 window_size=window_size,
                 mlp_ratio=mlp_ratio,
                 qkv_bias=qkv_bias,
                 proj_drop=proj_drop_rate,
                 attn_drop=attn_drop_rate,
                 drop_path=dpr[i],
+                act_layer=act_layer,
                 norm_layer=norm_layer,
                 pretrained_window_size=pretrained_window_sizes[i],
             )]
             in_dim = out_dim
             if i > 0:
                 scale *= 2
             self.feature_info += [dict(num_chs=out_dim, reduction=4 * scale, module=f'layers.{i}')]
@@ -591,18 +601,84 @@
         for l in self.layers:
             l.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         self.head.reset(num_classes, global_pool)
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to compatible intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output shape must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.layers), indices)
+
+        # forward pass
+        x = self.patch_embed(x)
+
+        num_stages = len(self.layers)
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            stages = self.layers
+        else:
+            stages = self.layers[:max_index + 1]
+        for i, stage in enumerate(stages):
+            x = stage(x)
+            if i in take_indices:
+                if norm and i == num_stages - 1:
+                    x_inter = self.norm(x)  # applying final norm last intermediate
+                else:
+                    x_inter = x
+                x_inter = x_inter.permute(0, 3, 1, 2).contiguous()
+                intermediates.append(x_inter)
+
+        if intermediates_only:
+            return intermediates
+
+        x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.layers), indices)
+        self.layers = self.layers[:max_index + 1]  # truncate blocks
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.patch_embed(x)
         x = self.layers(x)
         x = self.norm(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
@@ -636,15 +712,15 @@
                 )
 
         if not native_checkpoint:
             # skip layer remapping for updated checkpoints
             k = re.sub(r'layers.(\d+).downsample', lambda x: f'layers.{int(x.group(1)) + 1}.downsample', k)
             k = k.replace('head.', 'head.fc.')
         out_dict[k] = v
-      
+
     return out_dict
 
 
 def _create_swin_transformer_v2(variant, pretrained=False, **kwargs):
     default_out_indices = tuple(i for i, _ in enumerate(kwargs.get('depths', (1, 1, 1, 1))))
     out_indices = kwargs.pop('out_indices', default_out_indices)
```

### Comparing `timm-0.9.9/timm/models/swin_transformer_v2_cr.py` & `timm-1.0.3/timm/models/swin_transformer_v2_cr.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,17 @@
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.checkpoint as checkpoint
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
-from timm.layers import DropPath, Mlp, ClassifierHead, to_2tuple, _assert
+from timm.layers import DropPath, Mlp, ClassifierHead, to_2tuple, _assert, ndgrid
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._features_fx import register_notrace_function
 from ._manipulate import named_apply
 from ._registry import generate_default_cfgs, register_model
 
 __all__ = ['SwinTransformerV2Cr']  # model_registry will add each entrypoint fn to this
 
 _logger = logging.getLogger(__name__)
@@ -137,17 +138,18 @@
         # NOTE old checkpoints used inverse of logit_scale ('tau') following the paper, see conversion fn
         self.logit_scale = nn.Parameter(torch.log(10 * torch.ones(num_heads)))
         self._make_pair_wise_relative_positions()
 
     def _make_pair_wise_relative_positions(self) -> None:
         """Method initializes the pair-wise relative positions to compute the positional biases."""
         device = self.logit_scale.device
-        coordinates = torch.stack(torch.meshgrid([
+        coordinates = torch.stack(ndgrid(
             torch.arange(self.window_size[0], device=device),
-            torch.arange(self.window_size[1], device=device)]), dim=0).flatten(1)
+            torch.arange(self.window_size[1], device=device)
+        ), dim=0).flatten(1)
         relative_coordinates = coordinates[:, :, None] - coordinates[:, None, :]
         relative_coordinates = relative_coordinates.permute(1, 2, 0).reshape(-1, 2).float()
         relative_coordinates_log = torch.sign(relative_coordinates) * torch.log(
             1.0 + relative_coordinates.abs())
         self.register_buffer("relative_coordinates_log", relative_coordinates_log, persistent=False)
 
     def update_input_size(self, new_window_size: int, **kwargs: Any) -> None:
@@ -713,14 +715,70 @@
         Args:
             num_classes (int): Number of classes to be predicted
             global_pool (str): Unused
         """
         self.num_classes = num_classes
         self.head.reset(num_classes, global_pool)
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to compatible intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output shape must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.stages), indices)
+
+        # forward pass
+        x = self.patch_embed(x)
+
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            stages = self.stages
+        else:
+            stages = self.stages[:max_index + 1]
+        for i, stage in enumerate(stages):
+            x = stage(x)
+            if i in take_indices:
+                intermediates.append(x)
+
+        if intermediates_only:
+            return intermediates
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.stages), indices)
+        self.stages = self.stages[:max_index + 1]  # truncate blocks
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x: torch.Tensor) -> torch.Tensor:
         x = self.patch_embed(x)
         x = self.stages(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
         return self.head(x, pre_logits=True) if pre_logits else self.head(x)
```

### Comparing `timm-0.9.9/timm/models/tiny_vit.py` & `timm-1.0.3/timm/models/tiny_vit.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,17 @@
     - https://arxiv.org/abs/2207.10666
 
 Adapted from official impl at https://github.com/microsoft/Cream/tree/main/TinyViT
 """
 
 __all__ = ['TinyVit']
 
-import math
 import itertools
 from functools import partial
-from typing import Dict
+from typing import Dict, Optional
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import LayerNorm2d, NormMlpClassifierHead, DropPath,\
@@ -529,17 +528,17 @@
     def set_grad_checkpointing(self, enable=True):
         self.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
-        self.head.reset(num_classes, global_pool=global_pool)
+        self.head.reset(num_classes, pool_type=global_pool)
 
     def forward_features(self, x):
         x = self.patch_embed(x)
         if self.grad_checkpointing and not torch.jit.is_scripting():
             x = checkpoint_seq(self.stages, x)
         else:
             x = self.stages(x)
```

### Comparing `timm-0.9.9/timm/models/tnt.py` & `timm-1.0.3/timm/models/tnt.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 A PyTorch implement of TNT as described in
 'Transformer in Transformer' - https://arxiv.org/abs/2103.00112
 
 The official mindspore code is released and available at
 https://gitee.com/mindspore/mindspore/tree/master/model_zoo/research/cv/TNT
 """
 import math
+from typing import Optional
 
 import torch
 import torch.nn as nn
 from torch.utils.checkpoint import checkpoint
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import Mlp, DropPath, trunc_normal_, _assert, to_2tuple
@@ -294,15 +295,15 @@
     def set_grad_checkpointing(self, enable=True):
         self.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             assert global_pool in ('', 'token', 'avg')
         self.head = nn.Linear(self.embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
     def forward_features(self, x):
         B = x.shape[0]
```

### Comparing `timm-0.9.9/timm/models/tresnet.py` & `timm-1.0.3/timm/models/tresnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 https://arxiv.org/pdf/2003.13630.pdf
 
 Original model: https://github.com/mrT23/TResNet
 
 """
 from collections import OrderedDict
 from functools import partial
+from typing import Optional
 
 import torch
 import torch.nn as nn
 
 from timm.layers import SpaceToDepth, BlurPool2d, ClassifierHead, SEModule,\
     ConvNormActAa, ConvNormAct, DropPath
 from ._builder import build_model_with_cfg
@@ -229,15 +230,15 @@
     def set_grad_checkpointing(self, enable=True):
         self.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head.fc
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.head.reset(num_classes, pool_type=global_pool)
 
     def forward_features(self, x):
         if self.grad_checkpointing and not torch.jit.is_scripting():
             x = self.body.s2d(x)
             x = self.body.conv1(x)
             x = checkpoint_seq([
@@ -321,34 +322,34 @@
     'tresnet_v2_l.miil_in21k_ft_in1k': _cfg(hf_hub_id='timm/'),
     'tresnet_v2_l.miil_in21k': _cfg(hf_hub_id='timm/', num_classes=11221),
 })
 
 
 @register_model
 def tresnet_m(pretrained=False, **kwargs) -> TResNet:
-    model_kwargs = dict(layers=[3, 4, 11, 3], **kwargs)
-    return _create_tresnet('tresnet_m', pretrained=pretrained, **model_kwargs)
+    model_args = dict(layers=[3, 4, 11, 3])
+    return _create_tresnet('tresnet_m', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def tresnet_l(pretrained=False, **kwargs) -> TResNet:
-    model_kwargs = dict(layers=[4, 5, 18, 3], width_factor=1.2, **kwargs)
-    return _create_tresnet('tresnet_l', pretrained=pretrained, **model_kwargs)
+    model_args = dict(layers=[4, 5, 18, 3], width_factor=1.2)
+    return _create_tresnet('tresnet_l', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def tresnet_xl(pretrained=False, **kwargs) -> TResNet:
-    model_kwargs = dict(layers=[4, 5, 24, 3], width_factor=1.3, **kwargs)
-    return _create_tresnet('tresnet_xl', pretrained=pretrained, **model_kwargs)
+    model_args = dict(layers=[4, 5, 24, 3], width_factor=1.3)
+    return _create_tresnet('tresnet_xl', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def tresnet_v2_l(pretrained=False, **kwargs) -> TResNet:
-    model_kwargs = dict(layers=[3, 4, 23, 3], width_factor=1.0, v2=True, **kwargs)
-    return _create_tresnet('tresnet_v2_l', pretrained=pretrained, **model_kwargs)
+    model_args = dict(layers=[3, 4, 23, 3], width_factor=1.0, v2=True)
+    return _create_tresnet('tresnet_v2_l', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 register_model_deprecations(__name__, {
     'tresnet_m_miil_in21k': 'tresnet_m.miil_in21k',
     'tresnet_m_448': 'tresnet_m.miil_in1k_448',
     'tresnet_l_448': 'tresnet_l.miil_in1k_448',
     'tresnet_xl_448': 'tresnet_xl.miil_in1k_448',
```

### Comparing `timm-0.9.9/timm/models/twins.py` & `timm-1.0.3/timm/models/twins.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 # Twins
 # Copyright (c) 2021 Meituan
 # Licensed under The Apache 2.0 License [see LICENSE for details]
 # Written by Xinjie Li, Xiangxiang Chu
 # --------------------------------------------------------
 import math
 from functools import partial
-from typing import Tuple
+from typing import List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import Mlp, DropPath, to_2tuple, trunc_normal_, use_fused_attn
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._features_fx import register_notrace_module
 from ._registry import register_model, generate_default_cfgs
 from .vision_transformer import Attention
 
 __all__ = ['Twins']  # model_registry will add each entrypoint fn to this
 
 Size_ = Tuple[int, int]
@@ -320,14 +321,15 @@
             self.patch_embeds.append(PatchEmbed(img_size, patch_size, prev_chs, embed_dims[i]))
             self.pos_drops.append(nn.Dropout(p=pos_drop_rate))
             prev_chs = embed_dims[i]
             img_size = tuple(t // patch_size for t in img_size)
             patch_size = 2
 
         self.blocks = nn.ModuleList()
+        self.feature_info = []
         dpr = [x.item() for x in torch.linspace(0, drop_path_rate, sum(depths))]  # stochastic depth decay rule
         cur = 0
         for k in range(len(depths)):
             _block = nn.ModuleList([block_cls(
                 dim=embed_dims[k],
                 num_heads=num_heads[k],
                 mlp_ratio=mlp_ratios[k],
@@ -335,14 +337,15 @@
                 attn_drop=attn_drop_rate,
                 drop_path=dpr[cur + i],
                 norm_layer=norm_layer,
                 sr_ratio=sr_ratios[k],
                 ws=1 if wss is None or i % 2 == 1 else wss[k]) for i in range(depths[k])],
             )
             self.blocks.append(_block)
+            self.feature_info += [dict(module=f'block.{k}', num_chs=embed_dims[k], reduction=2**(2+k))]
             cur += depths[k]
 
         self.pos_block = nn.ModuleList([PosConv(embed_dim, embed_dim) for embed_dim in embed_dims])
 
         self.norm = norm_layer(self.num_features)
 
         # classification head
@@ -375,15 +378,15 @@
     def set_grad_checkpointing(self, enable=True):
         assert not enable, 'gradient checkpointing not supported'
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             assert global_pool in ('', 'avg')
             self.global_pool = global_pool
         self.head = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
 
     def _init_weights(self, m):
@@ -397,14 +400,85 @@
         elif isinstance(m, nn.Conv2d):
             fan_out = m.kernel_size[0] * m.kernel_size[1] * m.out_channels
             fan_out //= m.groups
             m.weight.data.normal_(0, math.sqrt(2.0 / fan_out))
             if m.bias is not None:
                 m.bias.data.zero_()
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to all intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt == 'NCHW', 'Output shape for Twins must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+
+        # FIXME slice block/pos_block if < max
+
+        # forward pass
+        B, _, height, width = x.shape
+        for i, (embed, drop, blocks, pos_blk) in enumerate(zip(
+                self.patch_embeds, self.pos_drops, self.blocks, self.pos_block)
+        ):
+            x, size = embed(x)
+            x = drop(x)
+            for j, blk in enumerate(blocks):
+                x = blk(x, size)
+                if j == 0:
+                    x = pos_blk(x, size)  # PEG here
+
+            if i < len(self.depths) - 1:
+                x = x.reshape(B, *size, -1).permute(0, 3, 1, 2).contiguous()
+                if i in take_indices:
+                    intermediates.append(x)
+            else:
+                if i in take_indices:
+                    # only last feature can be normed
+                    x_feat = self.norm(x) if norm else x
+                    intermediates.append(x_feat.reshape(B, *size, -1).permute(0, 3, 1, 2).contiguous())
+
+        if intermediates_only:
+            return intermediates
+
+        x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+        # FIXME add block pruning
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         B = x.shape[0]
         for i, (embed, drop, blocks, pos_blk) in enumerate(
                 zip(self.patch_embeds, self.pos_drops, self.blocks, self.pos_block)):
             x, size = embed(x)
             x = drop(x)
             for j, blk in enumerate(blocks):
@@ -425,18 +499,20 @@
     def forward(self, x):
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
 def _create_twins(variant, pretrained=False, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError('features_only not implemented for Vision Transformer models.')
-
-    model = build_model_with_cfg(Twins, variant, pretrained, **kwargs)
+    out_indices = kwargs.pop('out_indices', 4)
+    model = build_model_with_cfg(
+        Twins, variant, pretrained,
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
+        **kwargs,
+    )
     return model
 
 
 def _cfg(url='', **kwargs):
     return {
         'url': url,
         'num_classes': 1000, 'input_size': (3, 224, 224), 'pool_size': None,
```

### Comparing `timm-0.9.9/timm/models/vgg.py` & `timm-1.0.3/timm/models/vgg.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/visformer.py` & `timm-1.0.3/timm/models/visformer.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/vision_transformer.py` & `timm-1.0.3/timm/models/vision_transformer.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,65 +23,70 @@
 
 Hacked together by / Copyright 2020, Ross Wightman
 """
 import logging
 import math
 from collections import OrderedDict
 from functools import partial
-from typing import Callable, List, Optional, Sequence, Tuple, Type, Union
+from typing import Any, Callable, Dict, Optional, Set, Tuple, Type, Union, List
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.checkpoint
 from torch.jit import Final
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD, IMAGENET_INCEPTION_MEAN, IMAGENET_INCEPTION_STD, \
     OPENAI_CLIP_MEAN, OPENAI_CLIP_STD
 from timm.layers import PatchEmbed, Mlp, DropPath, AttentionPoolLatent, RmsNorm, PatchDropout, SwiGLUPacked, \
     trunc_normal_, lecun_normal_, resample_patch_embed, resample_abs_pos_embed, use_fused_attn, \
     get_act_layer, get_norm_layer, LayerType
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._manipulate import named_apply, checkpoint_seq, adapt_input_conv
 from ._registry import generate_default_cfgs, register_model, register_model_deprecations
 
 __all__ = ['VisionTransformer']  # model_registry will add each entrypoint fn to this
 
 
 _logger = logging.getLogger(__name__)
 
 
 class Attention(nn.Module):
     fused_attn: Final[bool]
 
     def __init__(
             self,
-            dim,
-            num_heads=8,
-            qkv_bias=False,
-            qk_norm=False,
-            attn_drop=0.,
-            proj_drop=0.,
-            norm_layer=nn.LayerNorm,
-    ):
+            dim: int,
+            num_heads: int = 8,
+            qkv_bias: bool = False,
+            qk_norm: bool = False,
+            attn_drop: float = 0.,
+            proj_drop: float = 0.,
+            norm_layer: nn.Module = nn.LayerNorm,
+    ) -> None:
         super().__init__()
         assert dim % num_heads == 0, 'dim should be divisible by num_heads'
         self.num_heads = num_heads
         self.head_dim = dim // num_heads
         self.scale = self.head_dim ** -0.5
         self.fused_attn = use_fused_attn()
 
         self.qkv = nn.Linear(dim, dim * 3, bias=qkv_bias)
         self.q_norm = norm_layer(self.head_dim) if qk_norm else nn.Identity()
         self.k_norm = norm_layer(self.head_dim) if qk_norm else nn.Identity()
         self.attn_drop = nn.Dropout(attn_drop)
         self.proj = nn.Linear(dim, dim)
         self.proj_drop = nn.Dropout(proj_drop)
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         B, N, C = x.shape
         qkv = self.qkv(x).reshape(B, N, 3, self.num_heads, self.head_dim).permute(2, 0, 3, 1, 4)
         q, k, v = qkv.unbind(0)
         q, k = self.q_norm(q), self.k_norm(k)
 
         if self.fused_attn:
             x = F.scaled_dot_product_attention(
@@ -98,40 +103,44 @@
         x = x.transpose(1, 2).reshape(B, N, C)
         x = self.proj(x)
         x = self.proj_drop(x)
         return x
 
 
 class LayerScale(nn.Module):
-    def __init__(self, dim, init_values=1e-5, inplace=False):
+    def __init__(
+            self,
+            dim: int,
+            init_values: float = 1e-5,
+            inplace: bool = False,
+    ) -> None:
         super().__init__()
         self.inplace = inplace
         self.gamma = nn.Parameter(init_values * torch.ones(dim))
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         return x.mul_(self.gamma) if self.inplace else x * self.gamma
 
 
 class Block(nn.Module):
-
     def __init__(
             self,
-            dim,
-            num_heads,
-            mlp_ratio=4.,
-            qkv_bias=False,
-            qk_norm=False,
-            proj_drop=0.,
-            attn_drop=0.,
-            init_values=None,
-            drop_path=0.,
-            act_layer=nn.GELU,
-            norm_layer=nn.LayerNorm,
-            mlp_layer=Mlp,
-    ):
+            dim: int,
+            num_heads: int,
+            mlp_ratio: float = 4.,
+            qkv_bias: bool = False,
+            qk_norm: bool = False,
+            proj_drop: float = 0.,
+            attn_drop: float = 0.,
+            init_values: Optional[float] = None,
+            drop_path: float = 0.,
+            act_layer: nn.Module = nn.GELU,
+            norm_layer: nn.Module = nn.LayerNorm,
+            mlp_layer: nn.Module = Mlp,
+    ) -> None:
         super().__init__()
         self.norm1 = norm_layer(dim)
         self.attn = Attention(
             dim,
             num_heads=num_heads,
             qkv_bias=qkv_bias,
             qk_norm=qk_norm,
@@ -148,37 +157,36 @@
             hidden_features=int(dim * mlp_ratio),
             act_layer=act_layer,
             drop=proj_drop,
         )
         self.ls2 = LayerScale(dim, init_values=init_values) if init_values else nn.Identity()
         self.drop_path2 = DropPath(drop_path) if drop_path > 0. else nn.Identity()
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         x = x + self.drop_path1(self.ls1(self.attn(self.norm1(x))))
         x = x + self.drop_path2(self.ls2(self.mlp(self.norm2(x))))
         return x
 
 
 class ResPostBlock(nn.Module):
-
     def __init__(
             self,
-            dim,
-            num_heads,
-            mlp_ratio=4.,
-            qkv_bias=False,
-            qk_norm=False,
-            proj_drop=0.,
-            attn_drop=0.,
-            init_values=None,
-            drop_path=0.,
-            act_layer=nn.GELU,
-            norm_layer=nn.LayerNorm,
-            mlp_layer=Mlp,
-    ):
+            dim: int,
+            num_heads: int,
+            mlp_ratio: float = 4.,
+            qkv_bias: bool = False,
+            qk_norm: bool = False,
+            proj_drop: float = 0.,
+            attn_drop: float = 0.,
+            init_values: Optional[float] = None,
+            drop_path: float = 0.,
+            act_layer: nn.Module = nn.GELU,
+            norm_layer: nn.Module = nn.LayerNorm,
+            mlp_layer: nn.Module = Mlp,
+    ) -> None:
         super().__init__()
         self.init_values = init_values
 
         self.attn = Attention(
             dim,
             num_heads=num_heads,
             qkv_bias=qkv_bias,
@@ -197,48 +205,48 @@
             drop=proj_drop,
         )
         self.norm2 = norm_layer(dim)
         self.drop_path2 = DropPath(drop_path) if drop_path > 0. else nn.Identity()
 
         self.init_weights()
 
-    def init_weights(self):
+    def init_weights(self) -> None:
         # NOTE this init overrides that base model init with specific changes for the block type
         if self.init_values is not None:
             nn.init.constant_(self.norm1.weight, self.init_values)
             nn.init.constant_(self.norm2.weight, self.init_values)
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         x = x + self.drop_path1(self.norm1(self.attn(x)))
         x = x + self.drop_path2(self.norm2(self.mlp(x)))
         return x
 
 
 class ParallelScalingBlock(nn.Module):
     """ Parallel ViT block (MLP & Attention in parallel)
     Based on:
       'Scaling Vision Transformers to 22 Billion Parameters` - https://arxiv.org/abs/2302.05442
     """
     fused_attn: Final[bool]
 
     def __init__(
             self,
-            dim,
-            num_heads,
-            mlp_ratio=4.,
-            qkv_bias=False,
-            qk_norm=False,
-            proj_drop=0.,
-            attn_drop=0.,
-            init_values=None,
-            drop_path=0.,
-            act_layer=nn.GELU,
-            norm_layer=nn.LayerNorm,
-            mlp_layer=None,  # NOTE: not used
-    ):
+            dim: int,
+            num_heads: int,
+            mlp_ratio: float = 4.,
+            qkv_bias: bool = False,
+            qk_norm: bool = False,
+            proj_drop: float = 0.,
+            attn_drop: float = 0.,
+            init_values: Optional[float] = None,
+            drop_path: float = 0.,
+            act_layer: nn.Module = nn.GELU,
+            norm_layer: nn.Module = nn.LayerNorm,
+            mlp_layer: Optional[nn.Module] = None,
+    ) -> None:
         super().__init__()
         assert dim % num_heads == 0, 'dim should be divisible by num_heads'
         self.num_heads = num_heads
         self.head_dim = dim // num_heads
         self.scale = self.head_dim ** -0.5
         self.fused_attn = use_fused_attn()
         mlp_hidden_dim = int(mlp_ratio * dim)
@@ -262,15 +270,15 @@
         self.mlp_drop = nn.Dropout(proj_drop)
         self.mlp_act = act_layer()
         self.mlp_out_proj = nn.Linear(mlp_hidden_dim, dim)
 
         self.ls = LayerScale(dim, init_values=init_values) if init_values is not None else nn.Identity()
         self.drop_path = DropPath(drop_path) if drop_path > 0. else nn.Identity()
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         B, N, C = x.shape
 
         # Combined MLP fc1 & qkv projections
         y = self.in_norm(x)
         if self.mlp_bias is not None:
             # Concat constant zero-bias for qkv w/ trainable mlp_bias.
             # Appears faster than adding to x_mlp separately
@@ -311,28 +319,28 @@
 class ParallelThingsBlock(nn.Module):
     """ Parallel ViT block (N parallel attention followed by N parallel MLP)
     Based on:
       `Three things everyone should know about Vision Transformers` - https://arxiv.org/abs/2203.09795
     """
     def __init__(
             self,
-            dim,
-            num_heads,
-            num_parallel=2,
-            mlp_ratio=4.,
-            qkv_bias=False,
-            qk_norm=False,
-            init_values=None,
-            proj_drop=0.,
-            attn_drop=0.,
-            drop_path=0.,
-            act_layer=nn.GELU,
-            norm_layer=nn.LayerNorm,
-            mlp_layer=Mlp,
-    ):
+            dim: int,
+            num_heads: int,
+            num_parallel: int = 2,
+            mlp_ratio: float = 4.,
+            qkv_bias: bool = False,
+            qk_norm: bool = False,
+            init_values: Optional[float] = None,
+            proj_drop: float = 0.,
+            attn_drop: float = 0.,
+            drop_path: float = 0.,
+            act_layer: nn.Module = nn.GELU,
+            norm_layer: nn.Module = nn.LayerNorm,
+            mlp_layer: nn.Module = Mlp,
+    ) -> None:
         super().__init__()
         self.num_parallel = num_parallel
         self.attns = nn.ModuleList()
         self.ffns = nn.ModuleList()
         for _ in range(num_parallel):
             self.attns.append(nn.Sequential(OrderedDict([
                 ('norm', norm_layer(dim)),
@@ -356,26 +364,26 @@
                     act_layer=act_layer,
                     drop=proj_drop,
                 )),
                 ('ls', LayerScale(dim, init_values=init_values) if init_values else nn.Identity()),
                 ('drop_path', DropPath(drop_path) if drop_path > 0. else nn.Identity())
             ])))
 
-    def _forward_jit(self, x):
+    def _forward_jit(self, x: torch.Tensor) -> torch.Tensor:
         x = x + torch.stack([attn(x) for attn in self.attns]).sum(dim=0)
         x = x + torch.stack([ffn(x) for ffn in self.ffns]).sum(dim=0)
         return x
 
     @torch.jit.ignore
-    def _forward(self, x):
+    def _forward(self, x: torch.Tensor) -> torch.Tensor:
         x = x + sum(attn(x) for attn in self.attns)
         x = x + sum(ffn(x) for ffn in self.ffns)
         return x
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         if torch.jit.is_scripting() or torch.jit.is_tracing():
             return self._forward_jit(x)
         else:
             return self._forward(x)
 
 
 class VisionTransformer(nn.Module):
@@ -388,15 +396,15 @@
 
     def __init__(
             self,
             img_size: Union[int, Tuple[int, int]] = 224,
             patch_size: Union[int, Tuple[int, int]] = 16,
             in_chans: int = 3,
             num_classes: int = 1000,
-            global_pool: str = 'token',
+            global_pool: Literal['', 'avg', 'token', 'map'] = 'token',
             embed_dim: int = 768,
             depth: int = 12,
             num_heads: int = 12,
             mlp_ratio: float = 4.,
             qkv_bias: bool = True,
             qk_norm: bool = False,
             init_values: Optional[float] = None,
@@ -409,21 +417,22 @@
             dynamic_img_pad: bool = False,
             drop_rate: float = 0.,
             pos_drop_rate: float = 0.,
             patch_drop_rate: float = 0.,
             proj_drop_rate: float = 0.,
             attn_drop_rate: float = 0.,
             drop_path_rate: float = 0.,
-            weight_init: str = '',
+            weight_init: Literal['skip', 'jax', 'jax_nlhb', 'moco', ''] = '',
+            fix_init: bool = False,
             embed_layer: Callable = PatchEmbed,
             norm_layer: Optional[LayerType] = None,
             act_layer: Optional[LayerType] = None,
             block_fn: Type[nn.Module] = Block,
             mlp_layer: Type[nn.Module] = Mlp,
-    ):
+    ) -> None:
         """
         Args:
             img_size: Input image size.
             patch_size: Patch size.
             in_chans: Number of image input channels.
             num_classes: Mumber of classes for classification head.
             global_pool: Type of global pooling for final sequence (default: 'token').
@@ -438,14 +447,15 @@
             reg_tokens: Number of register tokens.
             fc_norm: Pre head norm after pool (instead of before), if None, enabled when global_pool == 'avg'.
             drop_rate: Head dropout rate.
             pos_drop_rate: Position embedding dropout rate.
             attn_drop_rate: Attention dropout rate.
             drop_path_rate: Stochastic depth rate.
             weight_init: Weight initialization scheme.
+            fix_init: Apply weight initialization fix (scaling w/ layer index).
             embed_layer: Patch embedding layer.
             norm_layer: Normalization layer.
             act_layer: MLP activation layer.
             block_fn: Transformer block layer.
         """
         super().__init__()
         assert global_pool in ('', 'avg', 'token', 'map')
@@ -475,14 +485,15 @@
             in_chans=in_chans,
             embed_dim=embed_dim,
             bias=not pre_norm,  # disable bias if pre-norm is used (e.g. CLIP)
             dynamic_img_pad=dynamic_img_pad,
             **embed_args,
         )
         num_patches = self.patch_embed.num_patches
+        reduction = self.patch_embed.feat_ratio() if hasattr(self.patch_embed, 'feat_ratio') else patch_size
 
         self.cls_token = nn.Parameter(torch.zeros(1, 1, embed_dim)) if class_token else None
         self.reg_token = nn.Parameter(torch.zeros(1, reg_tokens, embed_dim)) if reg_tokens else None
         embed_len = num_patches if no_embed_class else num_patches + self.num_prefix_tokens
         self.pos_embed = nn.Parameter(torch.randn(1, embed_len, embed_dim) * .02)
         self.pos_drop = nn.Dropout(p=pos_drop_rate)
         if patch_drop_rate > 0:
@@ -507,14 +518,16 @@
                 attn_drop=attn_drop_rate,
                 drop_path=dpr[i],
                 norm_layer=norm_layer,
                 act_layer=act_layer,
                 mlp_layer=mlp_layer,
             )
             for i in range(depth)])
+        self.feature_info = [
+            dict(module=f'blocks.{i}', num_chs=embed_dim, reduction=reduction) for i in range(depth)]
         self.norm = norm_layer(embed_dim) if not use_fc_norm else nn.Identity()
 
         # Classifier Head
         if global_pool == 'map':
             self.attn_pool = AttentionPoolLatent(
                 self.embed_dim,
                 num_heads=num_heads,
@@ -525,62 +538,72 @@
             self.attn_pool = None
         self.fc_norm = norm_layer(embed_dim) if use_fc_norm else nn.Identity()
         self.head_drop = nn.Dropout(drop_rate)
         self.head = nn.Linear(self.embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
         if weight_init != 'skip':
             self.init_weights(weight_init)
+        if fix_init:
+            self.fix_init_weight()
 
-    def init_weights(self, mode=''):
+    def fix_init_weight(self):
+        def rescale(param, _layer_id):
+            param.div_(math.sqrt(2.0 * _layer_id))
+
+        for layer_id, layer in enumerate(self.blocks):
+            rescale(layer.attn.proj.weight.data, layer_id + 1)
+            rescale(layer.mlp.fc2.weight.data, layer_id + 1)
+
+    def init_weights(self, mode: str = '') -> None:
         assert mode in ('jax', 'jax_nlhb', 'moco', '')
         head_bias = -math.log(self.num_classes) if 'nlhb' in mode else 0.
         trunc_normal_(self.pos_embed, std=.02)
         if self.cls_token is not None:
             nn.init.normal_(self.cls_token, std=1e-6)
         named_apply(get_init_weights_vit(mode, head_bias), self)
 
-    def _init_weights(self, m):
+    def _init_weights(self, m: nn.Module) -> None:
         # this fn left here for compat with downstream users
         init_weights_vit_timm(m)
 
     @torch.jit.ignore()
-    def load_pretrained(self, checkpoint_path, prefix=''):
+    def load_pretrained(self, checkpoint_path: str, prefix: str = '') -> None:
         _load_weights(self, checkpoint_path, prefix)
 
     @torch.jit.ignore
-    def no_weight_decay(self):
+    def no_weight_decay(self) -> Set:
         return {'pos_embed', 'cls_token', 'dist_token'}
 
     @torch.jit.ignore
-    def group_matcher(self, coarse=False):
+    def group_matcher(self, coarse: bool = False) -> Dict:
         return dict(
             stem=r'^cls_token|pos_embed|patch_embed',  # stem and embed
             blocks=[(r'^blocks\.(\d+)', None), (r'^norm', (99999,))]
         )
 
     @torch.jit.ignore
-    def set_grad_checkpointing(self, enable=True):
+    def set_grad_checkpointing(self, enable: bool = True) -> None:
         self.grad_checkpointing = enable
 
     @torch.jit.ignore
-    def get_classifier(self):
+    def get_classifier(self) -> nn.Module:
         return self.head
 
-    def reset_classifier(self, num_classes: int, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool = None) -> None:
         self.num_classes = num_classes
         if global_pool is not None:
             assert global_pool in ('', 'avg', 'token', 'map')
             if global_pool == 'map' and self.attn_pool is None:
                 assert False, "Cannot currently add attention pooling in reset_classifier()."
             elif global_pool != 'map ' and self.attn_pool is not None:
                 self.attn_pool = None  # remove attention pooling
             self.global_pool = global_pool
         self.head = nn.Linear(self.embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
-    def _pos_embed(self, x):
+    def _pos_embed(self, x: torch.Tensor) -> torch.Tensor:
         if self.dynamic_img_size:
             B, H, W, C = x.shape
             pos_embed = resample_abs_pos_embed(
                 self.pos_embed,
                 (H, W),
                 num_prefix_tokens=0 if self.no_embed_class else self.num_prefix_tokens,
             )
@@ -605,103 +628,155 @@
             # pos_embed has entry for class token, concat then add
             if to_cat:
                 x = torch.cat(to_cat + [x], dim=1)
             x = x + pos_embed
 
         return self.pos_drop(x)
 
-    def _intermediate_layers(
+    def forward_intermediates(
             self,
             x: torch.Tensor,
-            n: Union[int, Sequence] = 1,
-    ):
-        outputs, num_blocks = [], len(self.blocks)
-        take_indices = set(range(num_blocks - n, num_blocks) if isinstance(n, int) else n)
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            return_prefix_tokens: bool = False,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            return_prefix_tokens: Return both prefix and spatial intermediate tokens
+            norm: Apply norm layer to all intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW', 'NLC'), 'Output format must be one of NCHW or NLC.'
+        reshape = output_fmt == 'NCHW'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
 
         # forward pass
+        B, _, height, width = x.shape
         x = self.patch_embed(x)
         x = self._pos_embed(x)
         x = self.patch_drop(x)
         x = self.norm_pre(x)
-        for i, blk in enumerate(self.blocks):
+
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            blocks = self.blocks
+        else:
+            blocks = self.blocks[:max_index + 1]
+        for i, blk in enumerate(blocks):
             x = blk(x)
             if i in take_indices:
-                outputs.append(x)
+                # normalize intermediates with final norm layer if enabled
+                intermediates.append(self.norm(x) if norm else x)
+
+        # process intermediates
+        if self.num_prefix_tokens:
+            # split prefix (e.g. class, distill) and spatial feature tokens
+            prefix_tokens = [y[:, 0:self.num_prefix_tokens] for y in intermediates]
+            intermediates = [y[:, self.num_prefix_tokens:] for y in intermediates]
+        if reshape:
+            # reshape to BCHW output format
+            H, W = self.patch_embed.dynamic_feat_size((height, width))
+            intermediates = [y.reshape(B, H, W, -1).permute(0, 3, 1, 2).contiguous() for y in intermediates]
+        if not torch.jit.is_scripting() and return_prefix_tokens:
+            # return_prefix not support in torchscript due to poor type handling
+            intermediates = list(zip(intermediates, prefix_tokens))
+
+        if intermediates_only:
+            return intermediates
+
+        x = self.norm(x)
+
+        return x, intermediates
 
-        return outputs
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+        self.blocks = self.blocks[:max_index + 1]  # truncate blocks
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.fc_norm = nn.Identity()
+            self.reset_classifier(0, '')
+        return take_indices
 
     def get_intermediate_layers(
             self,
             x: torch.Tensor,
-            n: Union[int, Sequence] = 1,
+            n: Union[int, List[int], Tuple[int]] = 1,
             reshape: bool = False,
             return_prefix_tokens: bool = False,
             norm: bool = False,
-    ) -> Tuple[Union[torch.Tensor, Tuple[torch.Tensor]]]:
-        """ Intermediate layer accessor (NOTE: This is a WIP experiment).
-        Inspired by DINO / DINOv2 interface
+    ) -> List[torch.Tensor]:
+        """ Intermediate layer accessor inspired by DINO / DINOv2 interface.
+        NOTE: This API is for backwards compat, favour using forward_intermediates() directly.
         """
-        # take last n blocks if n is an int, if in is a sequence, select by matching indices
-        outputs = self._intermediate_layers(x, n)
-        if norm:
-            outputs = [self.norm(out) for out in outputs]
-        prefix_tokens = [out[:, 0:self.num_prefix_tokens] for out in outputs]
-        outputs = [out[:, self.num_prefix_tokens:] for out in outputs]
-
-        if reshape:
-            grid_size = self.patch_embed.grid_size
-            outputs = [
-                out.reshape(x.shape[0], grid_size[0], grid_size[1], -1).permute(0, 3, 1, 2).contiguous()
-                for out in outputs
-            ]
-
-        if return_prefix_tokens:
-            return tuple(zip(outputs, prefix_tokens))
-        return tuple(outputs)
+        return self.forward_intermediates(
+            x, n,
+            return_prefix_tokens=return_prefix_tokens,
+            norm=norm,
+            output_fmt='NCHW' if reshape else 'NLC',
+            intermediates_only=True,
+        )
 
-    def forward_features(self, x):
+    def forward_features(self, x: torch.Tensor) -> torch.Tensor:
         x = self.patch_embed(x)
         x = self._pos_embed(x)
         x = self.patch_drop(x)
         x = self.norm_pre(x)
         if self.grad_checkpointing and not torch.jit.is_scripting():
             x = checkpoint_seq(self.blocks, x)
         else:
             x = self.blocks(x)
         x = self.norm(x)
         return x
 
-    def forward_head(self, x, pre_logits: bool = False):
+    def forward_head(self, x: torch.Tensor, pre_logits: bool = False) -> torch.Tensor:
         if self.attn_pool is not None:
             x = self.attn_pool(x)
         elif self.global_pool == 'avg':
             x = x[:, self.num_prefix_tokens:].mean(dim=1)
         elif self.global_pool:
             x = x[:, 0]  # class token
         x = self.fc_norm(x)
         x = self.head_drop(x)
         return x if pre_logits else self.head(x)
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
-def init_weights_vit_timm(module: nn.Module, name: str = ''):
+def init_weights_vit_timm(module: nn.Module, name: str = '') -> None:
     """ ViT weight initialization, original timm impl (for reproducibility) """
     if isinstance(module, nn.Linear):
         trunc_normal_(module.weight, std=.02)
         if module.bias is not None:
             nn.init.zeros_(module.bias)
     elif hasattr(module, 'init_weights'):
         module.init_weights()
 
 
-def init_weights_vit_jax(module: nn.Module, name: str = '', head_bias: float = 0.):
+def init_weights_vit_jax(module: nn.Module, name: str = '', head_bias: float = 0.0) -> None:
     """ ViT weight initialization, matching JAX (Flax) impl """
     if isinstance(module, nn.Linear):
         if name.startswith('head'):
             nn.init.zeros_(module.weight)
             nn.init.constant_(module.bias, head_bias)
         else:
             nn.init.xavier_uniform_(module.weight)
@@ -711,78 +786,72 @@
         lecun_normal_(module.weight)
         if module.bias is not None:
             nn.init.zeros_(module.bias)
     elif hasattr(module, 'init_weights'):
         module.init_weights()
 
 
-def init_weights_vit_moco(module: nn.Module, name: str = ''):
+def init_weights_vit_moco(module: nn.Module, name: str = '') -> None:
     """ ViT weight initialization, matching moco-v3 impl minus fixed PatchEmbed """
     if isinstance(module, nn.Linear):
         if 'qkv' in name:
             # treat the weights of Q, K, V separately
             val = math.sqrt(6. / float(module.weight.shape[0] // 3 + module.weight.shape[1]))
             nn.init.uniform_(module.weight, -val, val)
         else:
             nn.init.xavier_uniform_(module.weight)
         if module.bias is not None:
             nn.init.zeros_(module.bias)
     elif hasattr(module, 'init_weights'):
         module.init_weights()
 
 
-def get_init_weights_vit(mode='jax', head_bias: float = 0.):
+def get_init_weights_vit(mode: str = 'jax', head_bias: float = 0.0) -> Callable:
     if 'jax' in mode:
         return partial(init_weights_vit_jax, head_bias=head_bias)
     elif 'moco' in mode:
         return init_weights_vit_moco
     else:
         return init_weights_vit_timm
 
 
 def resize_pos_embed(
-        posemb,
-        posemb_new,
-        num_prefix_tokens=1,
-        gs_new=(),
-        interpolation='bicubic',
-        antialias=False,
-):
+        posemb: torch.Tensor,
+        posemb_new: torch.Tensor,
+        num_prefix_tokens: int = 1,
+        gs_new: Tuple[int, int] = (),
+        interpolation: str = 'bicubic',
+        antialias: bool = False,
+) -> torch.Tensor:
     """ Rescale the grid of position embeddings when loading from state_dict.
-
-    *DEPRECATED* This function is being deprecated in favour of resample_abs_pos_embed
-
-    Adapted from:
-        https://github.com/google-research/vision_transformer/blob/00883dd691c63a6830751563748663526e811cee/vit_jax/checkpoint.py#L224
+    *DEPRECATED* This function is being deprecated in favour of using resample_abs_pos_embed
     """
-    ntok_new = posemb_new.shape[1]
-    if num_prefix_tokens:
-        posemb_prefix, posemb_grid = posemb[:, :num_prefix_tokens], posemb[0, num_prefix_tokens:]
-        ntok_new -= num_prefix_tokens
-    else:
-        posemb_prefix, posemb_grid = posemb[:, :0], posemb[0]
-    gs_old = int(math.sqrt(len(posemb_grid)))
+    ntok_new = posemb_new.shape[1] - num_prefix_tokens
+    ntok_old = posemb.shape[1] - num_prefix_tokens
+    gs_old = [int(math.sqrt(ntok_old))] * 2
     if not len(gs_new):  # backwards compatibility
         gs_new = [int(math.sqrt(ntok_new))] * 2
-    assert len(gs_new) >= 2
-    _logger.info(f'Resized position embedding: {posemb.shape} ({[gs_old, gs_old]}) to {posemb_new.shape} ({gs_new}).')
-    posemb_grid = posemb_grid.reshape(1, gs_old, gs_old, -1).permute(0, 3, 1, 2)
-    posemb_grid = F.interpolate(posemb_grid, size=gs_new, mode=interpolation, antialias=antialias, align_corners=False)
-    posemb_grid = posemb_grid.permute(0, 2, 3, 1).reshape(1, gs_new[0] * gs_new[1], -1)
-    posemb = torch.cat([posemb_prefix, posemb_grid], dim=1)
-    return posemb
+    return resample_abs_pos_embed(
+        posemb, gs_new, gs_old,
+        num_prefix_tokens=num_prefix_tokens,
+        interpolation=interpolation,
+        antialias=antialias,
+        verbose=True,
+    )
 
 
 @torch.no_grad()
-def _load_weights(model: VisionTransformer, checkpoint_path: str, prefix: str = ''):
+def _load_weights(model: VisionTransformer, checkpoint_path: str, prefix: str = '') -> None:
     """ Load weights from .npz checkpoints for official Google Brain Flax implementation
     """
     import numpy as np
 
-    def _n2p(w, t=True):
+    def _n2p(w, t=True, idx=None):
+        if idx is not None:
+            w = w[idx]
         if w.ndim == 4 and w.shape[0] == w.shape[1] == w.shape[2] == 1:
             w = w.flatten()
         if t:
             if w.ndim == 4:
                 w = w.transpose([3, 2, 0, 1])
             elif w.ndim == 3:
                 w = w.transpose([2, 0, 1])
@@ -884,37 +953,55 @@
         model.attn_pool.norm.bias.copy_(_n2p(w[f'{block_prefix}LayerNorm_0/bias']))
         for r in range(2):
             getattr(model.attn_pool.mlp, f'fc{r + 1}').weight.copy_(_n2p(w[f'{block_prefix}MlpBlock_0/Dense_{r}/kernel']))
             getattr(model.attn_pool.mlp, f'fc{r + 1}').bias.copy_(_n2p(w[f'{block_prefix}MlpBlock_0/Dense_{r}/bias']))
 
     mha_sub, b_sub, ln1_sub = (0, 0, 1) if big_vision else (1, 3, 2)
     for i, block in enumerate(model.blocks.children()):
-        block_prefix = f'{prefix}Transformer/encoderblock_{i}/'
+        if f'{prefix}Transformer/encoderblock/LayerNorm_0/scale' in w:
+            block_prefix = f'{prefix}Transformer/encoderblock/'
+            idx = i
+        else:
+            block_prefix = f'{prefix}Transformer/encoderblock_{i}/'
+            idx = None
         mha_prefix = block_prefix + f'MultiHeadDotProductAttention_{mha_sub}/'
-        block.norm1.weight.copy_(_n2p(w[f'{block_prefix}LayerNorm_0/scale']))
-        block.norm1.bias.copy_(_n2p(w[f'{block_prefix}LayerNorm_0/bias']))
+        block.norm1.weight.copy_(_n2p(w[f'{block_prefix}LayerNorm_0/scale'], idx=idx))
+        block.norm1.bias.copy_(_n2p(w[f'{block_prefix}LayerNorm_0/bias'], idx=idx))
         block.attn.qkv.weight.copy_(torch.cat([
-            _n2p(w[f'{mha_prefix}{n}/kernel'], t=False).flatten(1).T for n in ('query', 'key', 'value')]))
+            _n2p(w[f'{mha_prefix}{n}/kernel'], t=False, idx=idx).flatten(1).T for n in ('query', 'key', 'value')]))
         block.attn.qkv.bias.copy_(torch.cat([
-            _n2p(w[f'{mha_prefix}{n}/bias'], t=False).reshape(-1) for n in ('query', 'key', 'value')]))
-        block.attn.proj.weight.copy_(_n2p(w[f'{mha_prefix}out/kernel']).flatten(1))
-        block.attn.proj.bias.copy_(_n2p(w[f'{mha_prefix}out/bias']))
-        block.norm2.weight.copy_(_n2p(w[f'{block_prefix}LayerNorm_{ln1_sub}/scale']))
-        block.norm2.bias.copy_(_n2p(w[f'{block_prefix}LayerNorm_{ln1_sub}/bias']))
+            _n2p(w[f'{mha_prefix}{n}/bias'], t=False, idx=idx).reshape(-1) for n in ('query', 'key', 'value')]))
+        block.attn.proj.weight.copy_(_n2p(w[f'{mha_prefix}out/kernel'], idx=idx).flatten(1))
+        block.attn.proj.bias.copy_(_n2p(w[f'{mha_prefix}out/bias'], idx=idx))
+        block.norm2.weight.copy_(_n2p(w[f'{block_prefix}LayerNorm_{ln1_sub}/scale'], idx=idx))
+        block.norm2.bias.copy_(_n2p(w[f'{block_prefix}LayerNorm_{ln1_sub}/bias'], idx=idx))
         for r in range(2):
-            getattr(block.mlp, f'fc{r + 1}').weight.copy_(_n2p(w[f'{block_prefix}MlpBlock_{b_sub}/Dense_{r}/kernel']))
-            getattr(block.mlp, f'fc{r + 1}').bias.copy_(_n2p(w[f'{block_prefix}MlpBlock_{b_sub}/Dense_{r}/bias']))
+            getattr(block.mlp, f'fc{r + 1}').weight.copy_(
+                _n2p(w[f'{block_prefix}MlpBlock_{b_sub}/Dense_{r}/kernel'], idx=idx))
+            getattr(block.mlp, f'fc{r + 1}').bias.copy_(
+                _n2p(w[f'{block_prefix}MlpBlock_{b_sub}/Dense_{r}/bias'], idx=idx))
 
 
-def _convert_openai_clip(state_dict, model, prefix='visual.'):
+def _convert_openai_clip(
+        state_dict: Dict[str, torch.Tensor],
+        model: VisionTransformer,
+        prefix: str = 'visual.',
+) -> Dict[str, torch.Tensor]:
     out_dict = {}
     swaps = [
-        ('conv1', 'patch_embed.proj'), ('positional_embedding', 'pos_embed'),
-        ('transformer.resblocks.', 'blocks.'), ('ln_pre', 'norm_pre'), ('ln_post', 'norm'), ('ln_', 'norm'),
-        ('in_proj_', 'qkv.'), ('out_proj', 'proj'), ('mlp.c_fc', 'mlp.fc1'), ('mlp.c_proj', 'mlp.fc2'),
+        ('conv1', 'patch_embed.proj'),
+        ('positional_embedding', 'pos_embed'),
+        ('transformer.resblocks.', 'blocks.'),
+        ('ln_pre', 'norm_pre'),
+        ('ln_post', 'norm'),
+        ('ln_', 'norm'),
+        ('in_proj_', 'qkv.'),
+        ('out_proj', 'proj'),
+        ('mlp.c_fc', 'mlp.fc1'),
+        ('mlp.c_proj', 'mlp.fc2'),
     ]
     for k, v in state_dict.items():
         if not k.startswith(prefix):
             continue
         k = k.replace(prefix, '')
         for sp in swaps:
             k = k.replace(sp[0], sp[1])
@@ -924,27 +1011,22 @@
             v = v.transpose(0, 1)
             out_dict['head.bias'] = torch.zeros(v.shape[0])
         elif k == 'class_embedding':
             k = 'cls_token'
             v = v.unsqueeze(0).unsqueeze(1)
         elif k == 'pos_embed':
             v = v.unsqueeze(0)
-            if v.shape[1] != model.pos_embed.shape[1]:
-                # To resize pos embedding when using model at different size from pretrained weights
-                v = resize_pos_embed(
-                    v,
-                    model.pos_embed,
-                    0 if getattr(model, 'no_embed_class') else getattr(model, 'num_prefix_tokens', 1),
-                    model.patch_embed.grid_size
-                )
         out_dict[k] = v
     return out_dict
 
 
-def _convert_dinov2(state_dict, model):
+def _convert_dinov2(
+        state_dict: Dict[str, torch.Tensor],
+        model: VisionTransformer,
+) -> Dict[str, torch.Tensor]:
     import re
     out_dict = {}
     state_dict.pop("mask_token", None)
     if 'register_tokens' in state_dict:
         # convert dinov2 w/ registers to no_embed_class timm model (neither cls or reg tokens overlap pos embed)
         out_dict['reg_token'] = state_dict.pop('register_tokens')
         out_dict['cls_token'] = state_dict.pop('cls_token') + state_dict['pos_embed'][:, 0]
@@ -957,41 +1039,39 @@
             out_dict[k.replace("w3", "fc2")] = v
             continue
         out_dict[k] = v
     return out_dict
 
 
 def checkpoint_filter_fn(
-        state_dict,
-        model,
-        adapt_layer_scale=False,
-        interpolation='bicubic',
-        antialias=True,
-):
+        state_dict: Dict[str, torch.Tensor],
+        model: VisionTransformer,
+        adapt_layer_scale: bool = False,
+        interpolation: str = 'bicubic',
+        antialias: bool = True,
+) -> Dict[str, torch.Tensor]:
     """ convert patch embedding weight from manual patchify + linear proj to conv"""
     import re
     out_dict = {}
     state_dict = state_dict.get('model', state_dict)
     state_dict = state_dict.get('state_dict', state_dict)
     prefix = ''
 
     if 'visual.class_embedding' in state_dict:
-        return _convert_openai_clip(state_dict, model)
+        state_dict = _convert_openai_clip(state_dict, model)
     elif 'module.visual.class_embedding' in state_dict:
-        return _convert_openai_clip(state_dict, model, prefix='module.visual.')
-
-    if "mask_token" in state_dict:
+        state_dict = _convert_openai_clip(state_dict, model, prefix='module.visual.')
+    elif "mask_token" in state_dict:
         state_dict = _convert_dinov2(state_dict, model)
-
-    if "encoder" in state_dict:
+    elif "encoder" in state_dict:
+        # IJEPA, vit in an 'encoder' submodule
         state_dict = state_dict['encoder']
         prefix = 'module.'
-
-    if 'visual.trunk.pos_embed' in state_dict:
-        # convert an OpenCLIP model with timm vision encoder
+    elif 'visual.trunk.pos_embed' in state_dict:
+        # OpenCLIP model with timm vision encoder
         # FIXME remap final nn.Linear if it exists outside of the timm .trunk (ie in visual.head.proj)
         prefix = 'visual.trunk.'
 
     if prefix:
         # filter on & remove prefix string from keys
         state_dict = {k[len(prefix):]: v for k, v in state_dict.items() if k.startswith(prefix)}
 
@@ -1027,25 +1107,30 @@
         elif 'pre_logits' in k:
             # NOTE representation layer removed as not used in latest 21k/1k pretrained weights
             continue
         out_dict[k] = v
     return out_dict
 
 
-def _cfg(url='', **kwargs):
+def _cfg(url: str = '', **kwargs) -> Dict[str, Any]:
     return {
         'url': url,
-        'num_classes': 1000, 'input_size': (3, 224, 224), 'pool_size': None,
-        'crop_pct': .9, 'interpolation': 'bicubic', 'fixed_input_size': True,
-        'mean': IMAGENET_INCEPTION_MEAN, 'std': IMAGENET_INCEPTION_STD,
-        'first_conv': 'patch_embed.proj', 'classifier': 'head',
-        **kwargs
+        'num_classes': 1000,
+        'input_size': (3, 224, 224),
+        'pool_size': None,
+        'crop_pct': 0.9,
+        'interpolation': 'bicubic',
+        'fixed_input_size': True,
+        'mean': IMAGENET_INCEPTION_MEAN,
+        'std': IMAGENET_INCEPTION_STD,
+        'first_conv': 'patch_embed.proj',
+        'classifier': 'head',
+        **kwargs,
     }
 
-
 default_cfgs = {
 
     # re-finetuned augreg 21k FT on in1k weights
     'vit_base_patch16_224.augreg2_in21k_ft_in1k': _cfg(
         hf_hub_id='timm/'),
     'vit_base_patch16_384.augreg2_in21k_ft_in1k': _cfg(),
     'vit_base_patch8_224.augreg2_in21k_ft_in1k': _cfg(
@@ -1145,23 +1230,34 @@
         custom_load=True, input_size=(3, 384, 384), crop_pct=1.0),
 
     'vit_large_patch14_224.untrained': _cfg(url=''),
     'vit_huge_patch14_224.untrained': _cfg(url=''),
     'vit_giant_patch14_224.untrained': _cfg(url=''),
     'vit_gigantic_patch14_224.untrained': _cfg(url=''),
 
-    # patch models, imagenet21k (weights from official Google JAX impl)
+    # patch models, imagenet21k (weights from official Google JAX impl), classifier not valid
+    'vit_base_patch32_224.orig_in21k': _cfg(
+        #url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-vitjx/jx_vit_base_patch32_224_in21k-8db57226.pth',
+        hf_hub_id='timm/',
+        num_classes=0),
+    'vit_base_patch16_224.orig_in21k': _cfg(
+        #url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-vitjx/jx_vit_base_patch16_224_in21k-e5005f0a.pth',
+        hf_hub_id='timm/',
+        num_classes=0),
     'vit_large_patch32_224.orig_in21k': _cfg(
-        url='https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-vitjx/jx_vit_large_patch32_224_in21k-9046d2e7.pth',
+        #url='https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-vitjx/jx_vit_large_patch32_224_in21k-9046d2e7.pth',
         hf_hub_id='timm/',
-        num_classes=21843),
+        num_classes=0),
+    'vit_large_patch16_224.orig_in21k': _cfg(
+        #url='https://github.com/huggingface/pytorch-image-models/releases/download/v0.1-vitjx/jx_vit_large_patch16_224_in21k-606da67d.pth',
+        hf_hub_id='timm/',
+        num_classes=0),
     'vit_huge_patch14_224.orig_in21k': _cfg(
-        url='https://storage.googleapis.com/vit_models/imagenet21k/ViT-H_14.npz',
         hf_hub_id='timm/',
-        custom_load=True, num_classes=21843),
+        num_classes=0),
 
     # How to train your ViT (augreg) weights, pretrained on in21k
     'vit_tiny_patch16_224.augreg_in21k': _cfg(
         url='https://storage.googleapis.com/vit_models/augreg/Ti_16-i21k-300ep-lr_0.001-aug_none-wd_0.03-do_0.0-sd_0.0.npz',
         hf_hub_id='timm/',
         custom_load=True, num_classes=21843),
     'vit_small_patch32_224.augreg_in21k': _cfg(
@@ -1494,27 +1590,27 @@
         hf_hub_id='facebook/metaclip-h14-fullcc2.5b',
         hf_hub_filename='metaclip_h14_fullcc2.5b.bin',
         license='cc-by-nc-4.0',
         notes=('natively QuickGELU, use quickgelu model variant for original results',),
         mean=OPENAI_CLIP_MEAN, std=OPENAI_CLIP_STD, crop_pct=1.0, num_classes=1024),
 
     'vit_base_patch32_clip_224.openai': _cfg(
-        hf_hub_id='timm/',
+        hf_hub_id='timm/vit_base_patch32_clip_224.openai',
         notes=('natively QuickGELU, use quickgelu model variant for original results',),
         mean=OPENAI_CLIP_MEAN, std=OPENAI_CLIP_STD, num_classes=512),
     'vit_base_patch16_clip_224.openai': _cfg(
-        hf_hub_id='timm/',
+        hf_hub_id='timm/vit_base_patch16_clip_224.openai',
         notes=('natively QuickGELU, use quickgelu model variant for original results',),
         mean=OPENAI_CLIP_MEAN, std=OPENAI_CLIP_STD, num_classes=512),
     'vit_large_patch14_clip_224.openai': _cfg(
-        hf_hub_id='timm/',
+        hf_hub_id='timm/vit_large_patch14_clip_224.openai',
         notes=('natively QuickGELU, use quickgelu model variant for original results',),
         mean=OPENAI_CLIP_MEAN, std=OPENAI_CLIP_STD, crop_pct=1.0, num_classes=768),
     'vit_large_patch14_clip_336.openai': _cfg(
-        hf_hub_id='timm/', hf_hub_filename='open_clip_pytorch_model.bin',
+        hf_hub_id='timm/vit_large_patch14_clip_336.openai', hf_hub_filename='open_clip_pytorch_model.bin',
         notes=('natively QuickGELU, use quickgelu model variant for original results',),
         mean=OPENAI_CLIP_MEAN, std=OPENAI_CLIP_STD,
         crop_pct=1.0, input_size=(3, 336, 336), num_classes=768),
 
     # experimental (may be removed)
     'vit_base_patch32_plus_256.untrained': _cfg(url='', input_size=(3, 256, 256), crop_pct=0.95),
     'vit_base_patch16_plus_240.untrained': _cfg(url='', input_size=(3, 240, 240), crop_pct=0.95),
@@ -1678,19 +1774,144 @@
         num_classes=0),
     'vit_so400m_patch14_siglip_384.webli': _cfg(
         hf_hub_id='timm/ViT-SO400M-14-SigLIP-384',
         hf_hub_filename='open_clip_pytorch_model.bin',
         input_size=(3, 384, 384),
         num_classes=0),
 
-    'vit_medium_patch16_reg4_256': _cfg(
+    'vit_base_patch16_siglip_gap_224.webli': _cfg(
+        hf_hub_id='timm/ViT-B-16-SigLIP',
+        hf_hub_filename='open_clip_pytorch_model.bin',
+        num_classes=0),
+    'vit_base_patch16_siglip_gap_256.webli': _cfg(
+        hf_hub_id='timm/ViT-B-16-SigLIP-256',
+        hf_hub_filename='open_clip_pytorch_model.bin',
+        input_size=(3, 256, 256),
+        num_classes=0),
+    'vit_base_patch16_siglip_gap_384.webli': _cfg(
+        hf_hub_id='timm/ViT-B-16-SigLIP-384',
+        hf_hub_filename='open_clip_pytorch_model.bin',
+        input_size=(3, 384, 384),
+        num_classes=0),
+    'vit_base_patch16_siglip_gap_512.webli': _cfg(
+        hf_hub_id='timm/ViT-B-16-SigLIP-512',
+        hf_hub_filename='open_clip_pytorch_model.bin',
+        input_size=(3, 512, 512),
+        num_classes=0),
+    'vit_large_patch16_siglip_gap_256.webli': _cfg(
+        hf_hub_id='timm/ViT-L-16-SigLIP-256',
+        hf_hub_filename='open_clip_pytorch_model.bin',
+        input_size=(3, 256, 256),
+        num_classes=0),
+    'vit_large_patch16_siglip_gap_384.webli': _cfg(
+        hf_hub_id='timm/ViT-L-16-SigLIP-384',
+        hf_hub_filename='open_clip_pytorch_model.bin',
+        input_size=(3, 384, 384),
+        num_classes=0),
+    'vit_so400m_patch14_siglip_gap_224.webli': _cfg(
+        hf_hub_id='timm/ViT-SO400M-14-SigLIP',
+        hf_hub_filename='open_clip_pytorch_model.bin',
+        num_classes=0),
+    'vit_so400m_patch14_siglip_gap_224.pali_mix': _cfg(
+        hf_hub_id='google/paligemma-3b-mix-224-jax',
+        hf_hub_filename='paligemma-3b-mix-224.npz',
+        custom_load='hf',
+        num_classes=0),
+    'vit_so400m_patch14_siglip_gap_224.pali_pt': _cfg(
+        hf_hub_id='google/paligemma-3b-pt-224-jax',
+        hf_hub_filename='paligemma-3b-pt-224.npz',
+        custom_load='hf',
+        num_classes=0),
+    'vit_so400m_patch14_siglip_gap_384.webli': _cfg(
+        hf_hub_id='timm/ViT-SO400M-14-SigLIP-384',
+        hf_hub_filename='open_clip_pytorch_model.bin',
+        input_size=(3, 384, 384), crop_pct=1.0,
+        num_classes=0),
+    'vit_so400m_patch14_siglip_gap_448.pali_mix': _cfg(
+        hf_hub_id='google/paligemma-3b-mix-448-jax',
+        hf_hub_filename='paligemma-3b-mix-448.npz',
+        custom_load='hf',
+        input_size=(3, 448, 448), crop_pct=1.0,
+        num_classes=0),
+    'vit_so400m_patch14_siglip_gap_448.pali_pt': _cfg(
+        hf_hub_id='google/paligemma-3b-pt-448-jax',
+        hf_hub_filename='paligemma-3b-pt-448.npz',
+        custom_load='hf',
+        input_size=(3, 448, 448), crop_pct=1.0,
+        num_classes=0),
+    'vit_so400m_patch14_siglip_gap_896.pali_pt': _cfg(
+        hf_hub_id='google/paligemma-3b-pt-896-jax',
+        hf_hub_filename='paligemma-3b-pt-896.npz',
+        custom_load='hf',
+        input_size=(3, 896, 896), crop_pct=1.0,
+        num_classes=0),
+
+    'vit_xsmall_patch16_clip_224.tinyclip_yfcc15m': _cfg(
+        hf_hub_id='timm/',
+        hf_hub_filename='open_clip_pytorch_model.bin',
+        license='mit',
+        mean=OPENAI_CLIP_MEAN, std=OPENAI_CLIP_STD, num_classes=512),
+    'vit_medium_patch32_clip_224.tinyclip_laion400m': _cfg(
+        hf_hub_id='timm/',
+        hf_hub_filename='open_clip_pytorch_model.bin',
+        license='mit',
+        mean=OPENAI_CLIP_MEAN, std=OPENAI_CLIP_STD, num_classes=512),
+    'vit_medium_patch16_clip_224.tinyclip_yfcc15m': _cfg(
+        hf_hub_id='timm/',
+        hf_hub_filename='open_clip_pytorch_model.bin',
+        license='mit',
+        mean=OPENAI_CLIP_MEAN, std=OPENAI_CLIP_STD, num_classes=512),
+    'vit_betwixt_patch32_clip_224.tinyclip_laion400m': _cfg(
+        hf_hub_id='timm/',
+        hf_hub_filename='open_clip_pytorch_model.bin',
+        license='mit',
+        mean=OPENAI_CLIP_MEAN, std=OPENAI_CLIP_STD, num_classes=512),
+
+    'vit_wee_patch16_reg1_gap_256.sbb_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95),
+    'vit_pwee_patch16_reg1_gap_256.sbb_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95),
+    'vit_little_patch16_reg4_gap_256.sbb_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95),
+    'vit_medium_patch16_reg1_gap_256.sbb_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95),
+    'vit_medium_patch16_reg4_gap_256.sbb_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95),
+    'vit_mediumd_patch16_reg4_gap_256.sbb_in12k_ft_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95),
+    'vit_mediumd_patch16_reg4_gap_256.sbb_in12k': _cfg(
+        hf_hub_id='timm/',
+        num_classes=11821,
+        input_size=(3, 256, 256), crop_pct=0.95),
+    'vit_betwixt_patch16_reg1_gap_256.sbb_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95),
+    'vit_betwixt_patch16_reg4_gap_256.sbb_in12k_ft_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95),
+    'vit_betwixt_patch16_reg4_gap_256.sbb_in1k': _cfg(
+        hf_hub_id='timm/',
+        input_size=(3, 256, 256), crop_pct=0.95),
+    'vit_betwixt_patch16_reg4_gap_256.sbb_in12k': _cfg(
+        hf_hub_id='timm/',
+        num_classes=11821,
+        input_size=(3, 256, 256), crop_pct=0.95),
+    'vit_base_patch16_reg4_gap_256': _cfg(
         input_size=(3, 256, 256)),
-    'vit_medium_patch16_reg4_gap_256': _cfg(
+
+    'vit_so150m_patch16_reg4_gap_256': _cfg(
+        input_size=(3, 256, 256)),
+    'vit_so150m_patch16_reg4_map_256': _cfg(
         input_size=(3, 256, 256)),
-    'vit_base_patch16_reg8_gap_256': _cfg(input_size=(3, 256, 256)),
 }
 
 _quick_gelu_cfgs = [
     'vit_large_patch14_clip_224.dfn2b',
     'vit_huge_patch14_clip_224.dfn5b',
     'vit_huge_patch14_clip_378.dfn5b',
     'vit_base_patch32_clip_224.metaclip_2pt5b',
@@ -1704,18 +1925,16 @@
 ]
 default_cfgs.update({
     n.replace('_clip_', '_clip_quickgelu_'): default_cfgs[n] for n in _quick_gelu_cfgs
 })
 default_cfgs = generate_default_cfgs(default_cfgs)
 
 
-def _create_vision_transformer(variant, pretrained=False, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError('features_only not implemented for Vision Transformer models.')
-
+def _create_vision_transformer(variant: str, pretrained: bool = False, **kwargs) -> VisionTransformer:
+    out_indices = kwargs.pop('out_indices', 3)
     if 'flexi' in variant:
         # FIXME Google FlexiViT pretrained models have a strong preference for bilinear patch / embed
         # interpolation, other pretrained models resize better w/ anti-aliased bicubic interpolation.
         _filter_fn = partial(checkpoint_filter_fn, interpolation='bilinear', antialias=False)
     else:
         _filter_fn = checkpoint_filter_fn
 
@@ -1726,752 +1945,802 @@
 
     return build_model_with_cfg(
         VisionTransformer,
         variant,
         pretrained,
         pretrained_filter_fn=_filter_fn,
         pretrained_strict=strict,
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
         **kwargs,
     )
 
 
 @register_model
-def vit_tiny_patch16_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_tiny_patch16_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Tiny (Vit-Ti/16)
     """
     model_args = dict(patch_size=16, embed_dim=192, depth=12, num_heads=3)
     model = _create_vision_transformer('vit_tiny_patch16_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_tiny_patch16_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_tiny_patch16_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Tiny (Vit-Ti/16) @ 384x384.
     """
     model_args = dict(patch_size=16, embed_dim=192, depth=12, num_heads=3)
     model = _create_vision_transformer('vit_tiny_patch16_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_small_patch32_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_small_patch32_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Small (ViT-S/32)
     """
     model_args = dict(patch_size=32, embed_dim=384, depth=12, num_heads=6)
     model = _create_vision_transformer('vit_small_patch32_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_small_patch32_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_small_patch32_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Small (ViT-S/32) at 384x384.
     """
     model_args = dict(patch_size=32, embed_dim=384, depth=12, num_heads=6)
     model = _create_vision_transformer('vit_small_patch32_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_small_patch16_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_small_patch16_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Small (ViT-S/16)
     """
     model_args = dict(patch_size=16, embed_dim=384, depth=12, num_heads=6)
     model = _create_vision_transformer('vit_small_patch16_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_small_patch16_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_small_patch16_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Small (ViT-S/16)
     """
     model_args = dict(patch_size=16, embed_dim=384, depth=12, num_heads=6)
     model = _create_vision_transformer('vit_small_patch16_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_small_patch8_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_small_patch8_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Small (ViT-S/8)
     """
     model_args = dict(patch_size=8, embed_dim=384, depth=12, num_heads=6)
     model = _create_vision_transformer('vit_small_patch8_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch32_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch32_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Base (ViT-B/32) from original paper (https://arxiv.org/abs/2010.11929).
     ImageNet-1k weights fine-tuned from in21k, source https://github.com/google-research/vision_transformer.
     """
     model_args = dict(patch_size=32, embed_dim=768, depth=12, num_heads=12)
     model = _create_vision_transformer('vit_base_patch32_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch32_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch32_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Base model (ViT-B/32) from original paper (https://arxiv.org/abs/2010.11929).
     ImageNet-1k weights fine-tuned from in21k @ 384x384, source https://github.com/google-research/vision_transformer.
     """
     model_args = dict(patch_size=32, embed_dim=768, depth=12, num_heads=12)
     model = _create_vision_transformer('vit_base_patch32_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Base (ViT-B/16) from original paper (https://arxiv.org/abs/2010.11929).
     ImageNet-1k weights fine-tuned from in21k @ 224x224, source https://github.com/google-research/vision_transformer.
     """
     model_args = dict(patch_size=16, embed_dim=768, depth=12, num_heads=12)
     model = _create_vision_transformer('vit_base_patch16_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Base model (ViT-B/16) from original paper (https://arxiv.org/abs/2010.11929).
     ImageNet-1k weights fine-tuned from in21k @ 384x384, source https://github.com/google-research/vision_transformer.
     """
     model_args = dict(patch_size=16, embed_dim=768, depth=12, num_heads=12)
     model = _create_vision_transformer('vit_base_patch16_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch8_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch8_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Base (ViT-B/8) from original paper (https://arxiv.org/abs/2010.11929).
     ImageNet-1k weights fine-tuned from in21k @ 224x224, source https://github.com/google-research/vision_transformer.
     """
     model_args = dict(patch_size=8, embed_dim=768, depth=12, num_heads=12)
     model = _create_vision_transformer('vit_base_patch8_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch32_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch32_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Large model (ViT-L/32) from original paper (https://arxiv.org/abs/2010.11929). No pretrained weights.
     """
     model_args = dict(patch_size=32, embed_dim=1024, depth=24, num_heads=16)
     model = _create_vision_transformer('vit_large_patch32_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch32_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch32_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Large model (ViT-L/32) from original paper (https://arxiv.org/abs/2010.11929).
     ImageNet-1k weights fine-tuned from in21k @ 384x384, source https://github.com/google-research/vision_transformer.
     """
     model_args = dict(patch_size=32, embed_dim=1024, depth=24, num_heads=16)
     model = _create_vision_transformer('vit_large_patch32_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch16_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch16_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Large model (ViT-L/16) from original paper (https://arxiv.org/abs/2010.11929).
     ImageNet-1k weights fine-tuned from in21k @ 224x224, source https://github.com/google-research/vision_transformer.
     """
     model_args = dict(patch_size=16, embed_dim=1024, depth=24, num_heads=16)
     model = _create_vision_transformer('vit_large_patch16_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch16_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch16_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Large model (ViT-L/16) from original paper (https://arxiv.org/abs/2010.11929).
     ImageNet-1k weights fine-tuned from in21k @ 384x384, source https://github.com/google-research/vision_transformer.
     """
     model_args = dict(patch_size=16, embed_dim=1024, depth=24, num_heads=16)
     model = _create_vision_transformer('vit_large_patch16_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch14_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch14_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Large model (ViT-L/14)
     """
     model_args = dict(patch_size=14, embed_dim=1024, depth=24, num_heads=16)
     model = _create_vision_transformer('vit_large_patch14_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_huge_patch14_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_huge_patch14_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Huge model (ViT-H/14) from original paper (https://arxiv.org/abs/2010.11929).
     """
     model_args = dict(patch_size=14, embed_dim=1280, depth=32, num_heads=16)
     model = _create_vision_transformer('vit_huge_patch14_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_giant_patch14_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_giant_patch14_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Giant (little-g) model (ViT-g/14) from `Scaling Vision Transformers` - https://arxiv.org/abs/2106.04560
     """
     model_args = dict(patch_size=14, embed_dim=1408, mlp_ratio=48/11, depth=40, num_heads=16)
     model = _create_vision_transformer('vit_giant_patch14_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_gigantic_patch14_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_gigantic_patch14_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Gigantic (big-G) model (ViT-G/14) from `Scaling Vision Transformers` - https://arxiv.org/abs/2106.04560
     """
     model_args = dict(patch_size=14, embed_dim=1664, mlp_ratio=64/13, depth=48, num_heads=16)
     model = _create_vision_transformer(
         'vit_gigantic_patch14_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_224_miil(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_224_miil(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Base (ViT-B/16) from original paper (https://arxiv.org/abs/2010.11929).
     Weights taken from: https://github.com/Alibaba-MIIL/ImageNet21K
     """
     model_args = dict(patch_size=16, embed_dim=768, depth=12, num_heads=12, qkv_bias=False)
     model = _create_vision_transformer(
         'vit_base_patch16_224_miil', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_medium_patch16_gap_240(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_medium_patch16_gap_240(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Medium (ViT-M/16) w/o class token, w/ avg-pool @ 240x240
     """
     model_args = dict(
         patch_size=16, embed_dim=512, depth=12, num_heads=8, class_token=False,
         global_pool='avg', qkv_bias=False, init_values=1e-6, fc_norm=False)
     model = _create_vision_transformer(
         'vit_medium_patch16_gap_240', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_medium_patch16_gap_256(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_medium_patch16_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Medium (ViT-M/16) w/o class token, w/ avg-pool @ 256x256
     """
     model_args = dict(
         patch_size=16, embed_dim=512, depth=12, num_heads=8, class_token=False,
         global_pool='avg', qkv_bias=False, init_values=1e-6, fc_norm=False)
     model = _create_vision_transformer(
         'vit_medium_patch16_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_medium_patch16_gap_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_medium_patch16_gap_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Medium (ViT-M/16) w/o class token, w/ avg-pool @ 384x384
     """
     model_args = dict(
         patch_size=16, embed_dim=512, depth=12, num_heads=8, class_token=False,
         global_pool='avg', qkv_bias=False, init_values=1e-6, fc_norm=False)
     model = _create_vision_transformer(
         'vit_medium_patch16_gap_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_gap_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_betwixt_patch16_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    """ ViT-Betwixt (ViT-b/16) w/o class token, w/ avg-pool @ 256x256
+    """
+    model_args = dict(
+        patch_size=16, embed_dim=640, depth=12, num_heads=10, class_token=False,
+        global_pool='avg', qkv_bias=False, init_values=1e-6, fc_norm=False)
+    model = _create_vision_transformer(
+        'vit_medium_patch16_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_base_patch16_gap_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Base (ViT-B/16) w/o class token, w/ avg-pool @ 224x224
     """
     model_args = dict(
         patch_size=16, embed_dim=768, depth=12, num_heads=16, class_token=False, global_pool='avg', fc_norm=False)
     model = _create_vision_transformer(
         'vit_base_patch16_gap_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_huge_patch14_gap_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_huge_patch14_gap_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Huge model (ViT-H/14) w/ no class token, avg pool
     """
     model_args = dict(
         patch_size=14, embed_dim=1280, depth=32, num_heads=16, class_token=False, global_pool='avg', fc_norm=False)
     model = _create_vision_transformer(
         'vit_huge_patch14_gap_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_huge_patch16_gap_448(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_huge_patch16_gap_448(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Huge model (ViT-H/16) w/ no class token, avg pool @ 448x448
     """
     model_args = dict(
         patch_size=16, embed_dim=1280, depth=32, num_heads=16, class_token=False, global_pool='avg', fc_norm=False)
     model = _create_vision_transformer(
         'vit_huge_patch16_gap_448', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_giant_patch16_gap_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_giant_patch16_gap_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Giant (little-gg) model (ViT-g/16) w/ no class token, avg pool
     """
     model_args = dict(
         patch_size=16, embed_dim=1408, depth=40, num_heads=16, mlp_ratio=48/11,
         class_token=False, global_pool='avg', fc_norm=False)
     model = _create_vision_transformer(
         'vit_giant_patch16_gap_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch32_clip_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_xsmall_patch16_clip_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    # TinyCLIP 8M
+    model_args = dict(embed_dim=256, depth=10, num_heads=4, pre_norm=True, norm_layer=nn.LayerNorm)
+    model = _create_vision_transformer(
+        'vit_xsmall_patch16_clip_224', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_medium_patch32_clip_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    # TinyCLIP 40M
+    model_args = dict(
+        patch_size=32, embed_dim=512, depth=12, num_heads=8, pre_norm=True, norm_layer=nn.LayerNorm)
+    model = _create_vision_transformer(
+        'vit_medium_patch32_clip_224', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_medium_patch16_clip_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    # TinyCLIP 39M
+    model_args = dict(embed_dim=512, depth=12, num_heads=8, pre_norm=True, norm_layer=nn.LayerNorm)
+    model = _create_vision_transformer(
+        'vit_medium_patch16_clip_224', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_betwixt_patch32_clip_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    # TinyCLIP 61M
+    model_args = dict(
+        patch_size=32, embed_dim=640, depth=12, num_heads=10, pre_norm=True, norm_layer=nn.LayerNorm)
+    model = _create_vision_transformer(
+        'vit_betwixt_patch32_clip_224', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_base_patch32_clip_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-B/32 CLIP image tower @ 224x224
     """
     model_args = dict(
         patch_size=32, embed_dim=768, depth=12, num_heads=12, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_base_patch32_clip_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch32_clip_256(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch32_clip_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-B/32 CLIP image tower @ 256x256
     """
     model_args = dict(
         patch_size=32, embed_dim=768, depth=12, num_heads=12, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_base_patch32_clip_256', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch32_clip_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch32_clip_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-B/32 CLIP image tower @ 384x384
     """
     model_args = dict(
         patch_size=32, embed_dim=768, depth=12, num_heads=12, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_base_patch32_clip_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch32_clip_448(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch32_clip_448(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-B/32 CLIP image tower @ 448x448
     """
     model_args = dict(
         patch_size=32, embed_dim=768, depth=12, num_heads=12, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_base_patch32_clip_448', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_clip_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_clip_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-B/16 CLIP image tower
     """
     model_args = dict(patch_size=16, embed_dim=768, depth=12, num_heads=12, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_base_patch16_clip_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_clip_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_clip_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-B/16 CLIP image tower @ 384x384
     """
     model_args = dict(patch_size=16, embed_dim=768, depth=12, num_heads=12, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_base_patch16_clip_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch14_clip_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch14_clip_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Large model (ViT-L/14) CLIP image tower
     """
     model_args = dict(patch_size=14, embed_dim=1024, depth=24, num_heads=16, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_large_patch14_clip_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch14_clip_336(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch14_clip_336(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Large model (ViT-L/14) CLIP image tower @ 336x336
     """
     model_args = dict(patch_size=14, embed_dim=1024, depth=24, num_heads=16, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_large_patch14_clip_336', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_huge_patch14_clip_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_huge_patch14_clip_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Huge model (ViT-H/14) CLIP image tower.
     """
     model_args = dict(patch_size=14, embed_dim=1280, depth=32, num_heads=16, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_huge_patch14_clip_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_huge_patch14_clip_336(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_huge_patch14_clip_336(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Huge model (ViT-H/14) CLIP image tower @ 336x336
     """
     model_args = dict(patch_size=14, embed_dim=1280, depth=32, num_heads=16, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_huge_patch14_clip_336', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_huge_patch14_clip_378(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_huge_patch14_clip_378(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Huge model (ViT-H/14) CLIP image tower @ 378x378
     """
     model_args = dict(patch_size=14, embed_dim=1280, depth=32, num_heads=16, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_huge_patch14_clip_378', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_giant_patch14_clip_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_giant_patch14_clip_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Giant (little-g) model (ViT-g/14) from `Scaling Vision Transformers` - https://arxiv.org/abs/2106.04560
     Pretrained weights from CLIP image tower.
     """
     model_args = dict(
         patch_size=14, embed_dim=1408, mlp_ratio=48/11, depth=40, num_heads=16, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_giant_patch14_clip_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_gigantic_patch14_clip_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_gigantic_patch14_clip_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-bigG model (ViT-G/14) from `Scaling Vision Transformers` - https://arxiv.org/abs/2106.04560
     Pretrained weights from CLIP image tower.
     """
     model_args = dict(
         patch_size=14, embed_dim=1664, mlp_ratio=64/13, depth=48, num_heads=16, pre_norm=True, norm_layer=nn.LayerNorm)
     model = _create_vision_transformer(
         'vit_gigantic_patch14_clip_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch32_clip_quickgelu_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch32_clip_quickgelu_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-B/32 CLIP image tower @ 224x224
     """
     model_args = dict(
         patch_size=32, embed_dim=768, depth=12, num_heads=12, pre_norm=True,
         norm_layer=nn.LayerNorm, act_layer='quick_gelu')
     model = _create_vision_transformer(
         'vit_base_patch32_clip_quickgelu_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_clip_quickgelu_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_clip_quickgelu_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-B/16 CLIP image tower w/ QuickGELU act
     """
     model_args = dict(
         patch_size=16, embed_dim=768, depth=12, num_heads=12, pre_norm=True,
         norm_layer=nn.LayerNorm, act_layer='quick_gelu')
     model = _create_vision_transformer(
         'vit_base_patch16_clip_quickgelu_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch14_clip_quickgelu_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch14_clip_quickgelu_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Large model (ViT-L/14) CLIP image tower w/ QuickGELU act
     """
-    from timm.layers import get_act_layer
     model_args = dict(
         patch_size=14, embed_dim=1024, depth=24, num_heads=16, pre_norm=True,
         norm_layer=nn.LayerNorm, act_layer='quick_gelu')
     model = _create_vision_transformer(
         'vit_large_patch14_clip_quickgelu_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch14_clip_quickgelu_336(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch14_clip_quickgelu_336(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Large model (ViT-L/14) CLIP image tower @ 336x336 w/ QuickGELU act
     """
     model_args = dict(
         patch_size=14, embed_dim=1024, depth=24, num_heads=16, pre_norm=True,
         norm_layer=nn.LayerNorm, act_layer='quick_gelu')
     model = _create_vision_transformer(
         'vit_large_patch14_clip_quickgelu_336', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_huge_patch14_clip_quickgelu_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_huge_patch14_clip_quickgelu_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Huge model (ViT-H/14) CLIP image tower w/ QuickGELU act.
     """
     model_args = dict(
         patch_size=14, embed_dim=1280, depth=32, num_heads=16, pre_norm=True,
         norm_layer=nn.LayerNorm, act_layer='quick_gelu')
     model = _create_vision_transformer(
         'vit_huge_patch14_clip_quickgelu_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_huge_patch14_clip_quickgelu_378(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_huge_patch14_clip_quickgelu_378(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Huge model (ViT-H/14) CLIP image tower @ 378x378 w/ QuickGELU act
     """
     model_args = dict(
         patch_size=14, embed_dim=1280, depth=32, num_heads=16, pre_norm=True,
         norm_layer=nn.LayerNorm, act_layer='quick_gelu')
     model = _create_vision_transformer(
         'vit_huge_patch14_clip_quickgelu_378', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 # Experimental models below
 
 @register_model
-def vit_base_patch32_plus_256(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch32_plus_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Base (ViT-B/32+)
     """
     model_args = dict(patch_size=32, embed_dim=896, depth=12, num_heads=14, init_values=1e-5)
     model = _create_vision_transformer(
         'vit_base_patch32_plus_256', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_plus_240(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_plus_240(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Base (ViT-B/16+)
     """
     model_args = dict(patch_size=16, embed_dim=896, depth=12, num_heads=14, init_values=1e-5)
     model = _create_vision_transformer(
         'vit_base_patch16_plus_240', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_rpn_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_rpn_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Base (ViT-B/16) w/ residual post-norm
     """
     model_args = dict(
         patch_size=16, embed_dim=768, depth=12, num_heads=12, qkv_bias=False, init_values=1e-5,
         class_token=False, block_fn=ResPostBlock, global_pool='avg')
     model = _create_vision_transformer(
         'vit_base_patch16_rpn_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_small_patch16_36x1_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_small_patch16_36x1_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Base w/ LayerScale + 36 x 1 (36 block serial) config. Experimental, may remove.
     Based on `Three things everyone should know about Vision Transformers` - https://arxiv.org/abs/2203.09795
     Paper focuses on 24x2 + 48x1 for 'Small' width but those are extremely slow.
     """
     model_args = dict(patch_size=16, embed_dim=384, depth=36, num_heads=6, init_values=1e-5)
     model = _create_vision_transformer(
         'vit_small_patch16_36x1_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_small_patch16_18x2_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_small_patch16_18x2_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Small w/ LayerScale + 18 x 2 (36 block parallel) config. Experimental, may remove.
     Based on `Three things everyone should know about Vision Transformers` - https://arxiv.org/abs/2203.09795
     Paper focuses on 24x2 + 48x1 for 'Small' width but those are extremely slow.
     """
     model_args = dict(
         patch_size=16, embed_dim=384, depth=18, num_heads=6, init_values=1e-5, block_fn=ParallelThingsBlock)
     model = _create_vision_transformer(
         'vit_small_patch16_18x2_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_18x2_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_18x2_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Base w/ LayerScale + 18 x 2 (36 block parallel) config. Experimental, may remove.
     Based on `Three things everyone should know about Vision Transformers` - https://arxiv.org/abs/2203.09795
     """
     model_args = dict(
         patch_size=16, embed_dim=768, depth=18, num_heads=12, init_values=1e-5, block_fn=ParallelThingsBlock)
     model = _create_vision_transformer(
         'vit_base_patch16_18x2_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def eva_large_patch14_196(pretrained=False, **kwargs) -> VisionTransformer:
+def eva_large_patch14_196(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ EVA-large model https://arxiv.org/abs/2211.07636 /via MAE MIM pretrain"""
     model_args = dict(patch_size=14, embed_dim=1024, depth=24, num_heads=16, global_pool='avg')
     model = _create_vision_transformer(
         'eva_large_patch14_196', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def eva_large_patch14_336(pretrained=False, **kwargs) -> VisionTransformer:
+def eva_large_patch14_336(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ EVA-large model https://arxiv.org/abs/2211.07636 via MAE MIM pretrain"""
     model_args = dict(patch_size=14, embed_dim=1024, depth=24, num_heads=16, global_pool='avg')
     model = _create_vision_transformer('eva_large_patch14_336', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def flexivit_small(pretrained=False, **kwargs) -> VisionTransformer:
+def flexivit_small(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ FlexiViT-Small
     """
     model_args = dict(patch_size=16, embed_dim=384, depth=12, num_heads=6, no_embed_class=True)
     model = _create_vision_transformer('flexivit_small', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def flexivit_base(pretrained=False, **kwargs) -> VisionTransformer:
+def flexivit_base(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ FlexiViT-Base
     """
     model_args = dict(patch_size=16, embed_dim=768, depth=12, num_heads=12, no_embed_class=True)
     model = _create_vision_transformer('flexivit_base', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def flexivit_large(pretrained=False, **kwargs) -> VisionTransformer:
+def flexivit_large(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ FlexiViT-Large
     """
     model_args = dict(patch_size=16, embed_dim=1024, depth=24, num_heads=16, no_embed_class=True)
     model = _create_vision_transformer('flexivit_large', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_xp_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_xp_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Large model (ViT-L/14) w/ parallel blocks and qk norm enabled.
     """
     model_args = dict(
         patch_size=16, embed_dim=768, depth=12, num_heads=12, pre_norm=True, no_embed_class=True,
         norm_layer=RmsNorm, block_fn=ParallelScalingBlock, qkv_bias=False, qk_norm=True,
     )
     model = _create_vision_transformer(
         'vit_base_patch16_xp_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch14_xp_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch14_xp_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Large model (ViT-L/14) w/ parallel blocks and qk norm enabled.
     """
     model_args = dict(
         patch_size=14, embed_dim=1024, depth=24, num_heads=16, pre_norm=True, no_embed_class=True,
         norm_layer=RmsNorm, block_fn=ParallelScalingBlock, qkv_bias=False, qk_norm=True,
     )
     model = _create_vision_transformer(
         'vit_large_patch14_xp_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_huge_patch14_xp_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_huge_patch14_xp_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-Huge model (ViT-H/14) w/ parallel blocks and qk norm enabled.
     """
     model_args = dict(
         patch_size=14, embed_dim=1280, depth=32, num_heads=16, pre_norm=True, no_embed_class=True,
         norm_layer=RmsNorm, block_fn=ParallelScalingBlock, qkv_bias=False, qk_norm=True,
     )
     model = _create_vision_transformer(
         'vit_huge_patch14_xp_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_small_patch14_dinov2(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_small_patch14_dinov2(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-S/14 for DINOv2
     """
-    model_args = dict(patch_size=14, embed_dim=384, depth=12, num_heads=6, init_values=1e-5, img_size=518)
+    model_args = dict(patch_size=14, embed_dim=384, depth=12, num_heads=6, init_values=1e-5)
     model = _create_vision_transformer(
         'vit_small_patch14_dinov2', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch14_dinov2(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch14_dinov2(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-B/14 for DINOv2
     """
-    model_args = dict(patch_size=14, embed_dim=768, depth=12, num_heads=12, init_values=1e-5, img_size=518)
+    model_args = dict(patch_size=14, embed_dim=768, depth=12, num_heads=12, init_values=1e-5)
     model = _create_vision_transformer(
         'vit_base_patch14_dinov2', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch14_dinov2(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch14_dinov2(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-L/14 for DINOv2
     """
-    model_args = dict(patch_size=14, embed_dim=1024, depth=24, num_heads=16, init_values=1e-5, img_size=518)
+    model_args = dict(patch_size=14, embed_dim=1024, depth=24, num_heads=16, init_values=1e-5)
     model = _create_vision_transformer(
         'vit_large_patch14_dinov2', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_giant_patch14_dinov2(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_giant_patch14_dinov2(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-G/14 for DINOv2
     """
     # The hidden_features of SwiGLU is calculated by:
     # hidden_features = (int(hidden_features * 2 / 3) + 7) // 8 * 8
     # When embed_dim=1536, hidden_features=4096
     # With SwiGLUPacked, we need to set hidden_features = 2 * 4096 = 8192
     model_args = dict(
         patch_size=14, embed_dim=1536, depth=40, num_heads=24, init_values=1e-5,
-        mlp_ratio=2.66667 * 2, mlp_layer=SwiGLUPacked, img_size=518, act_layer=nn.SiLU
+        mlp_ratio=2.66667 * 2, mlp_layer=SwiGLUPacked, act_layer=nn.SiLU
     )
     model = _create_vision_transformer(
         'vit_giant_patch14_dinov2', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_small_patch14_reg4_dinov2(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_small_patch14_reg4_dinov2(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-S/14 for DINOv2 w/ 4 registers
     """
     model_args = dict(
         patch_size=14, embed_dim=384, depth=12, num_heads=6, init_values=1e-5,
         reg_tokens=4, no_embed_class=True,
     )
     model = _create_vision_transformer(
         'vit_small_patch14_reg4_dinov2', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch14_reg4_dinov2(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch14_reg4_dinov2(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-B/14 for DINOv2 w/ 4 registers
     """
     model_args = dict(
         patch_size=14, embed_dim=768, depth=12, num_heads=12, init_values=1e-5,
         reg_tokens=4, no_embed_class=True,
     )
     model = _create_vision_transformer(
         'vit_base_patch14_reg4_dinov2', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch14_reg4_dinov2(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch14_reg4_dinov2(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-L/14 for DINOv2 w/ 4 registers
     """
     model_args = dict(
         patch_size=14, embed_dim=1024, depth=24, num_heads=16, init_values=1e-5,
         reg_tokens=4, no_embed_class=True,
     )
     model = _create_vision_transformer(
         'vit_large_patch14_reg4_dinov2', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_giant_patch14_reg4_dinov2(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_giant_patch14_reg4_dinov2(pretrained: bool = False, **kwargs) -> VisionTransformer:
     """ ViT-G/14 for DINOv2
     """
     # The hidden_features of SwiGLU is calculated by:
     # hidden_features = (int(hidden_features * 2 / 3) + 7) // 8 * 8
     # When embed_dim=1536, hidden_features=4096
     # With SwiGLUPacked, we need to set hidden_features = 2 * 4096 = 8192
     model_args = dict(
@@ -2480,123 +2749,325 @@
     )
     model = _create_vision_transformer(
         'vit_giant_patch14_reg4_dinov2', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_siglip_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_siglip_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     model_args = dict(
         patch_size=16, embed_dim=768, depth=12, num_heads=12, class_token=False, global_pool='map',
     )
     model = _create_vision_transformer(
         'vit_base_patch16_siglip_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_siglip_256(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_siglip_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
     model_args = dict(
         patch_size=16, embed_dim=768, depth=12, num_heads=12, class_token=False, global_pool='map',
     )
     model = _create_vision_transformer(
         'vit_base_patch16_siglip_256', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_siglip_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_siglip_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     model_args = dict(
         patch_size=16, embed_dim=768, depth=12, num_heads=12, class_token=False, global_pool='map',
     )
     model = _create_vision_transformer(
         'vit_base_patch16_siglip_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_siglip_512(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_siglip_512(pretrained: bool = False, **kwargs) -> VisionTransformer:
     model_args = dict(
         patch_size=16, embed_dim=768, depth=12, num_heads=12, class_token=False, global_pool='map',
     )
     model = _create_vision_transformer(
         'vit_base_patch16_siglip_512', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch16_siglip_256(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch16_siglip_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
     model_args = dict(
         patch_size=16, embed_dim=1024, depth=24, num_heads=16, class_token=False, global_pool='map',
     )
     model = _create_vision_transformer(
         'vit_large_patch16_siglip_256', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_large_patch16_siglip_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_large_patch16_siglip_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     model_args = dict(
         patch_size=16, embed_dim=1024, depth=24, num_heads=16, class_token=False, global_pool='map',
     )
     model = _create_vision_transformer(
         'vit_large_patch16_siglip_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_so400m_patch14_siglip_224(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_so400m_patch14_siglip_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
     model_args = dict(
         patch_size=14, embed_dim=1152, depth=27, num_heads=16, mlp_ratio=3.7362, class_token=False, global_pool='map',
     )
     model = _create_vision_transformer(
         'vit_so400m_patch14_siglip_224', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_so400m_patch14_siglip_384(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_so400m_patch14_siglip_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
     model_args = dict(
         patch_size=14, embed_dim=1152, depth=27, num_heads=16, mlp_ratio=3.7362, class_token=False, global_pool='map',
     )
     model = _create_vision_transformer(
         'vit_so400m_patch14_siglip_384', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_medium_patch16_reg4_256(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_base_patch16_siglip_gap_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    """ A SigLIP variant of ViT with global average pooling (GAP) instead of attention pooling (MAP)."""
+    model_args = dict(
+        patch_size=16, embed_dim=768, depth=12, num_heads=12, class_token=False, global_pool='avg', fc_norm=False,
+    )
+    model = _create_vision_transformer(
+        'vit_base_patch16_siglip_gap_224', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_base_patch16_siglip_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    """ A SigLIP variant of ViT with global average pooling (GAP) instead of attention pooling (MAP)."""
+    model_args = dict(
+        patch_size=16, embed_dim=768, depth=12, num_heads=12, class_token=False, global_pool='avg', fc_norm=False,
+    )
+    model = _create_vision_transformer(
+        'vit_base_patch16_siglip_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_base_patch16_siglip_gap_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    """ A SigLIP variant of ViT with global average pooling (GAP) instead of attention pooling (MAP)."""
+    model_args = dict(
+        patch_size=16, embed_dim=768, depth=12, num_heads=12, class_token=False, global_pool='avg', fc_norm=False,
+    )
+    model = _create_vision_transformer(
+        'vit_base_patch16_siglip_gap_384', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_base_patch16_siglip_gap_512(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    """ A SigLIP variant of ViT with global average pooling (GAP) instead of attention pooling (MAP)."""
+    model_args = dict(
+        patch_size=16, embed_dim=768, depth=12, num_heads=12, class_token=False, global_pool='avg', fc_norm=False,
+    )
+    model = _create_vision_transformer(
+        'vit_base_patch16_siglip_gap_512', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_large_patch16_siglip_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    """ A SigLIP variant of ViT with global average pooling (GAP) instead of attention pooling (MAP)."""
+    model_args = dict(
+        patch_size=16, embed_dim=1024, depth=24, num_heads=16, class_token=False, global_pool='avg', fc_norm=False,
+    )
+    model = _create_vision_transformer(
+        'vit_large_patch16_siglip_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_large_patch16_siglip_gap_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    """ A SigLIP variant of ViT with global average pooling (GAP) instead of attention pooling (MAP)."""
+    model_args = dict(
+        patch_size=16, embed_dim=1024, depth=24, num_heads=16, class_token=False, global_pool='avg', fc_norm=False,
+    )
+    model = _create_vision_transformer(
+        'vit_large_patch16_siglip_gap_384', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_so400m_patch14_siglip_gap_224(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    """ A SigLIP variant of ViT with global average pooling (GAP) instead of attention pooling (MAP)."""
+    model_args = dict(
+        patch_size=14, embed_dim=1152, depth=27, num_heads=16, mlp_ratio=3.7362,
+        class_token=False, global_pool='avg', fc_norm=False,
+    )
+    model = _create_vision_transformer(
+        'vit_so400m_patch14_siglip_gap_224', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_so400m_patch14_siglip_gap_384(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    """ A SigLIP variant of ViT with global average pooling (GAP) instead of attention pooling (MAP)."""
+    model_args = dict(
+        patch_size=14, embed_dim=1152, depth=27, num_heads=16, mlp_ratio=3.7362,
+        class_token=False, global_pool='avg', fc_norm=False,
+    )
+    model = _create_vision_transformer(
+        'vit_so400m_patch14_siglip_gap_384', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_so400m_patch14_siglip_gap_448(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    """ A SigLIP variant of ViT with global average pooling (GAP) instead of attention pooling (MAP)."""
+    model_args = dict(
+        patch_size=14, embed_dim=1152, depth=27, num_heads=16, mlp_ratio=3.7362,
+        class_token=False, global_pool='avg', fc_norm=False,
+    )
+    model = _create_vision_transformer(
+        'vit_so400m_patch14_siglip_gap_448', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_so400m_patch14_siglip_gap_896(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    """ A SigLIP variant of ViT with global average pooling (GAP) instead of attention pooling (MAP)."""
+    model_args = dict(
+        patch_size=14, embed_dim=1152, depth=27, num_heads=16, mlp_ratio=3.7362,
+        class_token=False, global_pool='avg', fc_norm=False,
+    )
+    model = _create_vision_transformer(
+        'vit_so400m_patch14_siglip_gap_896', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_wee_patch16_reg1_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
     model_args = dict(
-        patch_size=16, embed_dim=512, depth=12, num_heads=8, class_token=True,
-        no_embed_class=True, reg_tokens=4,
+        patch_size=16, embed_dim=256, depth=14, num_heads=4, init_values=1e-5, mlp_ratio=5,
+        class_token=False, no_embed_class=True, reg_tokens=1, global_pool='avg',
     )
     model = _create_vision_transformer(
-        'vit_medium_patch16_reg4_256', pretrained=pretrained, **dict(model_args, **kwargs))
+        'vit_wee_patch16_reg1_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_medium_patch16_reg4_gap_256(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_pwee_patch16_reg1_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
     model_args = dict(
-        patch_size=16, embed_dim=512, depth=12, num_heads=8,
+        patch_size=16, embed_dim=256, depth=16, num_heads=4, init_values=1e-5, mlp_ratio=5,
+        class_token=False, no_embed_class=True, reg_tokens=1, global_pool='avg', block_fn=ParallelScalingBlock,
+    )
+    model = _create_vision_transformer(
+        'vit_pwee_patch16_reg1_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_little_patch16_reg4_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    model_args = dict(
+        patch_size=16, embed_dim=320, depth=14, num_heads=5, init_values=1e-5, mlp_ratio=5.6,
+        class_token=False, no_embed_class=True, reg_tokens=4, global_pool='avg',
+    )
+    model = _create_vision_transformer(
+        'vit_little_patch16_reg4_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_medium_patch16_reg1_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    model_args = dict(
+        patch_size=16, embed_dim=512, depth=12, num_heads=8, init_values=1e-5,
+        class_token=False, no_embed_class=True, reg_tokens=1, global_pool='avg',
+    )
+    model = _create_vision_transformer(
+        'vit_medium_patch16_reg1_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_medium_patch16_reg4_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    model_args = dict(
+        patch_size=16, embed_dim=512, depth=12, num_heads=8, init_values=1e-5,
         class_token=False, no_embed_class=True, reg_tokens=4, global_pool='avg',
     )
     model = _create_vision_transformer(
         'vit_medium_patch16_reg4_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 @register_model
-def vit_base_patch16_reg8_gap_256(pretrained=False, **kwargs) -> VisionTransformer:
+def vit_mediumd_patch16_reg4_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    model_args = dict(
+        patch_size=16, embed_dim=512, depth=20, num_heads=8, init_values=1e-5,
+        class_token=False, no_embed_class=True, reg_tokens=4, global_pool='avg',
+    )
+    model = _create_vision_transformer(
+        'vit_mediumd_patch16_reg4_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_betwixt_patch16_reg1_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    model_args = dict(
+        patch_size=16, embed_dim=640, depth=12, num_heads=10, init_values=1e-5,
+        class_token=False, no_embed_class=True, reg_tokens=1, global_pool='avg',
+    )
+    model = _create_vision_transformer(
+        'vit_betwixt_patch16_reg1_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_betwixt_patch16_reg4_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    model_args = dict(
+        patch_size=16, embed_dim=640, depth=12, num_heads=10, init_values=1e-5,
+        class_token=False, no_embed_class=True, reg_tokens=4, global_pool='avg',
+    )
+    model = _create_vision_transformer(
+        'vit_betwixt_patch16_reg4_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_base_patch16_reg4_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
     model_args = dict(
         patch_size=16, embed_dim=768, depth=12, num_heads=12, class_token=False,
-        no_embed_class=True, global_pool='avg', reg_tokens=8,
+        no_embed_class=True, global_pool='avg', reg_tokens=4,
+    )
+    model = _create_vision_transformer(
+        'vit_base_patch16_reg4_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_so150m_patch16_reg4_map_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    model_args = dict(
+        patch_size=16, embed_dim=896, depth=18, num_heads=14, mlp_ratio=2.572,
+        class_token=False, reg_tokens=4, global_pool='map',
+    )
+    model = _create_vision_transformer(
+        'vit_so150m_patch16_reg4_map_256', pretrained=pretrained, **dict(model_args, **kwargs))
+    return model
+
+
+@register_model
+def vit_so150m_patch16_reg4_gap_256(pretrained: bool = False, **kwargs) -> VisionTransformer:
+    model_args = dict(
+        patch_size=16, embed_dim=896, depth=18, num_heads=14, mlp_ratio=2.572,
+        class_token=False, reg_tokens=4, global_pool='avg', fc_norm=False,
     )
     model = _create_vision_transformer(
-        'vit_base_patch16_reg8_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
+        'vit_so150m_patch16_reg4_gap_256', pretrained=pretrained, **dict(model_args, **kwargs))
     return model
 
 
 register_model_deprecations(__name__, {
     'vit_tiny_patch16_224_in21k': 'vit_tiny_patch16_224.augreg_in21k',
     'vit_small_patch32_224_in21k': 'vit_small_patch32_224.augreg_in21k',
     'vit_small_patch16_224_in21k': 'vit_small_patch16_224.augreg_in21k',
```

### Comparing `timm-0.9.9/timm/models/vision_transformer_hybrid.py` & `timm-1.0.3/timm/models/vision_transformer_hybrid.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,17 @@
     - https://arxiv.org/abs/2106.10270
 
 NOTE These hybrid model definitions depend on code in vision_transformer.py.
 They were moved here to keep file sizes sane.
 
 Hacked together by / Copyright 2020, Ross Wightman
 """
+import math
 from functools import partial
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from timm.layers import StdConv2dSame, StdConv2d, to_2tuple, Format, nchw_to
@@ -37,14 +38,15 @@
 
     def __init__(
             self,
             backbone,
             img_size=224,
             patch_size=1,
             feature_size=None,
+            feature_ratio=None,
             in_chans=3,
             embed_dim=768,
             bias=True,
             flatten: bool = True,
             output_fmt: Optional[str] = None,
             strict_img_size: bool = True,
             dynamic_img_pad: bool = False,
@@ -64,36 +66,60 @@
                     backbone.eval()
                 o = self.backbone(torch.zeros(1, in_chans, img_size[0], img_size[1]))
                 if isinstance(o, (list, tuple)):
                     o = o[-1]  # last feature if backbone outputs list/tuple of features
                 feature_size = o.shape[-2:]
                 feature_dim = o.shape[1]
                 backbone.train(training)
+            feature_ratio = tuple([s // f for s, f in zip(img_size, feature_size)])
         else:
+
             feature_size = to_2tuple(feature_size)
+            feature_ratio = to_2tuple(feature_ratio or 16)
             if hasattr(self.backbone, 'feature_info'):
                 feature_dim = self.backbone.feature_info.channels()[-1]
             else:
                 feature_dim = self.backbone.num_features
         if not dynamic_img_pad:
             assert feature_size[0] % patch_size[0] == 0 and feature_size[1] % patch_size[1] == 0
-        self.grid_size = (feature_size[0] // patch_size[0], feature_size[1] // patch_size[1])
+        self.feature_size = feature_size
+        self.feature_ratio = feature_ratio
+        self.grid_size = tuple([f // p for f, p in zip(self.feature_size, self.patch_size)])
         self.num_patches = self.grid_size[0] * self.grid_size[1]
         if output_fmt is not None:
             self.flatten = False
             self.output_fmt = Format(output_fmt)
         else:
             # flatten spatial dim and transpose to channels last, kept for bwd compat
             self.flatten = flatten
             self.output_fmt = Format.NCHW
         self.strict_img_size = strict_img_size
         self.dynamic_img_pad = dynamic_img_pad
 
         self.proj = nn.Conv2d(feature_dim, embed_dim, kernel_size=patch_size, stride=patch_size, bias=bias)
 
+    def feat_ratio(self, as_scalar=True) -> Union[Tuple[int, int], int]:
+        total_reduction = (
+            self.feature_ratio[0] * self.patch_size[0],
+            self.feature_ratio[1] * self.patch_size[1]
+        )
+        if as_scalar:
+            return max(total_reduction)
+        else:
+            return total_reduction
+
+    def dynamic_feat_size(self, img_size: Tuple[int, int]) -> Tuple[int, int]:
+        """ Get feature grid size taking account dynamic padding and backbone network feat reduction
+        """
+        feat_size = (img_size[0] // self.feature_ratio[0], img_size[1] // self.feature_ratio[1])
+        if self.dynamic_img_pad:
+            return math.ceil(feat_size[0] / self.patch_size[0]), math.ceil(feat_size[1] / self.patch_size[1])
+        else:
+            return feat_size[0] // self.patch_size[0], feat_size[1] // self.patch_size[1]
+
     def forward(self, x):
         x = self.backbone(x)
         if isinstance(x, (list, tuple)):
             x = x[-1]  # last feature if backbone outputs list/tuple of features
         _, _, H, W = x.shape
         if self.dynamic_img_pad:
             pad_h = (self.patch_size[0] - H % self.patch_size[0]) % self.patch_size[0]
@@ -213,17 +239,17 @@
         hf_hub_id='timm/',
         num_classes=21843, crop_pct=0.9, first_conv='patch_embed.backbone.conv', custom_load=True),
     'vit_small_r26_s32_224.augreg_in21k': _cfg(
         url='https://storage.googleapis.com/vit_models/augreg/R26_S_32-i21k-300ep-lr_0.001-aug_medium2-wd_0.03-do_0.0-sd_0.0.npz',
         hf_hub_id='timm/',
         num_classes=21843, crop_pct=0.9, custom_load=True),
     'vit_base_r50_s16_224.orig_in21k': _cfg(
-        url='https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-vitjx/jx_vit_base_resnet50_224_in21k-6f7c7740.pth',
+        #url='https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-vitjx/jx_vit_base_resnet50_224_in21k-6f7c7740.pth',
         hf_hub_id='timm/',
-        num_classes=21843, crop_pct=0.9),
+        num_classes=0, crop_pct=0.9),
     'vit_large_r50_s32_224.augreg_in21k': _cfg(
         url='https://storage.googleapis.com/vit_models/augreg/R50_L_32-i21k-300ep-lr_0.001-aug_medium2-wd_0.1-do_0.0-sd_0.0.npz',
         hf_hub_id='timm/',
         num_classes=21843, crop_pct=0.9, custom_load=True),
 
     # hybrid models (using timm resnet backbones)
     'vit_small_resnet26d_224.untrained': _cfg(
```

### Comparing `timm-0.9.9/timm/models/vision_transformer_relpos.py` & `timm-1.0.3/timm/models/vision_transformer_relpos.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,33 @@
 NOTE: these models are experimental / WIP, expect changes
 
 Hacked together by / Copyright 2022, Ross Wightman
 """
 import logging
 import math
 from functools import partial
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple, Type, Union
+
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
 
 import torch
 import torch.nn as nn
 from torch.jit import Final
 from torch.utils.checkpoint import checkpoint
 
 from timm.data import IMAGENET_INCEPTION_MEAN, IMAGENET_INCEPTION_STD
-from timm.layers import PatchEmbed, Mlp, DropPath, RelPosMlp, RelPosBias, use_fused_attn
+from timm.layers import PatchEmbed, Mlp, DropPath, RelPosMlp, RelPosBias, use_fused_attn, LayerType
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
+from ._manipulate import named_apply
 from ._registry import generate_default_cfgs, register_model
+from .vision_transformer import get_init_weights_vit
 
 __all__ = ['VisionTransformerRelPos']  # model_registry will add each entrypoint fn to this
 
 _logger = logging.getLogger(__name__)
 
 
 class RelPosAttention(nn.Module):
@@ -211,67 +219,69 @@
       * defaults to no class token (can be enabled)
       * defaults to global avg pool for head (can be changed)
       * layer-scale (residual branch gain) enabled
     """
 
     def __init__(
             self,
-            img_size=224,
-            patch_size=16,
-            in_chans=3,
-            num_classes=1000,
-            global_pool='avg',
-            embed_dim=768,
-            depth=12,
-            num_heads=12,
-            mlp_ratio=4.,
-            qkv_bias=True,
-            qk_norm=False,
-            init_values=1e-6,
-            class_token=False,
-            fc_norm=False,
-            rel_pos_type='mlp',
-            rel_pos_dim=None,
-            shared_rel_pos=False,
-            drop_rate=0.,
-            proj_drop_rate=0.,
-            attn_drop_rate=0.,
-            drop_path_rate=0.,
-            weight_init='skip',
-            embed_layer=PatchEmbed,
-            norm_layer=None,
-            act_layer=None,
-            block_fn=RelPosBlock
+            img_size: Union[int, Tuple[int, int]] = 224,
+            patch_size: Union[int, Tuple[int, int]] = 16,
+            in_chans: int = 3,
+            num_classes: int = 1000,
+            global_pool: Literal['', 'avg', 'token', 'map'] = 'avg',
+            embed_dim: int = 768,
+            depth: int = 12,
+            num_heads: int = 12,
+            mlp_ratio: float = 4.,
+            qkv_bias: bool = True,
+            qk_norm: bool = False,
+            init_values: Optional[float] = 1e-6,
+            class_token: bool = False,
+            fc_norm: bool = False,
+            rel_pos_type: str = 'mlp',
+            rel_pos_dim: Optional[int] = None,
+            shared_rel_pos: bool = False,
+            drop_rate: float = 0.,
+            proj_drop_rate: float = 0.,
+            attn_drop_rate: float = 0.,
+            drop_path_rate: float = 0.,
+            weight_init: Literal['skip', 'jax', 'moco', ''] = 'skip',
+            fix_init: bool = False,
+            embed_layer: Type[nn.Module] = PatchEmbed,
+            norm_layer: Optional[LayerType] = None,
+            act_layer: Optional[LayerType] = None,
+            block_fn: Type[nn.Module] = RelPosBlock
     ):
         """
         Args:
-            img_size (int, tuple): input image size
-            patch_size (int, tuple): patch size
-            in_chans (int): number of input channels
-            num_classes (int): number of classes for classification head
-            global_pool (str): type of global pooling for final sequence (default: 'avg')
-            embed_dim (int): embedding dimension
-            depth (int): depth of transformer
-            num_heads (int): number of attention heads
-            mlp_ratio (int): ratio of mlp hidden dim to embedding dim
-            qkv_bias (bool): enable bias for qkv if True
-            qk_norm (bool): Enable normalization of query and key in attention
-            init_values: (float): layer-scale init values
-            class_token (bool): use class token (default: False)
-            fc_norm (bool): use pre classifier norm instead of pre-pool
-            rel_pos_ty pe (str): type of relative position
-            shared_rel_pos (bool): share relative pos across all blocks
-            drop_rate (float): dropout rate
-            proj_drop_rate (float): projection dropout rate
-            attn_drop_rate (float): attention dropout rate
-            drop_path_rate (float): stochastic depth rate
-            weight_init (str): weight init scheme
-            embed_layer (nn.Module): patch embedding layer
-            norm_layer: (nn.Module): normalization layer
-            act_layer: (nn.Module): MLP activation layer
+            img_size: input image size
+            patch_size: patch size
+            in_chans: number of input channels
+            num_classes: number of classes for classification head
+            global_pool: type of global pooling for final sequence (default: 'avg')
+            embed_dim: embedding dimension
+            depth: depth of transformer
+            num_heads: number of attention heads
+            mlp_ratio: ratio of mlp hidden dim to embedding dim
+            qkv_bias: enable bias for qkv if True
+            qk_norm: Enable normalization of query and key in attention
+            init_values: layer-scale init values
+            class_token: use class token (default: False)
+            fc_norm: use pre classifier norm instead of pre-pool
+            rel_pos_type: type of relative position
+            shared_rel_pos: share relative pos across all blocks
+            drop_rate: dropout rate
+            proj_drop_rate: projection dropout rate
+            attn_drop_rate: attention dropout rate
+            drop_path_rate: stochastic depth rate
+            weight_init: weight init scheme
+            fix_init: apply weight initialization fix (scaling w/ layer index)
+            embed_layer: patch embedding layer
+            norm_layer: normalization layer
+            act_layer: MLP activation layer
         """
         super().__init__()
         assert global_pool in ('', 'avg', 'token')
         assert class_token or global_pool != 'token'
         norm_layer = norm_layer or partial(nn.LayerNorm, eps=1e-6)
         act_layer = act_layer or nn.GELU
 
@@ -284,14 +294,15 @@
         self.patch_embed = embed_layer(
             img_size=img_size,
             patch_size=patch_size,
             in_chans=in_chans,
             embed_dim=embed_dim,
         )
         feat_size = self.patch_embed.grid_size
+        r = self.patch_embed.feat_ratio() if hasattr(self.patch_embed, 'feat_ratio') else patch_size
 
         rel_pos_args = dict(window_size=feat_size, prefix_tokens=self.num_prefix_tokens)
         if rel_pos_type.startswith('mlp'):
             if rel_pos_dim:
                 rel_pos_args['hidden_dim'] = rel_pos_dim
             if 'swin' in rel_pos_type:
                 rel_pos_args['mode'] = 'swin'
@@ -319,30 +330,41 @@
                 proj_drop=proj_drop_rate,
                 attn_drop=attn_drop_rate,
                 drop_path=dpr[i],
                 norm_layer=norm_layer,
                 act_layer=act_layer,
             )
             for i in range(depth)])
+        self.feature_info = [
+            dict(module=f'blocks.{i}', num_chs=embed_dim, reduction=r) for i in range(depth)]
         self.norm = norm_layer(embed_dim) if not fc_norm else nn.Identity()
 
         # Classifier Head
         self.fc_norm = norm_layer(embed_dim) if fc_norm else nn.Identity()
         self.head_drop = nn.Dropout(drop_rate)
         self.head = nn.Linear(self.embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
         if weight_init != 'skip':
             self.init_weights(weight_init)
+        if fix_init:
+            self.fix_init_weight()
 
     def init_weights(self, mode=''):
         assert mode in ('jax', 'moco', '')
         if self.cls_token is not None:
             nn.init.normal_(self.cls_token, std=1e-6)
-        # FIXME weight init scheme using PyTorch defaults curently
-        #named_apply(get_init_weights_vit(mode, head_bias), self)
+        named_apply(get_init_weights_vit(mode), self)
+
+    def fix_init_weight(self):
+        def rescale(param, _layer_id):
+            param.div_(math.sqrt(2.0 * _layer_id))
+
+        for layer_id, layer in enumerate(self.blocks):
+            rescale(layer.attn.proj.weight.data, layer_id + 1)
+            rescale(layer.mlp.fc2.weight.data, layer_id + 1)
 
     @torch.jit.ignore
     def no_weight_decay(self):
         return {'cls_token'}
 
     @torch.jit.ignore
     def group_matcher(self, coarse=False):
@@ -362,14 +384,96 @@
     def reset_classifier(self, num_classes: int, global_pool=None):
         self.num_classes = num_classes
         if global_pool is not None:
             assert global_pool in ('', 'avg', 'token')
             self.global_pool = global_pool
         self.head = nn.Linear(self.embed_dim, num_classes) if num_classes > 0 else nn.Identity()
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            return_prefix_tokens: bool = False,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            return_prefix_tokens: Return both prefix and spatial intermediate tokens
+            norm: Apply norm layer to all intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW', 'NLC'), 'Output format must be one of NCHW or NLC.'
+        reshape = output_fmt == 'NCHW'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+
+        # forward pass
+        B, _, height, width = x.shape
+        x = self.patch_embed(x)
+        if self.cls_token is not None:
+            x = torch.cat((self.cls_token.expand(x.shape[0], -1, -1), x), dim=1)
+
+        shared_rel_pos = self.shared_rel_pos.get_bias() if self.shared_rel_pos is not None else None
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            blocks = self.blocks
+        else:
+            blocks = self.blocks[:max_index + 1]
+        for i, blk in enumerate(blocks):
+            x = blk(x, shared_rel_pos=shared_rel_pos)
+            if i in take_indices:
+                # normalize intermediates with final norm layer if enabled
+                intermediates.append(self.norm(x) if norm else x)
+
+        # process intermediates
+        if self.num_prefix_tokens:
+            # split prefix (e.g. class, distill) and spatial feature tokens
+            prefix_tokens = [y[:, 0:self.num_prefix_tokens] for y in intermediates]
+            intermediates = [y[:, self.num_prefix_tokens:] for y in intermediates]
+        if reshape:
+            # reshape to BCHW output format
+            H, W = self.patch_embed.dynamic_feat_size((height, width))
+            intermediates = [y.reshape(B, H, W, -1).permute(0, 3, 1, 2).contiguous() for y in intermediates]
+        if not torch.jit.is_scripting() and return_prefix_tokens:
+            # return_prefix not support in torchscript due to poor type handling
+            intermediates = list(zip(intermediates, prefix_tokens))
+
+        if intermediates_only:
+            return intermediates
+
+        x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+        self.blocks = self.blocks[:max_index + 1]  # truncate blocks
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.fc_norm = nn.Identity()
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.patch_embed(x)
         if self.cls_token is not None:
             x = torch.cat((self.cls_token.expand(x.shape[0], -1, -1), x), dim=1)
 
         shared_rel_pos = self.shared_rel_pos.get_bias() if self.shared_rel_pos is not None else None
         for blk in self.blocks:
@@ -390,18 +494,20 @@
     def forward(self, x):
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
 def _create_vision_transformer_relpos(variant, pretrained=False, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError('features_only not implemented for Vision Transformer models.')
-
-    model = build_model_with_cfg(VisionTransformerRelPos, variant, pretrained, **kwargs)
+    out_indices = kwargs.pop('out_indices', 3)
+    model = build_model_with_cfg(
+        VisionTransformerRelPos, variant, pretrained,
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
+        **kwargs,
+    )
     return model
 
 
 def _cfg(url='', **kwargs):
     return {
         'url': url,
         'num_classes': 1000, 'input_size': (3, 224, 224), 'pool_size': None,
```

### Comparing `timm-0.9.9/timm/models/vision_transformer_sam.py` & `timm-1.0.3/timm/models/vision_transformer_sam.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 
 'Segment Anything Model (SAM)'
     - https://github.com/facebookresearch/segment-anything/
 
 """
 import logging
 from functools import partial
-from typing import Callable, Optional, Tuple
+from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.checkpoint
-from torch.jit import Final
-
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD, IMAGENET_INCEPTION_MEAN, IMAGENET_INCEPTION_STD
-from timm.layers import PatchEmbed, Mlp, DropPath, PatchDropout, LayerNorm2d, ClassifierHead, NormMlpClassifierHead,\
+from timm.layers import PatchEmbed, Mlp, DropPath, PatchDropout, LayerNorm2d, ClassifierHead, NormMlpClassifierHead, \
     Format, resample_abs_pos_embed_nhwc, RotaryEmbeddingCat, apply_rot_embed_cat, to_2tuple, use_fused_attn
+from torch.jit import Final
+
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
+from ._features_fx import register_notrace_function
 from ._manipulate import checkpoint_seq
 from ._registry import generate_default_cfgs, register_model
-from ._features_fx import register_notrace_function
 
 # model_registry will add each entrypoint fn to this
 __all__ = ['VisionTransformerSAM']
 
 
 _logger = logging.getLogger(__name__)
 
@@ -339,16 +340,15 @@
             drop_rate: float = 0.,
             pos_drop_rate: float = 0.,
             patch_drop_rate: float = 0.,
             proj_drop_rate: float = 0.,
             attn_drop_rate: float = 0.,
             drop_path_rate: float = 0.,
             weight_init: str = '',
-            embed_layer: Callable = partial(
-                PatchEmbed, output_fmt=Format.NHWC, strict_img_size=False),
+            embed_layer: Callable = partial(PatchEmbed, output_fmt=Format.NHWC, strict_img_size=False),
             norm_layer: Optional[Callable] = nn.LayerNorm,
             act_layer: Optional[Callable] = nn.GELU,
             block_fn: Callable = Block,
             mlp_layer: Callable = Mlp,
             use_abs_pos: bool = True,
             use_rel_pos: bool = False,
             use_rope: bool = False,
@@ -404,14 +404,16 @@
             img_size=img_size,
             patch_size=patch_size,
             in_chans=in_chans,
             embed_dim=embed_dim,
             bias=not pre_norm,  # disable bias if pre-norm is used
         )
         grid_size = self.patch_embed.grid_size
+        r = self.patch_embed.feat_ratio() if hasattr(self.patch_embed, 'feat_ratio') else patch_size
+
         if use_abs_pos:
             # Initialize absolute positional embedding with pretrain image size.
             self.pos_embed = nn.Parameter(torch.zeros(1, grid_size[0], grid_size[1], embed_dim))
         else:
             self.pos_embed = None
         self.pos_drop = nn.Dropout(p=pos_drop_rate)
         if patch_drop_rate > 0:
@@ -465,14 +467,16 @@
                 mlp_layer=mlp_layer,
                 use_rel_pos=use_rel_pos,
                 window_size=window_size if i not in global_attn_indexes else 0,
                 input_size=grid_size,
                 rope=self.rope_window if i not in global_attn_indexes else self.rope_global,
             )
             for i in range(depth)])
+        self.feature_info = [
+            dict(module=f'blocks.{i}', num_chs=embed_dim, reduction=r) for i in range(depth)]
 
         if neck_chans:
             self.neck = nn.Sequential(
                 nn.Conv2d(
                     embed_dim,
                     neck_chans,
                     kernel_size=1,
@@ -532,14 +536,87 @@
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
     def reset_classifier(self, num_classes=0, global_pool=None):
         self.head.reset(num_classes, global_pool)
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to all intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt == 'NCHW', 'Output shape for ViT-SAM must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+
+        # forward pass, collect intermediates
+        x = self.patch_embed(x)
+        if self.pos_embed is not None:
+            # dynamically resize abs pos embedding if needed
+            x = x + resample_abs_pos_embed_nhwc(self.pos_embed, x.shape[1:3])
+        x = self.pos_drop(x)
+        x = self.patch_drop(x)
+        x = self.norm_pre(x)
+
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            blocks = self.blocks
+        else:
+            blocks = self.blocks[:max_index + 1]
+        for i, blk in enumerate(blocks):
+            x = blk(x)
+            if i in take_indices:
+                # make output BCHW
+                if norm:
+                    # norm is intertwined with neck convs so apply both, changes the dim
+                    # FIXME only apply to final? Need experiments
+                    intermediates.append(self.neck(x.permute(0, 3, 1, 2)))
+                else:
+                    intermediates.append(x.permute(0, 3, 1, 2))
+
+        if intermediates_only:
+            return intermediates
+
+        x = self.neck(x.permute(0, 3, 1, 2))
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+        self.blocks = self.blocks[:max_index + 1]  # truncate blocks
+        if prune_norm:
+            # neck is being treated as equivalent to final norm here
+            self.neck = nn.Identity()
+        if prune_head:
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.patch_embed(x)
         if self.pos_embed is not None:
             # dynamically resize abs pos embedding if needed
             x = x + resample_abs_pos_embed_nhwc(self.pos_embed, x.shape[1:3])
         x = self.pos_drop(x)
         x = self.patch_drop(x)
@@ -614,23 +691,21 @@
     'samvit_base_patch16_224': _cfg(
         mean=IMAGENET_DEFAULT_MEAN, std=IMAGENET_DEFAULT_STD, num_classes=1000,
         input_size=(3, 224, 224), crop_pct=0.9),
 })
 
 
 def _create_vision_transformer(variant, pretrained=False, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError(
-            'features_only not implemented for Vision Transformer models.')
-
+    out_indices = kwargs.pop('out_indices', 3)
     return build_model_with_cfg(
         VisionTransformerSAM,
         variant,
         pretrained,
         pretrained_filter_fn=checkpoint_filter_fn,
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
         **kwargs,
     )
 
 
 @register_model
 def samvit_base_patch16(pretrained=False, **kwargs) -> VisionTransformerSAM:
     """ ViT-B/16 for Segment-Anything
```

### Comparing `timm-0.9.9/timm/models/volo.py` & `timm-1.0.3/timm/models/volo.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import math
+from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils.checkpoint import checkpoint
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
-from timm.layers import DropPath, Mlp, to_2tuple, to_ntuple, trunc_normal_
+from timm.layers import DropPath, Mlp, to_2tuple, to_ntuple, trunc_normal_, use_fused_attn
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._registry import register_model, generate_default_cfgs
 
 __all__ = ['VOLO']  # model_registry will add each entrypoint fn to this
 
 
 class OutlookAttention(nn.Module):
 
@@ -115,62 +117,71 @@
             num_heads,
             kernel_size=kernel_size,
             padding=padding,
             stride=stride,
             qkv_bias=qkv_bias,
             attn_drop=attn_drop,
         )
-
-        self.drop_path = DropPath(drop_path) if drop_path > 0. else nn.Identity()
+        self.drop_path1 = DropPath(drop_path) if drop_path > 0. else nn.Identity()
 
         self.norm2 = norm_layer(dim)
-        mlp_hidden_dim = int(dim * mlp_ratio)
         self.mlp = Mlp(
             in_features=dim,
-            hidden_features=mlp_hidden_dim,
+            hidden_features=int(dim * mlp_ratio),
             act_layer=act_layer,
         )
+        self.drop_path2 = DropPath(drop_path) if drop_path > 0. else nn.Identity()
 
     def forward(self, x):
-        x = x + self.drop_path(self.attn(self.norm1(x)))
-        x = x + self.drop_path(self.mlp(self.norm2(x)))
+        x = x + self.drop_path1(self.attn(self.norm1(x)))
+        x = x + self.drop_path2(self.mlp(self.norm2(x)))
         return x
 
 
 class Attention(nn.Module):
+    fused_attn: torch.jit.Final[bool]
 
     def __init__(
             self,
             dim,
             num_heads=8,
             qkv_bias=False,
             attn_drop=0.,
             proj_drop=0.,
     ):
         super().__init__()
         self.num_heads = num_heads
         head_dim = dim // num_heads
         self.scale = head_dim ** -0.5
+        self.fused_attn = use_fused_attn()
 
         self.qkv = nn.Linear(dim, dim * 3, bias=qkv_bias)
         self.attn_drop = nn.Dropout(attn_drop)
         self.proj = nn.Linear(dim, dim)
         self.proj_drop = nn.Dropout(proj_drop)
 
     def forward(self, x):
         B, H, W, C = x.shape
 
         qkv = self.qkv(x).reshape(B, H * W, 3, self.num_heads, C // self.num_heads).permute(2, 0, 3, 1, 4)
         q, k, v = qkv.unbind(0)
 
-        attn = (q @ k.transpose(-2, -1)) * self.scale
-        attn = attn.softmax(dim=-1)
-        attn = self.attn_drop(attn)
+        if self.fused_attn:
+            x = F.scaled_dot_product_attention(
+                q, k, v,
+                dropout_p=self.attn_drop.p if self.training else 0.,
+            )
+        else:
+            q = q * self.scale
+            attn = q @ k.transpose(-2, -1)
+            attn = attn.softmax(dim=-1)
+            attn = self.attn_drop(attn)
+            x = attn @ v
 
-        x = (attn @ v).transpose(1, 2).reshape(B, H, W, C)
+        x = x.transpose(1, 2).reshape(B, H, W, C)
         x = self.proj(x)
         x = self.proj_drop(x)
 
         return x
 
 
 class Transformer(nn.Module):
@@ -185,25 +196,23 @@
             drop_path=0.,
             act_layer=nn.GELU,
             norm_layer=nn.LayerNorm,
     ):
         super().__init__()
         self.norm1 = norm_layer(dim)
         self.attn = Attention(dim, num_heads=num_heads, qkv_bias=qkv_bias, attn_drop=attn_drop)
-
-        # NOTE: drop path for stochastic depth, we shall see if this is better than dropout here
-        self.drop_path = DropPath(drop_path) if drop_path > 0. else nn.Identity()
+        self.drop_path1 = DropPath(drop_path) if drop_path > 0. else nn.Identity()
 
         self.norm2 = norm_layer(dim)
-        mlp_hidden_dim = int(dim * mlp_ratio)
-        self.mlp = Mlp(in_features=dim, hidden_features=mlp_hidden_dim, act_layer=act_layer)
+        self.mlp = Mlp(in_features=dim, hidden_features=int(dim * mlp_ratio), act_layer=act_layer)
+        self.drop_path2 = DropPath(drop_path) if drop_path > 0. else nn.Identity()
 
     def forward(self, x):
-        x = x + self.drop_path(self.attn(self.norm1(x)))
-        x = x + self.drop_path(self.mlp(self.norm2(x)))
+        x = x + self.drop_path1(self.attn(self.norm1(x)))
+        x = x + self.drop_path2(self.mlp(self.norm2(x)))
         return x
 
 
 class ClassAttention(nn.Module):
 
     def __init__(
             self,
@@ -230,16 +239,17 @@
         self.proj_drop = nn.Dropout(proj_drop)
 
     def forward(self, x):
         B, N, C = x.shape
 
         kv = self.kv(x).reshape(B, N, 2, self.num_heads, self.head_dim).permute(2, 0, 3, 1, 4)
         k, v = kv.unbind(0)
-        q = self.q(x[:, :1, :]).reshape(B, self.num_heads, 1, self.head_dim)
-        attn = ((q * self.scale) @ k.transpose(-2, -1))
+        q = self.q(x[:, :1, :]).reshape(B, self.num_heads, 1, self.head_dim) * self.scale
+
+        attn = q @ k.transpose(-2, -1)
         attn = attn.softmax(dim=-1)
         attn = self.attn_drop(attn)
 
         cls_embed = (attn @ v).transpose(1, 2).reshape(B, 1, self.head_dim * self.num_heads)
         cls_embed = self.proj(cls_embed)
         cls_embed = self.proj_drop(cls_embed)
         return cls_embed
@@ -266,29 +276,29 @@
             dim,
             num_heads=num_heads,
             head_dim=head_dim,
             qkv_bias=qkv_bias,
             attn_drop=attn_drop,
             proj_drop=drop,
         )
-        # NOTE: drop path for stochastic depth
-        self.drop_path = DropPath(drop_path) if drop_path > 0. else nn.Identity()
+        self.drop_path1 = DropPath(drop_path) if drop_path > 0. else nn.Identity()
+
         self.norm2 = norm_layer(dim)
-        mlp_hidden_dim = int(dim * mlp_ratio)
         self.mlp = Mlp(
             in_features=dim,
-            hidden_features=mlp_hidden_dim,
+            hidden_features=int(dim * mlp_ratio),
             act_layer=act_layer,
             drop=drop,
         )
+        self.drop_path2 = DropPath(drop_path) if drop_path > 0. else nn.Identity()
 
     def forward(self, x):
         cls_embed = x[:, :1]
-        cls_embed = cls_embed + self.drop_path(self.attn(self.norm1(x)))
-        cls_embed = cls_embed + self.drop_path(self.mlp(self.norm2(cls_embed)))
+        cls_embed = cls_embed + self.drop_path1(self.attn(self.norm1(x)))
+        cls_embed = cls_embed + self.drop_path2(self.mlp(self.norm2(cls_embed)))
         return torch.cat([cls_embed, x[:, 1:]], dim=1)
 
 
 def get_block(block_type, **kargs):
     if block_type == 'ca':
         return ClassBlock(**kargs)
 
@@ -491,56 +501,63 @@
             stem_conv=True,
             stem_stride=2,
             patch_size=patch_size,
             in_chans=in_chans,
             hidden_dim=stem_hidden_dim,
             embed_dim=embed_dims[0],
         )
+        r = patch_size
 
         # inital positional encoding, we add positional encoding after outlooker blocks
         patch_grid = (img_size[0] // patch_size // pooling_scale, img_size[1] // patch_size // pooling_scale)
         self.pos_embed = nn.Parameter(torch.zeros(1, patch_grid[0], patch_grid[1], embed_dims[-1]))
         self.pos_drop = nn.Dropout(p=pos_drop_rate)
 
         # set the main block in network
+        self.stage_ends = []
+        self.feature_info = []
         network = []
+        block_idx = 0
         for i in range(len(layers)):
             if outlook_attention[i]:
                 # stage 1
                 stage = outlooker_blocks(
                     Outlooker,
                     i,
                     embed_dims[i],
                     layers,
                     num_heads[i],
                     mlp_ratio=mlp_ratio[i],
                     qkv_bias=qkv_bias,
                     attn_drop=attn_drop_rate,
                     norm_layer=norm_layer,
                 )
-                network.append(stage)
             else:
                 # stage 2
                 stage = transformer_blocks(
                     Transformer,
                     i,
                     embed_dims[i],
                     layers,
                     num_heads[i],
                     mlp_ratio=mlp_ratio[i],
                     qkv_bias=qkv_bias,
                     drop_path_rate=drop_path_rate,
                     attn_drop=attn_drop_rate,
                     norm_layer=norm_layer,
                 )
-                network.append(stage)
-
+            network.append(stage)
+            self.stage_ends.append(block_idx)
+            self.feature_info.append(dict(num_chs=embed_dims[i], reduction=r, module=f'network.{block_idx}'))
+            block_idx += 1
             if downsamples[i]:
                 # downsampling between two stages
                 network.append(Downsample(embed_dims[i], embed_dims[i + 1], 2))
+                r *= 2
+                block_idx += 1
 
         self.network = nn.ModuleList(network)
 
         # set post block, for example, class attention layers
         self.post_network = None
         if post_layers is not None:
             self.post_network = nn.ModuleList([
@@ -601,15 +618,15 @@
     def set_grad_checkpointing(self, enable=True):
         self.grad_checkpointing = enable
 
     @torch.jit.ignore
     def get_classifier(self):
         return self.head
 
-    def reset_classifier(self, num_classes, global_pool=None):
+    def reset_classifier(self, num_classes: int, global_pool: Optional[str] = None):
         self.num_classes = num_classes
         if global_pool is not None:
             self.global_pool = global_pool
         self.head = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
         if self.aux_head is not None:
             self.aux_head = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
 
@@ -687,14 +704,94 @@
             temp_x[:, bbx1:bbx2, bby1:bby2, :] = x_aux.flip(0)[:, bbx1:bbx2, bby1:bby2, :]
             x_aux = temp_x
             x_aux = x_aux.reshape(x_aux.shape[0], patch_h * patch_w, x_aux.shape[-1])
 
         # return these: 1. class token, 2. classes from all feature tokens, 3. bounding box
         return x_cls, x_aux, (bbx1, bby1, bbx2, bby2)
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to all intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW',), 'Output format must be NCHW.'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.stage_ends), indices)
+        take_indices = [self.stage_ends[i] for i in take_indices]
+        max_index = self.stage_ends[max_index]
+
+        # forward pass
+        B, _, height, width = x.shape
+        x = self.patch_embed(x).permute(0, 2, 3, 1)  # B,C,H,W-> B,H,W,C
+
+        # step2: tokens learning in the two stages
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            network = self.network
+        else:
+            network = self.network[:max_index + 1]
+        for idx, block in enumerate(network):
+            if idx == 2:
+                # add positional encoding after outlooker blocks
+                x = x + self.pos_embed
+                x = self.pos_drop(x)
+            x = block(x)
+            if idx in take_indices:
+                if norm and idx >= 2:
+                    x_inter = self.norm(x)
+                else:
+                    x_inter = x
+                intermediates.append(x_inter.permute(0, 3, 1, 2))
+
+        if intermediates_only:
+            return intermediates
+
+        # NOTE not supporting return of class tokens
+        # step3: post network, apply class attention or not
+        B, H, W, C = x.shape
+        x = x.reshape(B, -1, C)
+        if self.post_network is not None:
+            x = self.forward_cls(x)
+        x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.stage_ends), indices)
+        max_index = self.stage_ends[max_index]
+        self.network = self.network[:max_index + 1]  # truncate blocks
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.post_network = nn.ModuleList()  # prune token blocks with head
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         x = self.patch_embed(x).permute(0, 2, 3, 1)  # B,C,H,W-> B,H,W,C
 
         # step2: tokens learning in the two stages
         x = self.forward_tokens(x)
 
         # step3: post network, apply class attention or not
@@ -724,20 +821,20 @@
         """ simplified forward (without mix token training) """
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
 def _create_volo(variant, pretrained=False, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError('features_only not implemented for Vision Transformer models.')
+    out_indices = kwargs.pop('out_indices', 3)
     return build_model_with_cfg(
         VOLO,
         variant,
         pretrained,
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
         **kwargs,
     )
 
 
 def _cfg(url='', **kwargs):
     return {
         'url': url,
```

### Comparing `timm-0.9.9/timm/models/vovnet.py` & `timm-1.0.3/timm/models/vovnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         self.head = ClassifierHead(self.num_features, num_classes, pool_type=global_pool, drop_rate=self.drop_rate)
 
     def forward_features(self, x):
         x = self.stem(x)
         return self.stages(x)
 
     def forward_head(self, x, pre_logits: bool = False):
-        return self.head(x, pre_logits=pre_logits)
+        return self.head(x, pre_logits=pre_logits) if pre_logits else self.head(x)
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
```

### Comparing `timm-0.9.9/timm/models/xception.py` & `timm-1.0.3/timm/models/xception.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/models/xception_aligned.py` & `timm-1.0.3/timm/models/xception_aligned.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,39 +2,40 @@
 
 This is a correct, from scratch impl of Aligned Xception (Deeplab) models compatible with TF weights at
 https://github.com/tensorflow/models/blob/master/research/deeplab/g3doc/model_zoo.md
 
 Hacked together by / Copyright 2020 Ross Wightman
 """
 from functools import partial
+from typing import List, Dict, Type, Optional
 
 import torch
 import torch.nn as nn
 
 from timm.data import IMAGENET_INCEPTION_MEAN, IMAGENET_INCEPTION_STD
-from timm.layers import ClassifierHead, ConvNormAct, create_conv2d, get_norm_act_layer
+from timm.layers import ClassifierHead, ConvNormAct, DropPath, PadType, create_conv2d, get_norm_act_layer
 from timm.layers.helpers import to_3tuple
 from ._builder import build_model_with_cfg
 from ._manipulate import checkpoint_seq
 from ._registry import register_model, generate_default_cfgs
 
 __all__ = ['XceptionAligned']
 
 
 class SeparableConv2d(nn.Module):
     def __init__(
             self,
-            in_chs,
-            out_chs,
-            kernel_size=3,
-            stride=1,
-            dilation=1,
-            padding='',
-            act_layer=nn.ReLU,
-            norm_layer=nn.BatchNorm2d,
+            in_chs: int,
+            out_chs: int,
+            kernel_size: int = 3,
+            stride: int = 1,
+            dilation: int = 1,
+            padding: PadType = '',
+            act_layer: Type[nn.Module] = nn.ReLU,
+            norm_layer: Type[nn.Module] = nn.BatchNorm2d,
     ):
         super(SeparableConv2d, self).__init__()
         self.kernel_size = kernel_size
         self.dilation = dilation
 
         # depthwise convolution
         self.conv_dw = create_conv2d(
@@ -57,23 +58,23 @@
         x = self.act_pw(x)
         return x
 
 
 class PreSeparableConv2d(nn.Module):
     def __init__(
             self,
-            in_chs,
-            out_chs,
-            kernel_size=3,
-            stride=1,
-            dilation=1,
-            padding='',
-            act_layer=nn.ReLU,
-            norm_layer=nn.BatchNorm2d,
-            first_act=True,
+            in_chs: int,
+            out_chs: int,
+            kernel_size: int = 3,
+            stride: int = 1,
+            dilation: int = 1,
+            padding: PadType = '',
+            act_layer: Type[nn.Module] = nn.ReLU,
+            norm_layer: Type[nn.Module] = nn.BatchNorm2d,
+            first_act: bool = True,
     ):
         super(PreSeparableConv2d, self).__init__()
         norm_act_layer = get_norm_act_layer(norm_layer, act_layer=act_layer)
         self.kernel_size = kernel_size
         self.dilation = dilation
 
         self.norm = norm_act_layer(in_chs, inplace=True) if first_act else nn.Identity()
@@ -91,23 +92,24 @@
         x = self.conv_pw(x)
         return x
 
 
 class XceptionModule(nn.Module):
     def __init__(
             self,
-            in_chs,
-            out_chs,
-            stride=1,
-            dilation=1,
-            pad_type='',
-            start_with_relu=True,
-            no_skip=False,
-            act_layer=nn.ReLU,
-            norm_layer=None,
+            in_chs: int,
+            out_chs: int,
+            stride: int = 1,
+            dilation: int = 1,
+            pad_type: PadType = '',
+            start_with_relu: bool = True,
+            no_skip: bool = False,
+            act_layer: Type[nn.Module] = nn.ReLU,
+            norm_layer: Optional[Type[nn.Module]] = None,
+            drop_path: Optional[nn.Module] = None
     ):
         super(XceptionModule, self).__init__()
         out_chs = to_3tuple(out_chs)
         self.in_channels = in_chs
         self.out_channels = out_chs[-1]
         self.no_skip = no_skip
         if not no_skip and (self.out_channels != self.in_channels or stride != 1):
@@ -122,35 +124,40 @@
             if start_with_relu:
                 self.stack.add_module(f'act{i + 1}', act_layer(inplace=i > 0))
             self.stack.add_module(f'conv{i + 1}', SeparableConv2d(
                 in_chs, out_chs[i], 3, stride=stride if i == 2 else 1, dilation=dilation, padding=pad_type,
                 act_layer=separable_act_layer, norm_layer=norm_layer))
             in_chs = out_chs[i]
 
+        self.drop_path = drop_path
+
     def forward(self, x):
         skip = x
         x = self.stack(x)
         if self.shortcut is not None:
             skip = self.shortcut(skip)
         if not self.no_skip:
+            if self.drop_path is not None:
+                x = self.drop_path(x)
             x = x + skip
         return x
 
 
 class PreXceptionModule(nn.Module):
     def __init__(
             self,
-            in_chs,
-            out_chs,
-            stride=1,
-            dilation=1,
-            pad_type='',
-            no_skip=False,
-            act_layer=nn.ReLU,
-            norm_layer=None,
+            in_chs: int,
+            out_chs: int,
+            stride: int = 1,
+            dilation: int = 1,
+            pad_type: PadType = '',
+            no_skip: bool = False,
+            act_layer: Type[nn.Module] = nn.ReLU,
+            norm_layer: Optional[Type[nn.Module]] = None,
+            drop_path: Optional[nn.Module] = None
     ):
         super(PreXceptionModule, self).__init__()
         out_chs = to_3tuple(out_chs)
         self.in_channels = in_chs
         self.out_channels = out_chs[-1]
         self.no_skip = no_skip
         if not no_skip and (self.out_channels != self.in_channels or stride != 1):
@@ -170,38 +177,43 @@
                 padding=pad_type,
                 act_layer=act_layer,
                 norm_layer=norm_layer,
                 first_act=i > 0,
             ))
             in_chs = out_chs[i]
 
+        self.drop_path = drop_path
+
     def forward(self, x):
         x = self.norm(x)
         skip = x
         x = self.stack(x)
         if not self.no_skip:
+            if self.drop_path is not None:
+                x = self.drop_path(x)
             x = x + self.shortcut(skip)
         return x
 
 
 class XceptionAligned(nn.Module):
     """Modified Aligned Xception
     """
 
     def __init__(
             self,
-            block_cfg,
-            num_classes=1000,
-            in_chans=3,
-            output_stride=32,
-            preact=False,
-            act_layer=nn.ReLU,
-            norm_layer=nn.BatchNorm2d,
-            drop_rate=0.,
-            global_pool='avg',
+            block_cfg: List[Dict],
+            num_classes: int = 1000,
+            in_chans: int = 3,
+            output_stride: int = 32,
+            preact: bool = False,
+            act_layer: Type[nn.Module] = nn.ReLU,
+            norm_layer: Type[nn.Module] = nn.BatchNorm2d,
+            drop_rate: float = 0.,
+            drop_path_rate: float = 0.,
+            global_pool: str = 'avg',
     ):
         super(XceptionAligned, self).__init__()
         assert output_stride in (8, 16, 32)
         self.num_classes = num_classes
         self.drop_rate = drop_rate
         self.grad_checkpointing = False
 
@@ -213,27 +225,32 @@
         ])
 
         curr_dilation = 1
         curr_stride = 2
         self.feature_info = []
         self.blocks = nn.Sequential()
         module_fn = PreXceptionModule if preact else XceptionModule
+        net_num_blocks = len(block_cfg)
+        net_block_idx = 0
         for i, b in enumerate(block_cfg):
+            block_dpr = drop_path_rate * net_block_idx / (net_num_blocks - 1)  # stochastic depth linear decay rule
+            b['drop_path'] = DropPath(block_dpr) if block_dpr > 0. else None
             b['dilation'] = curr_dilation
             if b['stride'] > 1:
                 name = f'blocks.{i}.stack.conv2' if preact else f'blocks.{i}.stack.act3'
                 self.feature_info += [dict(num_chs=to_3tuple(b['out_chs'])[-2], reduction=curr_stride, module=name)]
                 next_stride = curr_stride * b['stride']
                 if next_stride > output_stride:
                     curr_dilation *= b['stride']
                     b['stride'] = 1
                 else:
                     curr_stride = next_stride
             self.blocks.add_module(str(i), module_fn(**b, **layer_args))
             self.num_features = self.blocks[-1].out_channels
+            net_block_idx += 1
 
         self.feature_info += [dict(
             num_chs=self.num_features, reduction=curr_stride, module='blocks.' + str(len(self.blocks) - 1))]
         self.act = act_layer(inplace=True) if preact else nn.Identity()
         self.head = ClassifierHead(
             in_features=self.num_features,
             num_classes=num_classes,
@@ -265,15 +282,15 @@
             x = checkpoint_seq(self.blocks, x)
         else:
             x = self.blocks(x)
         x = self.act(x)
         return x
 
     def forward_head(self, x, pre_logits: bool = False):
-        return self.head(x, pre_logits=pre_logits)
+        return self.head(x, pre_logits=pre_logits) if pre_logits else self.head(x)
 
     def forward(self, x):
         x = self.forward_features(x)
         x = self.forward_head(x)
         return x
 
 
@@ -330,16 +347,16 @@
         dict(in_chs=256, out_chs=728, stride=2),
         # middle flow
         *([dict(in_chs=728, out_chs=728, stride=1)] * 8),
         # exit flow
         dict(in_chs=728, out_chs=(728, 1024, 1024), stride=2),
         dict(in_chs=1024, out_chs=(1536, 1536, 2048), stride=1, no_skip=True, start_with_relu=False),
     ]
-    model_args = dict(block_cfg=block_cfg, norm_layer=partial(nn.BatchNorm2d, eps=.001, momentum=.1), **kwargs)
-    return _xception('xception41', pretrained=pretrained, **model_args)
+    model_args = dict(block_cfg=block_cfg, norm_layer=partial(nn.BatchNorm2d, eps=.001, momentum=.1))
+    return _xception('xception41', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def xception65(pretrained=False, **kwargs) -> XceptionAligned:
     """ Modified Aligned Xception-65
     """
     block_cfg = [
@@ -349,16 +366,16 @@
         dict(in_chs=256, out_chs=728, stride=2),
         # middle flow
         *([dict(in_chs=728, out_chs=728, stride=1)] * 16),
         # exit flow
         dict(in_chs=728, out_chs=(728, 1024, 1024), stride=2),
         dict(in_chs=1024, out_chs=(1536, 1536, 2048), stride=1, no_skip=True, start_with_relu=False),
     ]
-    model_args = dict(block_cfg=block_cfg, norm_layer=partial(nn.BatchNorm2d, eps=.001, momentum=.1), **kwargs)
-    return _xception('xception65', pretrained=pretrained, **model_args)
+    model_args = dict(block_cfg=block_cfg, norm_layer=partial(nn.BatchNorm2d, eps=.001, momentum=.1))
+    return _xception('xception65', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def xception71(pretrained=False, **kwargs) -> XceptionAligned:
     """ Modified Aligned Xception-71
     """
     block_cfg = [
@@ -370,16 +387,16 @@
         dict(in_chs=728, out_chs=728, stride=2),
         # middle flow
         *([dict(in_chs=728, out_chs=728, stride=1)] * 16),
         # exit flow
         dict(in_chs=728, out_chs=(728, 1024, 1024), stride=2),
         dict(in_chs=1024, out_chs=(1536, 1536, 2048), stride=1, no_skip=True, start_with_relu=False),
     ]
-    model_args = dict(block_cfg=block_cfg, norm_layer=partial(nn.BatchNorm2d, eps=.001, momentum=.1), **kwargs)
-    return _xception('xception71', pretrained=pretrained, **model_args)
+    model_args = dict(block_cfg=block_cfg, norm_layer=partial(nn.BatchNorm2d, eps=.001, momentum=.1))
+    return _xception('xception71', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def xception41p(pretrained=False, **kwargs) -> XceptionAligned:
     """ Modified Aligned Xception-41 w/ Pre-Act
     """
     block_cfg = [
@@ -389,16 +406,16 @@
         dict(in_chs=256, out_chs=728, stride=2),
         # middle flow
         *([dict(in_chs=728, out_chs=728, stride=1)] * 8),
         # exit flow
         dict(in_chs=728, out_chs=(728, 1024, 1024), stride=2),
         dict(in_chs=1024, out_chs=(1536, 1536, 2048), no_skip=True, stride=1),
     ]
-    model_args = dict(block_cfg=block_cfg, preact=True, norm_layer=nn.BatchNorm2d, **kwargs)
-    return _xception('xception41p', pretrained=pretrained, **model_args)
+    model_args = dict(block_cfg=block_cfg, preact=True, norm_layer=nn.BatchNorm2d)
+    return _xception('xception41p', pretrained=pretrained, **dict(model_args, **kwargs))
 
 
 @register_model
 def xception65p(pretrained=False, **kwargs) -> XceptionAligned:
     """ Modified Aligned Xception-65 w/ Pre-Act
     """
     block_cfg = [
@@ -409,9 +426,9 @@
         # middle flow
         *([dict(in_chs=728, out_chs=728, stride=1)] * 16),
         # exit flow
         dict(in_chs=728, out_chs=(728, 1024, 1024), stride=2),
         dict(in_chs=1024, out_chs=(1536, 1536, 2048), stride=1, no_skip=True),
     ]
     model_args = dict(
-        block_cfg=block_cfg, preact=True, norm_layer=partial(nn.BatchNorm2d, eps=.001, momentum=.1), **kwargs)
-    return _xception('xception65p', pretrained=pretrained, **model_args)
+        block_cfg=block_cfg, preact=True, norm_layer=partial(nn.BatchNorm2d, eps=.001, momentum=.1))
+    return _xception('xception65p', pretrained=pretrained, **dict(model_args, **kwargs))
```

### Comparing `timm-0.9.9/timm/models/xcit.py` & `timm-1.0.3/timm/models/xcit.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 Modifications and additions for timm hacked together by / Copyright 2021, Ross Wightman
 """
 # Copyright (c) 2015-present, Facebook, Inc.
 # All rights reserved.
 
 import math
 from functools import partial
+from typing import List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 from torch.utils.checkpoint import checkpoint
 
 from timm.data import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
-from timm.layers import DropPath, trunc_normal_, to_2tuple
+from timm.layers import DropPath, trunc_normal_, to_2tuple, use_fused_attn
 from ._builder import build_model_with_cfg
+from ._features import feature_take_indices
 from ._features_fx import register_notrace_module
 from ._registry import register_model, generate_default_cfgs, register_model_deprecations
 from .cait import ClassAttn
 from .vision_transformer import Mlp
 
 __all__ = ['Xcit']  # model_registry will add each entrypoint fn to this
 
@@ -44,26 +46,27 @@
         self.temperature = temperature
         self.hidden_dim = hidden_dim
         self.dim = dim
         self.eps = 1e-6
 
     def forward(self, B: int, H: int, W: int):
         device = self.token_projection.weight.device
-        y_embed = torch.arange(1, H+1, dtype=torch.float32, device=device).unsqueeze(1).repeat(1, 1, W)
-        x_embed = torch.arange(1, W+1, dtype=torch.float32, device=device).repeat(1, H, 1)
+        dtype = self.token_projection.weight.dtype
+        y_embed = torch.arange(1, H + 1, device=device).to(torch.float32).unsqueeze(1).repeat(1, 1, W)
+        x_embed = torch.arange(1, W + 1, device=device).to(torch.float32).repeat(1, H, 1)
         y_embed = y_embed / (y_embed[:, -1:, :] + self.eps) * self.scale
         x_embed = x_embed / (x_embed[:, :, -1:] + self.eps) * self.scale
-        dim_t = torch.arange(self.hidden_dim, dtype=torch.float32, device=device)
+        dim_t = torch.arange(self.hidden_dim, device=device).to(torch.float32)
         dim_t = self.temperature ** (2 * torch.div(dim_t, 2, rounding_mode='floor') / self.hidden_dim)
         pos_x = x_embed[:, :, :, None] / dim_t
         pos_y = y_embed[:, :, :, None] / dim_t
         pos_x = torch.stack([pos_x[:, :, :, 0::2].sin(), pos_x[:, :, :, 1::2].cos()], dim=4).flatten(3)
         pos_y = torch.stack([pos_y[:, :, :, 0::2].sin(), pos_y[:, :, :, 1::2].cos()], dim=4).flatten(3)
         pos = torch.cat((pos_y, pos_x), dim=3).permute(0, 3, 1, 2)
-        pos = self.token_projection(pos)
+        pos = self.token_projection(pos.to(dtype))
         return pos.repeat(B, 1, 1, 1)  # (B, C, H, W)
 
 
 def conv3x3(in_planes, out_planes, stride=1):
     """3x3 convolution + batch norm"""
     return torch.nn.Sequential(
         nn.Conv2d(in_planes, out_planes, kernel_size=3, stride=stride, padding=1, bias=False),
@@ -190,43 +193,50 @@
         cls_token = self.gamma2 * self.mlp(cls_token)
         x = torch.cat([cls_token, x[:, 1:]], dim=1)
         x = x_res + self.drop_path(x)
         return x
 
 
 class XCA(nn.Module):
+    fused_attn: torch.jit.Final[bool]
     """ Cross-Covariance Attention (XCA)
     Operation where the channels are updated using a weighted sum. The weights are obtained from the (softmax
     normalized) Cross-covariance matrix (Q^T \\cdot K \\in d_h \\times d_h)
     """
 
     def __init__(self, dim, num_heads=8, qkv_bias=False, attn_drop=0., proj_drop=0.):
         super().__init__()
         self.num_heads = num_heads
+        self.fused_attn = use_fused_attn(experimental=True)
         self.temperature = nn.Parameter(torch.ones(num_heads, 1, 1))
         self.qkv = nn.Linear(dim, dim * 3, bias=qkv_bias)
         self.attn_drop = nn.Dropout(attn_drop)
         self.proj = nn.Linear(dim, dim)
         self.proj_drop = nn.Dropout(proj_drop)
 
     def forward(self, x):
         B, N, C = x.shape
         # Result of next line is (qkv, B, num (H)eads,  (C')hannels per head, N)
         qkv = self.qkv(x).reshape(B, N, 3, self.num_heads, C // self.num_heads).permute(2, 0, 3, 4, 1)
         q, k, v = qkv.unbind(0)  # make torchscript happy (cannot use tensor as tuple)
-        
-        # Paper section 3.2 l2-Normalization and temperature scaling
-        q = torch.nn.functional.normalize(q, dim=-1)
-        k = torch.nn.functional.normalize(k, dim=-1)
-        attn = (q @ k.transpose(-2, -1)) * self.temperature
-        attn = attn.softmax(dim=-1)
-        attn = self.attn_drop(attn)
 
-        # (B, H, C', N), permute -> (B, N, H, C')
-        x = (attn @ v).permute(0, 3, 1, 2).reshape(B, N, C)
+        if self.fused_attn:
+            q = torch.nn.functional.normalize(q, dim=-1) * self.temperature
+            k = torch.nn.functional.normalize(k, dim=-1)
+            x = torch.nn.functional.scaled_dot_product_attention(q, k, v, scale=1.0)
+        else:
+            # Paper section 3.2 l2-Normalization and temperature scaling
+            q = torch.nn.functional.normalize(q, dim=-1)
+            k = torch.nn.functional.normalize(k, dim=-1)
+            attn = (q @ k.transpose(-2, -1)) * self.temperature
+            attn = attn.softmax(dim=-1)
+            attn = self.attn_drop(attn)
+            x = attn @ v
+
+        x = x.permute(0, 3, 1, 2).reshape(B, N, C)
         x = self.proj(x)
         x = self.proj_drop(x)
         return x
 
     @torch.jit.ignore
     def no_weight_decay(self):
         return {'temperature'}
@@ -343,14 +353,15 @@
         self.patch_embed = ConvPatchEmbed(
             img_size=img_size,
             patch_size=patch_size,
             in_chans=in_chans,
             embed_dim=embed_dim,
             act_layer=act_layer,
         )
+        r = patch_size
 
         self.cls_token = nn.Parameter(torch.zeros(1, 1, embed_dim))
         if use_pos_embed:
             self.pos_embed = PositionalEncodingFourier(dim=embed_dim)
         else:
             self.pos_embed = None
         self.pos_drop = nn.Dropout(p=pos_drop_rate)
@@ -365,14 +376,15 @@
                 attn_drop=attn_drop_rate,
                 drop_path=drop_path_rate,
                 act_layer=act_layer,
                 norm_layer=norm_layer,
                 eta=eta,
             )
             for _ in range(depth)])
+        self.feature_info = [dict(num_chs=embed_dim, reduction=r, module=f'blocks.{i}') for i in range(depth)]
 
         self.cls_attn_blocks = nn.ModuleList([
             ClassAttentionBlock(
                 dim=embed_dim,
                 num_heads=num_heads,
                 mlp_ratio=mlp_ratio,
                 qkv_bias=qkv_bias,
@@ -423,14 +435,92 @@
     def reset_classifier(self, num_classes, global_pool=''):
         self.num_classes = num_classes
         if global_pool is not None:
             assert global_pool in ('', 'avg', 'token')
             self.global_pool = global_pool
         self.head = nn.Linear(self.num_features, num_classes) if num_classes > 0 else nn.Identity()
 
+    def forward_intermediates(
+            self,
+            x: torch.Tensor,
+            indices: Optional[Union[int, List[int], Tuple[int]]] = None,
+            norm: bool = False,
+            stop_early: bool = False,
+            output_fmt: str = 'NCHW',
+            intermediates_only: bool = False,
+    ) -> Union[List[torch.Tensor], Tuple[torch.Tensor, List[torch.Tensor]]]:
+        """ Forward features that returns intermediates.
+
+        Args:
+            x: Input image tensor
+            indices: Take last n blocks if int, all if None, select matching indices if sequence
+            norm: Apply norm layer to all intermediates
+            stop_early: Stop iterating over blocks when last desired intermediate hit
+            output_fmt: Shape of intermediate feature outputs
+            intermediates_only: Only return intermediate features
+        Returns:
+
+        """
+        assert output_fmt in ('NCHW', 'NLC'), 'Output format must be one of NCHW or NLC.'
+        reshape = output_fmt == 'NCHW'
+        intermediates = []
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+
+        # forward pass
+        B, _, height, width = x.shape
+        x, (Hp, Wp) = self.patch_embed(x)
+        if self.pos_embed is not None:
+            # `pos_embed` (B, C, Hp, Wp), reshape -> (B, C, N), permute -> (B, N, C)
+            pos_encoding = self.pos_embed(B, Hp, Wp).reshape(B, -1, x.shape[1]).permute(0, 2, 1)
+            x = x + pos_encoding
+        x = self.pos_drop(x)
+
+        if torch.jit.is_scripting() or not stop_early:  # can't slice blocks in torchscript
+            blocks = self.blocks
+        else:
+            blocks = self.blocks[:max_index + 1]
+        for i, blk in enumerate(blocks):
+            x = blk(x, Hp, Wp)
+            if i in take_indices:
+                # normalize intermediates with final norm layer if enabled
+                intermediates.append(self.norm(x) if norm else x)
+
+        # process intermediates
+        if reshape:
+            # reshape to BCHW output format
+            intermediates = [y.reshape(B, Hp, Wp, -1).permute(0, 3, 1, 2).contiguous() for y in intermediates]
+
+        if intermediates_only:
+            return intermediates
+
+        # NOTE not supporting return of class tokens
+        x = torch.cat((self.cls_token.expand(B, -1, -1), x), dim=1)
+        for blk in self.cls_attn_blocks:
+                x = blk(x)
+        x = self.norm(x)
+
+        return x, intermediates
+
+    def prune_intermediate_layers(
+            self,
+            indices: Union[int, List[int], Tuple[int]] = 1,
+            prune_norm: bool = False,
+            prune_head: bool = True,
+    ):
+        """ Prune layers not required for specified intermediates.
+        """
+        take_indices, max_index = feature_take_indices(len(self.blocks), indices)
+        self.blocks = self.blocks[:max_index + 1]  # truncate blocks
+        if prune_norm:
+            self.norm = nn.Identity()
+        if prune_head:
+            self.cls_attn_blocks = nn.ModuleList()  # prune token blocks with head
+            self.reset_classifier(0, '')
+        return take_indices
+
     def forward_features(self, x):
         B = x.shape[0]
         # x is (B, N, C). (Hp, Hw) is (height in units of patches, width in units of patches)
         x, (Hp, Wp) = self.patch_embed(x)
 
         if self.pos_embed is not None:
             # `pos_embed` (B, C, Hp, Wp), reshape -> (B, C, N), permute -> (B, N, C)
@@ -493,22 +583,21 @@
                 qkv_bias = qkv_bias.reshape(3, -1)
                 for j, subscript in enumerate('qkv'):
                     state_dict[f'cls_attn_blocks.{i}.attn.{subscript}.bias'] = qkv_bias[j]
     return state_dict
 
 
 def _create_xcit(variant, pretrained=False, default_cfg=None, **kwargs):
-    if kwargs.get('features_only', None):
-        raise RuntimeError('features_only not implemented for Cross-Covariance Image Transformers models.')
-
+    out_indices = kwargs.pop('out_indices', 3)
     model = build_model_with_cfg(
         Xcit,
         variant,
         pretrained,
         pretrained_filter_fn=checkpoint_filter_fn,
+        feature_cfg=dict(out_indices=out_indices, feature_cls='getter'),
         **kwargs,
     )
     return model
 
 
 def _cfg(url='', **kwargs):
     return {
@@ -886,14 +975,15 @@
     'xcit_tiny_12_p16_224_dist': 'xcit_tiny_12_p16_224.fb_dist_in1k',
     'xcit_tiny_12_p16_384_dist': 'xcit_tiny_12_p16_384.fb_dist_in1k',
     'xcit_tiny_24_p16_224_dist': 'xcit_tiny_24_p16_224.fb_dist_in1k',
     'xcit_tiny_24_p16_384_dist': 'xcit_tiny_24_p16_384.fb_dist_in1k',
     'xcit_small_12_p16_224_dist': 'xcit_small_12_p16_224.fb_dist_in1k',
     'xcit_small_12_p16_384_dist': 'xcit_small_12_p16_384.fb_dist_in1k',
     'xcit_small_24_p16_224_dist': 'xcit_small_24_p16_224.fb_dist_in1k',
+    'xcit_small_24_p16_384_dist': 'xcit_small_24_p16_384.fb_dist_in1k',
     'xcit_medium_24_p16_224_dist': 'xcit_medium_24_p16_224.fb_dist_in1k',
     'xcit_medium_24_p16_384_dist': 'xcit_medium_24_p16_384.fb_dist_in1k',
     'xcit_large_24_p16_224_dist': 'xcit_large_24_p16_224.fb_dist_in1k',
     'xcit_large_24_p16_384_dist': 'xcit_large_24_p16_384.fb_dist_in1k',
 
     # Patch size 8
     'xcit_nano_12_p8_224_dist': 'xcit_nano_12_p8_224.fb_dist_in1k',
```

### Comparing `timm-0.9.9/timm/optim/__init__.py` & `timm-1.0.3/timm/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/adabelief.py` & `timm-1.0.3/timm/optim/adabelief.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/adafactor.py` & `timm-1.0.3/timm/optim/adafactor.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/adahessian.py` & `timm-1.0.3/timm/optim/adahessian.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/adamp.py` & `timm-1.0.3/timm/optim/adamp.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/adamw.py` & `timm-1.0.3/timm/optim/adamw.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/adan.py` & `timm-1.0.3/timm/optim/adan.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/lamb.py` & `timm-1.0.3/timm/optim/lamb.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/lars.py` & `timm-1.0.3/timm/optim/lars.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/lion.py` & `timm-1.0.3/timm/optim/lion.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/lookahead.py` & `timm-1.0.3/timm/optim/lookahead.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/madgrad.py` & `timm-1.0.3/timm/optim/madgrad.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/nadam.py` & `timm-1.0.3/timm/optim/nadam.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/nadamw.py` & `timm-1.0.3/timm/optim/nadamw.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/nvnovograd.py` & `timm-1.0.3/timm/optim/nvnovograd.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/optim_factory.py` & `timm-1.0.3/timm/optim/optim_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .madgrad import MADGRAD
 from .nadam import Nadam
 from .nadamw import NAdamW
 from .nvnovograd import NvNovoGrad
 from .radam import RAdam
 from .rmsprop_tf import RMSpropTF
 from .sgdp import SGDP
+from .sgdw import SGDW
 
 
 _logger = logging.getLogger(__name__)
 
 
 # optimizers to default to multi-tensor
 _DEFAULT_FOREACH = {
@@ -284,14 +285,21 @@
         opt_args.pop('eps', None)
         optimizer = optim.SGD(parameters, momentum=momentum, nesterov=True, **opt_args)
     elif opt_lower == 'momentum':
         opt_args.pop('eps', None)
         optimizer = optim.SGD(parameters, momentum=momentum, nesterov=False, **opt_args)
     elif opt_lower == 'sgdp':
         optimizer = SGDP(parameters, momentum=momentum, nesterov=True, **opt_args)
+    elif opt_lower == 'sgdw' or opt_lower == 'nesterovw':
+        # NOTE 'sgd' refers to SGD + nesterov momentum for legacy / backwards compat reasons
+        opt_args.pop('eps', None)
+        optimizer = SGDW(parameters, momentum=momentum, nesterov=True, **opt_args)
+    elif opt_lower == 'momentumw':
+        opt_args.pop('eps', None)
+        optimizer = SGDW(parameters, momentum=momentum, nesterov=False, **opt_args)
 
     # adaptive
     elif opt_lower == 'adam':
         optimizer = optim.Adam(parameters, **opt_args) 
     elif opt_lower == 'adamw':
         optimizer = optim.AdamW(parameters, **opt_args)
     elif opt_lower == 'adamp':
```

### Comparing `timm-0.9.9/timm/optim/radam.py` & `timm-1.0.3/timm/optim/radam.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/rmsprop_tf.py` & `timm-1.0.3/timm/optim/rmsprop_tf.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/optim/sgdp.py` & `timm-1.0.3/timm/optim/sgdp.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/scheduler/cosine_lr.py` & `timm-1.0.3/timm/scheduler/cosine_lr.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Hacked together by / Copyright 2021 Ross Wightman
 """
 import logging
 import math
 import numpy as np
 import torch
+from typing import List
 
 from .scheduler import Scheduler
 
 
 _logger = logging.getLogger(__name__)
 
 
@@ -73,15 +74,15 @@
         self.k_decay = k_decay
         if self.warmup_t:
             self.warmup_steps = [(v - warmup_lr_init) / self.warmup_t for v in self.base_values]
             super().update_groups(self.warmup_lr_init)
         else:
             self.warmup_steps = [1 for _ in self.base_values]
 
-    def _get_lr(self, t):
+    def _get_lr(self, t: int) -> List[float]:
         if t < self.warmup_t:
             lrs = [self.warmup_lr_init + t * s for s in self.warmup_steps]
         else:
             if self.warmup_prefix:
                 t = t - self.warmup_t
 
             if self.cycle_mul != 1:
```

### Comparing `timm-0.9.9/timm/scheduler/multistep_lr.py` & `timm-1.0.3/timm/scheduler/multistep_lr.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             self.warmup_steps = [1 for _ in self.base_values]
 
     def get_curr_decay_steps(self, t):
         # find where in the array t goes,
         # assumes self.decay_t is sorted
         return bisect.bisect_right(self.decay_t, t + 1)
 
-    def _get_lr(self, t):
+    def _get_lr(self, t: int) -> List[float]:
         if t < self.warmup_t:
             lrs = [self.warmup_lr_init + t * s for s in self.warmup_steps]
         else:
             if self.warmup_prefix:
                 t = t - self.warmup_t
             lrs = [v * (self.decay_rate ** self.get_curr_decay_steps(t)) for v in self.base_values]
         return lrs
```

### Comparing `timm-0.9.9/timm/scheduler/plateau_lr.py` & `timm-1.0.3/timm/scheduler/plateau_lr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ Plateau Scheduler
 
 Adapts PyTorch plateau scheduler and allows application of noise, warmup.
 
 Hacked together by / Copyright 2020 Ross Wightman
 """
 import torch
+from typing import List
 
 from .scheduler import Scheduler
 
 
 class PlateauLRScheduler(Scheduler):
     """Decay the LR by a factor every time the validation loss plateaus."""
 
@@ -102,9 +103,9 @@
         for i, param_group in enumerate(self.optimizer.param_groups):
             old_lr = float(param_group['lr'])
             restore_lr.append(old_lr)
             new_lr = old_lr + old_lr * noise
             param_group['lr'] = new_lr
         self.restore_lr = restore_lr
 
-    def _get_lr(self, t: int) -> float:
+    def _get_lr(self, t: int) -> List[float]:
         assert False, 'should not be called as step is overridden'
```

### Comparing `timm-0.9.9/timm/scheduler/poly_lr.py` & `timm-1.0.3/timm/scheduler/poly_lr.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Polynomial LR schedule with warmup, noise.
 
 Hacked together by / Copyright 2021 Ross Wightman
 """
 import math
 import logging
+from typing import List
 
 import torch
 
 from .scheduler import Scheduler
 
 
 _logger = logging.getLogger(__name__)
@@ -69,15 +70,15 @@
         self.k_decay = k_decay
         if self.warmup_t:
             self.warmup_steps = [(v - warmup_lr_init) / self.warmup_t for v in self.base_values]
             super().update_groups(self.warmup_lr_init)
         else:
             self.warmup_steps = [1 for _ in self.base_values]
 
-    def _get_lr(self, t):
+    def _get_lr(self, t: int) -> List[float]:
         if t < self.warmup_t:
             lrs = [self.warmup_lr_init + t * s for s in self.warmup_steps]
         else:
             if self.warmup_prefix:
                 t = t - self.warmup_t
 
             if self.cycle_mul != 1:
```

### Comparing `timm-0.9.9/timm/scheduler/scheduler.py` & `timm-1.0.3/timm/scheduler/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 from abc import ABC
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 import torch
 
 
 class Scheduler(ABC):
     """ Parameter Scheduler Base Class
     A scheduler base class that can be used to schedule any optimizer parameter groups.
@@ -61,18 +61,18 @@
     def state_dict(self) -> Dict[str, Any]:
         return {key: value for key, value in self.__dict__.items() if key != 'optimizer'}
 
     def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
         self.__dict__.update(state_dict)
 
     @abc.abstractmethod
-    def _get_lr(self, t: int) -> float:
+    def _get_lr(self, t: int) -> List[float]:
         pass
 
-    def _get_values(self, t: int, on_epoch: bool = True) -> Optional[float]:
+    def _get_values(self, t: int, on_epoch: bool = True) -> Optional[List[float]]:
         proceed = (on_epoch and self.t_in_epochs) or (not on_epoch and not self.t_in_epochs)
         if not proceed:
             return None
         return self._get_lr(t)
 
     def step(self, epoch: int, metric: float = None) -> None:
         self.metric = metric
```

### Comparing `timm-0.9.9/timm/scheduler/scheduler_factory.py` & `timm-1.0.3/timm/scheduler/scheduler_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """ Scheduler Factory
 Hacked together by / Copyright 2021 Ross Wightman
 """
-from typing import List, Union
+from typing import List, Optional, Union
 
 from torch.optim import Optimizer
 
 from .cosine_lr import CosineLRScheduler
 from .multistep_lr import MultiStepLRScheduler
 from .plateau_lr import PlateauLRScheduler
 from .poly_lr import PolyLRScheduler
 from .step_lr import StepLRScheduler
 from .tanh_lr import TanhLRScheduler
 
 
-def scheduler_kwargs(cfg):
+def scheduler_kwargs(cfg, decreasing_metric: Optional[bool] = None):
     """ cfg/argparse to kwargs helper
     Convert scheduler args in argparse args or cfg (.dot) like object to keyword args.
     """
     eval_metric = getattr(cfg, 'eval_metric', 'top1')
-    plateau_mode = 'min' if 'loss' in eval_metric else 'max'
+    if decreasing_metric is not None:
+        plateau_mode = 'min' if decreasing_metric else 'max'
+    else:
+        plateau_mode = 'min' if 'loss' in eval_metric else 'max'
     kwargs = dict(
         sched=cfg.sched,
         num_epochs=getattr(cfg, 'epochs', 100),
         decay_epochs=getattr(cfg, 'decay_epochs', 30),
         decay_milestones=getattr(cfg, 'decay_milestones', [30, 60]),
         warmup_epochs=getattr(cfg, 'warmup_epochs', 5),
         cooldown_epochs=getattr(cfg, 'cooldown_epochs', 0),
```

### Comparing `timm-0.9.9/timm/scheduler/step_lr.py` & `timm-1.0.3/timm/scheduler/step_lr.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 Basic step LR schedule with warmup, noise.
 
 Hacked together by / Copyright 2020 Ross Wightman
 """
 import math
 import torch
+from typing import List
+
 
 from .scheduler import Scheduler
 
 
 class StepLRScheduler(Scheduler):
     """
     """
@@ -47,15 +49,15 @@
         self.warmup_prefix = warmup_prefix
         if self.warmup_t:
             self.warmup_steps = [(v - warmup_lr_init) / self.warmup_t for v in self.base_values]
             super().update_groups(self.warmup_lr_init)
         else:
             self.warmup_steps = [1 for _ in self.base_values]
 
-    def _get_lr(self, t):
+    def _get_lr(self, t: int) -> List[float]:
         if t < self.warmup_t:
             lrs = [self.warmup_lr_init + t * s for s in self.warmup_steps]
         else:
             if self.warmup_prefix:
                 t = t - self.warmup_t
             lrs = [v * (self.decay_rate ** (t // self.decay_t)) for v in self.base_values]
         return lrs
```

### Comparing `timm-0.9.9/timm/scheduler/tanh_lr.py` & `timm-1.0.3/timm/scheduler/tanh_lr.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Hacked together by / Copyright 2021 Ross Wightman
 """
 import logging
 import math
 import numpy as np
 import torch
+from typing import List
 
 from .scheduler import Scheduler
 
 
 _logger = logging.getLogger(__name__)
 
 
@@ -71,15 +72,15 @@
         if self.warmup_t:
             t_v = self.base_values if self.warmup_prefix else self._get_lr(self.warmup_t)
             self.warmup_steps = [(v - warmup_lr_init) / self.warmup_t for v in t_v]
             super().update_groups(self.warmup_lr_init)
         else:
             self.warmup_steps = [1 for _ in self.base_values]
 
-    def _get_lr(self, t):
+    def _get_lr(self, t: int) -> List[float]:
         if t < self.warmup_t:
             lrs = [self.warmup_lr_init + t * s for s in self.warmup_steps]
         else:
             if self.warmup_prefix:
                 t = t - self.warmup_t
 
             if self.cycle_mul != 1:
```

### Comparing `timm-0.9.9/timm/utils/__init__.py` & `timm-1.0.3/timm/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .agc import adaptive_clip_grad
+from .attention_extract import AttentionExtract
 from .checkpoint_saver import CheckpointSaver
 from .clip_grad import dispatch_clip_grad
 from .cuda import ApexScaler, NativeScaler
 from .decay_batch import decay_batch_step, check_batch_size_retry
 from .distributed import distribute_bn, reduce_tensor, init_distributed_device,\
     world_info_from_env, is_distributed_env, is_primary
 from .jit import set_jit_legacy, set_jit_fuser
 from .log import setup_default_logging, FormatterNoInfo
 from .metrics import AverageMeter, accuracy
 from .misc import natural_key, add_bool_arg, ParseKwargs
 from .model import unwrap_model, get_state_dict, freeze, unfreeze, reparameterize_model
-from .model_ema import ModelEma, ModelEmaV2
+from .model_ema import ModelEma, ModelEmaV2, ModelEmaV3
 from .random import random_seed
 from .summary import update_summary, get_outdir
```

### Comparing `timm-0.9.9/timm/utils/agc.py` & `timm-1.0.3/timm/utils/agc.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/utils/checkpoint_saver.py` & `timm-1.0.3/timm/utils/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/utils/clip_grad.py` & `timm-1.0.3/timm/utils/clip_grad.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/utils/cuda.py` & `timm-1.0.3/timm/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/utils/decay_batch.py` & `timm-1.0.3/timm/utils/decay_batch.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/utils/distributed.py` & `timm-1.0.3/timm/utils/distributed.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """ Distributed training/validation utils
 
 Hacked together by / Copyright 2020 Ross Wightman
 """
+import logging
 import os
+from typing import Optional
 
 import torch
 from torch import distributed as dist
 
-try:
-    import horovod.torch as hvd
-except ImportError:
-    hvd = None
-
 from .model import unwrap_model
 
+_logger = logging.getLogger(__name__)
+
 
 def reduce_tensor(tensor, n):
     rt = tensor.clone()
     dist.all_reduce(rt, op=dist.ReduceOp.SUM)
     rt /= n
     return rt
 
@@ -80,58 +79,101 @@
 def init_distributed_device(args):
     # Distributed training = training on more than one GPU.
     # Works in both single and multi-node scenarios.
     args.distributed = False
     args.world_size = 1
     args.rank = 0  # global rank
     args.local_rank = 0
+    result = init_distributed_device_so(
+        device=getattr(args, 'device', 'cuda'),
+        dist_backend=getattr(args, 'dist_backend', None),
+        dist_url=getattr(args, 'dist_url', None),
+    )
+    args.device = result['device']
+    args.world_size = result['world_size']
+    args.rank = result['global_rank']
+    args.local_rank = result['local_rank']
+    args.distributed = result['distributed']
+    device = torch.device(args.device)
+    return device
+
+
+def init_distributed_device_so(
+        device: str = 'cuda',
+        dist_backend: Optional[str] = None,
+        dist_url: Optional[str] = None,
+):
+    # Distributed training = training on more than one GPU.
+    # Works in both single and multi-node scenarios.
+    distributed = False
+    world_size = 1
+    global_rank = 0
+    local_rank = 0
+    device_type, *device_idx = device.split(':', maxsplit=1)
+
+    if dist_backend is None:
+        # FIXME: verify that ROCm transform nccl to rccl
+        dist_backends = {
+            "xpu": "ccl",
+            "hpu": "hccl",
+            "cuda": "nccl",
+        }
+        dist_backend = dist_backends.get(device_type, 'gloo')
+    dist_url = dist_url or 'env://'
 
     # TBD, support horovod?
     # if args.horovod:
+    #     import horovod.torch as hvd
     #     assert hvd is not None, "Horovod is not installed"
     #     hvd.init()
     #     args.local_rank = int(hvd.local_rank())
     #     args.rank = hvd.rank()
     #     args.world_size = hvd.size()
     #     args.distributed = True
     #     os.environ['LOCAL_RANK'] = str(args.local_rank)
     #     os.environ['RANK'] = str(args.rank)
     #     os.environ['WORLD_SIZE'] = str(args.world_size)
-    dist_backend = getattr(args, 'dist_backend', 'nccl')
-    dist_url = getattr(args, 'dist_url', 'env://')
     if is_distributed_env():
         if 'SLURM_PROCID' in os.environ:
             # DDP via SLURM
-            args.local_rank, args.rank, args.world_size = world_info_from_env()
+            local_rank, global_rank, world_size = world_info_from_env()
             # SLURM var -> torch.distributed vars in case needed
-            os.environ['LOCAL_RANK'] = str(args.local_rank)
-            os.environ['RANK'] = str(args.rank)
-            os.environ['WORLD_SIZE'] = str(args.world_size)
+            os.environ['LOCAL_RANK'] = str(local_rank)
+            os.environ['RANK'] = str(global_rank)
+            os.environ['WORLD_SIZE'] = str(world_size)
             torch.distributed.init_process_group(
                 backend=dist_backend,
                 init_method=dist_url,
-                world_size=args.world_size,
-                rank=args.rank,
+                world_size=world_size,
+                rank=global_rank,
             )
         else:
             # DDP via torchrun, torch.distributed.launch
-            args.local_rank, _, _ = world_info_from_env()
+            local_rank, _, _ = world_info_from_env()
             torch.distributed.init_process_group(
                 backend=dist_backend,
                 init_method=dist_url,
             )
-            args.world_size = torch.distributed.get_world_size()
-            args.rank = torch.distributed.get_rank()
-        args.distributed = True
-
-    if torch.cuda.is_available():
-        if args.distributed:
-            device = 'cuda:%d' % args.local_rank
-        else:
-            device = 'cuda:0'
+            world_size = torch.distributed.get_world_size()
+            global_rank = torch.distributed.get_rank()
+        distributed = True
+
+    if device_type == 'cuda':
+        assert torch.cuda.is_available(), f'CUDA is not available but {device} was specified.'
+
+    if distributed and device != 'cpu':
+        # Ignore manually specified device index in distributed mode and
+        # override with resolved local rank, fewer headaches in most setups.
+        if device_idx:
+            _logger.warning(f'device index {device_idx[0]} removed from specified ({device}).')
+        device = f'{device_type}:{local_rank}'
+
+    if device.startswith('cuda:'):
         torch.cuda.set_device(device)
-    else:
-        device = 'cpu'
 
-    args.device = device
-    device = torch.device(device)
-    return device
+    return dict(
+        device=device,
+        global_rank=global_rank,
+        local_rank=local_rank,
+        world_size=world_size,
+        distributed=distributed,
+    )
```

### Comparing `timm-0.9.9/timm/utils/jit.py` & `timm-1.0.3/timm/utils/jit.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/utils/log.py` & `timm-1.0.3/timm/utils/log.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/utils/metrics.py` & `timm-1.0.3/timm/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/utils/misc.py` & `timm-1.0.3/timm/utils/misc.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/utils/model.py` & `timm-1.0.3/timm/utils/model.py`

 * *Files identical despite different names*

### Comparing `timm-0.9.9/timm/utils/onnx.py` & `timm-1.0.3/timm/utils/onnx.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         check_forward: bool = False,
         batch_size: int = 64,
         input_size: Tuple[int, int, int] = None,
         opset: Optional[int] = None,
         dynamic_size: bool = False,
         aten_fallback: bool = False,
         keep_initializers: Optional[bool] = None,
+        use_dynamo: bool = False,
         input_names: List[str] = None,
         output_names: List[str] = None,
 ):
     import onnx
 
     if training:
         training_mode = torch.onnx.TrainingMode.TRAINING
@@ -49,47 +50,60 @@
     # Run model once before export trace, sets padding for models with Conv2dSameExport. This means
     # that the padding for models with Conv2dSameExport (most models with tf_ prefix) is fixed for
     # the input img_size specified in this script.
 
     # Opset >= 11 should allow for dynamic padding, however I cannot get it to work due to
     # issues in the tracing of the dynamic padding or errors attempting to export the model after jit
     # scripting it (an approach that should work). Perhaps in a future PyTorch or ONNX versions...
-    original_out = model(example_input)
+    with torch.no_grad():
+        original_out = model(example_input)
 
     input_names = input_names or ["input0"]
     output_names = output_names or ["output0"]
 
     dynamic_axes = {'input0': {0: 'batch'}, 'output0': {0: 'batch'}}
     if dynamic_size:
         dynamic_axes['input0'][2] = 'height'
         dynamic_axes['input0'][3] = 'width'
 
     if aten_fallback:
         export_type = torch.onnx.OperatorExportTypes.ONNX_ATEN_FALLBACK
     else:
         export_type = torch.onnx.OperatorExportTypes.ONNX
 
-    torch_out = torch.onnx._export(
-        model,
-        example_input,
-        output_file,
-        training=training_mode,
-        export_params=True,
-        verbose=verbose,
-        input_names=input_names,
-        output_names=output_names,
-        keep_initializers_as_inputs=keep_initializers,
-        dynamic_axes=dynamic_axes,
-        opset_version=opset,
-        operator_export_type=export_type
-    )
+    if use_dynamo:
+        export_options = torch.onnx.ExportOptions(dynamic_shapes=dynamic_size)
+        export_output = torch.onnx.dynamo_export(
+            model,
+            example_input,
+            export_options=export_options,
+        )
+        export_output.save(output_file)
+        torch_out = None
+    else:
+        torch_out = torch.onnx._export(
+            model,
+            example_input,
+            output_file,
+            training=training_mode,
+            export_params=True,
+            verbose=verbose,
+            input_names=input_names,
+            output_names=output_names,
+            keep_initializers_as_inputs=keep_initializers,
+            dynamic_axes=dynamic_axes,
+            opset_version=opset,
+            operator_export_type=export_type
+        )
 
     if check:
         onnx_model = onnx.load(output_file)
         onnx.checker.check_model(onnx_model, full_check=True)  # assuming throw on error
         if check_forward and not training:
             import numpy as np
             onnx_out = onnx_forward(output_file, example_input)
-            np.testing.assert_almost_equal(torch_out.data.numpy(), onnx_out, decimal=3)
-            np.testing.assert_almost_equal(original_out.data.numpy(), torch_out.data.numpy(), decimal=5)
-
+            if torch_out is not None:
+                np.testing.assert_almost_equal(torch_out.numpy(), onnx_out, decimal=3)
+                np.testing.assert_almost_equal(original_out.numpy(), torch_out.numpy(), decimal=5)
+            else:
+                np.testing.assert_almost_equal(original_out.numpy(), onnx_out, decimal=3)
```

### Comparing `timm-0.9.9/timm/utils/summary.py` & `timm-1.0.3/timm/utils/summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         filename,
         lr=None,
         write_header=False,
         log_wandb=False,
 ):
     rowd = OrderedDict(epoch=epoch)
     rowd.update([('train_' + k, v) for k, v in train_metrics.items()])
-    rowd.update([('eval_' + k, v) for k, v in eval_metrics.items()])
+    if eval_metrics:
+        rowd.update([('eval_' + k, v) for k, v in eval_metrics.items()])
     if lr is not None:
         rowd['lr'] = lr
     if log_wandb:
         wandb.log(rowd)
     with open(filename, mode='a') as cf:
         dw = csv.DictWriter(cf, fieldnames=rowd.keys())
         if write_header:  # first iteration (epoch == 1 can't be used)
```

