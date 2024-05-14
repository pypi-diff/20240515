# Comparing `tmp/vis4d-0.0.tar.gz` & `tmp/vis4d-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vis4d-0.0.tar", last modified: Tue Nov  2 16:43:18 2021, max compression
+gzip compressed data, was "vis4d-0.1.tar", last modified: Tue May 14 22:03:16 2024, max compression
```

## Comparing `vis4d-0.0.tar` & `vis4d-0.1.tar`

### file list

```diff
@@ -1,175 +1,514 @@
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.380727 vis4d-0.0/
--rw-r--r--   0 fisher     (501) staff       (20)    10803 2021-08-12 15:17:48.000000 vis4d-0.0/LICENSE
--rw-r--r--   0 fisher     (501) staff       (20)     2480 2021-11-02 16:43:18.380837 vis4d-0.0/PKG-INFO
--rw-r--r--   0 fisher     (501) staff       (20)     1868 2021-11-02 16:40:34.000000 vis4d-0.0/README.md
--rw-r--r--   0 fisher     (501) staff       (20)      633 2021-07-23 10:07:49.000000 vis4d-0.0/pyproject.toml
--rw-r--r--   0 fisher     (501) staff       (20)     1657 2021-11-02 16:43:18.381775 vis4d-0.0/setup.cfg
--rwxr-xr-x   0 fisher     (501) staff       (20)     1373 2021-11-02 16:40:34.000000 vis4d-0.0/setup.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.342465 vis4d-0.0/vis4d/
--rw-r--r--   0 fisher     (501) staff       (20)       31 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/__init__.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.344793 vis4d-0.0/vis4d/common/
--rw-r--r--   0 fisher     (501) staff       (20)       27 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/__init__.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.345413 vis4d-0.0/vis4d/common/bbox/
--rw-r--r--   0 fisher     (501) staff       (20)       33 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/__init__.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.346908 vis4d-0.0/vis4d/common/bbox/coders/
--rw-r--r--   0 fisher     (501) staff       (20)      412 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/coders/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     2355 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/coders/base.py
--rw-r--r--   0 fisher     (501) staff       (20)     5320 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/coders/box3d_coder.py
--rw-r--r--   0 fisher     (501) staff       (20)      691 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/coders/box3d_coder_test.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.348481 vis4d-0.0/vis4d/common/bbox/matchers/
--rw-r--r--   0 fisher     (501) staff       (20)      248 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/matchers/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     1420 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/matchers/base.py
--rw-r--r--   0 fisher     (501) staff       (20)     4919 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/matchers/max_iou.py
--rw-r--r--   0 fisher     (501) staff       (20)     1179 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/matchers/max_iou_test.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.350002 vis4d-0.0/vis4d/common/bbox/poolers/
--rw-r--r--   0 fisher     (501) staff       (20)      248 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/poolers/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     1133 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/poolers/base.py
--rw-r--r--   0 fisher     (501) staff       (20)     6235 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/poolers/roi_pooler.py
--rw-r--r--   0 fisher     (501) staff       (20)     1940 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/poolers/roi_pooler_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     2422 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/poolers/utils.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.352417 vis4d-0.0/vis4d/common/bbox/samplers/
--rw-r--r--   0 fisher     (501) staff       (20)      404 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/samplers/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     2433 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/samplers/base.py
--rw-r--r--   0 fisher     (501) staff       (20)     8946 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/samplers/combined.py
--rw-r--r--   0 fisher     (501) staff       (20)     3117 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/samplers/combined_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     2150 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/samplers/random.py
--rw-r--r--   0 fisher     (501) staff       (20)     2012 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/samplers/random_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     1481 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/samplers/utils.py
--rw-r--r--   0 fisher     (501) staff       (20)     1792 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/bbox/utils.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.354707 vis4d-0.0/vis4d/common/geometry/
--rw-r--r--   0 fisher     (501) staff       (20)       28 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/geometry/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     2539 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/geometry/projection.py
--rw-r--r--   0 fisher     (501) staff       (20)     1803 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/geometry/projection_test.py
--rw-r--r--   0 fisher     (501) staff       (20)    14841 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/geometry/rotation.py
--rw-r--r--   0 fisher     (501) staff       (20)     8266 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/geometry/rotation_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     1332 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/geometry/transform.py
--rw-r--r--   0 fisher     (501) staff       (20)     1847 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/geometry/transform_test.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.356019 vis4d-0.0/vis4d/common/io/
--rw-r--r--   0 fisher     (501) staff       (20)      259 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/io/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     1727 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/io/backend_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     1102 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/io/base.py
--rw-r--r--   0 fisher     (501) staff       (20)      648 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/io/file.py
--rw-r--r--   0 fisher     (501) staff       (20)     2244 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/io/hdf5.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.356570 vis4d-0.0/vis4d/common/layers/
--rw-r--r--   0 fisher     (501) staff       (20)      112 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/layers/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     2460 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/layers/conv2d.py
--rw-r--r--   0 fisher     (501) staff       (20)     2015 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/registry.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.357647 vis4d-0.0/vis4d/common/utils/
--rw-r--r--   0 fisher     (501) staff       (20)      148 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/utils/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     6369 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/utils/distributed.py
--rw-r--r--   0 fisher     (501) staff       (20)     1639 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/common/utils/time.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.358932 vis4d-0.0/vis4d/config/
--rw-r--r--   0 fisher     (501) staff       (20)      215 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/config/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     6530 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/config/config.py
--rw-r--r--   0 fisher     (501) staff       (20)     1443 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/config/config_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     1702 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/config/defaults.py
--rw-r--r--   0 fisher     (501) staff       (20)      620 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/config/defaults_test.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.360462 vis4d-0.0/vis4d/data/
--rw-r--r--   0 fisher     (501) staff       (20)      288 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     5639 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/build.py
--rw-r--r--   0 fisher     (501) staff       (20)    22054 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/dataset.py
--rw-r--r--   0 fisher     (501) staff       (20)     7466 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/dataset_test.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.363083 vis4d-0.0/vis4d/data/datasets/
--rw-r--r--   0 fisher     (501) staff       (20)      606 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/datasets/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     4845 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/datasets/base.py
--rw-r--r--   0 fisher     (501) staff       (20)      987 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/datasets/bdd100k.py
--rw-r--r--   0 fisher     (501) staff       (20)     1048 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/datasets/coco.py
--rw-r--r--   0 fisher     (501) staff       (20)     1746 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/datasets/custom.py
--rw-r--r--   0 fisher     (501) staff       (20)     1490 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/datasets/kitti.py
--rw-r--r--   0 fisher     (501) staff       (20)     2060 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/datasets/nuscenes.py
--rw-r--r--   0 fisher     (501) staff       (20)      801 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/datasets/scalabel.py
--rw-r--r--   0 fisher     (501) staff       (20)     2885 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/datasets/to_hdf5.py
--rw-r--r--   0 fisher     (501) staff       (20)      994 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/datasets/to_hdf5_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     2332 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/datasets/waymo.py
--rw-r--r--   0 fisher     (501) staff       (20)     1931 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/samplers.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.365272 vis4d-0.0/vis4d/data/transforms/
--rw-r--r--   0 fisher     (501) staff       (20)      570 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/transforms/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)    16927 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/transforms/augmentations.py
--rw-r--r--   0 fisher     (501) staff       (20)     5554 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/transforms/augmentations_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     4182 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/transforms/base.py
--rw-r--r--   0 fisher     (501) staff       (20)     1642 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/transforms/base_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     4724 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/transforms/kornia_wrappers.py
--rw-r--r--   0 fisher     (501) staff       (20)     4154 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/transforms/kornia_wrappers_test.py
--rw-r--r--   0 fisher     (501) staff       (20)      728 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/transforms/utils.py
--rw-r--r--   0 fisher     (501) staff       (20)     1587 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/transforms/utils_test.py
--rw-r--r--   0 fisher     (501) staff       (20)    10923 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/data/utils.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.366929 vis4d-0.0/vis4d/engine/
--rw-r--r--   0 fisher     (501) staff       (20)       32 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/engine/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     9077 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/engine/evaluator.py
--rw-r--r--   0 fisher     (501) staff       (20)     8700 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/engine/trainer.py
--rw-r--r--   0 fisher     (501) staff       (20)     7990 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/engine/trainer_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     6196 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/engine/utils.py
--rw-r--r--   0 fisher     (501) staff       (20)     1154 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/engine/utils_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     4210 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/engine/writer.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.367875 vis4d-0.0/vis4d/model/
--rw-r--r--   0 fisher     (501) staff       (20)      341 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     6301 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/base.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.369519 vis4d-0.0/vis4d/model/detect/
--rw-r--r--   0 fisher     (501) staff       (20)      280 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/detect/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     1763 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/detect/base.py
--rw-r--r--   0 fisher     (501) staff       (20)     5874 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/detect/d2_utils.py
--rw-r--r--   0 fisher     (501) staff       (20)      991 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/detect/d2_utils_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     7922 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/detect/d2_wrapper.py
--rw-r--r--   0 fisher     (501) staff       (20)     8775 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/detect/mmdet_utils.py
--rw-r--r--   0 fisher     (501) staff       (20)     8667 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/detect/mmdet_wrapper.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.370404 vis4d-0.0/vis4d/model/detect/roi_head/
--rw-r--r--   0 fisher     (501) staff       (20)      234 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/detect/roi_head/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     2130 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/detect/roi_head/base.py
--rw-r--r--   0 fisher     (501) staff       (20)    13604 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/detect/roi_head/qd_3dt_bbox3d_head.py
--rw-r--r--   0 fisher     (501) staff       (20)     2925 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/detect/roi_head/qd_3dt_bbox3d_head_test.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.372115 vis4d-0.0/vis4d/model/losses/
--rw-r--r--   0 fisher     (501) staff       (20)      424 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/losses/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     1066 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/losses/base.py
--rw-r--r--   0 fisher     (501) staff       (20)     4399 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/losses/box3d_uncertainty_loss.py
--rw-r--r--   0 fisher     (501) staff       (20)     3584 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/losses/embedding_distance.py
--rw-r--r--   0 fisher     (501) staff       (20)     5213 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/losses/losses_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     2267 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/losses/multi_pos_cross_entropy.py
--rw-r--r--   0 fisher     (501) staff       (20)     2344 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/losses/utils.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.372878 vis4d-0.0/vis4d/model/optimize/
--rw-r--r--   0 fisher     (501) staff       (20)      407 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/optimize/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     1555 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/optimize/optimizer.py
--rw-r--r--   0 fisher     (501) staff       (20)     3332 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/optimize/scheduler.py
--rw-r--r--   0 fisher     (501) staff       (20)     5719 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/qd_3dt.py
--rwxr-xr-x   0 fisher     (501) staff       (20)     7463 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/qdtrack.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.373913 vis4d-0.0/vis4d/model/segment/
--rw-r--r--   0 fisher     (501) staff       (20)      151 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/segment/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     1203 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/segment/base.py
--rw-r--r--   0 fisher     (501) staff       (20)     3734 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/segment/mmseg_utils.py
--rw-r--r--   0 fisher     (501) staff       (20)     7077 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/segment/mmseg_wrapper.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.374451 vis4d-0.0/vis4d/model/track/
--rw-r--r--   0 fisher     (501) staff       (20)       30 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/track/__init__.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.375573 vis4d-0.0/vis4d/model/track/graph/
--rw-r--r--   0 fisher     (501) staff       (20)      253 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/track/graph/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     1685 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/track/graph/base.py
--rw-r--r--   0 fisher     (501) staff       (20)    10251 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/track/graph/quasi_dense.py
--rw-r--r--   0 fisher     (501) staff       (20)     2831 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/track/graph/quasi_dense_test.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.376310 vis4d-0.0/vis4d/model/track/similarity/
--rw-r--r--   0 fisher     (501) staff       (20)      303 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/track/similarity/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     2523 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/track/similarity/base.py
--rwxr-xr-x   0 fisher     (501) staff       (20)    11643 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/track/similarity/quasi_dense_embedding_head.py
--rw-r--r--   0 fisher     (501) staff       (20)     1667 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/model/track/utils.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.378450 vis4d-0.0/vis4d/struct/
--rw-r--r--   0 fisher     (501) staff       (20)      724 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/struct/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     7350 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/struct/data.py
--rw-r--r--   0 fisher     (501) staff       (20)     2310 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/struct/data_test.py
--rw-r--r--   0 fisher     (501) staff       (20)    29556 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/struct/labels.py
--rw-r--r--   0 fisher     (501) staff       (20)    13819 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/struct/labels_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     5862 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/struct/sample.py
--rw-r--r--   0 fisher     (501) staff       (20)     2173 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/struct/structures.py
--rw-r--r--   0 fisher     (501) staff       (20)     2018 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/struct/utils.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.378957 vis4d-0.0/vis4d/unittest/
--rw-r--r--   0 fisher     (501) staff       (20)       30 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/unittest/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     4099 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/unittest/utils.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.380486 vis4d-0.0/vis4d/vis/
--rw-r--r--   0 fisher     (501) staff       (20)      128 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/vis/__init__.py
--rw-r--r--   0 fisher     (501) staff       (20)     6353 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/vis/image.py
--rw-r--r--   0 fisher     (501) staff       (20)     1926 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/vis/track.py
--rw-r--r--   0 fisher     (501) staff       (20)     1149 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/vis/track_test.py
--rw-r--r--   0 fisher     (501) staff       (20)     7801 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/vis/utils.py
--rw-r--r--   0 fisher     (501) staff       (20)     4294 2021-11-02 16:40:34.000000 vis4d-0.0/vis4d/vis/utils_test.py
-drwxr-xr-x   0 fisher     (501) staff       (20)        0 2021-11-02 16:43:18.344175 vis4d-0.0/vis4d.egg-info/
--rw-r--r--   0 fisher     (501) staff       (20)     2480 2021-11-02 16:43:18.000000 vis4d-0.0/vis4d.egg-info/PKG-INFO
--rw-r--r--   0 fisher     (501) staff       (20)     4456 2021-11-02 16:43:18.000000 vis4d-0.0/vis4d.egg-info/SOURCES.txt
--rw-r--r--   0 fisher     (501) staff       (20)        1 2021-11-02 16:43:18.000000 vis4d-0.0/vis4d.egg-info/dependency_links.txt
--rw-r--r--   0 fisher     (501) staff       (20)      113 2021-11-02 16:43:18.000000 vis4d-0.0/vis4d.egg-info/requires.txt
--rw-r--r--   0 fisher     (501) staff       (20)        6 2021-11-02 16:43:18.000000 vis4d-0.0/vis4d.egg-info/top_level.txt
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.695811 vis4d-0.1/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10804 2023-03-14 17:53:09.000000 vis4d-0.1/LICENSE
+-rw-r--r--   0 yangyun  (577304) yangyun-group (478020)     4929 2024-05-14 22:03:16.683811 vis4d-0.1/PKG-INFO
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3612 2024-05-08 13:14:51.000000 vis4d-0.1/README.md
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3380 2024-05-14 21:54:27.000000 vis4d-0.1/pyproject.toml
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.303809 vis4d-0.1/requirements/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      429 2024-04-18 19:32:08.000000 vis4d-0.1/requirements/install.txt
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       38 2024-05-14 22:03:16.695811 vis4d-0.1/setup.cfg
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.335809 vis4d-0.1/vis4d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      621 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       91 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/__main__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.499809 vis4d-0.1/vis4d/common/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      692 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5822 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/array.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14835 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/ckpt.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2886 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/dict.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13271 2024-04-09 12:01:41.000000 vis4d-0.1/vis4d/common/distributed.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1821 2024-04-24 13:26:36.000000 vis4d-0.1/vis4d/common/imports.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4308 2024-04-24 13:26:36.000000 vis4d-0.1/vis4d/common/logging.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1478 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/named_tuple.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2580 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/prettyprint.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1666 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/progress.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2039 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/slurm.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1733 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/time.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2207 2024-04-24 13:26:36.000000 vis4d-0.1/vis4d/common/typing.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3092 2024-04-24 13:26:36.000000 vis4d-0.1/vis4d/common/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.543809 vis4d-0.1/vis4d/config/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      321 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/config/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    19095 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/config/config_dict.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8582 2024-04-24 13:26:36.000000 vis4d-0.1/vis4d/config/registry.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    11670 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/config/replicator.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    17951 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/config/show_connection.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1247 2024-04-24 13:26:36.000000 vis4d-0.1/vis4d/config/sweep.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6716 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/config/typing.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.599809 vis4d-0.1/vis4d/data/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      555 2023-07-03 10:21:11.000000 vis4d-0.1/vis4d/data/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4778 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/cbgs.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4818 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/const.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5210 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/data_pipe.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.667809 vis4d-0.1/vis4d/data/datasets/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      419 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3694 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2935 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10743 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/coco.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5656 2023-07-03 10:21:11.000000 vis4d-0.1/vis4d/data/datasets/imagenet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    34589 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/datasets/nuscenes.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3510 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/nuscenes_detection.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8589 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/nuscenes_mono.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8796 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/nuscenes_trajectory.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8331 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/s3dis.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    27184 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/scalabel.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    21176 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4312 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/torchvision.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12456 2024-04-30 12:05:33.000000 vis4d-0.1/vis4d/data/datasets/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.695809 vis4d-0.1/vis4d/data/io/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      231 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/io/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2403 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/io/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2255 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/io/file.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10602 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/io/hdf5.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      521 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/io/util.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7138 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/io/zip.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3819 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/iterable.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8037 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/loader.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7868 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/reference.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2611 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/resample.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3252 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/samplers.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.799809 vis4d-0.1/vis4d/data/transforms/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      120 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9528 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/affine.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6781 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/autoaugment.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8674 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    17604 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/crop.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    11967 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/flip.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2210 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/mask.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13546 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/mixup.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12423 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/mosaic.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1615 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/normalize.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5295 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/pad.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12307 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/photometric.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8694 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/point_sampling.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9324 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/points.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5447 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/post_process.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3493 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/random_erasing.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    18353 2024-05-02 21:04:55.000000 vis4d-0.1/vis4d/data/transforms/resize.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1687 2023-08-03 09:28:00.000000 vis4d-0.1/vis4d/data/transforms/select_sensor.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1517 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/to_tensor.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      615 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/typing.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.831809 vis4d-0.1/vis4d/engine/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       25 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/engine/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.895809 vis4d-0.1/vis4d/engine/callbacks/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      676 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6127 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3112 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/checkpoint.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1139 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/ema.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4410 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/engine/callbacks/evaluator.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4304 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/logging.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1607 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/trainer_state.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3585 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/visualizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7348 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/yolox_callbacks.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.935809 vis4d-0.1/vis4d/engine/connectors/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      725 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/connectors/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3752 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/connectors/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5124 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/connectors/multi_sensor.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4910 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/connectors/util.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7811 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/engine/experiment.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1093 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/flag.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7286 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/loss_module.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.963809 vis4d-0.1/vis4d/engine/optim/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      292 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/optim/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5863 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/optim/optimizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9222 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/engine/optim/scheduler.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7243 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/engine/parser.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2361 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/run.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14371 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/trainer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7431 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.975809 vis4d-0.1/vis4d/eval/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      114 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6203 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/base.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.995809 vis4d-0.1/vis4d/eval/bdd100k/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      249 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/bdd100k/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      995 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/bdd100k/detect.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3341 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/bdd100k/seg.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2803 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/bdd100k/track.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.003809 vis4d-0.1/vis4d/eval/coco/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      104 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/coco/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9593 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/coco/detect.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.027809 vis4d-0.1/vis4d/eval/common/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      350 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/common/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6427 2023-06-09 09:06:39.000000 vis4d-0.1/vis4d/eval/common/binary.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4445 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/common/cls.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7563 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/eval/common/depth.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4933 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/common/flow.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6603 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/common/seg.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.035809 vis4d-0.1/vis4d/eval/kitti/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       98 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/kitti/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2683 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/kitti/depth.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.047809 vis4d-0.1/vis4d/eval/metrics/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       20 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/metrics/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1049 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/metrics/cls.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4852 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/eval/metrics/depth.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1558 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/metrics/flow.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.063809 vis4d-0.1/vis4d/eval/nuscenes/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      184 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/nuscenes/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    11306 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/nuscenes/detect3d.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5327 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/nuscenes/track3d.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.111810 vis4d-0.1/vis4d/eval/scalabel/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      250 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/scalabel/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2215 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/scalabel/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4614 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/scalabel/detect.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5177 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/scalabel/track.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.143810 vis4d-0.1/vis4d/eval/shift/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      465 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/shift/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1465 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/shift/depth.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      556 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/shift/detect.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      552 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/shift/flow.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10530 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/shift/multitask_writer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1831 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/shift/seg.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      629 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/shift/track.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      822 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/utils.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.155809 vis4d-0.1/vis4d/model/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      232 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/model/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.167810 vis4d-0.1/vis4d/model/adapter/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      129 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/adapter/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3991 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/adapter/ema.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1399 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/model/adapter/flops.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.215810 vis4d-0.1/vis4d/model/cls/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      158 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/cls/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      257 2023-07-03 10:21:11.000000 vis4d-0.1/vis4d/model/cls/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4842 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/cls/vit.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.235810 vis4d-0.1/vis4d/model/detect/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       70 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/model/detect/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6511 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/detect/faster_rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7952 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/detect/mask_rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6381 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/detect/retinanet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5310 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/detect/yolox.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.243810 vis4d-0.1/vis4d/model/detect3d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       27 2023-08-25 09:31:21.000000 vis4d-0.1/vis4d/model/detect3d/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5221 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/detect3d/bevformer.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.259810 vis4d-0.1/vis4d/model/motion/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       21 2023-07-25 13:00:55.000000 vis4d-0.1/vis4d/model/motion/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9736 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/motion/velo_lstm.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.271810 vis4d-0.1/vis4d/model/seg/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       36 2023-04-14 18:49:01.000000 vis4d-0.1/vis4d/model/seg/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2301 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/seg/fcn_resnet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4601 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/model/seg/semantic_fpn.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.279810 vis4d-0.1/vis4d/model/segment3d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4288 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/segment3d/pointnet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2838 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/model/segment3d/pointnetpp.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.291810 vis4d-0.1/vis4d/model/track/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       57 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/model/track/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    20090 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/track/qdtrack.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      668 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/track/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.299810 vis4d-0.1/vis4d/model/track3d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       57 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/model/track3d/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    20943 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/track3d/cc_3dt.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.311810 vis4d-0.1/vis4d/op/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      416 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/op/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.359810 vis4d-0.1/vis4d/op/base/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      218 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1754 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9731 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/csp_darknet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    15970 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/dla.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13764 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/pointnet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    15986 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/pointnetpp.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    20419 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/base/resnet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5751 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/unet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3581 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/vgg.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9246 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/vit.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.383810 vis4d-0.1/vis4d/op/box/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       39 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/op/box/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.399810 vis4d-0.1/vis4d/op/box/anchor/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      227 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/anchor/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13297 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/anchor/anchor_generator.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8162 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/anchor/point_generator.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      732 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/anchor/util.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14436 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/box/box2d.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4530 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/box3d.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.471810 vis4d-0.1/vis4d/op/box/encoder/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      291 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/encoder/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3807 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/encoder/bevformer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7631 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/encoder/delta_xywh.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5272 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/encoder/qd_3dt.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      972 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/encoder/yolox.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.487810 vis4d-0.1/vis4d/op/box/matchers/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      206 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/matchers/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1004 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/matchers/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4532 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/matchers/max_iou.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9330 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/matchers/sim_ota.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.503810 vis4d-0.1/vis4d/op/box/poolers/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      186 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/poolers/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      602 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/poolers/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6783 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/poolers/roi_pooler.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2458 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/poolers/utils.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.519810 vis4d-0.1/vis4d/op/box/samplers/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      355 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/samplers/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2356 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/samplers/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7931 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/samplers/combined.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1126 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/samplers/pseudo.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1982 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/samplers/random.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.579810 vis4d-0.1/vis4d/op/detect/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       23 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/op/detect/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      451 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12497 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/dense_anchor.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7840 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/faster_rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14343 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/mask_rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    16244 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/detect/rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14467 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/retinanet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    15586 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/rpn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    25636 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/yolox.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.599810 vis4d-0.1/vis4d/op/detect3d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       26 2023-07-25 13:00:55.000000 vis4d-0.1/vis4d/op/detect3d/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.667810 vis4d-0.1/vis4d/op/detect3d/bevformer/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      132 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10575 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/bevformer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14626 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/decoder.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14090 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/encoder.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2267 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/grid_mask.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14179 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/spatial_cross_attention.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10074 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/temporal_self_attention.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9741 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/transformer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      601 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    22844 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/detect3d/qd_3dt.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3865 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.699810 vis4d-0.1/vis4d/op/fpp/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      371 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/fpp/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      848 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/fpp/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5434 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/fpp/dla_up.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4289 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/fpp/fpn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5514 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/fpp/yolox_pafpn.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.711810 vis4d-0.1/vis4d/op/geometry/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       28 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/op/geometry/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4744 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/geometry/projection.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    17664 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/geometry/rotation.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3876 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/geometry/transform.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.823810 vis4d-0.1/vis4d/op/layer/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      602 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7960 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/layer/attention.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8467 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/conv2d.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4326 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/csp_layer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3123 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/deform_conv.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2090 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/drop.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3725 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/mlp.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12624 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/layer/ms_deform_attn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2971 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/patch_embed.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9019 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/positional_encoding.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8464 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/layer/transformer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2272 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/layer/util.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3856 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/weight_init.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.863810 vis4d-0.1/vis4d/op/loss/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      759 2023-07-27 00:26:02.000000 vis4d-0.1/vis4d/op/loss/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      758 2023-04-12 12:58:33.000000 vis4d-0.1/vis4d/op/loss/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3743 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/loss/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2422 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/loss/cross_entropy.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3616 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/loss/embedding_distance.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2657 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/loss/iou_loss.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2286 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/loss/multi_level_seg_loss.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1841 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/loss/multi_pos_cross_entropy.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1953 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/loss/orthogonal_transform_loss.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1700 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/loss/reducer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1426 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/loss/seg_cross_entropy_loss.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.879810 vis4d-0.1/vis4d/op/mask/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       43 2023-11-27 16:38:34.000000 vis4d-0.1/vis4d/op/mask/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9149 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/mask/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.891810 vis4d-0.1/vis4d/op/motion/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       25 2023-07-25 13:00:55.000000 vis4d-0.1/vis4d/op/motion/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2178 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/motion/kalman_filter.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1744 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/motion/velo_lstm.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.903810 vis4d-0.1/vis4d/op/seg/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       24 2023-04-14 18:49:01.000000 vis4d-0.1/vis4d/op/seg/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3791 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/seg/fcn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4284 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/seg/semantic_fpn.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.931810 vis4d-0.1/vis4d/op/track/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       30 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/op/track/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1962 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/track/assignment.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      571 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/track/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1472 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/track/matching.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    25273 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/track/qdtrack.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.947811 vis4d-0.1/vis4d/op/track3d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       33 2023-07-25 13:00:55.000000 vis4d-0.1/vis4d/op/track3d/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14273 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/track3d/cc_3dt.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      686 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/track3d/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      400 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/typing.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      878 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.967810 vis4d-0.1/vis4d/pl/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       57 2023-06-05 08:48:01.000000 vis4d-0.1/vis4d/pl/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       87 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/pl/__main__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.979810 vis4d-0.1/vis4d/pl/callbacks/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      222 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/pl/callbacks/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7531 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/pl/callbacks/callback_wrapper.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      970 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/pl/callbacks/scheduler.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1341 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/pl/data_module.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4754 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/pl/run.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5022 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/pl/trainer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6957 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/pl/training_module.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.979810 vis4d-0.1/vis4d/state/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       52 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/state/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.987810 vis4d-0.1/vis4d/state/track/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       48 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/state/track/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10268 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/state/track/qdtrack.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.999811 vis4d-0.1/vis4d/state/track3d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       51 2023-07-25 13:00:55.000000 vis4d-0.1/vis4d/state/track3d/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    18178 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/state/track3d/cc_3dt.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.015810 vis4d-0.1/vis4d/state/track3d/motion/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      205 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/state/track3d/motion/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1352 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/state/track3d/motion/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4296 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/state/track3d/motion/kf3d.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5066 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/state/track3d/motion/lstm_3d.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.027810 vis4d-0.1/vis4d/vis/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       64 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/vis/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1654 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/base.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.039811 vis4d-0.1/vis4d/vis/functional/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      482 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/functional/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    15103 2024-04-30 15:29:34.000000 vis4d-0.1/vis4d/vis/functional/image.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3137 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/functional/pointcloud.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.187811 vis4d-0.1/vis4d/vis/image/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      196 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    16159 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/bbox3d_visualizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12655 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/bev_visualizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7480 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/bounding_box_visualizer.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.199811 vis4d-0.1/vis4d/vis/image/canvas/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      168 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/canvas/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5476 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/canvas/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    21610 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/canvas/pillow_backend.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7634 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/seg_mask_visualizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13824 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/vis/image/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.211811 vis4d-0.1/vis4d/vis/image/viewer/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      198 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/viewer/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      945 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/viewer/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1205 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/viewer/matplotlib_viewer.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.227811 vis4d-0.1/vis4d/vis/pointcloud/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      133 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/pointcloud/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7081 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/pointcloud/pointcloud_visualizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9635 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/pointcloud/scene.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.243811 vis4d-0.1/vis4d/vis/pointcloud/viewer/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      226 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/pointcloud/viewer/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2773 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/pointcloud/viewer/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5933 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/pointcloud/viewer/open3d_viewer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      872 2024-04-10 22:23:17.000000 vis4d-0.1/vis4d/vis/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.251811 vis4d-0.1/vis4d/zoo/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1125 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.275811 vis4d-0.1/vis4d/zoo/base/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      571 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      565 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/callable.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.299811 vis4d-0.1/vis4d/zoo/base/data_connectors/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      490 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/data_connectors/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      413 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/data_connectors/cls.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      262 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/data_connectors/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      577 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/data_connectors/detection.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      680 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/data_connectors/seg.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      784 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/data_connectors/visualizers.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5379 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/dataloader.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.307811 vis4d-0.1/vis4d/zoo/base/datasets/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       31 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.323811 vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      506 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7383 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/detect.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6405 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/sem_seg.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6120 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/track.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.331811 vis4d-0.1/vis4d/zoo/base/datasets/coco/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      302 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/coco/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6759 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/coco/detection.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5451 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/coco/sem_seg.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5875 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/imagenet.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.343811 vis4d-0.1/vis4d/zoo/base/datasets/nuscenes/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      446 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/nuscenes/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3698 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/nuscenes/nuscenes.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1957 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/nuscenes/nuscenes_mono.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.355811 vis4d-0.1/vis4d/zoo/base/datasets/shift/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      705 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/shift/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13773 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/shift/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5261 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/shift/tasks.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.383811 vis4d-0.1/vis4d/zoo/base/models/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       29 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/models/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4828 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/models/faster_rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5067 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/models/mask_rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6488 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/models/qdtrack.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7288 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/models/yolox.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2733 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/optimizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1161 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/pl_trainer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2674 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/runtime.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.387811 vis4d-0.1/vis4d/zoo/bdd100k/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1056 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/bdd100k/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.399811 vis4d-0.1/vis4d/zoo/bdd100k/faster_rcnn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       32 2023-07-03 10:21:12.000000 vis4d-0.1/vis4d/zoo/bdd100k/faster_rcnn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5598 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/faster_rcnn/faster_rcnn_r50_1x_bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5625 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/faster_rcnn/faster_rcnn_r50_3x_bdd100k.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.415811 vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       30 2023-07-03 10:21:12.000000 vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5752 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_1x_bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5873 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_3x_bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5873 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_5x_bdd100k.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.423811 vis4d-0.1/vis4d/zoo/bdd100k/qdtrack/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       27 2023-12-01 09:54:18.000000 vis4d-0.1/vis4d/zoo/bdd100k/qdtrack/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4899 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/qdtrack/qdtrack_frcnn_r50_fpn_1x_bdd100k.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.451811 vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       32 2023-06-09 09:06:39.000000 vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6648 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r101_80k_bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6404 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r50_40k_bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6404 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r50_80k_bdd100k.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.483811 vis4d-0.1/vis4d/zoo/bevformer/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      224 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/bevformer/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5379 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bevformer/bevformer_base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6687 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bevformer/bevformer_tiny.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2009 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bevformer/bevformer_vis.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5718 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bevformer/data.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.535811 vis4d-0.1/vis4d/zoo/cc_3dt/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      536 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/cc_3dt/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4037 2024-04-12 10:27:07.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_bevformer_base_velo_lstm_nusc.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7309 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_kf3d_24e_nusc.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2885 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_pure_det_nusc.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1540 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_velo_lstm_24e_nusc.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7305 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r50_fpn_kf3d_12e_nusc.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3311 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_nusc_test.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2472 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_nusc_vis.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7583 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/data.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5445 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/model.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4905 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/velo_lstm_bevformer_base_100e_nusc.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4866 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/velo_lstm_frcnn_r101_fpn_100e_nusc.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.539811 vis4d-0.1/vis4d/zoo/faster_rcnn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      127 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/faster_rcnn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6830 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/faster_rcnn/faster_rcnn_coco.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.547811 vis4d-0.1/vis4d/zoo/fcn_resnet/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      116 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/fcn_resnet/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5676 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/fcn_resnet/fcn_resnet_coco.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.559811 vis4d-0.1/vis4d/zoo/mask_rcnn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      119 2023-12-01 09:54:19.000000 vis4d-0.1/vis4d/zoo/mask_rcnn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6332 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/mask_rcnn/mask_rcnn_coco.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.575811 vis4d-0.1/vis4d/zoo/qdtrack/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      348 2024-04-24 13:26:43.000000 vis4d-0.1/vis4d/zoo/qdtrack/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8435 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/qdtrack/data_yolox.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5952 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/qdtrack/qdtrack_frcnn_r50_fpn_augs_1x_bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5819 2024-04-24 13:26:43.000000 vis4d-0.1/vis4d/zoo/qdtrack/qdtrack_yolox_x_25e_bdd100k.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.583811 vis4d-0.1/vis4d/zoo/retinanet/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      119 2023-12-01 09:54:19.000000 vis4d-0.1/vis4d/zoo/retinanet/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6605 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/retinanet/retinanet_coco.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      719 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/run.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.587811 vis4d-0.1/vis4d/zoo/shift/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1283 2023-12-01 09:54:19.000000 vis4d-0.1/vis4d/zoo/shift/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.603811 vis4d-0.1/vis4d/zoo/shift/faster_rcnn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       30 2023-07-11 09:39:24.000000 vis4d-0.1/vis4d/zoo/shift/faster_rcnn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5898 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_12e_shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5899 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_36e_shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5851 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_6e_shift_all_domains.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.615811 vis4d-0.1/vis4d/zoo/shift/mask_rcnn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       28 2023-07-11 09:39:24.000000 vis4d-0.1/vis4d/zoo/shift/mask_rcnn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5970 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_12e_shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5971 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_36e_shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5923 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_6e_shift_all_domains.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.647811 vis4d-0.1/vis4d/zoo/shift/semantic_fpn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       30 2023-07-11 09:39:24.000000 vis4d-0.1/vis4d/zoo/shift/semantic_fpn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6573 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_160k_shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6543 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_160k_shift_all_domains.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6572 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_40k_shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6584 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_40k_shift_all_domains.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.659811 vis4d-0.1/vis4d/zoo/vit/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      211 2023-12-01 09:54:19.000000 vis4d-0.1/vis4d/zoo/vit/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5910 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/vit/vit_small_imagenet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5895 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/vit/vit_tiny_imagenet.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.675811 vis4d-0.1/vis4d/zoo/yolox/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      196 2023-12-01 09:54:19.000000 vis4d-0.1/vis4d/zoo/yolox/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7780 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/yolox/data.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5523 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/yolox/yolox_s_300e_coco.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5644 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/yolox/yolox_tiny_300e_coco.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.407809 vis4d-0.1/vis4d-workspace/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2129 2023-09-07 12:55:04.000000 vis4d-0.1/vis4d-workspace/convert.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4790 2024-04-11 16:51:37.000000 vis4d-0.1/vis4d-workspace/convert_bevformer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2904 2023-07-13 08:24:28.000000 vis4d-0.1/vis4d-workspace/eval_nusc.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.679811 vis4d-0.1/vis4d.egg-info/
+-rw-r--r--   0 yangyun  (577304) yangyun-group (478020)     4929 2024-05-14 22:02:22.000000 vis4d-0.1/vis4d.egg-info/PKG-INFO
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13499 2024-05-14 22:03:14.000000 vis4d-0.1/vis4d.egg-info/SOURCES.txt
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)        1 2024-05-14 22:02:22.000000 vis4d-0.1/vis4d.egg-info/dependency_links.txt
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      126 2024-05-14 22:02:22.000000 vis4d-0.1/vis4d.egg-info/entry_points.txt
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      321 2024-05-14 22:02:22.000000 vis4d-0.1/vis4d.egg-info/requires.txt
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       22 2024-05-14 22:02:22.000000 vis4d-0.1/vis4d.egg-info/top_level.txt
```

### Comparing `vis4d-0.0/LICENSE` & `vis4d-0.1/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -183,8 +183,8 @@
 
        https://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `vis4d-0.0/vis4d/common/bbox/poolers/roi_pooler.py` & `vis4d-0.1/vis4d/op/box/poolers/roi_pooler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,171 +1,193 @@
 """Vis4D RoI Pooling module."""
+
+from __future__ import annotations
+
+import abc
 import math
-from typing import List
 
 import torch
 from torchvision.ops import roi_align, roi_pool
 
-from vis4d.struct import Boxes2D
+from vis4d.common import ArgsType
 
-from .base import BaseRoIPooler, RoIPoolerConfig
+from .base import RoIPooler
 from .utils import assign_boxes_to_levels, boxes_to_tensor
 
 
-class MultiScaleRoIPoolerConfig(RoIPoolerConfig):
-    """MultiScaleRoIPoolerConfig config.
-
-    strides: feature map strides relative to the input.
-        The strides must be powers of 2 and a monotically decreasing geometric
-         sequence with a factor of 1/2.
-    sampling_ratio: Parameter for the RoIAlign (see torchvision).
-    pooler_type: Name of pooling operation that should be applied. "RoIPool" or
-        "RoIAlign".
-    canonical_box_size: A canonical box size in pixels (sqrt(box area)). The
-        default is heuristically defined as 224 pixels in the FPN paper
-        (based on ImageNet pre-training).
-    canonical_level (int): The feature map level index from which a canonical-
-        sized box should be placed. The default is defined as level 4
-        (stride=16) in the FPN paper, i.e., a box of size 224x224 will be
-        placed on the feature with stride=16.
-        The box placement for all boxes will be determined from their sizes
-        w.r.t canonical_box_size. For example, a box whose area is 4x that of a
-        canonical box should be used to pool features from feature level
-        ``canonical_level+1``.
-    aligned (bool): For roi_align op. Shift the box coordinates it by -0.5
-        for a better alignment with the two neighboring pixel indices.
-    """
-
-    pooling_op: str
-    strides: List[int]
-    sampling_ratio: int
-    canonical_box_size: int = 224
-    canonical_level: int = 4
-    aligned: bool = True
-
-
 # implementation modified from:
 # https://github.com/facebookresearch/detectron2/
-class MultiScaleRoIPooler(BaseRoIPooler):
-    """Vis4D wrapper for torchvision roi pooling class.
+class MultiScaleRoIPooler(RoIPooler):
+    """Wrapper for roi pooling that supports multi-scale feature maps."""
 
-    Supports multiple scales.
-    """
+    def __init__(
+        self,
+        resolution: tuple[int, int],
+        strides: list[int],
+        canonical_box_size: int = 224,
+        canonical_level: int = 4,
+        aligned: bool = True,
+    ):
+        """Multi-scale version of arbitrary RoI pooling operations.
 
-    def __init__(self, cfg: MultiScaleRoIPoolerConfig):
-        """Init."""
-        super().__init__()
-        self.cfg = MultiScaleRoIPoolerConfig(**cfg.dict())
-
-        assert self.cfg.pooling_op in [
-            "RoIAlign",
-            "RoIPool",
-        ], f"Unknown pooling_op: {self.cfg.pooling_op}"
+        Args:
+            resolution: Pooler resolution.
+            strides: Feature map strides relative to the input.
+                The strides must be powers of 2 and a monotically decreasing
+                geometric sequence with a factor of 1/2.
+            canonical_box_size: Canonical box size in pixels (sqrt(box area)).
+                The default is heuristically defined as 224 pixels in the FPN
+                paper (based on ImageNet pre-training).
+            canonical_level: The feature map level index from which a canonical
+                sized box should be placed. The default is defined as level 4
+                (stride=16) in the FPN paper, i.e., a box of size 224x224 will
+                be placed on the feature with stride=16.
+                The box placement for all boxes will be determined from their
+                sizes w.r.t canonical_box_size. For example, a box whose area
+                is 4x that of a canonical box should be used to pool features
+                from feature level ``canonical_level+1``.
+            aligned (bool): For roi_align op. Shift the box coordinates it by
+                -0.5 for a better alignment with the two neighboring pixel
+                indices.
+        """
+        super().__init__(resolution)
+        self.canonical_level = canonical_level
+        self.canonical_box_size = canonical_box_size
+        self.aligned = aligned
+        self.strides = strides
 
         # Map scale (defined as 1 / stride) to its feature map level under the
         # assumption that stride is a power of 2.
-        self.scales = [1 / s for s in self.cfg.strides]
+        self.scales = [1 / s for s in self.strides]
 
         min_level = -(math.log2(self.scales[0]))
         max_level = -(math.log2(self.scales[-1]))
         assert math.isclose(min_level, int(min_level)) and math.isclose(
             max_level, int(max_level)
         ), "Featuremap stride is not power of 2!"
         self.min_level = int(min_level)
         self.max_level = int(max_level)
         assert (
             len(self.scales) == self.max_level - self.min_level + 1
-        ), "[ROIPooler] Sizes of input featuremaps do not form a pyramid!"
+        ), "[ROIPooler] Sizes of input NamedTensors do not form a pyramid!"
         assert self.min_level >= 0 and self.min_level <= self.max_level
-        assert self.cfg.canonical_box_size > 0
+        assert self.canonical_box_size > 0
 
-    def pool(
-        self, features: List[torch.Tensor], boxes: List[Boxes2D]
+    def forward(
+        self, features: list[torch.Tensor], boxes: list[torch.Tensor]
     ) -> torch.Tensor:
         """Torchvision based roi pooling operation.
 
         Args:
-            features: list of image feature tensors (e.g.
-            fpn levels) - NCHW format
-            boxes: list of proposals (per image)
+            features: List of image feature tensors (e.g., fpn levels) - NCHW
+                format.
+            boxes: List of proposals (per image).
 
         Returns:
             torch.Tensor: NCHW format, where N = num boxes (total),
-            HW is roi size, C is feature dim. Boxes are concatenated along
-            dimension 0 for all batch elements.
+                HW is roi size, C is feature dim. Boxes are concatenated along
+                dimension 0 for all batch elements.
         """
         assert len(features) == len(self.scales), (
             f"unequal value, len(strides)={len(self.scales)}, "
             f"but x is list of {len(features)} Tensors"
         )
 
         assert len(boxes) == features[0].shape[0], (
             f"unequal value, x[0] batch dim 0 is {features[0].shape[0]}, "
             f"but box_list has length {len(boxes)}"
         )
         if len(boxes) == 0:
             return torch.zeros(
-                (0, features[0].shape[1]) + self.cfg.resolution,
+                (0, features[0].shape[1]) + self.resolution,
                 device=features[0].device,
                 dtype=features[0].dtype,
             )
 
         pooler_fmt_boxes = boxes_to_tensor(boxes)
-        if len(self.cfg.strides) == 1:
+        if len(self.scales) == 1:
             return self._pooling_op(
                 features[0],
                 pooler_fmt_boxes,
                 spatial_scale=self.scales[0],
             )
 
         level_assignments = assign_boxes_to_levels(
             boxes,
             self.min_level,
             self.max_level,
-            self.cfg.canonical_box_size,
-            self.cfg.canonical_level,
+            self.canonical_box_size,
+            self.canonical_level,
         )
 
         num_boxes = pooler_fmt_boxes.shape[0]
         num_channels = features[0].shape[1]
-        output_size = self.cfg.resolution[0]
+        output_size = self.resolution[0]
 
         dtype, device = features[0].dtype, features[0].device
         output = torch.zeros(
             (num_boxes, num_channels, output_size, output_size),
             dtype=dtype,
             device=device,
         )
 
         for level, scale in enumerate(self.scales):
-            inds = (level_assignments == level).nonzero()[:, 0]
+            inds = torch.eq(level_assignments, level).nonzero()[:, 0]
             pooler_fmt_boxes_level = pooler_fmt_boxes[inds]
             pooled_features = self._pooling_op(
-                features[level],
-                pooler_fmt_boxes_level,
-                spatial_scale=scale,
+                features[level], pooler_fmt_boxes_level, spatial_scale=scale
             )
             # Use index_put_ instead of advance indexing
             # avoids pytorch/issues/49852
             output.index_put_((inds,), pooled_features)
 
         return output
 
+    @abc.abstractmethod
     def _pooling_op(
         self,
         inputs: torch.Tensor,
         boxes: torch.Tensor,
         spatial_scale: float = 1.0,
     ) -> torch.Tensor:
         """Execute pooling op defined in config."""
-        if self.cfg.pooling_op == "RoIAlign":
-            return roi_align(
-                inputs,
-                boxes,
-                self.cfg.resolution,
-                spatial_scale,
-                self.cfg.sampling_ratio,
-                self.cfg.aligned,
-            )
-        if self.cfg.pooling_op == "RoIPool":
-            return roi_pool(inputs, boxes, self.cfg.resolution, spatial_scale)
-        raise ValueError(f"Unknown pooling_op: {self.cfg.pooling_op}")
+        raise NotImplementedError
+
+
+class MultiScaleRoIAlign(MultiScaleRoIPooler):
+    """RoI Align supporting multi-scale inputs."""
+
+    def __init__(
+        self, sampling_ratio: int, *args: ArgsType, **kwargs: ArgsType
+    ) -> None:
+        """Creates an instance of the class."""
+        super().__init__(*args, **kwargs)
+        self.sampling_ratio = sampling_ratio
+
+    def _pooling_op(
+        self,
+        inputs: torch.Tensor,
+        boxes: torch.Tensor,
+        spatial_scale: float = 1.0,
+    ) -> torch.Tensor:
+        """Roialign wrapper."""
+        return roi_align(
+            inputs,
+            boxes,
+            self.resolution,
+            spatial_scale,
+            self.sampling_ratio,
+            self.aligned,
+        )
+
+
+class MultiScaleRoIPool(MultiScaleRoIPooler):
+    """RoI Pool supporting multi-scale inputs."""
+
+    def _pooling_op(
+        self,
+        inputs: torch.Tensor,
+        boxes: torch.Tensor,
+        spatial_scale: float = 1.0,
+    ) -> torch.Tensor:
+        """Roipool wrapper."""
+        return roi_pool(inputs, boxes, self.resolution, spatial_scale)
```

### Comparing `vis4d-0.0/vis4d/common/bbox/poolers/utils.py` & `vis4d-0.1/vis4d/op/box/poolers/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""Utils for RoI poolers in Vis4D."""
-from typing import List
+"""Utility functions for RoI poolers."""
+
+from __future__ import annotations
 
 import torch
 
-from vis4d.struct import Boxes2D
+from ..box2d import bbox_area
 
 
 def assign_boxes_to_levels(
-    box_lists: List[Boxes2D],
+    box_lists: list[torch.Tensor],
     min_level: int,
     max_level: int,
     canonical_box_size: int,
     canonical_level: int,
 ) -> torch.Tensor:
     """Map each box to a feature map level index and return the assignment.
 
@@ -25,28 +26,30 @@
             canonically-sized box should be placed.
 
     Returns:
         Tensor (M,), where M is the total number of boxes in the list. Each
         element is the feature map index, as an offset from min_level, for the
         corresponding box (so value i means the box is at self.min_level + i).
     """
-    box_sizes = torch.sqrt(torch.cat([boxes.area for boxes in box_lists]))
+    box_sizes = torch.sqrt(
+        torch.cat([bbox_area(boxes) for boxes in box_lists])
+    )
     # Eqn.(1) in FPN paper
     level_assignments = torch.floor(
         canonical_level + torch.log2(box_sizes / canonical_box_size + 1e-8)
     )
     # clamp level to (min, max), in case the box size is too large or too small
     # for the available feature maps
     level_assignments = torch.clamp(
         level_assignments, min=min_level, max=max_level
     )
     return level_assignments.to(torch.int64) - min_level
 
 
-def boxes_to_tensor(boxes: List[Boxes2D]) -> torch.Tensor:
+def boxes_to_tensor(boxes: list[torch.Tensor]) -> torch.Tensor:
     """Convert all boxes into the tensor format used by ROI pooling ops.
 
     Args:
         boxes: List of Boxes
 
     Returns:
         A tensor of shape (M, 5), where M is the total number of boxes
@@ -60,11 +63,11 @@
             batch_i,
             dtype=box_tensor.dtype,
             device=box_tensor.device,
         )
         return torch.cat((repeated_index, box_tensor), dim=1)
 
     pooler_fmt_boxes = torch.cat(
-        [_fmt_box_list(boxs.boxes[:, :4], i) for i, boxs in enumerate(boxes)],
+        [_fmt_box_list(boxs[:, :4], i) for i, boxs in enumerate(boxes)],
         dim=0,
     )
     return pooler_fmt_boxes
```

### Comparing `vis4d-0.0/vis4d/common/bbox/samplers/base.py` & `vis4d-0.1/vis4d/op/box/samplers/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,71 @@
 """Interface for Vis4D bounding box samplers."""
+
+from __future__ import annotations
+
 import abc
-from typing import List, NamedTuple
+from typing import NamedTuple
 
 import torch
-from pydantic import BaseModel, Field
-
-from vis4d.common.registry import RegistryHolder
-from vis4d.struct import Boxes2D
+from torch import Tensor, nn
 
-from ..matchers.base import BaseMatcher, MatchResult
+from ..matchers import Matcher, MatchResult
 
 
 class SamplingResult(NamedTuple):
-    """Match result class. Stores expected result tensors.
+    """Sampling result class. Stores expected result tensors.
 
-    sampled_boxes: List[Boxes2D] Sampled Boxes.
-    sampled_targets: List[Boxes2D] Assigned target for each sampled box.
-    sampled_labels: List[Tensor] of {0, -1, 1} = {neg, ignore, pos}.
-    sampled_indices: List[Tensor] Index of input Boxes2D.
-    sampled_label_indices: List[Tensor] Index of assigned target for each
-        sampled box.
+    sampled_box_indices (Tensor): Index of sampled boxes from input.
+    sampled_target_indices (Tensor): Index of assigned target for each
+        positive sampled box.
+    sampled_labels (Tensor): {0, -1, 1} = {neg, ignore, pos}.
     """
 
-    sampled_boxes: List[Boxes2D]
-    sampled_targets: List[Boxes2D]
-    sampled_labels: List[torch.Tensor]
-    sampled_indices: List[torch.Tensor]
-    sampled_target_indices: List[torch.Tensor]
-
-
-class SamplerConfig(BaseModel, extra="allow"):
-    """Sampler base config."""
+    sampled_box_indices: Tensor
+    sampled_target_indices: Tensor
+    sampled_labels: Tensor
 
-    # Field(...) necessary for linter
-    # See https://github.com/samuelcolvin/pydantic/issues/1899
-    type: str = Field(...)
-    batch_size_per_image: int = Field(...)
-    positive_fraction: float = Field(...)
 
-
-class BaseSampler(metaclass=RegistryHolder):
+class Sampler(nn.Module):
     """Sampler base class."""
 
+    def __init__(self, batch_size: int, positive_fraction: float) -> None:
+        """Creates an instance of the class."""
+        super().__init__()
+        self.batch_size = batch_size
+        self.positive_fraction = positive_fraction
+
     @abc.abstractmethod
-    def sample(
-        self,
-        matching: List[MatchResult],
-        boxes: List[Boxes2D],
-        targets: List[Boxes2D],
-    ) -> SamplingResult:
+    def forward(self, matching: MatchResult) -> SamplingResult:
         """Sample bounding boxes according to their struct."""
         raise NotImplementedError
 
+    def __call__(self, matching: MatchResult) -> SamplingResult:
+        """Type declaration."""
+        return self._call_impl(matching)
 
-def build_sampler(cfg: SamplerConfig) -> BaseSampler:
-    """Build a bounding box sampler from config."""
-    registry = RegistryHolder.get_registry(BaseSampler)
-    if cfg.type in registry:
-        module = registry[cfg.type](cfg)
-        assert isinstance(module, BaseSampler)
-        return module
-    raise NotImplementedError(f"Sampler {cfg.type} not found.")
 
-
-@torch.no_grad()  # type: ignore
 def match_and_sample_proposals(
-    matcher: BaseMatcher,
-    sampler: BaseSampler,
-    proposals: List[Boxes2D],
-    targets: List[Boxes2D],
-    proposal_append_gt: bool,
-) -> SamplingResult:
-    """Match proposals to targets and subsample."""
-    if proposal_append_gt:
-        proposals = [Boxes2D.merge([p, t]) for p, t in zip(proposals, targets)]
-    matching = matcher.match(proposals, targets)
-    return sampler.sample(matching, proposals, targets)
+    matcher: Matcher,
+    sampler: Sampler,
+    proposal_boxes: list[Tensor],
+    target_boxes: list[Tensor],
+) -> tuple[list[Tensor], list[Tensor], list[Tensor]]:
+    """Match proposals to targets and subsample.
+
+    First, match the proposals to targets (ground truth labels) using the
+    matcher. It is usually IoU matcher. The matching labels the proposals with
+    positive or negative to show whether they are matched to an object.
+    Second, the sampler will choose proposals based on certain criteria such as
+    total proposal number and ratio of postives and negatives.
+    """
+    with torch.no_grad():
+        matchings = tuple(
+            matcher(prop_box, tgt_box)
+            for prop_box, tgt_box in zip(proposal_boxes, target_boxes)
+        )
+        sampling_results = tuple(sampler(matchs) for matchs in matchings)
+        return (
+            [s.sampled_box_indices for s in sampling_results],
+            [s.sampled_target_indices for s in sampling_results],
+            [s.sampled_labels for s in sampling_results],
+        )
```

### Comparing `vis4d-0.0/vis4d/common/bbox/samplers/combined.py` & `vis4d-0.1/vis4d/op/box/samplers/combined.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,127 +1,110 @@
 """Combined Sampler."""
-from collections import defaultdict
-from typing import Dict, List, Union
+
+from __future__ import annotations
 
 import torch
-from pydantic import validator
+from torch import Tensor
 
-from vis4d.struct import Boxes2D
+from vis4d.common import ArgsType
 
+from ..box2d import non_intersection, random_choice
 from ..matchers.base import MatchResult
-from ..utils import non_intersection, random_choice
-from .base import BaseSampler, SamplerConfig, SamplingResult
-from .utils import add_to_result
-
-
-class CombinedSamplerConfig(SamplerConfig):
-    """Config for CombinedSampler."""
-
-    pos_strategy: str
-    neg_strategy: str
-    neg_pos_ub: float = 3.0
-    floor_thr: float = -1.0
-    floor_fraction: float = 0.0
-    num_bins: int = 3
-
-    # Disable some pylint options in validator:
-    # https://github.com/samuelcolvin/pydantic/issues/568
-    @validator("pos_strategy", check_fields=False)
-    def validate_pos_strategy(  # pylint: disable=no-self-argument,no-self-use
-        cls, value: str
-    ) -> str:
-        """Check pos_strategy attribute."""
-        if not value in ["instance_balanced", "iou_balanced"]:
-            raise ValueError(
-                "pos_strategy must be in [instance_balanced, iou_balanced]"
-            )
-        return value
+from .base import Sampler, SamplingResult
 
-    @validator("neg_strategy", check_fields=False)
-    def validate_neg_strategy(  # pylint: disable=no-self-argument,no-self-use
-        cls, value: str
-    ) -> str:
-        """Check neg_strategy attribute."""
-        if not value in ["instance_balanced", "iou_balanced"]:
-            raise ValueError(
-                "neg_strategy must be in [instance_balanced, iou_balanced]"
-            )
-        return value
 
-
-class CombinedSampler(BaseSampler):
+class CombinedSampler(Sampler):
     """Combined sampler. Can have different strategies for pos/neg samples."""
 
-    def __init__(self, cfg: SamplerConfig):
-        """Init."""
-        super().__init__()
-        self.cfg = CombinedSamplerConfig(**cfg.dict())
-        self.bg_label = 0
-        self.pos_strategy = getattr(self, self.cfg.pos_strategy + "_sampling")
-        self.neg_strategy = getattr(self, self.cfg.neg_strategy + "_sampling")
+    def __init__(
+        self,
+        *args: ArgsType,
+        pos_strategy: str,
+        neg_strategy: str,
+        neg_pos_ub: float = 3.0,
+        floor_thr: float = -1.0,
+        floor_fraction: float = 0.0,
+        num_bins: int = 3,
+        bg_label: int = 0,
+        **kwargs: ArgsType,
+    ):
+        """Creates an instance of the class."""
+        super().__init__(*args, **kwargs)
+        self.neg_pos_ub = neg_pos_ub
+        self.floor_thr = floor_thr
+        self.floor_fraction = floor_fraction
+        self.num_bins = num_bins
+        self.bg_label = bg_label
+
+        if not pos_strategy in {
+            "instance_balanced",
+            "iou_balanced",
+        } or not neg_strategy in {"instance_balanced", "iou_balanced"}:
+            raise ValueError(
+                "strategies must be in [instance_balanced, iou_balanced]"
+            )
+
+        self.pos_strategy = getattr(self, pos_strategy + "_sampling")
+        self.neg_strategy = getattr(self, neg_strategy + "_sampling")
 
     @staticmethod
     def instance_balanced_sampling(
-        idx_tensor: torch.Tensor,
-        assigned_gts: torch.Tensor,
-        assigned_gt_ious: torch.Tensor,  # pylint: disable=unused-argument
+        idx_tensor: Tensor,
+        assigned_gts: Tensor,
+        assigned_gt_ious: Tensor,  # pylint: disable=unused-argument
         sample_size: int,
-    ) -> torch.Tensor:
+    ) -> Tensor:
         """Sample indices with balancing according to matched GT instance."""
         if idx_tensor.numel() <= sample_size:
             return idx_tensor
 
         unique_gt_inds = assigned_gts.unique()
         num_gts = len(unique_gt_inds)
         num_per_gt = int(sample_size / float(num_gts))
-        sampled_inds = []
+        sampled_inds_list = []
         # sample specific amount per gt instance
         for i in unique_gt_inds:
             inds = torch.nonzero(assigned_gts == i, as_tuple=False)
             inds = inds.squeeze(1)
             if len(inds) > num_per_gt:
                 inds = random_choice(inds, num_per_gt)
-            sampled_inds.append(inds)
-        sampled_inds = torch.cat(sampled_inds)
+            sampled_inds_list.append(inds)
+        sampled_inds = torch.cat(sampled_inds_list)
 
         # deal with edge cases
         if len(sampled_inds) < sample_size:
             num_extra = sample_size - len(sampled_inds)
             extra_inds = non_intersection(idx_tensor, sampled_inds)
             if len(extra_inds) > num_extra:
                 extra_inds = random_choice(extra_inds, num_extra)
             sampled_inds = torch.cat([sampled_inds, extra_inds])
         return sampled_inds
 
     def iou_balanced_sampling(
         self,
-        idx_tensor: torch.Tensor,
-        assigned_gts: torch.Tensor,  # pylint: disable=unused-argument
-        assigned_gt_ious: torch.Tensor,
+        idx_tensor: Tensor,
+        assigned_gts: Tensor,  # pylint: disable=unused-argument
+        assigned_gt_ious: Tensor,
         sample_size: int,
-    ) -> torch.Tensor:
+    ) -> Tensor:
         """Sample indices with balancing according to IoU with matched GT."""
         if idx_tensor.numel() <= sample_size:
             return idx_tensor
 
         # define 'floor' set - set with low iou samples
-        if self.cfg.floor_thr >= 0:
-            floor_set = idx_tensor[assigned_gt_ious <= self.cfg.floor_thr]
-            iou_sampling_set = idx_tensor[
-                assigned_gt_ious > self.cfg.floor_thr
-            ]
+        if self.floor_thr >= 0:
+            floor_set = idx_tensor[assigned_gt_ious <= self.floor_thr]
+            iou_sampling_set = idx_tensor[assigned_gt_ious > self.floor_thr]
         else:
             floor_set = None
-            iou_sampling_set = idx_tensor[
-                assigned_gt_ious > self.cfg.floor_thr
-            ]
+            iou_sampling_set = idx_tensor[assigned_gt_ious > self.floor_thr]
 
-        num_iou_set_samples = int(sample_size * (1 - self.cfg.floor_fraction))
+        num_iou_set_samples = int(sample_size * (1 - self.floor_fraction))
         if len(iou_sampling_set) > num_iou_set_samples:
-            if self.cfg.num_bins >= 2:
+            if self.num_bins >= 2:
                 iou_sampled_inds = self.sample_within_intervals(
                     idx_tensor, assigned_gt_ious, num_iou_set_samples
                 )
             else:
                 iou_sampled_inds = random_choice(
                     iou_sampling_set, num_iou_set_samples
                 )
@@ -145,89 +128,82 @@
             extra_inds = non_intersection(idx_tensor, sampled_inds)
             if len(extra_inds) > num_extra:
                 extra_inds = random_choice(extra_inds, num_extra)
             sampled_inds = torch.cat([sampled_inds, extra_inds])
 
         return sampled_inds
 
-    def sample(
-        self,
-        matching: List[MatchResult],
-        boxes: List[Boxes2D],
-        targets: List[Boxes2D],
-    ) -> SamplingResult:
+    def forward(self, matching: MatchResult) -> SamplingResult:
         """Sample boxes according to strategies defined in cfg."""
-        pos_sample_size = int(
-            self.cfg.batch_size_per_image * self.cfg.positive_fraction
+        pos_sample_size = int(self.batch_size * self.positive_fraction)
+
+        positive_mask: Tensor = (matching.assigned_labels != -1) & (
+            matching.assigned_labels != self.bg_label
         )
-        result: Dict[
-            str, Union[List[Boxes2D], List[torch.Tensor]]
-        ] = defaultdict(list)
-        for match, box, target in zip(matching, boxes, targets):
-            positive_mask = (match.assigned_labels != -1) & (
-                match.assigned_labels != self.bg_label
-            )
-            negative_mask = match.assigned_labels == self.bg_label
+        negative_mask = torch.eq(matching.assigned_labels, self.bg_label)
 
-            positive = positive_mask.nonzero()[:, 0]
-            negative = negative_mask.nonzero()[:, 0]
+        positive = positive_mask.nonzero()[:, 0]
+        negative = negative_mask.nonzero()[:, 0]
 
-            num_pos = min(positive.numel(), pos_sample_size)
-            num_neg = self.cfg.batch_size_per_image - num_pos
+        num_pos = min(positive.numel(), pos_sample_size)
+        num_neg = self.batch_size - num_pos
 
-            if self.cfg.neg_pos_ub >= 0:
-                neg_upper_bound = int(self.cfg.neg_pos_ub * num_pos)
-                num_neg = min(num_neg, neg_upper_bound)
-
-            pos_idx = self.pos_strategy(
-                idx_tensor=positive,
-                assigned_gts=match.assigned_gt_indices.long()[positive_mask],
-                assigned_gt_ious=match.assigned_gt_iou[positive_mask],
-                sample_size=num_pos,
-            )
+        if self.neg_pos_ub >= 0:
+            neg_upper_bound = int(self.neg_pos_ub * num_pos)
+            num_neg = min(num_neg, neg_upper_bound)
+
+        pos_idx = self.pos_strategy(
+            idx_tensor=positive,
+            assigned_gts=matching.assigned_gt_indices[positive_mask],
+            assigned_gt_ious=matching.assigned_gt_iou[positive_mask],
+            sample_size=num_pos,
+        )
 
-            neg_idx = self.neg_strategy(
-                idx_tensor=negative,
-                assigned_gts=match.assigned_gt_indices.long()[negative_mask],
-                assigned_gt_ious=match.assigned_gt_iou[negative_mask],
-                sample_size=num_neg,
-            )
-            sampled_idcs = torch.cat([pos_idx, neg_idx], dim=0)
-            add_to_result(result, sampled_idcs, box, target, match)
+        neg_idx = self.neg_strategy(
+            idx_tensor=negative,
+            assigned_gts=matching.assigned_gt_indices[negative_mask],
+            assigned_gt_ious=matching.assigned_gt_iou[negative_mask],
+            sample_size=num_neg,
+        )
+        sampled_idcs = torch.cat([pos_idx, neg_idx], dim=0)
 
-        return SamplingResult(**result)
+        return SamplingResult(
+            sampled_box_indices=sampled_idcs,
+            sampled_target_indices=matching.assigned_gt_indices[sampled_idcs],
+            sampled_labels=matching.assigned_labels[sampled_idcs],
+        )
 
     def sample_within_intervals(
         self,
-        idx_tensor: torch.Tensor,
-        assigned_gt_ious: torch.Tensor,
+        idx_tensor: Tensor,
+        assigned_gt_ious: Tensor,
         sample_size: int,
-    ) -> torch.Tensor:
+    ) -> Tensor:
         """Sample according to N iou intervals where N = num bins."""
-        floor_thr = max(self.cfg.floor_thr, 0.0)
+        floor_thr = max(self.floor_thr, 0.0)
         max_iou = assigned_gt_ious.max()
-        iou_interval = (max_iou - floor_thr) / self.cfg.num_bins
-        per_bin_samples = int(sample_size / self.cfg.num_bins)
+        iou_interval = (max_iou - floor_thr) / self.num_bins
+        per_bin_samples = int(sample_size / self.num_bins)
 
-        sampled_inds = []
-        for i in range(self.cfg.num_bins):
+        sampled_inds_list = []
+        for i in range(self.num_bins):
             start_iou = floor_thr + i * iou_interval
             end_iou = floor_thr + (i + 1) * iou_interval
             tmp_set = (
                 (start_iou <= assigned_gt_ious) & (assigned_gt_ious < end_iou)
             ).nonzero()[:, 0]
             if len(tmp_set) > per_bin_samples:
                 tmp_sampled_set = random_choice(
                     idx_tensor[tmp_set], per_bin_samples
                 )
             else:
                 tmp_sampled_set = idx_tensor[tmp_set]  # pragma: no cover
-            sampled_inds.append(tmp_sampled_set)
+            sampled_inds_list.append(tmp_sampled_set)
 
-        sampled_inds = torch.cat(sampled_inds)
+        sampled_inds = torch.cat(sampled_inds_list)
         if len(sampled_inds) < sample_size:
             num_extra = sample_size - len(sampled_inds)
             extra_inds = non_intersection(idx_tensor, sampled_inds)
             if len(extra_inds) > num_extra:
                 extra_inds = random_choice(extra_inds, num_extra)
             sampled_inds = torch.cat([sampled_inds, extra_inds])
```

### Comparing `vis4d-0.0/vis4d/common/bbox/samplers/combined_test.py` & `vis4d-0.1/vis4d/op/box/samplers/random.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,63 @@
-"""Testcases for combined sampler."""
-import unittest
-from typing import List, Tuple
+"""Random Sampler."""
+
+from __future__ import annotations
 
 import torch
 
-from vis4d.struct import Boxes2D
+from vis4d.common import ArgsType
 
 from ..matchers.base import MatchResult
-from .base import SamplerConfig
-from .combined import CombinedSampler
+from .base import Sampler, SamplingResult
 
 
-class TestCombined(unittest.TestCase):
-    """Test cases for combined sampler."""
+class RandomSampler(Sampler):
+    """Random sampler class."""
 
-    @staticmethod
-    def _get_boxes_targets(
-        num_gts: int, num_samples: int
-    ) -> Tuple[List[MatchResult], List[Boxes2D], List[Boxes2D]]:
-        """Generate match, box target."""
-        state = torch.random.get_rng_state()
-        torch.random.set_rng_state(torch.manual_seed(0).get_state())
-        matching = [
-            MatchResult(
-                assigned_gt_indices=torch.randint(0, num_gts, (num_samples,)),
-                assigned_gt_iou=torch.rand(num_samples),
-                assigned_labels=torch.randint(-1, 2, (num_samples,)),
-            )
-        ]
-        boxes = [Boxes2D(torch.rand(num_samples, 5))]
-        targets = [Boxes2D(torch.rand(num_gts, 5), torch.zeros(num_gts))]
-        torch.random.set_rng_state(state)
-        return matching, boxes, targets
-
-    def test_sample(self) -> None:
-        """Testcase for sample function."""
-        samples_per_img = 256
-        pos_fract = 0.5
-        num_samples = 512
-        num_gts = 3
-
-        sampler = CombinedSampler(
-            SamplerConfig(
-                type="combined",
-                batch_size_per_image=samples_per_img,
-                positive_fraction=pos_fract,
-                pos_strategy="instance_balanced",
-                neg_strategy="iou_balanced",
-            )
-        )
-        matching, boxes, targets = self._get_boxes_targets(
-            num_gts, num_samples
-        )
-        sampling_result = sampler.sample(matching, boxes, targets)
-        sampled_boxes, sampled_targets = (
-            sampling_result.sampled_boxes,
-            sampling_result.sampled_targets,
+    def __init__(
+        self,
+        *args: ArgsType,
+        bg_label: int = 0,
+        **kwargs: ArgsType,
+    ):
+        """Creates an instance of the class."""
+        super().__init__(*args, **kwargs)
+        self.bg_label = bg_label
+
+    def forward(
+        self,
+        matching: MatchResult,
+    ) -> SamplingResult:
+        """Sample boxes randomly."""
+        pos_idx, neg_idx = self._sample_labels(matching.assigned_labels)
+        sampled_idcs = torch.cat([pos_idx, neg_idx], dim=0)
+        return SamplingResult(
+            sampled_box_indices=sampled_idcs,
+            sampled_target_indices=matching.assigned_gt_indices[sampled_idcs],
+            sampled_labels=matching.assigned_labels[sampled_idcs],
         )
-        self.assertEqual(len(sampled_boxes[0]), samples_per_img)
-        self.assertEqual(len(sampled_boxes[0]), len(sampled_targets[0]))
 
-        sampled_idx = []
-        for sampled_target in sampled_targets[0]:
-            found = False
-            for i, target in enumerate(targets[0]):
-                if torch.isclose(target.boxes, sampled_target.boxes).all():
-                    sampled_idx.append(i)
-                    found = True
-            self.assertTrue(found)
-
-        self.assertEqual(set(sampled_idx), set(range(num_gts)))
-
-        sampler = CombinedSampler(
-            SamplerConfig(
-                type="combined",
-                batch_size_per_image=samples_per_img,
-                positive_fraction=pos_fract,
-                pos_strategy="instance_balanced",
-                neg_strategy="iou_balanced",
-                floor_thr=0.1,
-                num_bins=1,
-            )
-        )
-        matching, boxes, targets = self._get_boxes_targets(
-            num_gts, num_samples
-        )
-        sampler.sample(matching, boxes, targets)
+    def _sample_labels(
+        self, labels: torch.Tensor
+    ) -> tuple[torch.Tensor, torch.Tensor]:
+        """Randomly sample indices from given labels."""
+        positive = ((labels != -1) & (labels != self.bg_label)).nonzero()[:, 0]
+        negative = torch.eq(labels, self.bg_label).nonzero()[:, 0]
+
+        num_pos = int(self.batch_size * self.positive_fraction)
+        # protect against not enough positive examples
+        num_pos = min(positive.numel(), num_pos)
+        num_neg = self.batch_size - num_pos
+        # protect against not enough negative examples
+        num_neg = min(negative.numel(), num_neg)
+
+        # randomly select positive and negative examples
+        perm1 = torch.randperm(positive.numel(), device=positive.device)[
+            :num_pos
+        ]
+        perm2 = torch.randperm(negative.numel(), device=negative.device)[
+            :num_neg
+        ]
 
-        matching, boxes, targets = self._get_boxes_targets(num_gts, 128)
-        sampler.sample(matching, boxes, targets)
+        pos_idx = positive[perm1]
+        neg_idx = negative[perm2]
+        return pos_idx, neg_idx
```

### Comparing `vis4d-0.0/vis4d/common/geometry/rotation.py` & `vis4d-0.1/vis4d/op/geometry/rotation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,119 @@
 """Rotation utilities."""
+
 import functools
 
-import numpy as np
 import torch
 import torch.nn.functional as F
+from torch import Tensor
+
+from vis4d.data.const import AxisMode
+
+
+def normalize_angle(input_angles: Tensor) -> Tensor:
+    """Normalize content of input_angles to range [-pi, pi].
+
+    Args:
+        input_angles: (Tensor) tensor of any shape containing
+                       unnormalized angles.
+
+    Returns:
+        Tensor with angles normalized to +/- pi
+    """
+    return torch.sub((input_angles + torch.pi) % (2 * torch.pi), torch.pi)
+
 
+def acute_angle(theta_1: Tensor, theta_2: Tensor) -> Tensor:
+    """Update theta_1 to mkae the agnle between two thetas is acute."""
+    # Make sure the angle between two thetas is acute
+    if torch.pi / 2.0 < abs(theta_2 - theta_1) < torch.pi * 3 / 2.0:
+        theta_1 += torch.pi
+        if theta_1 > torch.pi:
+            theta_1 -= torch.pi * 2
+        if theta_1 < -torch.pi:
+            theta_1 += torch.pi * 2
 
-def normalize_angle(input_angles: torch.Tensor) -> torch.Tensor:
-    """Normalize content of input_angles to range [-pi, pi]."""
-    return (input_angles + np.pi) % (2 * np.pi) - np.pi
+    # Convert the case of > 270 to < 90
+    if abs(theta_2 - theta_1) >= torch.pi * 3 / 2.0:
+        if theta_2 > 0:
+            theta_1 += torch.pi * 2
+        else:
+            theta_1 -= torch.pi * 2
+    return theta_1
 
 
-def yaw2alpha(rot_y: torch.Tensor, center: torch.Tensor) -> torch.Tensor:
+def yaw2alpha(rot_y: Tensor, center: Tensor) -> Tensor:
     """Get alpha by vertical rotation - theta.
 
     Args:
         rot_y: Rotation around Y-axis in camera coordinates [-pi..pi]
         center: 3D object center in camera coordinates
 
     Returns:
         alpha: Observation angle of object, ranging [-pi..pi]
     """
     alpha = rot_y - torch.atan2(center[..., 0], center[..., 2])
     return normalize_angle(alpha)
 
 
-def alpha2yaw(alpha: torch.Tensor, center: torch.Tensor) -> torch.Tensor:
+def alpha2yaw(alpha: Tensor, center: Tensor) -> Tensor:
     """Get vertical rotation by alpha + theta.
 
     Args:
         alpha: Observation angle of object, ranging [-pi..pi]
         center: 3D object center in camera coordinates
 
     Returns:
         rot_y: Vertical rotation in camera coordinates [-pi..pi]
     """
     rot_y = alpha + torch.atan2(center[..., 0], center[..., 2])
     return normalize_angle(rot_y)
 
 
-def rotation_output_to_alpha(
-    output: torch.Tensor, num_bins: int = 2
-) -> torch.Tensor:
+def rotation_output_to_alpha(output: Tensor, num_bins: int = 2) -> Tensor:
     """Get alpha from bin-based regression output.
 
     Uses method described in (with two bins):
     See: 3D Bounding Box Estimation Using Deep Learning and Geometry,
-     Mousavian et al., CVPR'17
+    Mousavian et al., CVPR'17
+
+    Args:
+        output: (Tensor) bin based regressed output.
+        num_bins: (int) number of bins to use
+
+    Returns:
+        Tensor containing the angle from the bin-based regression output
     """
     out_range = torch.tensor(list(range(len(output))), device=output.device)
     bin_idx = output[:, :num_bins].argmax(dim=-1)
     res_idx = num_bins + 2 * bin_idx
     bin_centers = torch.arange(
-        -np.pi, np.pi, 2 * np.pi / num_bins, device=output.device
+        -torch.pi, torch.pi, 2 * torch.pi / num_bins, device=output.device
     )
-    bin_centers += np.pi / num_bins
+    bin_centers += torch.pi / num_bins
     alpha = (
         torch.atan(output[out_range, res_idx] / output[out_range, res_idx + 1])
         + bin_centers[bin_idx]
     )
     return alpha
 
 
-def generate_rotation_output(
-    pred: torch.Tensor, num_bins: int = 2
-) -> torch.Tensor:
+def generate_rotation_output(pred: Tensor, num_bins: int = 2) -> Tensor:
     """Convert output to bin confidence and cos / sin of residual.
 
     The viewpoint (alpha) prediction (N, num_bins + 2 * num_bins) consists of:
     bin confidences (N, num_bins): softmax logits for bin probability.
-        1st entry is probability for orientation being in bin 1,
-        2nd entry is probability for orientation being in bin 2,
-        and so on.
+    1st entry is probability for orientation being in bin 1,
+    2nd entry is probability for orientation being in bin 2,
+    and so on.
     bin residual (N, num_bins * 2): angle residual w.r.t. bin N orientation,
-        represented as sin and cos values.
+    represented as sin and cos values.
 
     See: 3D Bounding Box Estimation Using Deep Learning and Geometry,
-     Mousavian et al., CVPR'17
+    Mousavian et al., CVPR'17
     """
     pred = pred.view(pred.size(0), -1, 3 * num_bins)
     bin_logits = pred[..., :num_bins]
 
     bin_residuals = []
     for i in range(num_bins):
         res_idx = num_bins + 2 * i
@@ -92,15 +125,15 @@
 
     rot = torch.cat([bin_logits, *bin_residuals], -1)
     return rot
 
 
 # Rotation conversion functions adapted from:
 # https://github.com/facebookresearch/pytorch3d/blob/main/pytorch3d/transforms/rotation_conversions.py
-def _axis_angle_rotation(axis: str, angle: torch.Tensor) -> torch.Tensor:
+def _axis_angle_rotation(axis: str, angle: Tensor) -> Tensor:
     """Get rotation matrix for an angle around an axis.
 
     Args:
         axis: Axis label "X" or "Y or "Z".
         angle: any shape tensor of Euler angles in radians
 
     Returns:
@@ -118,22 +151,22 @@
     if axis == "Z":
         rot_flat = (cos, -sin, zero, sin, cos, zero, zero, zero, one)
 
     return torch.stack(rot_flat, -1).reshape(angle.shape + (3, 3))
 
 
 def euler_angles_to_matrix(
-    euler_angles: torch.Tensor, convention: str = "XYZ"
-) -> torch.Tensor:
+    euler_angles: Tensor, convention: str = "XYZ"
+) -> Tensor:
     """Convert rotations given as Euler angles in radians to rotation matrices.
 
     Args:
         euler_angles: Euler angles in radians as tensor of shape (..., 3).
         convention: Convention string of three uppercase letters from
-            {"X", "Y", and "Z"}.
+        "X", "Y", and "Z".
 
     Returns:
         Rotation matrices as tensor of shape (..., 3, 3).
 
     Raises:
         ValueError: if convention string is not a combination of XYZ
     """
@@ -142,38 +175,49 @@
     if len(convention) != 3:
         raise ValueError("Convention must have 3 letters.")
     if convention[1] in (convention[0], convention[2]):
         raise ValueError(f"Invalid convention {convention}.")
     for letter in convention:
         if letter not in ("X", "Y", "Z"):
             raise ValueError(f"Invalid letter {letter} in convention string.")
-    matrices = map(
-        _axis_angle_rotation, convention, torch.unbind(euler_angles, -1)
-    )
+    matrices = [
+        _axis_angle_rotation(c, a)
+        for c, a in zip(convention, torch.unbind(euler_angles, -1))
+    ]
     return functools.reduce(torch.matmul, matrices)
 
 
 def _index_from_letter(letter: str) -> int:  # pragma: no cover
-    """Retunr index from letter."""
+    """Return index from letter.
+
+    Args:
+        letter: (str) letter in [X,Y,Z]
+
+    Returns:
+        int mapping of the corresponding letter [0,1,2]
+
+    Raises:
+        ValueError: if the given letter is not valid
+    """
     if letter == "X":
         return 0
     if letter == "Y":
         return 1
     if letter == "Z":
         return 2
     raise ValueError("letter not valid!")
 
 
 def _angle_from_tan(
     axis: str,
     other_axis: str,
-    data: torch.Tensor,
+    data: Tensor,
     horizontal: bool,
     tait_bryan: bool,
-) -> torch.Tensor:
+) -> Tensor:
     """Helper function for matrix_to_euler_angles.
 
     Extracts the first or third Euler angle from the two members of
     the matrix which are positive constant times its sine and cosine.
 
     Args:
         axis: Axis label "X" or "Y or "Z" for the angle we are finding.
@@ -188,25 +232,23 @@
     Returns:
         Euler Angles in radians for each matrix in data as a tensor
         of shape (...).
     """
     i1, i2 = {"X": (2, 1), "Y": (0, 2), "Z": (1, 0)}[axis]
     if horizontal:
         i2, i1 = i1, i2
-    even = (axis + other_axis) in ["XY", "YZ", "ZX"]
+    even = axis + other_axis in {"XY", "YZ", "ZX"}
     if horizontal == even:
         return torch.atan2(data[..., i1], data[..., i2])
     if tait_bryan:
         return torch.atan2(-data[..., i2], data[..., i1])
     return torch.atan2(data[..., i2], -data[..., i1])
 
 
-def matrix_to_euler_angles(
-    matrix: torch.Tensor, convention: str = "XYZ"
-) -> torch.Tensor:
+def matrix_to_euler_angles(matrix: Tensor, convention: str = "XYZ") -> Tensor:
     """Convert rotations given as rotation matrices to Euler angles in radians.
 
     Args:
         matrix: Rotation matrices as tensor of shape (..., 3, 3).
         convention: Convention string of three uppercase letters.
 
     Returns:
@@ -224,16 +266,22 @@
             raise ValueError(f"Invalid letter {letter} in convention string.")
     if matrix.size(-1) != 3 or matrix.size(-2) != 3:
         raise ValueError(f"Invalid rotation matrix shape {matrix.shape}.")
     i0 = _index_from_letter(convention[0])
     i2 = _index_from_letter(convention[2])
     tait_bryan = i0 != i2
     if tait_bryan:
+        rads = matrix[..., i0, i2]
+        # safety for nan
+        rads[torch.where(rads > 1.0)] = rads.new_tensor([1.0]).to(rads.device)
+        rads[torch.where(rads < -1.0)] = rads.new_tensor([-1.0]).to(
+            rads.device
+        )
         central_angle = torch.asin(
-            matrix[..., i0, i2] * (-1.0 if i0 - i2 in [-1, 2] else 1.0)
+            rads * (-1.0 if i0 - i2 in [-1, 2] else 1.0)
         )
     else:
         central_angle = torch.acos(matrix[..., i0, i0])
 
     o = (
         _angle_from_tan(
             convention[0], convention[1], matrix[..., i2], False, tait_bryan
@@ -242,15 +290,15 @@
         _angle_from_tan(
             convention[2], convention[1], matrix[..., i0, :], True, tait_bryan
         ),
     )
     return torch.stack(o, -1)
 
 
-def quaternion_to_matrix(quaternions: torch.Tensor) -> torch.Tensor:
+def quaternion_to_matrix(quaternions: Tensor) -> Tensor:
     """Convert rotations given as quaternions to rotation matrices.
 
     Args:
         quaternions: quaternions with real part first,
             as tensor of shape (..., 4).
 
     Returns:
@@ -272,23 +320,23 @@
             1 - two_s * (i * i + j * j),
         ),
         -1,
     )
     return o.reshape(quaternions.shape[:-1] + (3, 3))
 
 
-def _sqrt_positive_part(quat: torch.Tensor) -> torch.Tensor:
+def _sqrt_positive_part(quat: Tensor) -> Tensor:
     """Returns sqrt(max(0, x)) but with a zero subgradient where x is 0."""
     ret = torch.zeros_like(quat)
     positive_mask = quat > 0
     ret[positive_mask] = torch.sqrt(quat[positive_mask])
     return ret
 
 
-def matrix_to_quaternion(matrix: torch.Tensor) -> torch.Tensor:
+def matrix_to_quaternion(matrix: Tensor) -> Tensor:
     """Convert rotations given as rotation matrices to quaternions.
 
     Args:
         matrix: Rotation matrices as tensor of shape (..., 3, 3).
 
     Returns:
         quaternions with real part first, as tensor of shape (..., 4).
@@ -342,37 +390,38 @@
     )
 
     # if not for numerical problems, quat_candidates[i] should be same
     # (up to a sign), forall i; we pick the best-conditioned one
     # (with the largest denominator)
 
     return quat_candidates[
-        F.one_hot(q_abs.argmax(dim=-1), num_classes=4) > 0.5,
+        F.one_hot(  # pylint: disable=not-callable
+            q_abs.argmax(dim=-1), num_classes=4
+        )
+        > 0.5,
         :,  # pyre-ignore[16]
     ].reshape(*batch_dim, 4)
 
 
-def standardize_quaternion(quaternions: torch.Tensor) -> torch.Tensor:
+def standardize_quaternion(quaternions: Tensor) -> Tensor:
     """Convert a unit quaternion to a standard form.
 
     Standard form: One in which the real part is non negative.
 
     Args:
         quaternions: Quaternions with real part first,
             as tensor of shape (..., 4).
 
     Returns:
         Standardized quaternions as tensor of shape (..., 4).
     """
     return torch.where(quaternions[..., 0:1] < 0, -quaternions, quaternions)
 
 
-def quaternion_raw_multiply(
-    quat1: torch.Tensor, quat2: torch.Tensor
-) -> torch.Tensor:
+def quaternion_raw_multiply(quat1: Tensor, quat2: Tensor) -> Tensor:
     """Multiply two quaternions.
 
     Usual torch rules for broadcasting apply.
 
     Args:
         quat1: Quaternions as tensor of shape (..., 4), real part first.
         quat2: Quaternions as tensor of shape (..., 4), real part first.
@@ -385,17 +434,15 @@
     ow = aw * bw - ax * bx - ay * by - az * bz
     ox = aw * bx + ax * bw + ay * bz - az * by
     oy = aw * by - ax * bz + ay * bw + az * bx
     oz = aw * bz + ax * by - ay * bx + az * bw
     return torch.stack((ow, ox, oy, oz), -1)
 
 
-def quaternion_multiply(
-    quat1: torch.Tensor, quat2: torch.Tensor
-) -> torch.Tensor:
+def quaternion_multiply(quat1: Tensor, quat2: Tensor) -> Tensor:
     """Multiply two quaternions representing rotations.
 
     Returns the quaternion representing their composition, i.e. the version
     with nonnegative real part. Usual torch rules for broadcasting apply.
 
     Args:
         quat1: Quaternions as tensor of shape (..., 4), real part first.
@@ -403,30 +450,28 @@
 
     Returns:
         The product of quat1 and quat2, tensor of quaternions shape (..., 4).
     """
     return standardize_quaternion(quaternion_raw_multiply(quat1, quat2))
 
 
-def quaternion_invert(quaternion: torch.Tensor) -> torch.Tensor:
+def quaternion_invert(quaternion: Tensor) -> Tensor:
     """Return quaternion that represents inverse rotation.
 
     Args:
         quaternion: Quaternions as tensor of shape (..., 4), with real part
             first, which must be versors (unit quaternions).
 
     Returns:
         The inverse, a tensor of quaternions of shape (..., 4).
     """
     return quaternion * quaternion.new_tensor([1, -1, -1, -1])
 
 
-def quaternion_apply(
-    quaternion: torch.Tensor, points: torch.Tensor
-) -> torch.Tensor:
+def quaternion_apply(quaternion: Tensor, points: Tensor) -> Tensor:
     """Apply the rotation given by a quaternion to a 3D point.
 
     Usual torch rules for broadcasting apply.
 
     Args:
         quaternion: Tensor of quaternions, real part first, of shape (..., 4).
         points: Tensor of 3D points of shape (..., 3).
@@ -442,7 +487,52 @@
     real_parts = points.new_zeros(points.shape[:-1] + (1,))
     point_as_quaternion = torch.cat((real_parts, points), -1)
     out = quaternion_raw_multiply(
         quaternion_raw_multiply(quaternion, point_as_quaternion),
         quaternion_invert(quaternion),
     )
     return out[..., 1:]
+
+
+def rotation_matrix_yaw(
+    rotation_matrix: Tensor, axis_mode: AxisMode
+) -> Tensor:
+    """Get yaw of 3D boxes in euler angle under given axis mode.
+
+    Args:
+        rotation_matrix (Tensor): [N, 3, 3] Rotation matrix of the object.
+        axis_mode (AxisMode): Coordinate system convention.
+
+    Returns:
+        orientation (Tensor): [N, 3] Yaw in euler angle.
+    """
+    orientation = rotation_matrix.new_zeros(rotation_matrix.shape[0], 3)
+
+    if axis_mode == AxisMode.OPENCV:
+        orientation[:, 1] = matrix_to_euler_angles(rotation_matrix, "YZX")[
+            :, 0
+        ]
+    else:
+        orientation[:, 2] = matrix_to_euler_angles(rotation_matrix, "ZYX")[
+            :, 0
+        ]
+    return orientation
+
+
+def rotate_orientation(
+    orientation: Tensor, extrinsics: Tensor, axis_mode: AxisMode = AxisMode.ROS
+) -> Tensor:
+    """Rotate the orientation of the object in different coordinate.
+
+    Args:
+        orientation (Tensor): [N, 3] Orientation of the object in euler angles.
+        extrinsics (Tensor): [4, 4] Extrinsic matrix of the object.
+        axis_mode (AxisMode): Coordinate system convention. Default:
+            AxisMode.ROS
+    """
+    rot = extrinsics[:3, :3] @ euler_angles_to_matrix(orientation)
+    return rotation_matrix_yaw(rot, axis_mode)
+
+
+def rotate_velocities(velocities: Tensor, extrinsics: Tensor) -> Tensor:
+    """Rotate the velocities of the object in different coordinate."""
+    return (extrinsics[:3, :3] @ velocities.unsqueeze(-1)).squeeze(-1)
```

### Comparing `vis4d-0.0/vis4d/common/layers/conv2d.py` & `vis4d-0.1/vis4d/op/layer/deform_conv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,93 @@
-"""Wrapper for conv2d."""
-from typing import Optional, Tuple
+"""Wrapper for deformable convolution."""
+
+from __future__ import annotations
 
 import torch
-from torch import nn
-from torch.nn import functional as F
+from torch import Tensor, nn
+from torchvision.ops import DeformConv2d
+
+from .weight_init import constant_init
 
 
-class Conv2d(torch.nn.Conv2d):  # type: ignore
-    """Wrapper around Conv2d to support empty inputs and norm/activation."""
+class DeformConv(DeformConv2d):  # type: ignore
+    """Wrapper around Deformable Convolution operator with norm/activation.
 
-    def __init__(self, *args, **kwargs) -> None:  # type: ignore
-        """Init."""
-        norm = kwargs.pop("norm", None)
-        activation = kwargs.pop("activation", None)
-        super().__init__(*args, **kwargs)
+    If norm is specified, it is initialized with 1.0 and bias with 0.0.
+    """
+
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+        kernel_size: int,
+        stride: int = 1,
+        padding: int = 0,
+        dilation: int = 1,
+        groups: int = 1,
+        bias: bool = True,
+        norm: nn.Module | None = None,
+        activation: nn.Module | None = None,
+    ) -> None:
+        """Creates an instance of the class.
+
+        Args:
+            in_channels (int): Input channels.
+            out_channels (int): Output channels.
+            kernel_size (int): Size of convolutional kernel.
+            stride (int, optional): Stride of convolutional layer. Defaults to
+                1.
+            padding (int, optional): Padding of convolutional layer. Defaults
+                to 0.
+            dilation (int, optional): Dilation of convolutional layer. Defaults
+                to 1.
+            groups (int, optional): Number of deformable groups. Defaults to 1.
+            bias (bool, optional): Whether to use bias in convolutional layer.
+                Defaults to True.
+            norm (nn.Module, optional): Normalization layer. Defaults to None.
+            activation (nn.Module, optional): Activation layer. Defaults to
+                None.
+        """
+        super().__init__(
+            in_channels,
+            out_channels,
+            kernel_size,
+            stride=stride,
+            padding=padding,
+            dilation=dilation,
+            groups=groups,
+            bias=bias,
+        )
+        self.conv_offset = nn.Conv2d(
+            self.in_channels,
+            self.groups * 3 * self.kernel_size[0] * self.kernel_size[1],
+            kernel_size=self.kernel_size,
+            stride=self.stride,
+            padding=self.padding,
+            dilation=self.dilation,
+            bias=True,
+        )
         self.norm = norm
         self.activation = activation
+        self.init_weights()
 
-    def forward(  # pylint: disable=arguments-renamed
-        self, x: torch.Tensor
-    ) -> torch.Tensor:
-        """Forward pass."""
-        if not torch.jit.is_scripting():
-            # https://github.com/pytorch/pytorch/issues/12013
-            if (
-                x.numel() == 0
-                and self.training
-                and isinstance(self.norm, torch.nn.SyncBatchNorm)
-            ):
-                raise ValueError(
-                    "SyncBatchNorm does not support empty inputs!"
-                )
-
-        x = F.conv2d(
-            x,
-            self.weight,
-            self.bias,
-            self.stride,
-            self.padding,
-            self.dilation,
-            self.groups,
-        )
+    def init_weights(self) -> None:
+        """Initialize weights of offset conv layer."""
+        self.conv_offset.weight.data.zero_()
+        self.conv_offset.bias.data.zero_()  # type: ignore
         if self.norm is not None:
-            x = self.norm(x)
-        if self.activation is not None:
-            x = self.activation(x)
-        return x
-
-
-def add_conv_branch(
-    num_branch_convs: int,
-    last_layer_dim: int,
-    conv_out_dim: int,
-    conv_has_bias: bool,
-    norm_cfg: Optional[str],
-    num_groups: int,
-) -> Tuple[nn.ModuleList, int]:
-    """Init conv branch for head."""
-    convs = nn.ModuleList()
-    if norm_cfg is not None:
-        norm = getattr(nn, norm_cfg)
-    else:
-        norm = None
-    if norm == nn.GroupNorm:
-        norm = lambda x: nn.GroupNorm(num_groups, x)
-    if num_branch_convs > 0:
-        for i in range(num_branch_convs):
-            conv_in_dim = last_layer_dim if i == 0 else conv_out_dim
-            convs.append(
-                Conv2d(
-                    conv_in_dim,
-                    conv_out_dim,
-                    kernel_size=3,
-                    padding=1,
-                    bias=conv_has_bias,
-                    norm=norm(conv_out_dim) if norm is not None else norm,
-                    activation=nn.ReLU(inplace=True),
-                )
-            )
-        last_layer_dim = conv_out_dim
+            constant_init(self.norm, 1.0, bias=0.0)
 
-    return convs, last_layer_dim
+    def forward(  # pylint: disable=arguments-differ
+        self, input_x: Tensor
+    ) -> Tensor:
+        """Forward."""
+        out = self.conv_offset(input_x)
+        o1, o2, mask = torch.chunk(out, 3, dim=1)
+        offset = torch.cat((o1, o2), dim=1)
+        mask = torch.sigmoid(mask)
+        input_x = super().forward(input_x, offset, mask)
+        if self.norm is not None:
+            input_x = self.norm(input_x)
+        if self.activation is not None:
+            input_x = self.activation(input_x)
+        return input_x
```

### Comparing `vis4d-0.0/vis4d/common/utils/time.py` & `vis4d-0.1/vis4d/common/time.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-"""Utilities for timing."""
+"""This module contains utilities for tracking execution time."""
+
+from __future__ import annotations
+
 from time import perf_counter
-from typing import Optional, no_type_check
+from typing import no_type_check
 
 
 @no_type_check
 def timeit(func):
     """Function to be used as decorator to time a function."""
 
     def timed(*args, **kwargs):
@@ -17,17 +20,17 @@
     return timed
 
 
 class Timer:  # pragma: no cover
     """Timer class based on perf_counter."""
 
     def __init__(self) -> None:
-        """Init."""
+        """Creates an instance of the class."""
         self._tic = perf_counter()
-        self._toc: Optional[float] = None
+        self._toc: None | float = None
         self.paused = False
 
     def reset(self) -> None:
         """Reset timer."""
         self._tic = perf_counter()
         self._toc = None
         self.paused = False
@@ -37,15 +40,15 @@
         if self.paused:
             raise ValueError("Timer already paused!")
         self._toc = perf_counter()
         self.paused = True
 
     def resume(self) -> None:
         """Resume function."""
-        if self.paused:
+        if not self.paused:
             raise ValueError("Timer is not paused!")
         assert self._toc is not None
         self._tic = perf_counter() - (self._toc - self._tic)
         self._toc = None
         self.paused = False
 
     def time(self, milliseconds: bool = False) -> float:
```

### Comparing `vis4d-0.0/vis4d/config/config.py` & `vis4d-0.1/vis4d/engine/parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,192 +1,218 @@
-"""Config definitions."""
-import os
-from argparse import Namespace
-from datetime import datetime
-from typing import Any, List, Optional
-
-import toml
-import yaml
-from pydantic import BaseModel, validator
-
-from vis4d.common.utils.distributed import get_rank
-from vis4d.data.datasets import BaseDatasetConfig
-from vis4d.model import BaseModelConfig
-from vis4d.struct import DictStrAny
-
-
-class Launch(BaseModel):
-    """Launch configuration.
-
-    Standard Options (command line only):
-    action (positional argument): train / test / predict
-    config: Filepath to config file
-
-    Launch Options:
-    work_dir: Specific directory to save checkpoints, logs, etc. Integrates
-    with exp_name and version to work_dir/exp_name/version.
-    Default: ./vis4d-workspace/
-    exp_name: Name of current experiment. Default: <name of model>
-    version: Version of current experiment. Default: <timestamp>
-    input_dir: Input directory in case you want to run inference on a folder
-    with input data (e.g. images that can be temporally sorted by name).
-    find_unused_parameters: Activates PyTorch checking for unused parameters
-    in DDP setting. Deactivated by default for better performance.
-    visualize: If you're running in predict mode, this option lets you
-    visualize the model predictions in the output_dir.
-    seed: Set random seed for numpy, torch, python. Default: None,
-    i.e. no specific random seed is chosen.
-    weights: Filepath for weights to load in test / predict. Default: "best",
-    will load the best checkpoint in work_dir/exp_name/version.
-    checkpoint_period: After N epochs, save out checkpoints. Default: 1
-    resume: Whether to resume from weights (if specified), or last ckpt in
-    work_dir/exp_name/version.
-    pin_memory: Enable/Disable pin_memory option for dataloader workers in
-    training.
-    wandb: Use weights and biases logging instead of tensorboard (default).
-    """
+"""Parser for config files that can be used with absl flags."""
 
-    action: str = ""
-    samples_per_gpu: int = 1
-    workers_per_gpu: int = 1
-    work_dir: str = "vis4d-workspace"
-    exp_name: str = ""
-    version: str = (
-        str(datetime.now())
-        .split(".", maxsplit=1)[0]
-        .replace(" ", "_")
-        .replace(":", "-")
-    )
-    input_dir: Optional[str]
-    find_unused_parameters: bool = False
-    visualize: bool = False
-    seed: Optional[int]
-    weights: Optional[str]
-    checkpoint_period: int = 1
-    resume: bool = False
-    pin_memory: bool = False
-    wandb: bool = False
-
-    @validator("version", always=True)
-    def validate_version(  # pylint: disable=no-self-argument,no-self-use
-        cls, value: str
-    ) -> str:
-        """Sync version in distributed setting."""
-        if get_rank() == 0:
-            os.environ["RUN_VERSION"] = value
-        else:
-            value = os.environ["RUN_VERSION"]
-        return value
-
-    @validator("input_dir", always=True)
-    def validate_input_dir(  # pylint: disable=no-self-argument,no-self-use
-        cls, value: Optional[str]
-    ) -> Optional[str]:
-        """Check if input dir exists."""
-        if value is not None:
-            if not os.path.exists(value):
-                raise FileNotFoundError(
-                    f"Input directory does not exist: {value}"
+from __future__ import annotations
+
+import logging
+import re
+import sys
+import traceback
+from typing import Any
+
+from absl import flags
+from ml_collections import ConfigDict, FieldReference
+from ml_collections.config_flags.config_flags import (
+    _ConfigFlag,
+    _ErrorConfig,
+    _LockConfig,
+)
+
+from vis4d.config import copy_and_resolve_references
+from vis4d.config.registry import get_config_by_name
+
+
+class ConfigFileParser(flags.ArgumentParser):  # type: ignore
+    """Parser for config files."""
+
+    def __init__(
+        self,
+        name: str,
+        lock_config: bool = True,
+        method_name: str = "get_config",
+    ) -> None:
+        """Initializes the parser.
+
+        Args:
+            name (str): The name of the flag (e.g. config for --config flag)
+            lock_config (bool, optional): Whether or not to lock the config.
+                Defaults to True.
+            method_name (str, optional): Name of the method to call in the
+                config. Defaults to "get_config".
+        """
+        self.name = name
+        self._lock_config = lock_config
+        self.method_name = method_name
+
+    def parse(  # pylint: disable=arguments-renamed
+        self, path: str
+    ) -> ConfigDict | _ErrorConfig:
+        """Loads a config module from `path` and returns the `method_name()`.
+
+        This implementation is based on the original ml_collections and
+        modified to allow for a custom method name.
+
+        If a colon is present in `path`, everything to the right of the first
+        colon is passed to `method_name` as an argument. This allows the
+        structure of what
+        is returned to be modified, which is useful when performing complex
+        hyperparameter sweeps.
+
+        Args:
+          path: string, path pointing to the config file to execute. May also
+              contain a config_string argument, e.g. be of the form
+              "config.py:some_configuration".
+
+        Returns:
+          Result of calling `method_name` in the specified module.
+        """
+        # This will be a 2 element list iff extra configuration args are
+        # present.
+        split_path = path.split(":", 1)
+
+        try:
+            config = get_config_by_name(
+                split_path[0],
+                *split_path[1:],
+                method_name=self.method_name,
+            )
+            if config is None:
+                logging.warning(
+                    "%s:%s() returned None, did you forget a return "
+                    "statement?",
+                    path,
+                    self.method_name,
                 )
-        return value
+        except IOError as e:
+            # Don't raise the error unless/until the config is
+            # actually accessed.
+            return _ErrorConfig(e)
+        # Third party flags library catches TypeError and ValueError
+        # and rethrows,
+        # removing useful information unless it is added here (b/63877430):
+        except (TypeError, ValueError) as e:
+            error_trace = traceback.format_exc()
+            raise type(e)(
+                "Error whilst parsing config file:\n\n" + error_trace
+            )
+
+        if self._lock_config:
+            _LockConfig(config)
+
+        return config
+
+    def flag_type(self) -> str:
+        """Returns the type of the flag."""
+        return "config object"
+
+
+def DEFINE_config_file(  # pylint: disable=invalid-name
+    name: str,
+    default: str | None = None,
+    help_string: str = "path to config file [.py |.yaml].",
+    lock_config: bool = False,
+    method_name: str = "get_config",
+) -> flags.FlagHolder:
+    """Registers a new flag for a config file.
+
+    Args:
+        name (str): The name of the flag (e.g. config for --config flag)
+        default (str | None, optional): Default Value. Defaults to None.
+        help_string (str, optional): Help String.
+            Defaults to "path to config file.".
+        lock_config (bool, optional): Whether or note to lock the returned
+            config. Defaults to False.
+        method_name (str, optional): Name of the method to call in the config.
 
+    Returns:
+        flags.FlagHolder: Flag holder instance.
+    """
+    parser = ConfigFileParser(
+        name=name, lock_config=lock_config, method_name=method_name
+    )
+    flag = _ConfigFlag(
+        parser=parser,
+        serializer=flags.ArgumentSerializer(),
+        name=name,
+        default=default,
+        help_string=help_string,
+        flag_values=flags.FLAGS,
+    )
+
+    # Get the module name for the frame at depth 1 in the call stack.
+    module_name = sys._getframe(  # pylint: disable=protected-access
+        1
+    ).f_globals.get("__name__", None)
+    module_name = sys.argv[0] if module_name == "__main__" else module_name
+    return flags.DEFINE_flag(flag, flags.FLAGS, module_name=module_name)
+
+
+def pprints_config(data: ConfigDict) -> str:
+    """Converts a Config Dict into a string with a .yaml like structure.
+
+    This function differs from __repr__ of ConfigDict in that it will not
+    encode python classes using binary formats but just prints the __repr__
+    of these classes.
 
-class Config(BaseModel, extra="allow"):
-    """Overall config object."""
+    Args:
+        data (ConfigDict): Configuration dict to convert to string
 
-    launch: Launch = Launch()
-    model: BaseModelConfig
-    train: List[BaseDatasetConfig] = []
-    test: List[BaseDatasetConfig] = []
-
-    def __init__(self, **data: Any) -> None:  # type: ignore
-        """Init config."""
-        super().__init__(**data)
-        if self.launch.exp_name == "":
-            self.launch.exp_name = self.model.type
-
-
-def parse_config(args: Namespace) -> Config:
-    """Read config, parse cmd line arguments."""
-    cfg = read_config(args.config)
-    for attr, value in args.__dict__.items():
-        if attr in Launch.__fields__ and value is not None:
-            setattr(cfg.launch, attr, getattr(args, attr))
-
-    if args.__dict__.get("cfg_options", "") != "":
-        cfg_dict = cfg.dict()
-        options = args.cfg_options.split(",")
-        for option in options:
-            key, value = option.split("=")
-            keylist_update(cfg_dict, key.split("."), value)
-        cfg = Config(**cfg_dict)
-    return cfg
-
-
-def load_config(filepath: str) -> DictStrAny:
-    """Load config from file to dict."""
-    ext = os.path.splitext(filepath)[1]
-    config_dict: DictStrAny
-    if ext == ".yaml":
-        with open(filepath, "r", encoding="utf-8") as f:
-            config_dict = yaml.load(f.read(), Loader=yaml.Loader)
-    elif ext == ".toml":
-        config_dict = dict(**toml.load(filepath))
-    else:
-        raise NotImplementedError(f"Config type {ext} not supported")
-    return config_dict
+    Returns:
+        str: A string representation of the ConfigDict
+    """
+    return _pprints_config(copy_and_resolve_references(data))
 
 
-def read_config(filepath: str) -> Config:
-    """Read config file and parse it into Config object.
+def _pprints_config(  # type: ignore
+    data: Any, prefix: str = "", n_indents: int = 1
+) -> str:
+    """Converts a ConfigDict into a string with a YAML like structure.
 
-    The config file can be in yaml or toml.
-    toml is recommended for readability.
-    """
-    config_dict = load_config(filepath)
-    if "config" in config_dict:
-        cwd = os.getcwd()
-        os.chdir(os.path.dirname(filepath))
-        subconfig_dict: DictStrAny = {}
-        for cfg in config_dict["config"]:
-            assert "path" in cfg, "Config arguments must have path!"
-            nested_update(subconfig_dict, load_config(cfg["path"]))
-
-        nested_update(subconfig_dict, config_dict)
-        config_dict = subconfig_dict
-        os.chdir(cwd)
-
-    config_dict = check_for_dicts(config_dict)
-    return Config(**config_dict)
-
-
-def keylist_update(  # type: ignore
-    my_dict: DictStrAny, key_list: List[str], value: Any
-) -> None:
-    """Update nested dict based on multiple keys saved in a list."""
-    cur_key = key_list.pop(0)
-    if len(key_list) == 0:
-        my_dict[cur_key] = value
-        return
-    keylist_update(my_dict[cur_key], key_list, value)
-
-
-def nested_update(ori: DictStrAny, new: DictStrAny) -> DictStrAny:
-    """Update function for updating a nested dict."""
-    for k, v in new.items():
-        if isinstance(v, dict) and not isinstance(
-            v, toml.decoder.InlineTableDict  # type: ignore
-        ):
-            ori[k] = nested_update(ori.get(k, {}), v)
-        else:
-            ori[k] = v
-    return ori
+    This is the recursive implementation of 'pprints_config' and will be called
+    recursively for every element in the dict.
 
+    This function differs from __repr__ of ConfigDict in that it will not
+    encode python classes using binary formats but just prints the __repr__
+    of these classes.
 
-def check_for_dicts(obj: Any) -> Any:  # type: ignore
-    """Fix pickle error with a class not being serializable.
+    Args:
+        data (Any): Configuration dict or object to convert to
+            string
+        prefix (str): Prefix to print on each new line
+        n_indents (int): Number of spaces to append for each nester property.
 
-    TomlDecoder.get_empty_inline_table.<locals>.DynamicInlineTableDict
+    Returns:
+        str: A string representation of the ConfigDict
     """
-    if isinstance(obj, dict):
-        return {k: check_for_dicts(v) for k, v in obj.items()}
-    return obj
+    string_repr = ""
+    if isinstance(data, FieldReference):
+        data = data.get()
+
+    if not isinstance(data, (dict, ConfigDict, list, tuple, dict)):
+        return str(data)
+
+    string_repr += "\n"
+
+    if isinstance(data, (ConfigDict, dict)):
+        for key in data:
+            value = data[key]
+            string_repr += (
+                prefix
+                + key
+                + ": "
+                + _pprints_config(value, prefix=prefix + " " * n_indents)
+            ) + "\n"
+
+    elif isinstance(data, (list, tuple)):
+        for value in data:
+            string_repr += prefix + "- "
+            if isinstance(value, (ConfigDict, dict)):
+                string_repr += "\n"
+
+            string_repr += (
+                _pprints_config(value, prefix=prefix + " " + " " * n_indents)
+                + "\n"
+            )
+        string_repr += " \n"  # Add newline after list for better readability.
+
+    # Clean up some formatting issues using regex. Could be done better
+    string_repr = re.sub("\n\n+", "\n", string_repr)
+    return re.sub("- +\n +", "- ", string_repr)
```

### Comparing `vis4d-0.0/vis4d/data/dataset_test.py` & `vis4d-0.1/vis4d/data/reference.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,233 +1,239 @@
-"""Testcases for Vis4D ScalabelDataset."""
-import unittest
-from typing import List
-
-import torch
-from scalabel.label.typing import (
-    Box2D,
-    Category,
-    Config,
-    Dataset,
-    Frame,
-    Label,
-)
-
-from ..struct import Boxes2D, Images, InputSample
-from .dataset import ScalabelDataset
-from .datasets.base import (
-    BaseDatasetConfig,
-    BaseDatasetLoader,
-    DataloaderConfig,
-    ReferenceSamplingConfig,
-)
-
-
-class MockDatasetLoader(BaseDatasetLoader):
-    """Scalabel dataset mockup."""
-
-    def __init__(self, cfg: BaseDatasetConfig, frames: List[Frame]) -> None:
-        """Init."""
-        self.frames = frames
-        super().__init__(cfg)
-
-    def load_dataset(self) -> Dataset:
-        """Load and possibly convert dataset to scalabel format."""
-        config = Config(categories=[Category(name="test")])
-        return Dataset(frames=self.frames, config=config)
-
-
-class TestScalabelDataset(unittest.TestCase):
-    """ScalabelDataset Testcase class."""
-
-    cfg = BaseDatasetConfig(
-        name="test",
-        type="Scalabel",
-        data_root="/path/to/root",
-        dataloader=DataloaderConfig(
-            ref_sampling=ReferenceSamplingConfig(
-                type="sequential",
-                num_ref_imgs=2,
-                scope=3,
-                frame_order="temporal",
+"""Reference View Sampling.
+
+These Classes sample reference views from a dataset that contains videos.
+This is usually used when a model needs multiple samples of a video during
+training.
+"""
+
+from __future__ import annotations
+
+from abc import abstractmethod
+from typing import Callable, List
+
+import numpy as np
+from torch.utils.data import Dataset
+
+from .const import CommonKeys as K
+from .datasets import VideoDataset
+from .typing import DictData
+
+SortingFunc = Callable[[DictData, list[DictData]], List[DictData]]
+
+
+def sort_key_first(
+    cur_sample: DictData, ref_data: list[DictData]
+) -> list[DictData]:
+    """Sort views as key first."""
+    return [cur_sample, *ref_data]
+
+
+def sort_temporal(
+    cur_sample: DictData, ref_data: list[DictData]
+) -> list[DictData]:
+    """Sort views temporally."""
+    return sorted([cur_sample, *ref_data], key=lambda x: x[K.frame_ids])
+
+
+class ReferenceViewSampler:
+    """Base reference view sampler."""
+
+    def __init__(self, num_ref_samples: int) -> None:
+        """Creates an instance of the class.
+
+        Args:
+            num_ref_samples (int): Number of reference views to sample.
+        """
+        self.num_ref_samples = num_ref_samples
+
+    @abstractmethod
+    def __call__(
+        self,
+        key_dataset_index: int,
+        indices_in_video: list[int],
+        frame_ids: list[int],
+    ) -> list[int]:
+        """Sample num_ref_samples reference view indices.
+
+        Args:
+            key_index (int): Index of key view in the video.
+            indices_in_video (list[int]): All dataset indices in the video.
+            frame_ids (list[int]): Frame ids of all views in the video.
+
+        Returns:
+            list[int]: dataset indices of reference views.
+        """
+        raise NotImplementedError
+
+
+class SequentialViewSampler(ReferenceViewSampler):
+    """Sequential View Sampler."""
+
+    def __call__(
+        self,
+        key_dataset_index: int,
+        indices_in_video: list[int],
+        frame_ids: list[int],
+    ) -> list[int]:
+        """Sample sequential reference views."""
+        assert len(frame_ids) >= self.num_ref_samples + 1
+
+        key_index = indices_in_video.index(key_dataset_index)
+
+        right = key_index + 1 + self.num_ref_samples
+        if right <= len(indices_in_video):
+            ref_dataset_indices = indices_in_video[key_index + 1 : right]
+        else:
+            left = key_index - (right - len(indices_in_video))
+            ref_dataset_indices = (
+                indices_in_video[left:key_index]
+                + indices_in_video[key_index + 1 :]
             )
-        ),
-    )
+        return ref_dataset_indices
+
+
+class UniformViewSampler(ReferenceViewSampler):
+    """View Sampler that chooses reference views uniform at random."""
+
+    def __init__(self, scope: int, num_ref_samples: int) -> None:
+        """Creates an instance of the class.
 
-    dataset_loader = MockDatasetLoader(
-        cfg,
-        [
-            Frame(
-                name=str(i),
-                videoName=str(i % 2),
-                frameIndex=i - i // 2 - i % 2,
+        Args:
+            scope (int): Define scope of neighborhood to key view to sample
+                from.
+            num_ref_samples (int): Number of reference views to sample.
+        """
+        super().__init__(num_ref_samples)
+        if scope != 0 and scope < num_ref_samples // 2:
+            raise ValueError("Scope must be higher than num_ref_imgs / 2.")
+        self.scope = scope
+
+    def _get_valid_indices(
+        self, key_index: int, indices_in_video: list[int], frame_ids: list[int]
+    ) -> list[int]:
+        """Get valid indices in video."""
+        key_fid = frame_ids[key_index]
+        min_fid = max(0, key_fid - self.scope)
+        max_fid = min(key_fid + self.scope, frame_ids[-1])
+
+        return [
+            ind
+            for i, ind in enumerate(indices_in_video)
+            if min_fid <= frame_ids[i] <= max_fid and i != key_index
+        ]
+
+    def __call__(
+        self,
+        key_dataset_index: int,
+        indices_in_video: list[int],
+        frame_ids: list[int],
+    ) -> list[int]:
+        """Uniformly sample reference views."""
+        if self.scope > 0:
+            key_index = indices_in_video.index(key_dataset_index)
+
+            valid_indices = self._get_valid_indices(
+                key_index, indices_in_video, frame_ids
             )
-            for i in range(200)
-        ],
-    )
-
-    dataset = ScalabelDataset(dataset_loader, True)
-
-    def test_reference_sampling(self) -> None:
-        """Testcase for reference view sampling."""
-        idcs = self.dataset.sample_ref_indices(str(0), 50)
-        self.assertTrue(idcs == [52, 54])
-        idcs = self.dataset.sample_ref_indices(str(0), 196)
-        self.assertTrue(idcs == [194, 198])
-
-    def test_getitem_fallback(self) -> None:
-        """Testcase for getitem fallback if None is returned."""
-        cfg = BaseDatasetConfig(
-            name="test",
-            type="Scalabel",
-            data_root="vis4d/engine/testcases/track/bdd100k-samples/images/",
-            dataloader=DataloaderConfig(
-                ref_sampling=ReferenceSamplingConfig(
-                    type="sequential",
-                    num_ref_imgs=1,
-                    scope=3,
-                    skip_nomatch_samples=True,
-                ),
-            ),
-        )
-
-        dataset_loader = MockDatasetLoader(
-            cfg,
-            [
-                Frame(
-                    name="00091078-875c1f73-0000167.jpg",
-                    videoName="00091078-875c1f73",
-                    frameIndex=i,
-                )
-                for i in range(6)
-            ],
-        )
-        dataset = ScalabelDataset(dataset_loader, True)
-        self.assertRaises(ValueError, dataset.__getitem__, 0)
-
-    def test_transform_input(self) -> None:
-        """Test the transform_input method in ScalabelDataset."""
-        input_sample = InputSample(
-            [Frame(name="0")],
-            Images(torch.zeros(1, 3, 128, 128), [(128, 128)]),
-        )
-        self.dataset.transform_input(input_sample, None)
-        self.assertEqual(len(input_sample.boxes2d[0]), 0)
-        self.dataset.transform_input(input_sample, [])
-        self.assertEqual(len(input_sample.boxes2d[0]), 0)
-
-        labels = [
-            Label(
-                id="a",
-                category="car",
-                box2d=Box2D(x1=10, y1=10, x2=20, y2=20),
-                attributes={"category_id": 0, "instance_id": 2},
-            ),
-            Label(
-                id="b",
-                category="car",
-                box2d=Box2D(x1=11, y1=10, x2=20, y2=20),
-                attributes={"category_id": 0, "instance_id": 1},
-            ),
-            Label(
-                id="c",
-                category="car",
-                box2d=Box2D(x1=12, y1=10, x2=20, y2=20),
-                attributes={"category_id": 0, "instance_id": 0},
-            ),
+
+            if len(valid_indices) > 0:
+                assert len(valid_indices) >= self.num_ref_samples
+                return np.random.choice(
+                    valid_indices, self.num_ref_samples, replace=False
+                ).tolist()
+
+        return [key_dataset_index] * self.num_ref_samples
+
+
+class MultiViewDataset(Dataset[list[DictData]]):
+    """Dataset that samples reference views from a video dataset."""
+
+    def __init__(
+        self,
+        dataset: VideoDataset,
+        sampler: ReferenceViewSampler,
+        sort_fn: SortingFunc = sort_key_first,
+        num_retry: int = 3,
+        match_key: str = K.boxes2d_track_ids,
+        skip_nomatch_samples: bool = False,
+    ) -> None:
+        """Creates an instance of the class.
+
+        Args:
+            dataset (Dataset): Video dataset to sample from.
+            sampler (ReferenceViewSampler): Sampler that samples reference
+                views.
+            sort_fn (SortingFunc, optional): Function that sorts key and
+                reference views. Defaults to sort_key_first.
+            num_retry (int, optional): Number of retries if no match is found.
+                Defaults to 3.
+            match_key (str, optional): Key to match reference views with key
+                view. Defaults to K.boxes2d_track_ids.
+            skip_nomatch_samples (bool, optional): Whether to skip samples
+                where no match is found. Defaults to False.
+        """
+        self.dataset = dataset
+        self.sampler = sampler
+        self.sort_fn = sort_fn
+        self.num_retry = num_retry
+        self.match_key = match_key
+        self.skip_nomatch_samples = skip_nomatch_samples
+
+    def has_matches(
+        self, key_data: DictData, ref_data: list[DictData]
+    ) -> bool:
+        """Check if key / ref data have matches."""
+        key_target = key_data[self.match_key]
+        for ref_view in ref_data:
+            ref_target = ref_view[self.match_key]
+            match = np.equal(
+                np.expand_dims(key_target, axis=1), ref_target[None]
+            )
+            if match.any():
+                return True
+        return False  # pragma: no cover
+
+    def __len__(self) -> int:
+        """Get length of dataset."""
+        return len(self.dataset)
+
+    def get_ref_data(self, ref_indices: list[int]) -> list[DictData]:
+        """Get reference data from dataset."""
+        ref_data = []
+        for ref_index in ref_indices:
+            ref_sample = self.dataset[ref_index]
+            ref_sample["keyframes"] = False
+            ref_data.append(ref_sample)
+
+        assert self.sampler.num_ref_samples == len(ref_data)
+        return ref_data
+
+    def __getitem__(self, index: int) -> list[DictData]:
+        """Get item from dataset."""
+        cur_sample = self.dataset[index]
+        cur_sample["keyframes"] = True
+
+        indices_in_video = self.dataset.video_mapping["video_to_indices"][
+            cur_sample[K.sequence_names]
         ]
-        input_sample.boxes2d = [
-            Boxes2D.from_scalabel(labels, {"car": 0}, {"a": 2, "b": 1, "c": 0})
+        frame_ids = self.dataset.video_mapping["video_to_frame_ids"][
+            cur_sample[K.sequence_names]
         ]
-        self.dataset.transform_input(input_sample, [])
 
-        self.assertTrue(all(input_sample.boxes2d[0].class_ids == 0))
-        self.assertEqual(input_sample.boxes2d[0].boxes[0, 0], 10)
-        self.assertEqual(input_sample.boxes2d[0].boxes[1, 0], 11)
-        self.assertEqual(input_sample.boxes2d[0].boxes[2, 0], 12)
-
-        self.assertEqual(input_sample.boxes2d[0].track_ids[0], 2)
-        self.assertEqual(input_sample.boxes2d[0].track_ids[1], 1)
-        self.assertEqual(input_sample.boxes2d[0].track_ids[2], 0)
-
-    def test_sort_samples(self) -> None:
-        """Test the sort_samples method in MapDataset."""
-        input_samples = [
-            InputSample(
-                [Frame(name="1", frameIndex=1)],
-                Images(torch.zeros(1, 3, 128, 128), [(128, 128)]),
-            ),
-            InputSample(
-                [Frame(name="0", frameIndex=0)],
-                Images(torch.zeros(1, 3, 128, 128), [(128, 128)]),
-            ),
-        ]
-        sorted_samples = self.dataset.sort_samples(input_samples)
-        self.assertEqual(sorted_samples[0].metadata[0].frameIndex, 0)
-        self.assertEqual(sorted_samples[1].metadata[0].frameIndex, 1)
-
-    def test_filter_attributes(self) -> None:
-        """Testcase for attribute filtering."""
-        cfg = BaseDatasetConfig(
-            name="test",
-            type="Scalabel",
-            data_root="/path/to/root",
-            dataloader=DataloaderConfig(
-                ref_sampling=ReferenceSamplingConfig(
-                    type="sequential",
-                    num_ref_imgs=2,
-                    scope=3,
-                    frame_order="temporal",
-                )
-            ),
-            attributes={"timeofday": ["daytime", "night"], "weather": "clear"},
-        )
-
-        # Testcase 1
-        dataset_loader = MockDatasetLoader(
-            cfg,
-            [
-                Frame(
-                    name=str(i),
-                    videoName=str(i % 2),
-                    frameIndex=i - i // 2 - i % 2,
-                    attributes={"timeofday": "daytime", "weather": "clear"},
-                )
-                for i in range(6)
-            ],
-        )
-
-        dataset = ScalabelDataset(dataset_loader, True)
-        self.assertTrue(len(dataset) == 6)
-
-        # Testcase 2
-        dataset_loader = MockDatasetLoader(
-            cfg,
-            [
-                Frame(
-                    name=str(i),
-                    videoName=str(i % 2),
-                    frameIndex=i - i // 2 - i % 2,
-                    attributes={"timeofday": "night", "weather": "clear"},
-                )
-                for i in range(6)
-            ],
-        )
-
-        dataset = ScalabelDataset(dataset_loader, True)
-        self.assertTrue(len(dataset) == 6)
-
-        # Testcase 3
-        dataset_loader = MockDatasetLoader(
-            cfg,
-            [
-                Frame(
-                    name=str(i),
-                    videoName=str(i % 2),
-                    frameIndex=i - i // 2 - i % 2,
-                    attributes={"timeofday": "daytime", "weather": "snowy"},
-                )
-                for i in range(6)
-            ],
-        )
+        if self.sampler.num_ref_samples > 0:
+            for _ in range(self.num_retry):
+                ref_indices = self.sampler(index, indices_in_video, frame_ids)
+
+                ref_data = self.get_ref_data(ref_indices)
+
+                if self.skip_nomatch_samples and not (
+                    self.has_matches(cur_sample, ref_data)
+                ):
+                    continue
+
+                return self.sort_fn(cur_sample, ref_data)
+
+            ref_indices = [index] * self.sampler.num_ref_samples
+            ref_data = self.get_ref_data(ref_indices)
+            return [cur_sample, *ref_data]
 
-        self.assertRaises(ValueError, ScalabelDataset, dataset_loader, True)
+        return [cur_sample]
```

### Comparing `vis4d-0.0/vis4d/data/transforms/augmentations.py` & `vis4d-0.1/vis4d/vis/image/bbox3d_visualizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,455 +1,419 @@
-"""Vis4D augmentations."""
-import random
-from typing import List, Optional, Tuple, Union
+"""Bounding box 3D visualizer."""
+
+from __future__ import annotations
+
+import os
+from collections import defaultdict
+from collections.abc import Sequence
+from dataclasses import dataclass
 
 import numpy as np
 import torch
-import torch.nn.functional as F
 
-from vis4d.common.bbox.utils import bbox_intersection
-from vis4d.data.utils import transform_bbox
-from vis4d.struct import (
-    Boxes2D,
-    Boxes3D,
-    Images,
-    InputSample,
-    Intrinsics,
-    TMasks,
+from vis4d.common.array import array_to_numpy
+from vis4d.common.typing import (
+    ArgsType,
+    ArrayLike,
+    ArrayLikeFloat,
+    ArrayLikeInt,
+    NDArrayF32,
+    NDArrayUI8,
 )
+from vis4d.data.const import AxisMode
+from vis4d.op.geometry.transform import inverse_rigid_transform
+from vis4d.vis.base import Visualizer
+from vis4d.vis.util import generate_color_map
+
+from .canvas import CanvasBackend, PillowCanvasBackend
+from .util import preprocess_boxes3d, preprocess_image, project_point
+from .viewer import ImageViewerBackend, MatplotlibImageViewer
+
+
+@dataclass
+class DetectionBox3D:
+    """Dataclass storing box informations."""
 
-from .base import AugParams, BaseAugmentation, BaseAugmentationConfig
+    corners: list[tuple[float, float, float]]
+    label: str
+    color: tuple[int, int, int]
+    track_id: int | None
 
 
-class ResizeConfig(BaseAugmentationConfig):
-    """Resize augmentation config.
+@dataclass
+class DataSample:
+    """Dataclass storing a data sample that can be visualized."""
 
-    shape: Image shape to be resized to in (H, W) format. In
-    multiscale mode 'list', shape represents the list of possible
-    shapes for resizing.
-    interpolation: Interpolation method. One of ["nearest", "bilinear",
-    "bicubic"]
-    keep_ratio: If aspect ratio of original image should be kept, the
-    new height will be scaled according to the new width and the
-    aspect ratio of the original image as:
-    new_h = new_w / (orginal_w / original_h)
-    multiscale_mode: one of [range, list],
-    scale_range: Range of sampled image scales in range mode, e.g.
-    (0.8, 1.2), indicating minimum of 0.8 * shape and maximum of
-    1.2 * shape.
-    return_transform: If the transform should be returned in matrix
-    format.
-    """
-
-    shape: Union[Tuple[int, int], List[Tuple[int, int]]]
-    keep_ratio: bool = False
-    multiscale_mode: str = "range"
-    scale_range: Tuple[float, float] = (1.0, 1.0)
-    interpolation: str = "bilinear"
+    image: NDArrayUI8
+    image_name: str
+    intrinsics: NDArrayF32
+    extrinsics: NDArrayF32 | None
+    sequence_name: str | None
+    camera_name: str | None
+    boxes: list[DetectionBox3D]
 
 
-class Resize(BaseAugmentation):
-    """Resize augmentation class."""
+class BoundingBox3DVisualizer(Visualizer):
+    """Bounding box 3D visualizer class."""
 
     def __init__(
         self,
-        cfg: BaseAugmentationConfig,
+        *args: ArgsType,
+        n_colors: int = 50,
+        cat_mapping: dict[str, int] | None = None,
+        file_type: str = "png",
+        image_mode: str = "RGB",
+        width: int = 2,
+        camera_near_clip: float = 0.15,
+        axis_mode: AxisMode = AxisMode.ROS,
+        trajectory_length: int = 10,
+        plot_trajectory: bool = True,
+        canvas: CanvasBackend | None = None,
+        viewer: ImageViewerBackend | None = None,
+        **kwargs: ArgsType,
     ) -> None:
-        """Init function.
+        """Creates a new Visualizer for Image and 3D Bounding Boxes.
 
         Args:
-            cfg: Augmentation config.
+            n_colors (int): How many colors should be used for the internal
+                color map. Defaults to 100.
+            cat_mapping (dict[str, int]): Mapping from class names to class
+                ids. Defaults to None.
+            file_type (str): Desired file type. Defaults to "png".
+            image_mode (str): Image channel mode (RGB or BGR). Defaults to
+                "RGB".
+            width (int): Width of the drawn bounding boxes. Defaults to 2.
+            camera_near_clip (float): Near clipping plane of the camera.
+                Defaults to 0.15.
+            axis_mode (AxisMode): Axis mode for the input bboxes. Defaults to
+                AxisMode.ROS (i.e. global coordinate).
+            trajectory_length (int): How many past frames should be used to
+                draw the trajectory. Defaults to 10.
+            plot_trajectory (bool): If the trajectory should be plotted.
+                Defaults to True.
+            canvas (CanvasBackend): Backend that is used to draw on images. If
+                None a PillowCanvasBackend is used.
+            viewer (ImageViewerBackend): Backend that is used show images. If
+                None a MatplotlibImageViewer is used.
         """
-        super().__init__(cfg)
-        self.cfg: ResizeConfig = ResizeConfig(**cfg.dict())
-        self.shape = self.cfg.shape
-        self.keep_ratio = self.cfg.keep_ratio
-        self.multiscale_mode = self.cfg.multiscale_mode
-        assert self.multiscale_mode in ["list", "range"]
-        self.scale_range = self.cfg.scale_range
-        if self.multiscale_mode == "list":
-            assert isinstance(
-                self.shape, list
-            ), "Specify shape as list when using multiscale mode list."
-            assert len(self.shape) >= 1
-            # pylint: disable=unsubscriptable-object
-            self.shape = [(int(s[0]), int(s[1])) for s in self.shape]
-        else:
-            assert isinstance(
-                self.shape, tuple
-            ), "Specify shape as tuple when using multiscale mode range."
-            self.shape = (int(self.shape[0]), int(self.shape[1]))
-            assert self.scale_range[0] <= self.scale_range[1], (
-                "Invalid scale range: "
-                f"{self.scale_range[1]} < {self.scale_range[0]}"
-            )
+        super().__init__(*args, **kwargs)
+        self._samples: list[DataSample] = []
+        self.axis_mode = axis_mode
+        self.trajectories: dict[int, list[tuple[float, float, float]]] = (
+            defaultdict(list)
+        )
+        self.trajectory_length = trajectory_length
+        self.plot_trajectory = plot_trajectory
 
-        self.interpolation = self.cfg.interpolation
-        assert self.interpolation in ["nearest", "bilinear", "bicubic"]
+        self.color_palette = generate_color_map(n_colors)
 
-    def generate_parameters(self, sample: InputSample) -> AugParams:
-        """Generate current parameters."""
-        params = super().generate_parameters(sample)
-        if self.multiscale_mode == "range":
-            assert isinstance(self.shape, tuple)
-            if self.scale_range[0] < self.scale_range[1]:  # do multi-scale
-                w_scale = (
-                    torch.rand((len(sample),))
-                    * (self.scale_range[1] - self.scale_range[0])
-                    + self.scale_range[0]
-                )
-                h_scale = (
-                    torch.rand((len(sample),))
-                    * (self.scale_range[1] - self.scale_range[0])
-                    + self.scale_range[0]
-                )
-            else:
-                h_scale = w_scale = 1.0
-
-            h_new = (
-                torch.tensor(self.shape[0]).repeat(len(sample)) * h_scale
-            ).int()
-            w_new = (
-                torch.tensor(self.shape[1]).repeat(len(sample)) * w_scale
-            ).int()
-            shape = torch.stack([h_new, w_new], -1)
-        else:
-            assert isinstance(self.shape, list)
-            shape = torch.tensor(random.sample(self.shape, k=len(sample)))
-
-        if self.keep_ratio:
-            for i, sh in enumerate(shape):
-                w, h = sample.images.image_sizes[i]
-                sh[0] = sh[1] / (w / h)
-
-        transform = (
-            torch.eye(3, device=sample.device)
-            .unsqueeze(0)
-            .repeat(len(sample), 1, 1)
-        )
-        for i, sh in enumerate(shape):
-            if params["apply"][i]:
-                w, h = sample.images.image_sizes[i]
-                transform[i, 0, 0] = sh[1] / w
-                transform[i, 1, 1] = sh[0] / h
-
-        params["shape"] = shape
-        params["transform"] = transform
-        return params
-
-    def _apply_tensor(
-        self, inputs: torch.Tensor, shape: torch.Tensor
-    ) -> torch.Tensor:
-        """Apply resize."""
-        align_corners = None if self.interpolation == "nearest" else False
-        output = F.interpolate(
-            inputs,
-            (shape[0], shape[1]),
-            mode=self.interpolation,
-            align_corners=align_corners,
+        self.class_id_mapping = (
+            {v: k for k, v in cat_mapping.items()}
+            if cat_mapping is not None
+            else {}
         )
-        return output
 
-    def apply_intrinsics(
-        self, intrinsics: Intrinsics, parameters: AugParams
-    ) -> Intrinsics:
-        """Transform intrinsic camera matrix according to augmentations."""
-        return Intrinsics(
-            torch.matmul(parameters["transform"], intrinsics.tensor)
-        )
+        self.file_type = file_type
+        self.image_mode = image_mode
+        self.width = width
+
+        self.camera_near_clip = camera_near_clip
+        self.canvas = canvas if canvas is not None else PillowCanvasBackend()
+        self.viewer = viewer if viewer is not None else MatplotlibImageViewer()
+
+    def reset(self) -> None:
+        """Reset visualizer."""
+        self._samples.clear()
 
-    def apply_image(self, images: Images, parameters: AugParams) -> Images:
-        """Apply augmentation to input image."""
-        all_ims = []
-        for i, im in enumerate(images):
-            if parameters["apply"][i]:
-                im_t = self._apply_tensor(im.tensor, parameters["shape"][i])
-                all_ims.append(Images(im_t, [(im_t.shape[3], im_t.shape[2])]))
-            else:
-                all_ims.append(im)
-
-        if len(all_ims) == 1:
-            return all_ims[0]
-        return Images.cat(all_ims)
-
-    def apply_box2d(
-        self, boxes: List[Boxes2D], parameters: AugParams
-    ) -> List[Boxes2D]:
-        """Apply augmentation to input box2d."""
-        for i, box in enumerate(boxes):
-            if len(box) > 0 and parameters["apply"][i]:
-                box.boxes[:, :4] = transform_bbox(
-                    parameters["transform"][i],
-                    box.boxes[:, :4],
-                )
-        return boxes
+    def process(  # type: ignore # pylint: disable=arguments-differ
+        self,
+        cur_iter: int,
+        images: list[ArrayLike],
+        image_names: list[str],
+        boxes3d: list[ArrayLikeFloat],
+        intrinsics: ArrayLikeFloat,
+        extrinsics: None | ArrayLikeFloat = None,
+        scores: None | list[ArrayLikeFloat] = None,
+        class_ids: None | list[ArrayLikeInt] = None,
+        track_ids: None | list[ArrayLikeInt] = None,
+        sequence_names: None | list[str] = None,
+    ) -> None:
+        """Processes a batch of data.
 
-    def apply_mask(
-        self, masks: List[TMasks], parameters: AugParams
-    ) -> List[TMasks]:
-        """Apply augmentation to input mask."""
-        interp = self.interpolation
-        self.interpolation = "nearest"
-        for i, mask in enumerate(masks):
-            if len(mask) > 0 and parameters["apply"][i]:
-                mask.masks = (
-                    self._apply_tensor(
-                        mask.masks.float().unsqueeze(1), parameters["shape"][i]
-                    )
-                    .squeeze(1)
-                    .type(mask.masks.dtype)
+        Args:
+            cur_iter (int): Current iteration.
+            images (list[ArrayLike]): Images to show.
+            image_names (list[str]): Image names.
+            boxes3d (list[ArrayLikeFloat]): List of predicted bounding boxes
+                with shape [B, N, 10].
+            intrinsics (ArrayLikeFloat): Camera intrinsics with shape
+                [B, 3, 3].
+            extrinsics (None | ArrayLikeFloat, optional): Camera extrinsics
+                with shape [B, 4, 4]. Defaults to None.
+            scores (None | list[ArrayLikeFloat], optional): List of predicted
+                box scores each of shape [B, N]. Defaults to None.
+            class_ids (None | list[ArrayLikeInt], optional): List of predicted
+                class ids each of shape [B, N]. Defaults to None.
+            track_ids (None | list[ArrayLikeInt], optional): List of predicted
+                track ids each of shape [B, N]. Defaults to None.
+            sequence_names (None | list[str], optional): List of sequence
+                names of shape [B,]. Defaults to None.
+        """
+        if self._run_on_batch(cur_iter):
+            for batch, image in enumerate(images):
+                self.process_single_image(
+                    image,
+                    image_names[batch],
+                    boxes3d[batch],
+                    intrinsics[batch],  # type: ignore
+                    (
+                        None if extrinsics is None else extrinsics[batch]  # type: ignore # pylint: disable=line-too-long
+                    ),
+                    None if scores is None else scores[batch],
+                    None if class_ids is None else class_ids[batch],
+                    None if track_ids is None else track_ids[batch],
+                    None if sequence_names is None else sequence_names[batch],
                 )
-        self.interpolation = interp
-        return masks
-
-
-class RandomCropConfig(BaseAugmentationConfig):
-    """Config for RandomCrop."""
-
-    shape: Union[
-        Tuple[float, float],
-        Tuple[int, int],
-        List[Tuple[float, float]],
-        List[Tuple[int, int]],
-    ]
-    crop_type: str = "absolute"
-    allow_empty_crop: bool = True
-    recompute_boxes2d: bool = False
-
 
-class RandomCrop(BaseAugmentation):
-    """RandomCrop augmentation class."""
+            for tid in self.trajectories:
+                if len(self.trajectories[tid]) > self.trajectory_length:
+                    self.trajectories[tid].pop(0)
 
-    def __init__(
+    def process_single_image(
         self,
-        cfg: BaseAugmentationConfig,
+        image: ArrayLike,
+        image_name: str,
+        boxes3d: ArrayLikeFloat,
+        intrinsics: ArrayLikeFloat,
+        extrinsics: None | ArrayLikeFloat = None,
+        scores: None | ArrayLikeFloat = None,
+        class_ids: None | ArrayLikeInt = None,
+        track_ids: None | ArrayLikeInt = None,
+        sequence_name: None | str = None,
+        camera_name: None | str = None,
     ) -> None:
-        """Init function.
+        """Processes a single image entry.
 
         Args:
-            cfg: Augmentation config.
+            image (ArrayLike): Image to show.
+            image_name (str): Image name.
+            boxes3d (ArrayLikeFloat): Predicted bounding boxes with shape
+                [N, 10], where  N is the number of boxes.
+            intrinsics (ArrayLikeFloat): Camera intrinsics with shape [3, 3].
+            extrinsics (None | ArrayLikeFloat, optional): Camera extrinsics
+                with shape [4, 4]. Defaults to None.
+            scores (None | ArrayLikeFloat, optional): Predicted box scores of
+                shape [N]. Defaults to None.
+            class_ids (None | ArrayLikeInt, optional): Predicted class ids of
+                shape [N]. Defaults to None.
+            track_ids (None | ArrayLikeInt, optional): Predicted track ids of
+                shape [N]. Defaults to None.
+            sequence_name (None | str, optional): Sequence name. Defaults to
+                None.
+            camera_name (None | str, optional): Camera name. Defaults to None.
         """
-        super().__init__(cfg)
-        self.cfg: RandomCropConfig = RandomCropConfig(**cfg.dict())
-        assert self.cfg.crop_type in [
-            "absolute",
-            "relative",
-            "absolute_range",
-            "relative_range",
-        ], f"Unknown crop type {self.cfg.crop_type}."
-
-        if self.cfg.crop_type == "absolute":
-            assert isinstance(self.cfg.shape, tuple)
-            assert self.cfg.shape[0] > 0 and self.cfg.shape[1] > 0
-            self.shape: Tuple[int, int] = (
-                int(self.cfg.shape[0]),
-                int(self.cfg.shape[1]),
-            )
+        img_normalized = preprocess_image(image, mode=self.image_mode)
+        image_hw = (img_normalized.shape[0], img_normalized.shape[1])
 
-        elif self.cfg.crop_type == "relative":
-            assert isinstance(self.cfg.shape, tuple)
-            assert 0 < self.cfg.shape[0] <= 1 and 0 < self.cfg.shape[1] <= 1
-            self.scale: Tuple[float, float] = self.cfg.shape
-
-        elif "range" in self.cfg.crop_type:
-            assert isinstance(self.cfg.shape, list)
-            assert len(self.cfg.shape) == 2
-            assert self.cfg.shape[1][0] >= self.cfg.shape[0][0]
-            assert self.cfg.shape[1][1] >= self.cfg.shape[0][1]
-
-            if "absolute" in self.cfg.crop_type:
-                for crop in self.cfg.shape:
-                    assert crop[0] > 0 and crop[1] > 0
-                self.shape_min: Tuple[int, int] = (
-                    int(self.cfg.shape[0][0]),
-                    int(self.cfg.shape[0][1]),
-                )
-                self.shape_max: Tuple[int, int] = (
-                    int(self.cfg.shape[1][0]),
-                    int(self.cfg.shape[1][1]),
+        intrinsics_np = array_to_numpy(intrinsics, n_dims=2, dtype=np.float32)
+        extrinsics_np = (
+            array_to_numpy(extrinsics, n_dims=2, dtype=np.float32)
+            if extrinsics is not None
+            else None
+        )
+        data_sample = DataSample(
+            img_normalized,
+            image_name,
+            intrinsics_np,  # type: ignore
+            extrinsics_np,  # type: ignore
+            sequence_name,
+            camera_name,
+            [],
+        )
+
+        for center, corners, label, color, track_id in zip(
+            *preprocess_boxes3d(
+                image_hw,
+                boxes3d,
+                intrinsics,
+                extrinsics,
+                scores,
+                class_ids,
+                track_ids,
+                self.color_palette,
+                self.class_id_mapping,
+                axis_mode=self.axis_mode,
+            )
+        ):
+            data_sample.boxes.append(
+                DetectionBox3D(
+                    corners=corners,
+                    label=label,
+                    color=color,
+                    track_id=track_id,
                 )
-            else:
-                for crop in self.cfg.shape:
-                    assert 0 < crop[0] <= 1 and 0 < crop[1] <= 1
-                self.scale_min: Tuple[float, float] = self.cfg.shape[0]
-                self.scale_max: Tuple[float, float] = self.cfg.shape[1]
-
-    def _get_crop_size(self, im_wh: torch.Tensor) -> Tuple[int, int]:
-        """Generate random absolute crop size."""
-        w, h = im_wh
-        if self.cfg.crop_type == "absolute":
-            return (
-                min(int(self.shape[0]), h),
-                min(int(self.shape[1]), w),
             )
-        if self.cfg.crop_type == "absolute_range":
-            crop_h = np.random.randint(
-                min(h, self.shape_min[0]), min(h, self.shape_max[0]) + 1
+            if track_id is not None:
+                self.trajectories[track_id].append(center)
+        self._samples.append(data_sample)
+
+    def show(self, cur_iter: int, blocking: bool = True) -> None:
+        """Shows the processed images in a interactive window.
+
+        Args:
+            cur_iter (int): Current iteration.
+            blocking (bool): If the visualizer should be blocking i.e. wait for
+                human input for each image. Defaults to True.
+        """
+        if self._run_on_batch(cur_iter):
+            image_data = [self._draw_image(d) for d in self._samples]
+            self.viewer.show_images(image_data, blocking=blocking)
+
+    def _draw_image(self, sample: DataSample) -> NDArrayUI8:
+        """Visualizes the datasample and returns is as numpy image.
+
+        Args:
+            sample (DataSample): The data sample to visualize.
+
+        Returns:
+            NDArrayUI8: A image with the visualized data sample.
+        """
+        self.canvas.create_canvas(sample.image)
+
+        global_to_cam = inverse_rigid_transform(
+            torch.from_numpy(sample.extrinsics)
+        ).numpy()
+
+        for box in sample.boxes:
+            self.canvas.draw_box_3d(
+                box.corners,
+                box.color,
+                sample.intrinsics,
+                self.width,
+                self.camera_near_clip,
             )
-            crop_w = np.random.randint(
-                min(w, self.shape_min[1]), min(w, self.shape_max[1]) + 1
+
+            selected_corner = project_point(box.corners[0], sample.intrinsics)
+            self.canvas.draw_text(
+                (selected_corner[0], selected_corner[1]),
+                box.label,
             )
-            return int(crop_h), int(crop_w)
-        if self.cfg.crop_type == "relative":
-            crop_h, crop_w = self.scale
-            return int(h * crop_h + 0.5), int(w * crop_w + 0.5)
-        # relative range
-        crop_h = (
-            np.random.rand() * (self.scale_max[0] - self.scale_min[0])
-            + self.scale_min[0]
-        )
-        crop_w = (
-            np.random.rand() * (self.scale_max[1] - self.scale_min[1])
-            + self.scale_min[1]
-        )
-        return int(h * crop_h + 0.5), int(w * crop_w + 0.5)
 
-    def _sample_crop(self, im_wh: torch.Tensor) -> torch.Tensor:
-        """Sample crop parameters according to config."""
-        crop_size = self._get_crop_size(im_wh)
-        margin_h = max(im_wh[1] - crop_size[0], 0)
-        margin_w = max(im_wh[0] - crop_size[1], 0)
-        offset_h = np.random.randint(0, margin_h + 1)
-        offset_w = np.random.randint(0, margin_w + 1)
-        crop_y1, crop_y2 = offset_h, offset_h + crop_size[0]
-        crop_x1, crop_x2 = offset_w, offset_w + crop_size[1]
-        return torch.LongTensor([crop_x1, crop_y1, crop_x2, crop_y2])
-
-    @staticmethod
-    def _get_keep_mask(
-        sample: InputSample, crop_param: torch.Tensor
-    ) -> torch.Tensor:
-        """Get mask for 2D annotations to keep."""
-        assert len(sample) == 1, "Please provide a single sample!"
-        assert len(crop_param.shape) == 1, "Please provide single crop_param"
-        if len(sample.boxes2d[0]) > 0:
-            assert len(sample.semantic_masks[0]) == 0, (
-                "Currently RandomCrop for both boxes2d and semantic_masks is "
-                "not supported"
-            )  # revisit in refactor-api
-            # will be better to compute mask intersection (if exists) instead
-            cropbox = Boxes2D(crop_param.float().unsqueeze(0))
-            overlap = bbox_intersection(sample.boxes2d[0], cropbox)
-            return overlap.squeeze(-1) > 0
-        return torch.tensor([True] * len(sample.semantic_masks[0]))
-
-    def generate_parameters(self, sample: InputSample) -> AugParams:
-        """Generate current parameters."""
-        parameters = super().generate_parameters(sample)
-        image_whs = []
-        crop_params = []
-        keep_masks = []
-        current_sample: InputSample
-        for i, current_sample in enumerate(sample):
-            im_wh = torch.tensor(current_sample.images.image_sizes[0])
-            image_whs.append(im_wh)
-            if not parameters["apply"][i]:
-                crop_params.append(torch.tensor([0, 0, *im_wh]))
-                num_objs = max(
-                    len(current_sample.boxes2d),
-                    len(current_sample.semantic_masks),
-                )
-                keep_masks.append(torch.tensor([True] * num_objs))
-                continue
+            if self.plot_trajectory:
+                assert (
+                    sample.extrinsics is not None and box.track_id is not None
+                ), "Extrinsics and track id must be set to plot trajectory."
+
+                trajectory = self.trajectories[box.track_id]
+                for center in trajectory:
+                    # Move global center to current camera frame
+                    center_cam = np.dot(global_to_cam, [*center, 1])[:3]
+
+                    if center_cam[2] > 0:
+                        projected_center = project_point(
+                            center_cam, sample.intrinsics
+                        )
+                        self.canvas.draw_circle(
+                            projected_center, box.color, self.width * 2
+                        )
 
-            crop_param = self._sample_crop(im_wh)
-            keep_mask = self._get_keep_mask(current_sample, crop_param)
-            while (
-                len(current_sample.boxes2d[0]) > 0
-                and not self.cfg.allow_empty_crop
-                and keep_mask.sum() == 0
-            ):  # pragma: no cover
-                crop_param = self._sample_crop(im_wh)
-                keep_mask = self._get_keep_mask(current_sample, crop_param)
-            crop_params.append(crop_param)
-            keep_masks.append(keep_mask)
-
-        parameters["image_wh"] = torch.stack(image_whs)
-        parameters["crop_params"] = torch.stack(crop_params)
-        parameters["keep"] = keep_masks
-        return parameters
-
-    def apply_image(self, images: Images, parameters: AugParams) -> Images:
-        """Apply augmentation to input image."""
-        all_ims: List[Images] = []
-        for i, im in enumerate(images):
-            if parameters["apply"][i]:
-                im_wh = im.image_sizes[0]
-                x1, y1, x2, y2 = parameters["crop_params"][i]
-                w, h = (x2 - x1).item(), (y2 - y1).item()
-                im.tensor = im.tensor[:, :, y1:y2, x1:x2]
-                im.image_sizes[i] = (min(im_wh[0], w), min(im_wh[1], h))
-            all_ims.append(im)
-        return Images.cat(all_ims)
+        return self.canvas.as_numpy_image()
 
-    def apply_box2d(
-        self,
-        boxes: List[Boxes2D],
-        parameters: AugParams,
-    ) -> List[Boxes2D]:
-        """Apply augmentation to input box2d."""
-        for i, box in enumerate(boxes):
-            if len(box) > 0 and parameters["apply"][i]:
-                offset = parameters["crop_params"][i, :2]
-                box.boxes[:, :4] -= torch.cat([offset, offset])
-                boxes[i] = box[parameters["keep"][i]]
-        return boxes
+    def save_to_disk(self, cur_iter: int, output_folder: str) -> None:
+        """Saves the visualization to disk.
 
-    def apply_box3d(
-        self,
-        boxes: List[Boxes3D],
-        parameters: AugParams,
-    ) -> List[Boxes3D]:
-        """Apply augmentation to input box3d."""
-        for i, box in enumerate(boxes):
-            if len(box) > 0 and parameters["apply"][i]:
-                boxes[i] = box[parameters["keep"][i]]
-        return boxes
+        Writes all processes samples to the output folder naming each image
+        <sample.image_name>.<filetype>.
 
-    def apply_intrinsics(
-        self,
-        intrinsics: Intrinsics,
-        parameters: AugParams,
-    ) -> Intrinsics:
-        """Apply augmentation to input intrinsics."""
-        x1, y1, _, _ = parameters["crop_params"].T
-        intrinsics.tensor[:, 0, 2] -= x1
-        intrinsics.tensor[:, 1, 2] -= y1
-        return intrinsics
+        Args:
+            cur_iter (int): Current iteration.
+            output_folder (str): Folder where the output should be written.
+        """
+        if self._run_on_batch(cur_iter):
+            for sample in self._samples:
+                output_dir = output_folder
+                image_name = f"{sample.image_name}.{self.file_type}"
+
+                self._draw_image(sample)
+
+                if sample.sequence_name is not None:
+                    output_dir = os.path.join(output_dir, sample.sequence_name)
+
+                if sample.camera_name is not None:
+                    output_dir = os.path.join(output_dir, sample.camera_name)
 
-    def apply_mask(
+                os.makedirs(output_dir, exist_ok=True)
+                self.canvas.save_to_disk(os.path.join(output_dir, image_name))
+
+
+class MultiCameraBBox3DVisualizer(BoundingBox3DVisualizer):
+    """Bounding box 3D visualizer class for multi-camera datasets."""
+
+    def __init__(
+        self, *args: ArgsType, cameras: Sequence[str], **kwargs: ArgsType
+    ) -> None:
+        """Creates a new Visualizer for Image and 3D Bounding Boxes.
+
+        Args:
+            cameras (Sequence[str]): Camera names.
+        """
+        super().__init__(*args, **kwargs)
+
+        self.cameras = cameras
+
+    def process(  # type: ignore # pylint: disable=arguments-differ
         self,
-        masks: List[TMasks],
-        parameters: AugParams,
-    ) -> List[TMasks]:
-        """Apply augmentation to input mask."""
-        for i, mask in enumerate(masks):
-            if len(mask) > 0 and parameters["apply"][i]:
-                x1, y1, x2, y2 = parameters["crop_params"][i]
-                mask.masks = mask.masks[:, y1:y2, x1:x2]
-                masks[i] = mask[parameters["keep"][i]]
-        return masks
-
-    def __call__(
-        self, sample: InputSample, parameters: Optional[AugParams] = None
-    ) -> Tuple[InputSample, AugParams]:
-        """Apply augmentations to input sample."""
-        # if parameters is given, still re-calculate keep / image_wh parameters
-        if parameters is not None:
-            parameters["image_wh"] = torch.stack(
-                [torch.tensor(s.images.image_sizes[0]) for s in sample]
-            )
-            parameters["keep"] = [
-                self._get_keep_mask(s, c)
-                for s, c in zip(sample, parameters["crop_params"])
-            ]
-        sample, parameters = super().__call__(sample, parameters)
-        if self.cfg.recompute_boxes2d:
-            for i in range(len(sample)):
-                assert len(sample.instance_masks[i]) == len(
-                    sample.boxes2d[i]
-                ), (
-                    "recompute_boxes2d activated but annotations do not "
-                    "contain instance masks!"
-                )
-                sample.boxes2d[i] = sample.instance_masks[i].get_boxes2d()
-        return sample, parameters
+        cur_iter: int,
+        images: list[list[ArrayLike]],
+        image_names: list[list[str]],
+        boxes3d: list[ArrayLikeFloat],
+        intrinsics: list[ArrayLikeFloat],
+        extrinsics: list[ArrayLikeFloat] | None = None,
+        scores: list[ArrayLikeFloat] | None = None,
+        class_ids: list[ArrayLikeInt] | None = None,
+        track_ids: list[ArrayLikeInt] | None = None,
+        sequence_names: list[str] | None = None,
+    ) -> None:
+        """Processes a batch of data.
+
+        Args:
+            cur_iter (int): Current iteration.
+            images (list[ArrayLike]): Images to show.
+            image_names (list[str]): Image names.
+            boxes3d (list[ArrayLikeFloat]): List of predicted bounding boxes
+                with shape [B, N, 10].
+            intrinsics (ArrayLikeFloat): Camera intrinsics with shape
+                [num_cam, B, 3, 3].
+            extrinsics (None | ArrayLikeFloat, optional): Camera extrinsics
+                with shape [num_cam, B, 4, 4]. Defaults to None.
+            scores (None | list[ArrayLikeFloat], optional): List of predicted
+                box scores each of shape [B, N]. Defaults to None.
+            class_ids (None | list[ArrayLikeInt], optional): List of predicted
+                class ids each of shape [B, N]. Defaults to None.
+            track_ids (None | list[ArrayLikeInt], optional): List of predicted
+                track ids each of shape [B, N]. Defaults to None.
+            sequence_names (None | list[str], optional): List of sequence
+                names of shape [B,]. Defaults to None.
+        """
+        if self._run_on_batch(cur_iter):
+            for idx, batch_images in enumerate(images):
+                for batch, image in enumerate(batch_images):
+                    self.process_single_image(
+                        image,
+                        image_names[idx][batch],
+                        boxes3d[batch],
+                        intrinsics[idx][batch],  # type: ignore
+                        (
+                            None
+                            if extrinsics is None
+                            else extrinsics[idx][batch]  # type: ignore
+                        ),
+                        None if scores is None else scores[batch],
+                        None if class_ids is None else class_ids[batch],
+                        None if track_ids is None else track_ids[batch],
+                        (
+                            None
+                            if sequence_names is None
+                            else sequence_names[batch]
+                        ),
+                        self.cameras[idx],
+                    )
```

### Comparing `vis4d-0.0/vis4d/engine/evaluator.py` & `vis4d-0.1/vis4d/data/datasets/nuscenes_trajectory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,270 +1,260 @@
-"""Evaluation components for tracking."""
-import copy
-import logging
-import os
-from collections import defaultdict
-from typing import Any, Dict, List, Optional
-
-import pytorch_lightning as pl
-from pytorch_lightning.callbacks import Callback
-from pytorch_lightning.utilities.types import STEP_OUTPUT
-from scalabel.common import mute
-from scalabel.eval.detect import evaluate_det
-from scalabel.eval.ins_seg import evaluate_ins_seg
-from scalabel.eval.mot import acc_single_video_mot, evaluate_track
-from scalabel.eval.mots import acc_single_video_mots, evaluate_seg_track
-from scalabel.eval.result import Result
-from scalabel.eval.sem_seg import evaluate_sem_seg
-from scalabel.label.io import group_and_sort, save
-from scalabel.label.typing import Config, Frame
-
-from ..data.datasets import BaseDatasetLoader
-from ..struct import InputSample, ModelOutput
-from .utils import all_gather_gts, all_gather_predictions
-
-mute(True)  # turn off undesired logs during eval
-logger = logging.getLogger("pytorch_lightning")
-
-
-def _detect(
-    pred: List[Frame],
-    gt: List[Frame],
-    cfg: Config,
-    ignore_unknown_cats: bool,  # pylint: disable=unused-argument
-) -> Result:
-    """Wrapper for evaluate_det function."""
-    return evaluate_det(gt, pred, cfg, nproc=1)
-
-
-def _ins_seg(
-    pred: List[Frame],
-    gt: List[Frame],
-    cfg: Config,
-    ignore_unknown_cats: bool,  # pylint: disable=unused-argument
-) -> Result:
-    """Wrapper for evaluate_ins_seg function."""
-    return evaluate_ins_seg(gt, pred, cfg, nproc=1)
-
-
-def _track(
-    pred: List[Frame], gt: List[Frame], cfg: Config, ignore_unknown_cats: bool
-) -> Result:
-    """Wrapper for evaluate_track function."""
-    return evaluate_track(
-        acc_single_video_mot,
-        group_and_sort(gt),
-        group_and_sort(pred),
-        cfg,
-        nproc=1,
-        ignore_unknown_cats=ignore_unknown_cats,
-    )
-
-
-def _seg_track(
-    pred: List[Frame], gt: List[Frame], cfg: Config, ignore_unknown_cats: bool
-) -> Result:
-    """Wrapper for evaluate_seg_track function."""
-    return evaluate_seg_track(
-        acc_single_video_mots,
-        group_and_sort(gt),
-        group_and_sort(pred),
-        cfg,
-        nproc=1,
-        ignore_unknown_cats=ignore_unknown_cats,
-    )
-
-
-def _sem_seg(
-    pred: List[Frame],
-    gt: List[Frame],
-    cfg: Config,
-    ignore_unknown_cats: bool,  # pylint: disable=unused-argument
-) -> Result:
-    """Wrapper for evaluate_sem_seg function."""
-    return evaluate_sem_seg(gt, pred, cfg, nproc=1)
-
-
-_eval_mapping = dict(
-    detect=_detect,
-    track=_track,
-    ins_seg=_ins_seg,
-    seg_track=_seg_track,
-    sem_seg=_sem_seg,
-)
+"""NuScenes trajectory dataset."""
 
+from __future__ import annotations
 
-class Vis4DEvaluatorCallback(Callback):
-    """Base class for Vis4D Evaluators.
+import json
 
-    This class will accumulate the inputs/outputs in 'process', and produce
-    evaluation results in 'evaluate'.
-    """
+import numpy as np
+from scipy.spatial.distance import cdist
+from tqdm import tqdm
 
-    def __init__(self, dataloader_idx: int, collect: str = "cpu") -> None:
-        """Init class."""
-        assert collect in ["cpu", "gpu"], f"Collect arg {collect} unknown."
-        self._predictions: Dict[str, List[Frame]] = defaultdict(list)
-        self._gts: List[Frame] = []
-        self.logger: Optional[pl.loggers.LightningLoggerBase] = None
-        self.logging_disabled = False
-        self.collect = collect
-        self.dataloader_idx = dataloader_idx
-
-    def reset(self) -> None:
-        """Preparation for a new round of evaluation."""
-        self._predictions = defaultdict(list)
-        self._gts = []
-
-    def gather(self, pl_module: pl.LightningModule) -> None:
-        """Gather accumulated data."""
-        preds = all_gather_predictions(
-            self._predictions, pl_module, self.collect
-        )
-        if preds is not None:
-            self._predictions = preds
-        gts = all_gather_gts(self._gts, pl_module, self.collect)
-        if gts is not None:
-            self._gts = gts
+from vis4d.common.imports import NUSCENES_AVAILABLE
+from vis4d.common.logging import rank_zero_info
+from vis4d.common.typing import DictStrAny, NDArrayF32
+from vis4d.data.typing import DictData
 
-    def process(
-        self, inputs: List[List[InputSample]], outputs: ModelOutput
-    ) -> None:
-        """Process the pair of inputs and outputs."""
-        raise NotImplementedError
+from .base import Dataset
+from .util import CacheMappingMixin
 
-    def evaluate(self, epoch: int) -> Dict[str, Result]:
-        """Evaluate the performance after processing all input/output pairs."""
-        raise NotImplementedError
+if NUSCENES_AVAILABLE:
+    from nuscenes import NuScenes as NuScenesDevkit
+    from nuscenes.eval.detection.utils import category_to_detection_name
+    from nuscenes.utils.data_classes import Quaternion
+    from nuscenes.utils.splits import create_splits_scenes
 
-    def setup(
-        self,
-        trainer: pl.Trainer,
-        pl_module: pl.LightningModule,
-        stage: Optional[str] = None,
-    ) -> None:
-        """Setup logging of results."""
-        self.logger = trainer.logger
 
-    def on_test_epoch_end(
-        self,
-        trainer: pl.Trainer,
-        pl_module: pl.LightningModule,
-    ) -> None:
-        """Wait for on_test_epoch_end PL hook to call 'evaluate'."""
-        self.gather(pl_module)
-        if trainer.is_global_zero:
-            self.evaluate(trainer.current_epoch)
-        self.reset()
+class NuScenesTrajectory(CacheMappingMixin, Dataset):
+    """NuScenes Trajectory dataset with given detection results.
 
-    def on_validation_epoch_end(
-        self, trainer: pl.Trainer, pl_module: pl.LightningModule
-    ) -> None:
-        """Wait for on_validation_epoch_end PL hook to call 'evaluate'."""
-        self.gather(pl_module)
-        if trainer.is_global_zero:
-            self.evaluate(trainer.current_epoch)
-        self.reset()
+    It will generate a trajectory data pair with minimum sequence length. The
+    detection results will be matched with the ground truth trajectory
+    according to the BEV distance.
+    """
 
-    def on_test_batch_end(  # type: ignore
+    def __init__(
         self,
-        trainer: pl.Trainer,
-        pl_module: pl.LightningModule,
-        outputs: Optional[STEP_OUTPUT],
-        batch: Any,
-        batch_idx: int,
-        dataloader_idx: int,
+        detector: str,
+        pure_detection: str,
+        data_root: str,
+        version: str = "v1.0-trainval",
+        split: str = "train",
+        min_seq_len: int = 10,
+        cache_as_binary: bool = False,
+        cached_file_path: str | None = None,
     ) -> None:
-        """Wait for on_test_batch_end PL hook to call 'process'."""
-        if dataloader_idx == self.dataloader_idx:
-            self.process(batch, outputs)  # type: ignore
+        """Init dataset.
+
+        Args:
+            detector (str): The detector name.
+            pure_detection (str): The path to the pure detection results. It
+                should be the same format as nuScenes submission format.
+            data_root (str): The root path of the dataset.
+            version (str, optional): The version of the dataset. Defaults to
+                "v1.0-trainval".
+            split (str, optional): The split of the dataset. Defaults to
+                "train".
+            min_seq_len (int, optional): The minimum sequence length of the
+                trajectory. Defaults to 10.
+            cache_as_binary (bool, optional): Whether to cache the dataset as
+                binary. Defaults to False.
+            cached_file_path (str | None, optional): The path to the cached
+                file. Defaults to None.
+        """
+        super().__init__()
+        self.data_root = data_root
+        self.version = version
+        self.split = split
+
+        self.detector = detector
+        self.min_seq_len = min_seq_len
+
+        self.pure_detection = pure_detection
+
+        # Load trajectories
+        self.samples, _ = self._load_mapping(
+            self._generate_data_mapping,
+            cache_as_binary=cache_as_binary,
+            cached_file_path=cached_file_path,
+        )
+        rank_zero_info(f"Generated {len(self.samples)} trajectories.")
 
-    def on_validation_batch_end(  # type: ignore
+    def __repr__(self) -> str:
+        """Concise representation of the dataset."""
+        return f"NuScenes Trajectory Data with {self.detector} detection"
+
+    def _match_gt_pred(
         self,
-        trainer: pl.Trainer,
-        pl_module: pl.LightningModule,
-        outputs: Optional[STEP_OUTPUT],
-        batch: Any,
-        batch_idx: int,
-        dataloader_idx: int,
-    ) -> None:
-        """Wait for on_validation_batch_end PL hook to call 'process'."""
-        if dataloader_idx == self.dataloader_idx:
-            self.process(batch, outputs)  # type: ignore
+        gt_world: NDArrayF32,
+        gt_class: str,
+        predictions: list[DictStrAny],
+    ) -> tuple[NDArrayF32, bool]:
+        """Match gt and pred according to BEV center distance.
+
+        If the distance is less than 2 meters, the prediction will be used
+        instead of the ground truth.
+        """
+        if len(predictions) > 0:
+            same_class_preds = [
+                pred
+                for pred in predictions
+                if pred["detection_name"] == gt_class
+            ]
+
+            if len(same_class_preds) > 0:
+                preds_center = [
+                    pred["translation"][:2] for pred in same_class_preds
+                ]
+                distance_matrix = cdist(
+                    gt_world[:, :2],
+                    np.array(preds_center).reshape(-1, 2),
+                )[0]
+
+                if distance_matrix[distance_matrix.argmin()] <= 2:
+                    match_pred = same_class_preds[distance_matrix.argmin()]
+
+                    # WLH -> HWL
+                    w, l, h = match_pred["size"]
+                    dimensions = [h, w, l]
+                    yaw = Quaternion(match_pred["rotation"]).yaw_pitch_roll[0]
+
+                    pred_world = np.array(
+                        [
+                            [
+                                *match_pred["translation"],
+                                *dimensions,
+                                yaw,
+                                match_pred["detection_score"],
+                            ]
+                        ],
+                        dtype=np.float32,
+                    )
+
+                    return pred_world, False
+
+        return gt_world, True
+
+    def _generate_data_mapping(self) -> list[dict[str, NDArrayF32]]:
+        """Generate trajectories predction and groundtruth.
+
+        Trajectories will be generated for each scene. Each trajectory consists
+        of [x, y, z, h, w, l, yaw, score] in world coordinate.
+
+        Returns:
+            list[dict[str, NDArrayF32]]: The list of trajectories.
+        """
+        data = NuScenesDevkit(
+            version=self.version, dataroot=self.data_root, verbose=False
+        )
 
-    def on_sanity_check_start(
-        self, trainer: pl.Trainer, pl_module: pl.LightningModule
-    ) -> None:
-        """Disable logging of results on sanity check."""
-        self.logging_disabled = True
+        scene_names_per_split = create_splits_scenes()
 
-    def on_sanity_check_end(
-        self, trainer: pl.Trainer, pl_module: pl.LightningModule
-    ) -> None:
-        """Enable logging of results after sanity check."""
-        self.logging_disabled = False
+        scenes = [
+            scene
+            for scene in data.scene
+            if scene["name"] in scene_names_per_split[self.split]
+        ]
 
+        instance_tokens = []
 
-class ScalabelEvaluatorCallback(Vis4DEvaluatorCallback):
-    """Evaluate model using metrics supported by Scalabel."""
+        with open(self.pure_detection, "r", encoding="utf-8") as f:
+            predictions = json.load(f)
 
-    def __init__(
-        self,
-        dataloader_idx: int,
-        dataset_loader: BaseDatasetLoader,
-        output_dir: Optional[str] = None,
-    ) -> None:
-        """Init."""
-        super().__init__(dataloader_idx, dataset_loader.cfg.collect_device)
-        self.output_dir = output_dir
-        self.ignore_unknown_cats = dataset_loader.cfg.ignore_unkown_cats
-        self.name = dataset_loader.cfg.name
-        self.dataset_config = dataset_loader.metadata_cfg
-
-        for metric in dataset_loader.cfg.eval_metrics:
-            if metric not in _eval_mapping.keys():  # pragma: no cover
-                raise KeyError(f"metric {metric} is not supported")
-        self.metrics = dataset_loader.cfg.eval_metrics
+        num_gt_boxes = 0
+        num_pred_boxes = 0
+        total_traj = []
+        for scene in tqdm(scenes):
+            local_traj: dict[int, dict[str, list[NDArrayF32]]] = {}
 
-    def process(
-        self, inputs: List[List[InputSample]], outputs: ModelOutput
-    ) -> None:
-        """Process the pair of inputs and outputs."""
-        for inp in inputs:
-            self._gts.append(copy.deepcopy(inp[0].metadata[0]))
-
-        for key, output in outputs.items():
-            for inp, out in zip(inputs, output):
-                prediction = copy.deepcopy(inp[0].metadata[0])
-                prediction.labels = out
-                self._predictions[key].append(prediction)
-
-    def evaluate(self, epoch: int) -> Dict[str, Result]:
-        """Evaluate the performance after processing all input/output pairs."""
-        results = {}
-        if not self.logging_disabled and len(self.metrics) > 0:
-            logger.info("Running evaluation on dataset %s...", self.name)
-        for key, predictions in self._predictions.items():
-            if self.output_dir:
-                os.makedirs(self.output_dir, exist_ok=True)
-                file_path = os.path.join(
-                    self.output_dir, f"{key}_predictions.json"
-                )
-                save(file_path, predictions)
-
-            if key in self.metrics:
-                results[key] = _eval_mapping[key](
-                    predictions,
-                    self._gts,
-                    self.dataset_config,
-                    self.ignore_unknown_cats,
-                )
-                if not self.logging_disabled:
-                    if self.logger is not None:
-                        log_dict = {
-                            f"{key}/{metric}": value
-                            for metric, value in results[key].summary().items()
-                        }
-                        self.logger.log_metrics(log_dict, epoch)
-                    logger.info("Showing results for %s", key)
-                    logger.info(results[key])
-        return results
+            sample_token = scene["first_sample_token"]
+            while sample_token:
+                sample = data.get("sample", sample_token)
+
+                preds = predictions["results"][sample_token]
+
+                for ann_token in sample["anns"]:
+                    ann_info = data.get("sample_annotation", ann_token)
+                    box3d_class = category_to_detection_name(
+                        ann_info["category_name"]
+                    )
+
+                    if box3d_class is None:
+                        continue
+
+                    box3d = data.get_box(ann_info["token"])
+
+                    instance_token = data.get(
+                        "sample_annotation", box3d.token
+                    )["instance_token"]
+
+                    if not instance_token in instance_tokens:
+                        instance_tokens.append(instance_token)
+                    track_id = instance_tokens.index(instance_token)
+
+                    if track_id not in local_traj:
+                        local_traj[track_id] = {"gt": [], "pred": []}
+
+                    # WLH -> HWL
+                    w, l, h = box3d.wlh
+                    dimensions = [h, w, l]
+                    yaw = box3d.orientation.yaw_pitch_roll[0]
+
+                    gt_world = np.array(
+                        [[*box3d.center, *dimensions, yaw, 1.0]],
+                        dtype=np.float32,
+                    )
+
+                    local_traj[track_id]["gt"].append(gt_world)
+
+                    matched_pred, is_gt = self._match_gt_pred(
+                        gt_world, box3d_class, preds
+                    )
+                    local_traj[track_id]["pred"].append(matched_pred)
+
+                    if is_gt:
+                        num_gt_boxes += 1
+                    else:
+                        num_pred_boxes += 1
+
+                sample_token = sample["next"]
+
+            for _, traj in local_traj.items():
+                if len(traj["gt"]) >= self.min_seq_len:
+                    trajectory = {
+                        "gt": np.concatenate(traj["gt"]),
+                        "pred": np.concatenate(traj["pred"]),
+                    }
+                    total_traj.append(trajectory)
+
+        rank_zero_info(f"Use {num_gt_boxes} gt boxes.")
+        rank_zero_info(f"Use {num_pred_boxes} pred boxes.")
+
+        return total_traj
+
+    def __len__(self) -> int:
+        """Return the length of the dataset."""
+        return len(self.samples)
+
+    def __getitem__(self, idx: int) -> DictData:
+        """Return the item at the given index.
+
+        The trajectory will be randomly cropped to the minimum sequence length.
+        """
+        trajectory = self.samples[idx]
+        data_dict: DictData = {}
+
+        traj_len = len(trajectory["gt"])
+
+        if traj_len > self.min_seq_len:
+            first_frame = np.random.randint(traj_len - self.min_seq_len)
+        else:
+            first_frame = 0
+
+        data_dict["gt_traj"] = trajectory["gt"][
+            first_frame : first_frame + self.min_seq_len
+        ]
+
+        data_dict["pred_traj"] = trajectory["pred"][
+            first_frame : first_frame + self.min_seq_len
+        ]
+
+        return data_dict
```

### Comparing `vis4d-0.0/vis4d/engine/writer.py` & `vis4d-0.1/vis4d/eval/scalabel/detect.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,135 @@
-"""Visualizer class."""
-import copy
-import os
-from collections import defaultdict
-from typing import Any, Dict, List, Sequence
-
-import pytorch_lightning as pl
-from pytorch_lightning.callbacks import Callback
-from pytorch_lightning.utilities.distributed import rank_zero_warn
-from scalabel.label.io import save
-from scalabel.label.typing import Frame, FrameGroup
-from scalabel.vis.label import LabelViewer
-
-from ..common.utils.distributed import get_rank, get_world_size
-from ..struct import InputSample, ModelOutput
-from ..vis.utils import preprocess_image
-
-
-class Vis4DWriterCallback(Callback):
-    """Vis4D prediction writer base class."""
-
-    def __init__(self, dataloader_idx: int, output_dir: str):
-        """Init."""
-        self._output_dir = output_dir
-        self._predictions: Dict[str, List[Frame]] = defaultdict(list)
-        self.dataloader_idx = dataloader_idx
-
-    def reset(self) -> None:
-        """Preparation for a new round of evaluation."""
-        self._predictions = defaultdict(list)
+"""Scalabel detection evaluator."""
 
-    def process(
-        self, inputs: List[List[InputSample]], outputs: ModelOutput
-    ) -> None:
-        """Process the pair of inputs and outputs."""
-        raise NotImplementedError
+from __future__ import annotations
 
-    def write(self) -> None:
-        """Write the aggregated output."""
-        raise NotImplementedError
+import numpy as np
 
-    def on_predict_batch_end(  # type: ignore
-        self,
-        trainer: pl.Trainer,
-        pl_module: pl.LightningModule,
-        outputs: Any,
-        batch: Any,
-        batch_idx: int,
-        dataloader_idx: int,
-    ) -> None:
-        """Hook for on_predict_batch_end."""
-        if dataloader_idx == self.dataloader_idx:
-            self.process(batch, outputs)
+from vis4d.common.array import array_to_numpy
+from vis4d.common.imports import SCALABEL_AVAILABLE
+from vis4d.common.typing import ArrayLike, MetricLogs
+
+from .base import ScalabelEvaluator
+
+if SCALABEL_AVAILABLE:
+    from scalabel.eval.detect import evaluate_det
+    from scalabel.eval.ins_seg import evaluate_ins_seg
+    from scalabel.label.transforms import mask_to_rle, xyxy_to_box2d
+    from scalabel.label.typing import Config, Frame, Label
 
-    def on_predict_epoch_end(  # type: ignore
-        self,
-        trainer: pl.Trainer,
-        pl_module: pl.LightningModule,
-        outputs: Sequence[Any],
-    ) -> None:
-        """Hook for on_predict_epoch_end."""
-        self.write()
-        self.reset()
 
+class ScalabelDetectEvaluator(ScalabelEvaluator):
+    """Scalabel 2D detection evaluation class."""
 
-class ScalabelWriterCallback(Vis4DWriterCallback):
-    """Run model and visualize & save output."""
+    METRICS_DET = "Det"
+    METRICS_INS_SEG = "InsSeg"
 
     def __init__(
         self,
-        dataloader_idx: int,
-        output_dir: str,
-        visualize: bool = True,
+        annotation_path: str,
+        config: Config | None = None,
+        mask_threshold: float = 0.0,
     ) -> None:
-        """Init."""
-        super().__init__(dataloader_idx, output_dir)
-        self._visualize = visualize
-        self.viewer = LabelViewer()
+        """Initialize the evaluator."""
+        super().__init__(annotation_path=annotation_path, config=config)
+        self.mask_threshold = mask_threshold
+
+    def __repr__(self) -> str:
+        """Concise representation of the dataset evaluator."""
+        return "Scalabel Detection Evaluator"
+
+    @property
+    def metrics(self) -> list[str]:
+        """Supported metrics."""
+        return [self.METRICS_DET, self.METRICS_INS_SEG]
 
-    def process(
-        self, inputs: List[List[InputSample]], outputs: ModelOutput
+    def process_batch(  # type: ignore # pylint: disable=arguments-differ
+        self,
+        frame_ids: list[int],
+        sample_names: list[str],
+        sequence_names: list[str],
+        pred_boxes: list[ArrayLike],
+        pred_classes: list[ArrayLike],
+        pred_scores: list[ArrayLike],
+        pred_masks: list[ArrayLike] | None = None,
     ) -> None:
-        """Process the pair of inputs and outputs."""
-        for key, output in outputs.items():
-            for inp, out in zip(inputs, output):
-                prediction = copy.deepcopy(inp[0].metadata[0])
-                prediction.labels = out
-                self._predictions[key].append(prediction)
-
-                if self._visualize and isinstance(prediction, FrameGroup):
-                    rank_zero_warn(  # pragma: no cover
-                        "Visualization not supported for multi-sensor datasets"
-                    )
-                elif self._visualize:
-                    video_name = (
-                        prediction.videoName
-                        if prediction.videoName is not None
-                        else ""
-                    )
-                    save_path = os.path.join(
-                        self._output_dir,
-                        f"{key}_visualization",
-                        video_name,
-                        prediction.name,
-                    )
-                    self.viewer.draw(
-                        preprocess_image(inp[0].images.tensor[0]), prediction
-                    )
-                    os.makedirs(os.path.dirname(save_path), exist_ok=True)
-                    self.viewer.save(save_path)
-
-    def write(self) -> None:
-        """Write the aggregated output."""
-        for key, predictions in self._predictions.items():
-            os.makedirs(os.path.join(self._output_dir, key), exist_ok=True)
-            if get_world_size() > 1:
-                filename = f"predictions_{get_rank()}.json"  # pragma: no cover
-            else:
-                filename = "predictions.json"
-            save(
-                os.path.join(self._output_dir, key, filename),
-                predictions,
+        """Process tracking results."""
+        for i, (
+            frame_id,
+            sample_name,
+            sequence_name,
+            boxes,
+            class_ids,
+            scores,
+        ) in enumerate(
+            zip(
+                frame_ids,
+                sample_names,
+                sequence_names,
+                pred_boxes,
+                pred_classes,
+                pred_scores,
+            )
+        ):
+            boxes = array_to_numpy(boxes, n_dims=None, dtype=np.float32)
+            class_ids = array_to_numpy(class_ids, n_dims=None, dtype=np.int64)
+            scores = array_to_numpy(scores, n_dims=None, dtype=np.float32)
+            if pred_masks:
+                masks = array_to_numpy(
+                    pred_masks[i], n_dims=None, dtype=np.float32
+                )
+            labels = []
+            for label_id, (box, score, class_id) in enumerate(
+                zip(boxes, scores, class_ids)
+            ):
+                box2d = xyxy_to_box2d(*box.tolist())
+                label = Label(
+                    id=str(label_id),
+                    box2d=box2d,
+                    category=(
+                        self.inverse_cat_map[int(class_id)]
+                        if self.inverse_cat_map != {}
+                        else str(class_id)
+                    ),
+                    score=float(score),
+                    rle=(
+                        mask_to_rle(
+                            (masks[label_id] > self.mask_threshold).astype(
+                                np.uint8
+                            )
+                        )
+                        if pred_masks
+                        else None
+                    ),
+                )
+                labels.append(label)
+            frame = Frame(
+                name=sample_name,
+                videoName=sequence_name,
+                frameIndex=frame_id,
+                labels=labels,
+            )
+            self.frames.append(frame)
+
+    def evaluate(self, metric: str) -> tuple[MetricLogs, str]:
+        """Evaluate the dataset."""
+        assert self.config is not None, "Scalabel config is not loaded."
+        metrics_log: MetricLogs = {}
+        short_description = ""
+
+        if metric == self.METRICS_DET:
+            results = evaluate_det(
+                self.gt_frames, self.frames, config=self.config, nproc=0
+            )
+            for metric_name, metric_value in results.summary().items():
+                metrics_log[metric_name] = metric_value
+            short_description += str(results) + "\n"
+
+        if metric == self.METRICS_INS_SEG:
+            results = evaluate_ins_seg(
+                self.gt_frames, self.frames, config=self.config, nproc=0
             )
+            for metric_name, metric_value in results.summary().items():
+                metrics_log[metric_name] = metric_value
+            short_description += str(results) + "\n"
+
+        return metrics_log, short_description
```

### Comparing `vis4d-0.0/vis4d/model/detect/d2_wrapper.py` & `vis4d-0.1/vis4d/model/detect/mask_rcnn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,218 +1,219 @@
-"""Detectron2 detector wrapper."""
-from typing import Dict, List, Optional, Tuple
+"""Mask RCNN model implementation and runtime."""
+
+from __future__ import annotations
+
+from typing import NamedTuple
 
 import torch
+from torch import nn
 
-try:
-    from detectron2.checkpoint import DetectionCheckpointer
-    from detectron2.modeling import GeneralizedRCNN
-    from detectron2.structures import Instances
-    from detectron2.utils.events import EventStorage
-
-    D2_INSTALLED = True
-except (ImportError, NameError):  # pragma: no cover
-    D2_INSTALLED = False
-
-
-from torch.nn.modules.batchnorm import _BatchNorm
-
-from vis4d.model.detect.d2_utils import (
-    D2TwoStageDetectorConfig,
-    box2d_to_proposal,
-    detections_to_box2d,
-    images_to_imagelist,
-    model_to_detectron2,
-    proposal_to_box2d,
-    segmentations_to_bitmask,
-    target_to_instance,
+from vis4d.common.ckpt import load_model_checkpoint
+from vis4d.op.base import BaseModel, ResNet
+from vis4d.op.box.box2d import apply_mask, scale_and_clip_boxes
+from vis4d.op.box.encoder import DeltaXYWHBBoxDecoder
+from vis4d.op.detect.common import DetOut
+from vis4d.op.detect.faster_rcnn import FasterRCNNHead, FRCNNOut
+from vis4d.op.detect.mask_rcnn import (
+    Det2Mask,
+    MaskOut,
+    MaskRCNNHead,
+    MaskRCNNHeadOut,
 )
-from vis4d.struct import (
-    Boxes2D,
-    InputSample,
-    InstanceMasks,
-    LossesType,
-    ModelOutput,
-)
-
-from ..base import BaseModelConfig
-from .base import BaseTwoStageDetector
+from vis4d.op.detect.rcnn import RoI2Det
+from vis4d.op.fpp.fpn import FPN
 
 
-class D2TwoStageDetector(BaseTwoStageDetector):
-    """Detectron2 two-stage detector wrapper."""
+class MaskDetectionOut(NamedTuple):
+    """Mask detection output."""
 
-    def __init__(self, cfg: BaseModelConfig):
-        """Init."""
-        assert (
-            D2_INSTALLED
-        ), "D2TwoStageDetector requires detectron2 to be installed!"
-        super().__init__(cfg)
-        self.cfg = D2TwoStageDetectorConfig(
-            **cfg.dict()
-        )  # type: D2TwoStageDetectorConfig
-        assert self.cfg.category_mapping is not None
-        self.cat_mapping = {v: k for k, v in self.cfg.category_mapping.items()}
-        self.d2_cfg = model_to_detectron2(self.cfg)
-        # pylint: disable=too-many-function-args,missing-kwoa
-        self.d2_detector = GeneralizedRCNN(self.d2_cfg)
-        # detectron2 requires an EventStorage for logging
-        self.d2_event_storage = EventStorage()
-        self.checkpointer = DetectionCheckpointer(self.d2_detector)
-        self.with_mask = self.d2_detector.roi_heads.mask_on
-        if self.d2_cfg.MODEL.WEIGHTS != "":
-            self.checkpointer.load(self.d2_cfg.MODEL.WEIGHTS)
-        if self.cfg.set_batchnorm_eval:
-            self.set_batchnorm_eval()
-
-    def set_batchnorm_eval(self) -> None:
-        """Set all batchnorm layers in backbone to eval mode."""
-        for m in self.d2_detector.modules():
-            if isinstance(m, _BatchNorm):
-                m.eval()
-
-    def preprocess_inputs(self, inputs: List[InputSample]) -> InputSample:
-        """Batch, pad (standard stride=32) and normalize the input images."""
-        batched_inputs = InputSample.cat(inputs, self.device)
-        batched_inputs.images.tensor = (
-            batched_inputs.images.tensor - self.d2_detector.pixel_mean
-        ) / self.d2_detector.pixel_std
-        return batched_inputs
+    boxes: DetOut
+    masks: MaskOut
+
+
+class MaskRCNNOut(NamedTuple):
+    """Mask RCNN output."""
+
+    boxes: FRCNNOut
+    masks: MaskRCNNHeadOut
+
+
+REV_KEYS = [
+    (r"^backbone\.", "basemodel."),
+    (r"^rpn_head.rpn_reg\.", "rpn_head.rpn_box."),
+    (r"^roi_head.bbox_head\.", "roi_head."),
+    (r"^roi_head.mask_head\.", "mask_head."),
+    (r"^convs\.", "mask_head.convs."),
+    (r"^upsample\.", "mask_head.upsample."),
+    (r"^conv_logits\.", "mask_head.conv_logits."),
+    (r"^roi_head\.", "faster_rcnn_head.roi_head."),
+    (r"^rpn_head\.", "faster_rcnn_head.rpn_head."),
+    (r"^neck.lateral_convs\.", "fpn.inner_blocks."),
+    (r"^neck.fpn_convs\.", "fpn.layer_blocks."),
+    (r"\.conv.weight", ".weight"),
+    (r"\.conv.bias", ".bias"),
+]
+
+
+class MaskRCNN(nn.Module):
+    """Mask RCNN model.
+
+    Args:
+        num_classes (int): Number of classes.
+        basemodel (BaseModel, optional): Base model network. Defaults to
+            None. If None, will use ResNet50.
+        faster_rcnn_head (FasterRCNNHead, optional): Faster RCNN head.
+            Defaults to None. if None, will use default FasterRCNNHead.
+        mask_head (MaskRCNNHead, optional): Mask RCNN head. Defaults to
+            None. if None, will use default MaskRCNNHead.
+        rcnn_box_decoder (DeltaXYWHBBoxDecoder, optional): Decoder for RCNN
+            bounding boxes. Defaults to None.
+        no_overlap (bool, optional): Whether to remove overlapping pixels
+            between masks. Defaults to False.
+        weights (None | str, optional): Weights to load for model. If set
+            to "mmdet", will load MMDetection pre-trained weights.
+            Defaults to None.
+    """
 
-    def forward_train(
+    def __init__(
         self,
-        batch_inputs: List[List[InputSample]],
-    ) -> LossesType:
-        """D2 model forward pass during training stage."""
-        assert all(
-            len(inp) == 1 for inp in batch_inputs
-        ), "No reference views allowed in D2TwoStageDetector training!"
-        raw_inputs = [inp[0] for inp in batch_inputs]
-
-        inputs = self.preprocess_inputs(raw_inputs)
-        features = self.extract_features(inputs)
-        proposals, rpn_losses = self.generate_proposals(inputs, features)
-        _, detect_losses, _ = self.generate_detections(
-            inputs, features, proposals, compute_detections=False
+        num_classes: int,
+        basemodel: BaseModel | None = None,
+        faster_rcnn_head: FasterRCNNHead | None = None,
+        mask_head: MaskRCNNHead | None = None,
+        rcnn_box_decoder: DeltaXYWHBBoxDecoder | None = None,
+        no_overlap: bool = False,
+        weights: None | str = None,
+    ) -> None:
+        """Creates an instance of the class."""
+        super().__init__()
+        self.basemodel = (
+            ResNet(resnet_name="resnet50", pretrained=True, trainable_layers=3)
+            if basemodel is None
+            else basemodel
         )
-        return {**rpn_losses, **detect_losses}
 
-    def forward_test(
-        self,
-        batch_inputs: List[List[InputSample]],
-    ) -> ModelOutput:
-        """Forward pass during testing stage."""
-        raw_inputs = [inp[0] for inp in batch_inputs]
-        inputs = self.preprocess_inputs(raw_inputs)
-        features = self.extract_features(inputs)
-        proposals, _ = self.generate_proposals(inputs, features)
-        detections, _, segmentations = self.generate_detections(
-            inputs, features, proposals
-        )
-        assert detections is not None
-        if segmentations is None:
-            segmentations = [None] * len(detections)  # type: ignore
-
-        for inp, det, segm in zip(inputs, detections, segmentations):
-            assert inp.metadata[0].size is not None
-            input_size = (
-                inp.metadata[0].size.width,
-                inp.metadata[0].size.height,
-            )
-            det.postprocess(input_size, inp.images.image_sizes[0])
-            if segm is not None:
-                segm.postprocess(input_size, inp.images.image_sizes[0], det)
+        self.fpn = FPN(self.basemodel.out_channels[2:], 256)
 
-        outputs = dict(
-            detect=[d.to_scalabel(self.cat_mapping) for d in detections]
-        )
-        if self.with_mask:
-            outputs.update(
-                ins_seg=[
-                    s.to_scalabel(self.cat_mapping) for s in segmentations
-                ]
-            )
-        return outputs
+        if faster_rcnn_head is None:
+            self.faster_rcnn_head = FasterRCNNHead(num_classes=num_classes)
+        else:
+            self.faster_rcnn_head = faster_rcnn_head
 
-    def extract_features(self, inputs: InputSample) -> Dict[str, torch.Tensor]:
-        """Detector feature extraction stage.
+        if mask_head is None:
+            self.mask_head = MaskRCNNHead(num_classes=num_classes)
+        else:
+            self.mask_head = mask_head
 
-        Return backbone output features.
-        """
-        return self.d2_detector.backbone(inputs.images.tensor)  # type: ignore
+        self.transform_outs = RoI2Det(rcnn_box_decoder)
+        self.det2mask = Det2Mask(no_overlap=no_overlap)
 
-    def generate_proposals(
-        self,
-        inputs: InputSample,
-        features: Dict[str, torch.Tensor],
-    ) -> Tuple[List[Boxes2D], LossesType]:
-        """Detector RPN stage.
+        if weights is not None:
+            if weights == "mmdet":
+                weights = (
+                    "mmdet://mask_rcnn/mask_rcnn_r50_fpn_2x_coco/"
+                    "mask_rcnn_r50_fpn_2x_coco_bbox_mAP-0.392__segm_mAP-0.354_"
+                    "20200505_003907-3e542a40.pth"
+                )
+            if weights.startswith("mmdet://") or weights.startswith(
+                "bdd100k://"
+            ):
+                load_model_checkpoint(self, weights, rev_keys=REV_KEYS)
+            else:
+                load_model_checkpoint(self, weights)
 
-        Return proposals per image and losses (empty if no targets).
+    def forward(
+        self,
+        images: torch.Tensor,
+        input_hw: list[tuple[int, int]],
+        boxes2d: None | list[torch.Tensor] = None,
+        boxes2d_classes: None | list[torch.Tensor] = None,
+        original_hw: None | list[tuple[int, int]] = None,
+    ) -> MaskRCNNOut | MaskDetectionOut:
+        """Forward pass.
+
+        Args:
+            images (torch.Tensor): Input images.
+            input_hw (list[tuple[int, int]]): Input image resolutions.
+            boxes2d (None | list[torch.Tensor], optional): Bounding box
+                labels. Required for training. Defaults to None.
+            boxes2d_classes (None | list[torch.Tensor], optional): Class
+                labels. Required for training. Defaults to None.
+            original_hw (None | list[tuple[int, int]], optional): Original
+                image resolutions (before padding and resizing). Required for
+                testing. Defaults to None.
+
+        Returns:
+            MaskRCNNOut | MaskDetectionOut: Either raw model
+                outputs (for training) or predicted outputs (for testing).
         """
-        images_d2 = images_to_imagelist(inputs.images)
-        is_training = self.d2_detector.proposal_generator.training
         if self.training:
-            targets: Optional[List[Instances]] = target_to_instance(
-                inputs.boxes2d, inputs.images.image_sizes
+            assert boxes2d is not None and boxes2d_classes is not None
+            return self.forward_train(
+                images, input_hw, boxes2d, boxes2d_classes
             )
-        else:
-            targets = None
-            self.d2_detector.proposal_generator.training = False
-
-        with self.d2_event_storage:
-            proposals, rpn_losses = self.d2_detector.proposal_generator(
-                images_d2, features, targets
-            )
-        self.d2_detector.proposal_generator.training = is_training
-        return proposal_to_box2d(proposals), rpn_losses
+        assert original_hw is not None
+        return self.forward_test(images, input_hw, original_hw)
 
-    def generate_detections(
+    def forward_train(
         self,
-        inputs: InputSample,
-        features: Dict[str, torch.Tensor],
-        proposals: Optional[List[Boxes2D]] = None,
-        compute_detections: bool = True,
-        compute_segmentations: bool = False,
-    ) -> Tuple[
-        Optional[List[Boxes2D]], LossesType, Optional[List[InstanceMasks]]
-    ]:
-        """Detector second stage (RoI Head).
+        images: torch.Tensor,
+        images_hw: list[tuple[int, int]],
+        target_boxes: list[torch.Tensor],
+        target_classes: list[torch.Tensor],
+    ) -> MaskRCNNOut:
+        """Forward training stage.
+
+        Args:
+            images (torch.Tensor): Input images.
+            images_hw (list[tuple[int, int]]): Input image resolutions.
+            target_boxes (list[torch.Tensor]): Bounding box labels. Required
+                for training. Defaults to None.
+            target_classes (list[torch.Tensor]): Class labels. Required for
+                training. Defaults to None.
 
-        Return losses (empty if no targets) and optionally detections.
+        Returns:
+            MaskRCNNOut: Raw model outputs.
         """
-        assert (
-            proposals is not None
-        ), "Generating detections with D2TwoStageDetector requires proposals."
-        images_d2 = images_to_imagelist(inputs.images)
-        proposals = box2d_to_proposal(proposals, inputs.images.image_sizes)
-        is_training = self.d2_detector.roi_heads.training
-        if self.training:
-            targets: Optional[List[Instances]] = target_to_instance(
-                inputs.boxes2d,
-                inputs.images.image_sizes,
-                inputs.instance_masks,
-            )
-        else:
-            targets = None
-            self.d2_detector.roi_heads.training = False
+        features = self.fpn(self.basemodel(images))
+        outputs = self.faster_rcnn_head(
+            features, images_hw, target_boxes, target_classes
+        )
+        assert outputs.sampled_proposals is not None
+        assert outputs.sampled_targets is not None
+        pos_proposals = apply_mask(
+            [torch.eq(label, 1) for label in outputs.sampled_targets.labels],
+            outputs.sampled_proposals.boxes,
+        )[0]
+        mask_outs = self.mask_head(features, pos_proposals)
+        return MaskRCNNOut(outputs, mask_outs)
 
-        with self.d2_event_storage:
-            detections, detect_losses = self.d2_detector.roi_heads(
-                images_d2,
-                features,
-                proposals,
-                targets,
-            )
-        self.d2_detector.roi_heads.training = is_training
-        segmentations = None
-        if not self.d2_detector.training:
-            if self.with_mask:
-                segmentations = segmentations_to_bitmask(detections)
-            detections = detections_to_box2d(detections)
-        elif compute_detections:  # pragma: no cover
-            if compute_segmentations:
-                segmentations = segmentations_to_bitmask(detections)
-            detections = proposal_to_box2d(detections)
-        else:
-            detections = None
-        return detections, detect_losses, segmentations
+    def forward_test(
+        self,
+        images: torch.Tensor,
+        images_hw: list[tuple[int, int]],
+        original_hw: list[tuple[int, int]],
+    ) -> MaskDetectionOut:
+        """Forward testing stage.
+
+        Args:
+            images (torch.Tensor): Input images.
+            images_hw (list[tuple[int, int]]): Input image resolutions.
+            original_hw (list[tuple[int, int]]): Original image resolutions
+                (before padding and resizing).
+
+        Returns:
+            MaskDetectionOut: Predicted outputs.
+        """
+        features = self.fpn(self.basemodel(images))
+        outs = self.faster_rcnn_head(features, images_hw)
+        boxes, scores, class_ids = self.transform_outs(
+            *outs.roi, outs.proposals.boxes, images_hw
+        )
+        mask_outs = self.mask_head(features, boxes)
+        for i, boxs in enumerate(boxes):
+            boxes[i] = scale_and_clip_boxes(boxs, original_hw[i], images_hw[i])
+        mask_preds = [m.sigmoid() for m in mask_outs.mask_pred]
+        masks = self.det2mask(
+            mask_preds, boxes, scores, class_ids, original_hw
+        )
+        return MaskDetectionOut(DetOut(boxes, scores, class_ids), masks)
```

### Comparing `vis4d-0.0/vis4d/model/detect/mmdet_utils.py` & `vis4d-0.1/vis4d/engine/experiment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,264 +1,257 @@
-"""Utilities for mmdet wrapper."""
+"""Implementation of a single experiment.
 
-import os
-from typing import Dict, List, Optional, Sequence, Tuple, Union
+Helper functions to execute a single experiment.
 
-import numpy as np
-import requests
-import torch
+This will be called for each experiment configuration.
+"""
 
-try:
-    from mmcv import Config as MMConfig
+from __future__ import annotations
 
-    MMCV_INSTALLED = True
-except (ImportError, NameError):  # pragma: no cover
-    MMCV_INSTALLED = False
-
-try:
-    from mmdet.core.mask import BitmapMasks
-
-    MMDET_INSTALLED = True
-except (ImportError, NameError):  # pragma: no cover
-    MMDET_INSTALLED = False
-
-from vis4d.struct import (
-    Boxes2D,
-    Images,
-    InputSample,
-    InstanceMasks,
-    LossesType,
-    NDArrayF64,
-    NDArrayUI8,
+import logging
+import os
+
+import torch
+from torch.distributed import destroy_process_group, init_process_group
+from torch.nn.parallel import DistributedDataParallel as DDP
+from torch.utils.collect_env import get_pretty_env_info
+
+from vis4d.common.ckpt import load_model_checkpoint
+from vis4d.common.distributed import (
+    broadcast,
+    get_local_rank,
+    get_rank,
+    get_world_size,
 )
+from vis4d.common.logging import (
+    _info,
+    dump_config,
+    rank_zero_info,
+    rank_zero_warn,
+    setup_logger,
+)
+from vis4d.common.slurm import init_dist_slurm
+from vis4d.common.util import init_random_seed, set_random_seed, set_tf32
+from vis4d.config import instantiate_classes
+from vis4d.config.typing import ExperimentConfig
+
+from .optim import set_up_optimizers
+from .parser import pprints_config
+from .trainer import Trainer
+
+
+def ddp_setup(
+    torch_distributed_backend: str = "nccl", slurm: bool = False
+) -> None:
+    """Setup DDP environment and init processes.
+
+    Args:
+        torch_distributed_backend (str): Backend to use (`nccl` or `gloo`)
+        slurm (bool): If set, setup slurm running jobs.
+    """
+    if slurm:
+        init_dist_slurm()
+
+    global_rank = get_rank()
+    world_size = get_world_size()
+    _info(
+        f"Initializing distributed: "
+        f"GLOBAL_RANK: {global_rank}, MEMBER: {global_rank + 1}/{world_size}"
+    )
+    init_process_group(
+        torch_distributed_backend, rank=global_rank, world_size=world_size
+    )
 
-from ..base import BaseModelConfig
+    # On rank=0 let everyone know training is starting
+    rank_zero_info(
+        f"{'-' * 100}\n"
+        f"distributed_backend={torch_distributed_backend}\n"
+        f"All distributed processes registered. "
+        f"Starting with {world_size} processes\n"
+        f"{'-' * 100}\n"
+    )
 
-MMDetMetaData = Dict[str, Union[Tuple[int, int, int], bool, NDArrayF64]]
-MMDetResult = List[torch.Tensor]
-MMSegmResult = List[List[NDArrayUI8]]
-MMResults = Union[List[MMDetResult], List[Tuple[MMDetResult, MMSegmResult]]]
-
-
-class MMTwoStageDetectorConfig(BaseModelConfig):
-    """Config for mmdetection two stage models."""
-
-    model_base: str
-    model_kwargs: Optional[Dict[str, Union[bool, float, str, List[float]]]]
-    pixel_mean: Tuple[float, float, float]
-    pixel_std: Tuple[float, float, float]
-    backbone_output_names: Optional[List[str]]
-    weights: Optional[str]
-
-
-def get_img_metas(images: Images) -> List[MMDetMetaData]:
-    """Create image metadata in mmdetection format."""
-    img_metas = []
-    _, c, padh, padw = images.tensor.shape  # type: Tuple[int, int, int, int]
-    for i in range(len(images)):
-        meta: MMDetMetaData = {}
-        w, h = images.image_sizes[i]
-        meta["img_shape"] = meta["ori_shape"] = (h, w, c)
-        meta["scale_factor"] = np.ones(4, dtype=np.float64)
-        meta["flip"] = False
-        meta["pad_shape"] = (padh, padw, c)
-        img_metas.append(meta)
-
-    return img_metas
-
-
-def proposals_from_mmdet(proposals: List[torch.Tensor]) -> List[Boxes2D]:
-    """Convert mmdetection proposals to Vis4D format."""
-    proposals_boxes2d = []
-    for proposal in proposals:
-        proposals_boxes2d.append(Boxes2D(proposal))
-    return proposals_boxes2d
-
-
-def proposals_to_mmdet(proposals: List[Boxes2D]) -> List[torch.Tensor]:
-    """Convert Vis4D format proposals to mmdetection."""
-    proposal_tensors = []
-    for proposal in proposals:
-        proposal_tensors.append(proposal.boxes)
-    return proposal_tensors
-
-
-def detections_from_mmdet(
-    bboxes: List[torch.Tensor], labels: List[torch.Tensor]
-) -> List[Boxes2D]:
-    """Convert mmdetection detections to Vis4D format."""
-    detections_boxes2d = []
-    for bbox, label in zip(bboxes, labels):
-        if not label.device == bbox.device:
-            label = label.to(bbox.device)  # pragma: no cover
-        detections_boxes2d.append(Boxes2D(bbox, label))
-    return detections_boxes2d
-
-
-def segmentations_from_mmdet(
-    masks: List[MMSegmResult], boxes: List[Boxes2D], device: torch.device
-) -> List[InstanceMasks]:
-    """Convert mmdetection segmentations to Vis4D format."""
-    segmentations_masks = []
-    for mask_res, box_res in zip(masks, boxes):
-        mask = segmentation_from_mmdet_results(mask_res, box_res, device)
-        segmentations_masks.append(mask)
-    return segmentations_masks
-
-
-def detection_from_mmdet_results(
-    detection: MMDetResult, device: torch.device
-) -> Boxes2D:
-    """Convert bbox_result to Vis4D format."""
-    if len(detection) == 0:  # pragma: no cover
-        return Boxes2D(torch.empty(0, 5), torch.empty(0), torch.empty(0))
-    bboxes = torch.from_numpy(np.vstack(detection)).to(device)  # Nx5
-    labels = [
-        torch.full((bbox.shape[0],), i, dtype=torch.int32, device=device)
-        for i, bbox in enumerate(detection)
-    ]
-    labels = torch.cat(labels)
-    return Boxes2D(bboxes, labels)
-
-
-def segmentation_from_mmdet_results(
-    segmentation: MMSegmResult, boxes: Boxes2D, device: torch.device
-) -> InstanceMasks:
-    """Convert segm_result to Vis4D format."""
-    segms = [
-        np.stack(segm) if len(segm) != 0 else np.empty_like(segm)
-        for segm in segmentation
-    ]
-    if len(segms) == 0 or sum([len(segm) for segm in segmentation]) == 0:
-        return InstanceMasks(torch.empty(0, 1, 1))  # pragma: no cover
-    masks_list, labels_list = [], []  # type: ignore
-    for class_id in boxes.class_ids:
-        masks_list.append(
-            torch.from_numpy(segms[class_id][labels_list.count(class_id)])
-            .type(torch.uint8)
-            .to(device)
-        )
-        labels_list.append(class_id)
-    masks = torch.stack(masks_list)
-    labels = torch.stack(labels_list)
-    scores = boxes.score
-    return InstanceMasks(masks, labels, score=scores)
+    local_rank = get_local_rank()
+    all_gpu_ids = ",".join(str(x) for x in range(torch.cuda.device_count()))
+    devices = os.getenv("CUDA_VISIBLE_DEVICES", all_gpu_ids)
+
+    torch.cuda.set_device(local_rank)
+
+    _info(f"LOCAL_RANK: {local_rank} - CUDA_VISIBLE_DEVICES: [{devices}]")
+
+
+def run_experiment(
+    config: ExperimentConfig,
+    mode: str,
+    num_gpus: int = 0,
+    show_config: bool = False,
+    use_slurm: bool = False,
+    ckpt_path: str | None = None,
+    resume: bool = False,
+) -> None:
+    """Entry point for running a single experiment.
+
+    Args:
+        config (ExperimentConfig): Configuration dictionary.
+        mode (str): Mode to run the experiment in. Either `fit` or `test`.
+        num_gpus (int): Number of GPUs to use.
+        show_config (bool): If set, prints the configuration.
+        use_slurm (bool): If set, setup slurm running jobs. This will set the
+            required environment variables for slurm.
+        ckpt_path (str | None): Path to a checkpoint to load.
+        resume (bool): If set, resume training from the checkpoint.
+
+    Raises:
+        ValueError: If `mode` is not `fit` or `test`.
+    """
+    # Setup logging
+    logger_vis4d = logging.getLogger("vis4d")
+    log_dir = os.path.join(config.output_dir, f"log_{config.timestamp}.txt")
+    setup_logger(logger_vis4d, log_dir)
+
+    # Dump config
+    config_file = os.path.join(
+        config.output_dir, f"config_{config.timestamp}.yaml"
+    )
+    dump_config(config, config_file)
 
+    rank_zero_info("Environment info: %s", get_pretty_env_info())
 
-def results_from_mmdet(
-    results: MMResults, device: torch.device, with_mask: bool
-) -> Tuple[List[Boxes2D], List[InstanceMasks]]:
-    """Convert mmdetection bbox_results and segm_results to Vis4D format."""
-    results_boxes2d, results_masks = [], []
-    for result in results:
-        if with_mask:
-            detection, segmentation = result
-        else:
-            detection = result
-        box2d = detection_from_mmdet_results(detection, device)
-        results_boxes2d.append(box2d)
-        if with_mask:
-            bitmask = segmentation_from_mmdet_results(
-                segmentation, box2d, device
+    # PyTorch Setting
+    set_tf32(config.use_tf32, config.tf32_matmul_precision)
+    torch.hub.set_dir(f"{config.work_dir}/.cache/torch/hub")
+    torch.backends.cudnn.benchmark = config.benchmark
+
+    if show_config:
+        rank_zero_info(pprints_config(config))
+
+    # Instantiate classes
+    model = instantiate_classes(config.model)
+
+    if config.get("sync_batchnorm", False):
+        if num_gpus > 1:
+            rank_zero_info(
+                "SyncBN enabled, converting BatchNorm layers to"
+                " SyncBatchNorm layers."
             )
-            results_masks.append(bitmask)
+            model = torch.nn.SyncBatchNorm.convert_sync_batchnorm(model)
         else:
-            results_masks.append(None)  # type: ignore
-    return results_boxes2d, results_masks
+            rank_zero_warn(
+                "use_sync_bn is True, but not in a distributed setting."
+                " BatchNorm layers are not converted."
+            )
 
+    # Callbacks
+    callbacks = [instantiate_classes(cb) for cb in config.callbacks]
 
-def masks_to_mmdet_masks(masks: Sequence[InstanceMasks]) -> BitmapMasks:
-    """Convert Vis4D Masks to mmdetection BitmapMasks."""
-    return [BitmapMasks(m.to_ndarray(), m.height, m.width) for m in masks]
-
-
-def targets_to_mmdet(
-    targets: InputSample,
-) -> Tuple[
-    List[torch.Tensor], List[torch.Tensor], Optional[Sequence[InstanceMasks]]
-]:
-    """Convert Vis4D targets to mmdetection compatible format."""
-    gt_bboxes = [t.boxes for t in targets.boxes2d]
-    gt_labels = [t.class_ids for t in targets.boxes2d]
-    gt_masks = (
-        masks_to_mmdet_masks(targets.instance_masks)
-        if len(targets.instance_masks) > 0
-        else None
-    )
-    return gt_bboxes, gt_labels, gt_masks
+    # Setup DDP & seed
+    seed = init_random_seed() if config.seed == -1 else config.seed
 
+    if num_gpus > 1:
+        ddp_setup(slurm=use_slurm)
 
-def load_config_from_mmdet(url: str) -> str:
-    """Get config from mmdetection GitHub repository."""
-    full_url = (
-        "https://raw.githubusercontent.com/"
-        "syscv/mmdetection/master/configs/" + url
-    )
-    response = requests.get(full_url)
-    assert (
-        response.status_code == 200
-    ), f"Request to {full_url} failed with code {response.status_code}!"
-    return response.text
-
-
-def get_mmdet_config(config: MMTwoStageDetectorConfig) -> MMConfig:
-    """Convert a Detector config to a mmdet readable config."""
-    if os.path.exists(config.model_base):
-        cfg = MMConfig.fromfile(config.model_base)
-        if cfg.get("model"):
-            cfg = cfg["model"]
-    elif config.model_base.startswith("mmdet://"):
-        ex = os.path.splitext(config.model_base)[1]
-        cfg = MMConfig.fromstring(
-            load_config_from_mmdet(config.model_base.split("mmdet://")[-1]), ex
-        ).model
-    else:
-        raise FileNotFoundError(
-            f"MMDetection config not found: {config.model_base}"
+        # broadcast seed to all processes
+        seed = broadcast(seed)
+
+    # Setup Dataloaders & seed
+    if mode == "fit":
+        set_random_seed(seed)
+        _info(f"[rank {get_rank()}] Global seed set to {seed}")
+        train_dataloader = instantiate_classes(
+            config.data.train_dataloader, seed=seed
+        )
+        train_data_connector = instantiate_classes(config.train_data_connector)
+        optimizers, lr_schedulers = set_up_optimizers(
+            config.optimizers, [model], len(train_dataloader)
         )
+        loss = instantiate_classes(config.loss)
+    else:
+        train_dataloader = None
+        train_data_connector = None
 
-    # convert detect attributes
-    assert config.category_mapping is not None
-    if "bbox_head" in cfg:  # pragma: no cover
-        cfg["bbox_head"]["num_classes"] = len(config.category_mapping)
-    if "roi_head" in cfg:
-        cfg["roi_head"]["bbox_head"]["num_classes"] = len(
-            config.category_mapping
+    if config.data.test_dataloader is not None:
+        test_dataloader = instantiate_classes(config.data.test_dataloader)
+    else:
+        test_dataloader = None
+
+    if config.test_data_connector is not None:
+        test_data_connector = instantiate_classes(config.test_data_connector)
+    else:
+        test_data_connector = None
+
+    # Setup Model
+    if num_gpus == 0:
+        device = torch.device("cpu")
+    else:
+        rank = get_local_rank()
+        device = torch.device(f"cuda:{rank}")
+
+    model.to(device)
+
+    if num_gpus > 1:
+        model = DDP(  # pylint: disable=redefined-variable-type
+            model, device_ids=[rank]
         )
-        if "mask_head" in cfg["roi_head"]:
-            cfg["roi_head"]["mask_head"]["num_classes"] = len(
-                config.category_mapping
+
+    # Setup Callbacks
+    for cb in callbacks:
+        cb.setup()
+
+    # Resume training
+    if resume:
+        if ckpt_path is None:
+            ckpt_path = os.path.join(
+                config.output_dir, "checkpoints/last.ckpt"
             )
+        rank_zero_info(
+            f"Restoring states from the checkpoint path at {ckpt_path}"
+        )
+        ckpt = torch.load(ckpt_path, map_location="cpu")
+
+        epoch = ckpt["epoch"] + 1
+        global_step = ckpt["global_step"]
+
+        for i, optimizer in enumerate(optimizers):
+            optimizer.load_state_dict(ckpt["optimizers"][i])
+
+        for i, lr_scheduler in enumerate(lr_schedulers):
+            lr_scheduler.load_state_dict(ckpt["lr_schedulers"][i])
+    else:
+        epoch = 0
+        global_step = 0
+
+    if ckpt_path is not None:
+        load_model_checkpoint(
+            model,
+            ckpt_path,
+            rev_keys=[(r"^model\.", ""), (r"^module\.", "")],
+        )
+
+    trainer = Trainer(
+        device=device,
+        output_dir=config.output_dir,
+        train_dataloader=train_dataloader,
+        test_dataloader=test_dataloader,
+        train_data_connector=train_data_connector,
+        test_data_connector=test_data_connector,
+        callbacks=callbacks,
+        num_epochs=config.params.get("num_epochs", -1),
+        num_steps=config.params.get("num_steps", -1),
+        epoch=epoch,
+        global_step=global_step,
+        check_val_every_n_epoch=config.get("check_val_every_n_epoch", 1),
+        val_check_interval=config.get("val_check_interval", None),
+        log_every_n_steps=config.get("log_every_n_steps", 50),
+    )
+
+    if resume:
+        rank_zero_info(
+            f"Restored all states from the checkpoint at {ckpt_path}"
+        )
 
-    # add keyword args in config
-    if config.model_kwargs:
-        for k, v in config.model_kwargs.items():
-            attr = cfg
-            partial_keys = k.split(".")
-            partial_keys, last_key = partial_keys[:-1], partial_keys[-1]
-            for part_k in partial_keys:
-                attr = attr.get(part_k)
-            if attr.get(last_key) is not None:
-                attr[last_key] = type(attr.get(last_key))(v)
-            else:
-                attr[last_key] = v
-
-    return cfg
-
-
-def _parse_losses(
-    losses: Dict[str, torch.Tensor], prefix: Optional[str] = None
-) -> LossesType:
-    """Parse losses to a scalar tensor."""
-    log_vars = {}
-    for name, value in losses.items():
-        if "loss" in name:
-            if prefix is not None:  # pragma: no cover
-                name = f"{prefix}.{name}"
-            if isinstance(value, torch.Tensor):
-                log_vars[name] = value.mean()
-            elif isinstance(value, list):
-                log_vars[name] = sum(_loss.mean() for _loss in value)
-            else:
-                raise ValueError(f"{name} is not a tensor or list of tensors")
+    if mode == "fit":
+        trainer.fit(model, optimizers, lr_schedulers, loss)
+    elif mode == "test":
+        trainer.test(model)
 
-    return log_vars
+    if num_gpus > 1:
+        destroy_process_group()
```

### Comparing `vis4d-0.0/vis4d/model/detect/roi_head/qd_3dt_bbox3d_head.py` & `vis4d-0.1/vis4d/op/base/pointnet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,416 +1,408 @@
-"""3D Box Head definition for QD-3DT."""
-from typing import Dict, List, Optional, Sequence, Tuple
+"""Operations for PointNet.
+
+Code taken from
+https://github.com/timothylimyl/PointNet-Pytorch/blob/master/pointnet/model.py
+and modified to allow for modular configuration.
+"""
+
+from __future__ import annotations
+
+from collections.abc import Callable, Iterable
+from typing import NamedTuple
 
-import numpy as np
 import torch
 from torch import nn
 
-from vis4d.common.bbox.coders import BaseBoxCoderConfig, build_box3d_coder
-from vis4d.common.bbox.matchers import MatcherConfig, build_matcher
-from vis4d.common.bbox.poolers import RoIPoolerConfig, build_roi_pooler
-from vis4d.common.bbox.samplers import (
-    SamplerConfig,
-    SamplingResult,
-    build_sampler,
-    match_and_sample_proposals,
-)
-from vis4d.common.geometry.rotation import generate_rotation_output
-from vis4d.common.layers import add_conv_branch
-from vis4d.model.losses import LossConfig, build_loss
-from vis4d.struct import (
-    Boxes2D,
-    Boxes3D,
-    InputSample,
-    Intrinsics,
-    LabelInstance,
-    LossesType,
-)
-
-from .base import BaseRoIHead, BaseRoIHeadConfig
-
-
-class QD3DTBBox3DHeadConfig(BaseRoIHeadConfig):
-    """QD-3DT 3D Bounding Box Head config."""
-
-    num_shared_convs: int = 2
-    num_shared_fcs: int = 0
-    num_dep_convs: int = 4
-    num_dep_fcs: int = 0
-    num_dim_convs: int = 4
-    num_dim_fcs: int = 0
-    num_rot_convs: int = 4
-    num_rot_fcs: int = 0
-    num_2dc_convs: int = 4
-    num_2dc_fcs: int = 0
-    in_channels: int = 256
-    conv_out_dim: int = 256
-    fc_out_dim: int = 1024
-    roi_feat_size: int = 7
-    num_classes: int
-    conv_has_bias: bool = False
-    norm: Optional[str] = None
-    num_groups: int = 32
-    num_rotation_bins: int = 2
-
-    loss: LossConfig
-    box3d_coder: BaseBoxCoderConfig
-
-    proposal_append_gt: bool
-    in_features: List[str] = ["p2", "p3", "p4", "p5"]
-    proposal_pooler: RoIPoolerConfig
-    proposal_sampler: SamplerConfig
-    proposal_matcher: MatcherConfig
+from vis4d.common.typing import ArgsType
 
 
-class QD3DTBBox3DHead(BaseRoIHead):
-    """QD-3DT 3D Bounding Box Head."""
+class PointNetEncoderOut(NamedTuple):
+    """Output of the PointNetEncoder.
 
-    def __init__(self, cfg: BaseRoIHeadConfig) -> None:
-        """Init."""
-        super().__init__()
-        self.cfg = QD3DTBBox3DHeadConfig(**cfg.dict())
+    features: Global features shape [N, feature_dim]
+    pointwise Features: Pointwise features shape [N, last_mlp_dim, n_pts]
+    transformations: list with all transformation matrixes that were used.
+                     Shape [N, d, d]
+    """
 
-        self.cls_out_channels = self.cfg.num_classes
+    features: torch.Tensor
+    pointwise_features: torch.Tensor  #
+    transformations: list[  # list with all transformation matrices [[B, d, d]]
+        torch.Tensor
+    ]
 
-        self.sampler = build_sampler(self.cfg.proposal_sampler)
-        self.matcher = build_matcher(self.cfg.proposal_matcher)
-        self.roi_pooler = build_roi_pooler(self.cfg.proposal_pooler)
-
-        self.bbox_coder = build_box3d_coder(self.cfg.box3d_coder)
-
-        # add shared convs and fcs
-        (
-            self.shared_convs,
-            self.shared_fcs,
-            self.shared_out_channels,
-        ) = self._add_conv_fc_branch(
-            self.cfg.num_shared_convs,
-            self.cfg.num_shared_fcs,
-            self.cfg.in_channels,
-            True,
-        )
-
-        # add depth specific branch
-        (
-            self.dep_convs,
-            self.dep_fcs,
-            self.dep_last_dim,
-        ) = self._add_conv_fc_branch(
-            self.cfg.num_dep_convs,
-            self.cfg.num_dep_fcs,
-            self.shared_out_channels,
-        )
-
-        # add dim specific branch
-        (
-            self.dim_convs,
-            self.dim_fcs,
-            self.dim_last_dim,
-        ) = self._add_conv_fc_branch(
-            self.cfg.num_dim_convs,
-            self.cfg.num_dim_fcs,
-            self.shared_out_channels,
-        )
-
-        # add rot specific branch
-        (
-            self.rot_convs,
-            self.rot_fcs,
-            self.rot_last_dim,
-        ) = self._add_conv_fc_branch(
-            self.cfg.num_rot_convs,
-            self.cfg.num_rot_fcs,
-            self.shared_out_channels,
-        )
-
-        # add 2dc specific branch
-        (
-            self.cen_2d_convs,
-            self.cen_2d_fcs,
-            self.cen_2d_last_dim,
-        ) = self._add_conv_fc_branch(
-            self.cfg.num_2dc_convs,
-            self.cfg.num_2dc_fcs,
-            self.shared_out_channels,
-        )
-
-        if self.cfg.num_shared_fcs == 0:
-            if self.cfg.num_dep_fcs == 0:
-                self.dep_last_dim *= (
-                    self.cfg.roi_feat_size * self.cfg.roi_feat_size
-                )
-            if self.cfg.num_dim_fcs == 0:
-                self.dim_last_dim *= (
-                    self.cfg.roi_feat_size * self.cfg.roi_feat_size
-                )
-            if self.cfg.num_rot_fcs == 0:
-                self.rot_last_dim *= (
-                    self.cfg.roi_feat_size * self.cfg.roi_feat_size
-                )
-            if self.cfg.num_2dc_fcs == 0:
-                self.cen_2d_last_dim *= (
-                    self.cfg.roi_feat_size * self.cfg.roi_feat_size
-                )
 
-        self.relu = nn.ReLU(inplace=True)
-        # reconstruct fc_cls and fc_reg since input channels are changed
-        out_dim_dep = self.cls_out_channels
-        self.fc_dep = nn.Linear(self.dep_last_dim, out_dim_dep)
+class PointNetSemanticsLoss(NamedTuple):
+    """Losses for the pointnet semantic segmentation network."""
 
-        self.fc_dep_uncer = nn.Linear(self.dep_last_dim, out_dim_dep)
+    semantic_loss: torch.Tensor
+    regularization_loss: torch.Tensor
 
-        out_dim_size = 3 * self.cls_out_channels
-        self.fc_dim = nn.Linear(self.dim_last_dim, out_dim_size)
 
-        out_rot_size = 3 * self.cfg.num_rotation_bins * self.cls_out_channels
-        self.fc_rot = nn.Linear(self.rot_last_dim, out_rot_size)
+class PointNetSemanticsOut(NamedTuple):
+    """Output of the PointNet Segmentation network."""
 
-        out_2dc_size = 2 * self.cls_out_channels
-        self.fc_2dc = nn.Linear(self.cen_2d_last_dim, out_2dc_size)
+    class_logits: torch.Tensor  # B, n_classes, n_pts
+    transformations: list[  # list with all transformation matrices [[B, d, d]]
+        torch.Tensor
+    ]
 
-        self._init_weights()
 
-        # losses
-        self.loss = build_loss(self.cfg.loss)
-        assert (
-            self.bbox_coder.cfg.num_rotation_bins  # type: ignore
-            == self.cfg.num_rotation_bins
-            == self.loss.cfg.num_rotation_bins
-        ), (
-            "num_rotation_bins must be consistent between head, "
-            "loss and box coder."
-        )
-
-    def _init_weights(self) -> None:
-        """Init weights of modules in head."""
-        module_lists = [self.shared_fcs]
-        module_lists += [self.fc_dep_uncer]
-        module_lists += [self.fc_dep, self.dep_fcs]
-        module_lists += [self.fc_dim, self.dim_fcs]
-        module_lists += [self.fc_rot, self.rot_fcs]
-        module_lists += [self.fc_2dc, self.cen_2d_fcs]
-
-        for module_list in module_lists:
-            for m in module_list.modules():
-                if isinstance(m, nn.Linear):
-                    nn.init.xavier_uniform_(m.weight)
-                    nn.init.constant_(m.bias, 0)
+class LinearTransform(nn.Module):
+    """Module that learns a linear transformation for a input pointcloud.
+
+    Code taken from
+    https://github.com/timothylimyl/PointNet-Pytorch/blob/master/pointnet/model.py
+    and modified to allow for modular configuration.
 
-    def _add_conv_fc_branch(
+    See T-Net in Pointnet publication (https://arxiv.org/pdf/1612.00593.pdf)
+    for more information
+    """
+
+    def __init__(
         self,
-        num_branch_convs: int,
-        num_branch_fcs: int,
-        in_channels: int,
-        is_shared: bool = False,
-    ) -> Tuple[torch.nn.ModuleList, torch.nn.ModuleList, int]:
-        """Init modules of head."""
-        last_layer_dim = in_channels
-        # add branch specific conv layers
-        convs, last_layer_dim = add_conv_branch(
-            num_branch_convs,
-            in_channels,
-            self.cfg.conv_out_dim,
-            self.cfg.conv_has_bias,
-            self.cfg.norm,
-            self.cfg.num_groups,
-        )
-
-        fcs = nn.ModuleList()
-        if num_branch_fcs > 0:
-            if is_shared or self.cfg.num_shared_fcs == 0:
-                last_layer_dim *= np.prod(self.cfg.proposal_pooler.resolution)
-            for i in range(num_branch_fcs):
-                fc_in_dim = last_layer_dim if i == 0 else self.cfg.fc_out_dim
-                fcs.append(
-                    nn.Sequential(
-                        nn.Linear(fc_in_dim, self.cfg.fc_out_dim),
-                        nn.ReLU(inplace=True),
-                    )
+        in_dimension: int = 3,
+        upsampling_dims: Iterable[int] = (64, 128, 1024),
+        downsampling_dims: Iterable[int] = (1024, 512, 256),
+        norm_cls: str | None = "BatchNorm1d",
+        activation_cls: str = "ReLU",
+    ) -> None:
+        """Creates a new LinearTransform.
+
+        This learns a transformation matrix from data.
+
+        Args:
+            in_dimension (int): input dimension
+            upsampling_dims (Iterable[int]): list of intermediate feature
+                                             shapes for upsampling
+            downsampling_dims (Iterable[int]): list of intermediate feature
+                                               shapes for downsampling.
+                                               Make sure this matches with the
+                                               last upsampling_dims
+            norm_cls (Optional(str)): class for norm (nn.'norm_cls') or None
+            activation_cls (str): class for activation (nn.'activation_cls')
+        """
+        super().__init__()
+        self.upsampling_dims = list(upsampling_dims)
+        self.downsampling_dims = list(downsampling_dims)
+
+        assert (
+            len(self.upsampling_dims) != 0 and len(self.downsampling_dims) != 0
+        )
+        assert self.upsampling_dims[-1] == self.downsampling_dims[0]
+
+        self.in_dimension_ = in_dimension
+        self.identity: torch.Tensor
+        self.register_buffer(
+            "identity", torch.eye(in_dimension).reshape(1, in_dimension**2)
+        )
+
+        # Create activation
+        self.activation_ = getattr(nn, activation_cls)()
+
+        # Create norms
+        norm_fn: Callable[[int], nn.Module] = (
+            getattr(nn, norm_cls) if norm_cls is not None else None
+        )
+
+        if norm_fn is not None:
+            self.norms_ = nn.ModuleList(
+                norm_fn(feature_size)
+                for feature_size in (
+                    *upsampling_dims,
+                    *self.downsampling_dims[1:],
                 )
-            last_layer_dim = self.cfg.fc_out_dim
-        return convs, fcs, last_layer_dim
+            )
 
-    def get_embeds(
-        self, feat: torch.Tensor
-    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
-        """Generate embedding from bbox feature."""
-        # shared part
-        if self.cfg.num_shared_convs > 0:
-            for conv in self.shared_convs:
-                feat = conv(feat)
-
-        if self.cfg.num_shared_fcs > 0:
-            feat = feat.view(feat.size(0), -1)
-            for fc in self.shared_fcs:
-                feat = self.relu(fc(feat))
-
-        # separate branches
-        x_dep = feat
-        x_dim = feat
-        x_rot = feat
-        x_2dc = feat
-
-        for conv in self.dep_convs:
-            x_dep = conv(x_dep)
-        if x_dep.dim() > 2:
-            x_dep = x_dep.view(x_dep.size(0), -1)
-        for fc in self.dep_fcs:
-            x_dep = self.relu(fc(x_dep))
-
-        for conv in self.dim_convs:
-            x_dim = conv(x_dim)
-        if x_dim.dim() > 2:
-            x_dim = x_dim.view(x_dim.size(0), -1)
-        for fc in self.dim_fcs:
-            x_dim = self.relu(fc(x_dim))
-
-        for conv in self.rot_convs:
-            x_rot = conv(x_rot)
-        if x_rot.dim() > 2:
-            x_rot = x_rot.view(x_rot.size(0), -1)
-        for fc in self.rot_fcs:
-            x_rot = self.relu(fc(x_rot))
-
-        for conv in self.cen_2d_convs:
-            x_2dc = conv(x_2dc)
-        if x_2dc.dim() > 2:
-            x_2dc = x_2dc.view(x_2dc.size(0), -1)
-        for fc in self.cen_2d_fcs:
-            x_2dc = self.relu(fc(x_2dc))
+        # Create upsampling layers
+        self.upsampling_layers = nn.ModuleList(
+            [nn.Conv1d(in_dimension, self.upsampling_dims[0], 1)]
+        )
+        for i in range(len(self.upsampling_dims) - 1):
+            self.upsampling_layers.append(
+                nn.Conv1d(
+                    self.upsampling_dims[i], self.upsampling_dims[i + 1], 1
+                )
+            )
 
-        return x_dep, x_dim, x_rot, x_2dc
+        # Create downsampling layers
+        self.downsampling_layers = nn.ModuleList(
+            [
+                nn.Linear(
+                    self.downsampling_dims[i], self.downsampling_dims[i + 1]
+                )
+                for i in range(len(self.downsampling_dims) - 1)
+            ]
+        )
+        self.downsampling_layers.append(
+            nn.Linear(self.downsampling_dims[-1], in_dimension**2)
+        )
 
-    def get_outputs(
+    def __call__(
         self,
-        x_dep: torch.Tensor,
-        x_dim: torch.Tensor,
-        x_rot: torch.Tensor,
-        x_2dc: torch.Tensor,
+        features: torch.Tensor,
     ) -> torch.Tensor:
-        """Generate output 3D bounding box parameters."""
-        depth = self.fc_dep(x_dep).view(-1, self.cfg.num_classes, 1)
-        depth_uncertainty = self.fc_dep_uncer(x_dep).view(
-            -1, self.cfg.num_classes, 1
-        )
-        dim = self.fc_dim(x_dim).view(-1, self.cfg.num_classes, 3)
-        alpha = generate_rotation_output(
-            self.fc_rot(x_rot), self.cfg.num_rotation_bins
-        )
-        delta_2dc = self.fc_2dc(x_2dc).view(-1, self.cfg.num_classes, 2)
-        return torch.cat([delta_2dc, depth, dim, alpha, depth_uncertainty], -1)
+        """Type definition for call implementation."""
+        return self._call_impl(features)
 
     def forward(
         self,
-        features_list: List[torch.Tensor],
-        boxes: List[Boxes2D],
-    ) -> List[torch.Tensor]:
-        """Forward 3D bounding box estimation."""
-        roi_feats = self.roi_pooler.pool(features_list, boxes)
-        x_dep, x_dim, x_rot, x_2dc = self.get_embeds(roi_feats)
-        outputs: List[torch.Tensor] = self.get_outputs(
-            x_dep, x_dim, x_rot, x_2dc
-        ).split([len(b) for b in boxes])
-        return outputs
+        features: torch.Tensor,
+    ) -> torch.Tensor:
+        """Linear Transform forward.
 
-    def get_targets(
-        self,
-        pos_assigned_gt_inds: List[torch.Tensor],
-        targets_2d: Sequence[Boxes2D],
-        targets_3d: Sequence[Boxes3D],
-        cam_intrinsics: Intrinsics,
-    ) -> Tuple[List[torch.Tensor], List[torch.Tensor]]:
-        """Get 3D bounding box targets for training."""
-        targets_2d = [b[p] for b, p in zip(targets_2d, pos_assigned_gt_inds)]
-        targets_3d = [b[p] for b, p in zip(targets_3d, pos_assigned_gt_inds)]
-
-        bbox_targets = self.bbox_coder.encode(
-            targets_2d, targets_3d, cam_intrinsics
-        )
-
-        labels = [
-            t.class_ids[p] for t, p in zip(targets_2d, pos_assigned_gt_inds)
-        ]
-        return bbox_targets, labels
+        Args:
+            features (Tensor[B, C, N]): Input features (e.g. points)
+
+        Returns:
+            Learned Canonical Transfomation Matrix for this input.
+            See T-Net in Pointnet publication
+            (https://arxiv.org/pdf/1612.00593.pdf)
+            for further information
+        """
+        batchsize = features.shape[0]
+        # Upsample features
+        for idx, layer in enumerate(self.upsampling_layers):
+            features = layer(features)
+            if self.norms_ is not None:
+                features = self.norms_[idx](features)
+            features = self.activation_(features)
+
+        features = torch.max(features, 2, keepdim=True)[0]
+        features = features.view(-1, self.upsampling_dims[-1])
+
+        # Downsample features
+        for idx, layer in enumerate(self.downsampling_layers):
+            features = layer(features)
+
+            # Do not apply norm and activation for
+            # final layer
+            if idx != len(self.downsampling_layers) - 1:
+                if self.norms_ is not None:
+                    norm_idx = idx + len(self.upsampling_layers)
+                    features = self.norms_[norm_idx](features)
+                features = self.activation_(features)
 
-    def forward_train(
+        identity_batch = self.identity.repeat(batchsize, 1)
+        transformations = features + identity_batch
+
+        return transformations.view(
+            batchsize, self.in_dimension_, self.in_dimension_
+        )
+
+
+class PointNetEncoder(nn.Module):
+    """PointNetEncoder.
+
+    Encodes a pointcloud and additional features into one feature description
+
+    See pointnet publication for more information
+    (https://arxiv.org/pdf/1612.00593.pdf)
+    """
+
+    def __init__(
         self,
-        inputs: InputSample,
-        boxes: List[Boxes2D],
-        features: Optional[Dict[str, torch.Tensor]] = None,
-    ) -> Tuple[LossesType, Optional[SamplingResult]]:
-        """Forward pass during training stage.
+        in_dimensions: int = 3,
+        out_dimensions: int = 1024,
+        mlp_dimensions: Iterable[Iterable[int]] = ((64, 64), (64, 128)),
+        norm_cls: str | None = "BatchNorm1d",
+        activation_cls: str = "ReLU",
+        **kwargs: ArgsType,
+    ):
+        """Creates a new PointNetEncoder.
+
+        Args:
+            in_dimensions (int): input dimension (e.g. 3 for xzy, 6 for xzyrgb)
+            out_dimensions (int): output dimensions
+            mlp_dimensions (Iterable[Iterable[int]]):(Dimensions of MLP layers)
+            norm_cls (Optional(str)): class for norm (nn.'norm_cls') or None
+            activation_cls (str): class for activation (nn.'activation_cls')
+            kwargs : See arguments of @LinearTransformStn
+        """
+        super().__init__()
+
+        self.out_dimension = out_dimensions
+
+        # Extend dimensions to upscale from input dimension
+        mlp_dim_list: list[list[int]] = [list(d) for d in mlp_dimensions]
+        mlp_dim_list[0].insert(0, in_dimensions)
+        mlp_dim_list[-1].append(out_dimensions)
+        self.mlp_dimensions = mlp_dim_list
+
+        # Learnable transformation layers.
+        self.trans_layers_ = nn.ModuleList(
+            [
+                LinearTransform(
+                    in_dimension=dims[0],
+                    norm_cls=norm_cls,
+                    activation_cls=activation_cls,
+                    **kwargs,
+                )
+                for dims in mlp_dim_list
+            ]
+        )
+
+        # MLP layers
+        self.mlp_layers_ = nn.ModuleList()
+
+        # Create activation
+        activation = getattr(nn, activation_cls)()
+
+        # Create norms
+        norm_fn: Callable[[int], nn.Module] = (
+            getattr(nn, norm_cls) if norm_cls is not None else None
+        )
+
+        for mlp_idx, mlp_dims in enumerate(mlp_dim_list):
+            layers: list[nn.Module] = []
+
+            for idx, (in_dim, out_dim) in enumerate(
+                zip(mlp_dims[:-1], mlp_dims[1:])
+            ):
+                # Create MLP
+                layers.append(torch.nn.Conv1d(in_dim, out_dim, 1))
+                # Create BN if needed
+                if norm_fn is not None:
+                    layers.append(norm_fn(out_dim))
+
+                # Only add activation if not last layer
+                if (
+                    mlp_idx != len(mlp_dim_list) - 1
+                    and idx != len(mlp_dims) - 2
+                ):
+                    layers.append(activation)
+
+            self.mlp_layers_.append(nn.Sequential(*layers))
+
+    def __call__(self, features: torch.Tensor) -> PointNetEncoderOut:
+        """Type definition for call implementation."""
+        return self._call_impl(features)
+
+    def forward(self, features: torch.Tensor) -> PointNetEncoderOut:
+        """Pointnet encoder forward.
 
         Args:
-            inputs: InputSamples (images, metadata, etc). Batched.
-            features: Input feature maps. Batched.
-            boxes: Input boxes to apply RoIHead on.
+            features (Tensor[B, C, N]): Input features stacked in channels.
+            e.g. raw point inputs: [B, 3, N] , w color : [B, 3+3, N], ...
 
         Returns:
-            LossesType: A dict of scalar loss tensors.
-            Optional[List[SamplingResult]]: Sampling result.
+            Extracted feature representation for input and all
+            applied transformations.
         """
-        assert features is not None, "QD-3DT box3D head requires features!"
-        features_list = [features[f] for f in self.cfg.in_features]
+        transforms: list[torch.Tensor] = []
 
-        # match and sample
-        sampling_results = match_and_sample_proposals(
-            self.matcher,
-            self.sampler,
-            boxes,
-            inputs.boxes2d,
-            self.cfg.proposal_append_gt,
-        )
-        positives = [l == 1 for l in sampling_results.sampled_labels]
-        pos_assigned_gt_inds = [
-            i[p]
-            for i, p in zip(sampling_results.sampled_target_indices, positives)
-        ]
-        pos_boxes = [
-            b[p] for b, p in zip(sampling_results.sampled_boxes, positives)
-        ]
-
-        predictions = self.forward(features_list, pos_boxes)
-
-        targets, labels = self.get_targets(
-            pos_assigned_gt_inds,
-            inputs.boxes2d,
-            inputs.boxes3d,
-            inputs.intrinsics,
-        )
-        loss = self.loss(
-            torch.cat(predictions), torch.cat(targets), torch.cat(labels)
+        for block_idx, trans_layer in enumerate(self.trans_layers_):
+            # Apply transformation
+            trans = trans_layer(features)
+            transforms.append(trans)
+            features = features.transpose(2, 1)
+            features = torch.bmm(features, trans)
+            features = features.transpose(2, 1)
+
+            if block_idx == len(self.trans_layers_) - 1:
+                pointwise_features = features.clone()
+
+            # Apply MLP
+            features = self.mlp_layers_[block_idx](features)
+
+        features = torch.max(features, 2, keepdim=True)[0]
+        features = features.view(-1, self.out_dimension)
+
+        return PointNetEncoderOut(
+            features=features,
+            transformations=transforms,
+            pointwise_features=pointwise_features,
         )
-        return loss, sampling_results
 
-    def forward_test(
+
+class PointNetSegmentation(nn.Module):
+    """Segmentation network using a simple pointnet as encoder."""
+
+    def __init__(
         self,
-        inputs: InputSample,
-        boxes: List[Boxes2D],
-        features: Optional[Dict[str, torch.Tensor]] = None,
-    ) -> Sequence[LabelInstance]:
-        """Forward pass during testing stage.
+        n_classes: int,
+        in_dimensions: int = 3,
+        feature_dimension: int = 1024,
+        norm_cls: str = "BatchNorm1d",
+        activation_cls: str = "ReLU",
+    ):
+        """Creates a new Point Net segementation network.
 
         Args:
-            inputs: InputSamples (images, metadata, etc). Batched.
-            features: Input feature maps. Batched.
-            boxes: Input boxes to apply RoIHead on.
+            n_classes (int): Number of semantic classes
+            in_dimensions (int): Input dimension (3 for xyz, 6 xyzrgb, ...)
+            feature_dimension (int): Size of feature from the encoder
+            norm_cls (Optional(str)): class for norm (nn.'norm_cls') or None
+            activation_cls (str): class for activation (nn.'activation_cls')
 
-        Returns:
-            List[LabelInstance]: Prediction output.
+        Raises:
+            ValueError: If dimensions are invalid
         """
-        assert features is not None, "QD-3DT box3D head requires features!"
-        if sum(len(b) for b in boxes) == 0:
-            dev = boxes[0].device
-            return [
-                Boxes3D(
-                    torch.empty(0, 10, device=dev),
-                    torch.empty(0, device=dev),
-                    torch.empty(0, device=dev),
-                )
-                for _ in range(len(boxes))
-            ]
+        super().__init__()
+        self.in_dimensions = in_dimensions
+
+        self.encoder = PointNetEncoder(
+            in_dimensions=in_dimensions,
+            out_dimensions=feature_dimension,
+            norm_cls=norm_cls,
+            activation_cls=activation_cls,
+        )
+        pc_feat_dim = self.encoder.mlp_dimensions[-1][0]
+
+        # Create activation
+        activation = getattr(nn, activation_cls)()
+
+        # Create norms
+        norm_fn: Callable[[int], nn.Module] = (
+            getattr(nn, norm_cls) if norm_cls is not None else None
+        )
+        self.classifier_dims = [feature_dimension + pc_feat_dim, 512, 256, 128]
+        # Build Model
+        self.classifier = nn.Sequential()
+        for in_dim, out_dim in zip(
+            self.classifier_dims[:-1], self.classifier_dims[1:]
+        ):
+            self.classifier.append(nn.Conv1d(in_dim, out_dim, 1))
+            if norm_fn is not None:
+                self.classifier.append(norm_fn(out_dim))
+            self.classifier.append(activation)
+
+        self.classifier.append(
+            nn.Conv1d(
+                out_dim,  # pylint: disable=undefined-loop-variable
+                n_classes,
+                1,
+            )
+        )
+
+    def __call__(self, points: torch.Tensor) -> PointNetSemanticsOut:
+        """Call function."""
+        return self._call_impl(points)
 
-        features_list = [features[f] for f in self.cfg.in_features]
-        predictions = self.forward(features_list, boxes)
+    def forward(self, points: torch.Tensor) -> PointNetSemanticsOut:
+        """Pointnet Segmenter Forward.
 
-        return self.bbox_coder.decode(boxes, predictions, inputs.intrinsics)
+        Args:
+            points (tensor) : inputs points dimension [B, in_dim, n_pts]
+
+        Returns:
+            Returns a list of tensors where the first element is
+            the desired segmentation [B, n_classes, n_pts] and the other
+            elements are the linear transformation matrices which
+            have been used to transform the pointclouds
+            @see LinearTransform
+        """
+        assert points.size(-2) == self.in_dimensions
+        n_pts = points.size(-1)
+        bs = points.size(0)
+        encoder_out = self.encoder(points)
+        global_features = encoder_out.features.view(bs, -1, 1).repeat(
+            1, 1, n_pts
+        )
+
+        x = torch.cat([global_features, encoder_out.pointwise_features], 1)
+
+        x = self.classifier(x)
+        return PointNetSemanticsOut(
+            class_logits=x, transformations=encoder_out.transformations
+        )
```

### Comparing `vis4d-0.0/vis4d/model/losses/embedding_distance.py` & `vis4d-0.1/vis4d/op/loss/embedding_distance.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,103 @@
 """Embedding distance loss."""
-from typing import Optional, Tuple
 
-import torch
-
-from vis4d.common.bbox.utils import random_choice
+from __future__ import annotations
 
-from .base import BaseLoss, LossConfig
-from .utils import l2_loss
+import torch
 
+from vis4d.op.box.box2d import random_choice
 
-class EmbeddingDistanceLossConfig(LossConfig):
-    """Config for embedding distance loss."""
+from .base import Loss
+from .common import l2_loss
+from .reducer import LossReducer, SumWeightedLoss, identity_loss
 
-    neg_pos_ub: float = -1.0
-    pos_margin: float = -1.0
-    neg_margin: float = -1.0
-    hard_mining: bool = False
 
+class EmbeddingDistanceLoss(Loss):
+    """Embedding distance loss for learning appearance similarity.
 
-class EmbeddingDistanceLoss(BaseLoss):
-    """Embedding distance loss."""
+    Computes the difference between the target distances and the predicted
+    distances of two sets of embedding vectors. Uses hard negative mining based
+    on the loss values to select pairs for overall loss computation.
+    """
 
-    def __init__(self, cfg: LossConfig):
-        """Init."""
-        super().__init__()
-        self.cfg = EmbeddingDistanceLossConfig(**cfg.dict())
+    def __init__(
+        self,
+        reducer: LossReducer = identity_loss,
+        neg_pos_ub: float = 3.0,
+        pos_margin: float = 0.0,
+        neg_margin: float = 0.3,
+        hard_mining: bool = True,
+    ):
+        """Creates an instance of the class."""
+        super().__init__(reducer)
+        self.neg_pos_ub = neg_pos_ub
+        self.neg_margin = neg_margin
+        self.pos_margin = pos_margin
+        self.hard_mining = hard_mining
 
-    def forward(  # type: ignore # pylint: disable=arguments-differ
+    def forward(  # pylint: disable=arguments-differ
         self,
         pred: torch.Tensor,
         target: torch.Tensor,
-        weight: Optional[torch.Tensor] = None,
-        reduction_override: Optional[str] = None,
+        weight: torch.Tensor | None = None,
     ) -> torch.Tensor:
         """Forward function.
 
         Args:
-            pred (torch.Tensor): The prediction.
-            target (torch.Tensor): The learning target of the prediction.
+            pred (torch.Tensor): The predicted distances between two sets of
+                predictions. Shape [N, M].
+            target (torch.Tensor): The corresponding target distances. Either
+                zero (different identity) or one (same identity).
             weight (torch.Tensor, optional): The weight of loss for each
                 prediction. Defaults to None.
-            reduction_override (str, optional): The reduction method used to
-                override the original reduction method of the loss.
-                Defaults to None.
 
         Returns:
             loss_bbox (torch.Tensor): embedding distance loss.
         """
-        assert reduction_override in (None, "none", "mean", "sum")
-        reduction = (
-            reduction_override
-            if reduction_override is not None
-            else self.cfg.reduction
-        )
+        if weight is None:
+            weight = target.new_ones(target.size())
         pred, weight, avg_factor = self.update_weight(pred, target, weight)
-        loss = self.cfg.loss_weight * l2_loss(
-            pred, target, weight, reduction=reduction, avg_factor=avg_factor
+        return l2_loss(
+            pred, target, reducer=SumWeightedLoss(weight, avg_factor)
         )
-        return loss
 
     def update_weight(
         self, pred: torch.Tensor, target: torch.Tensor, weight: torch.Tensor
-    ) -> Tuple[torch.Tensor, torch.Tensor, float]:
+    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         """Update element-wise loss weights.
 
         Exclude negatives according to maximum fraction of samples and/or
         hard negative mining.
         """
-        if weight is None:
-            weight = target.new_ones(target.size())
         invalid_inds = weight <= 0
         target[invalid_inds] = -1
-        pos_inds = target == 1
-        neg_inds = target == 0
+        pos_inds = torch.eq(target, 1)
+        neg_inds = torch.eq(target, 0)
 
-        if self.cfg.pos_margin > 0:
-            pred[pos_inds] -= self.cfg.pos_margin
-        if self.cfg.neg_margin > 0:
-            pred[neg_inds] -= self.cfg.neg_margin
+        if self.pos_margin > 0:
+            pred[pos_inds] -= self.pos_margin
+        if self.neg_margin > 0:
+            pred[neg_inds] -= self.neg_margin
         pred = torch.clamp(pred, min=0, max=1)
 
-        num_pos = max(1, int((target == 1).sum()))
-        num_neg = int((target == 0).sum())
-        if self.cfg.neg_pos_ub > 0 and num_neg / num_pos > self.cfg.neg_pos_ub:
-            num_neg = int(num_pos * self.cfg.neg_pos_ub)
-            neg_idx = torch.nonzero(target == 0, as_tuple=False)
+        num_pos = max(1, int(torch.eq(target, 1).sum()))
+        num_neg = int(torch.eq(target, 0).sum())
+        if self.neg_pos_ub > 0 and num_neg / num_pos > self.neg_pos_ub:
+            num_neg = int(num_pos * self.neg_pos_ub)
+            neg_idx = torch.nonzero(torch.eq(target, 0), as_tuple=False)
 
-            if self.cfg.hard_mining:
-                costs = l2_loss(pred, target, reduction="none")[
+            if self.hard_mining:
+                costs = l2_loss(pred, target)[
                     neg_idx[:, 0], neg_idx[:, 1]
                 ].detach()
                 neg_idx = neg_idx[costs.topk(num_neg)[1], :]
             else:
                 neg_idx = random_choice(neg_idx, num_neg)
 
             new_neg_inds = neg_inds.new_zeros(neg_inds.size()).bool()
             new_neg_inds[neg_idx[:, 0], neg_idx[:, 1]] = True
 
             invalid_neg_inds = torch.logical_xor(neg_inds, new_neg_inds)
             weight[invalid_neg_inds] = 0
 
-        avg_factor = (weight > 0).sum()
+        avg_factor = torch.greater(weight, 0).sum()
         return pred, weight, avg_factor
```

