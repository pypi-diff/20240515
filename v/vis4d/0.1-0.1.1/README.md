# Comparing `tmp/vis4d-0.1.tar.gz` & `tmp/vis4d-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vis4d-0.1.tar", last modified: Tue May 14 22:03:16 2024, max compression
+gzip compressed data, was "vis4d-0.1.1.tar", last modified: Wed May 15 09:35:50 2024, max compression
```

## Comparing `vis4d-0.1.tar` & `vis4d-0.1.1.tar`

### file list

```diff
@@ -1,514 +1,514 @@
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.695811 vis4d-0.1/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10804 2023-03-14 17:53:09.000000 vis4d-0.1/LICENSE
--rw-r--r--   0 yangyun  (577304) yangyun-group (478020)     4929 2024-05-14 22:03:16.683811 vis4d-0.1/PKG-INFO
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3612 2024-05-08 13:14:51.000000 vis4d-0.1/README.md
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3380 2024-05-14 21:54:27.000000 vis4d-0.1/pyproject.toml
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.303809 vis4d-0.1/requirements/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      429 2024-04-18 19:32:08.000000 vis4d-0.1/requirements/install.txt
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       38 2024-05-14 22:03:16.695811 vis4d-0.1/setup.cfg
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.335809 vis4d-0.1/vis4d/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      621 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       91 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/__main__.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.499809 vis4d-0.1/vis4d/common/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      692 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5822 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/array.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14835 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/ckpt.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2886 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/dict.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13271 2024-04-09 12:01:41.000000 vis4d-0.1/vis4d/common/distributed.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1821 2024-04-24 13:26:36.000000 vis4d-0.1/vis4d/common/imports.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4308 2024-04-24 13:26:36.000000 vis4d-0.1/vis4d/common/logging.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1478 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/named_tuple.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2580 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/prettyprint.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1666 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/progress.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2039 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/slurm.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1733 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/common/time.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2207 2024-04-24 13:26:36.000000 vis4d-0.1/vis4d/common/typing.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3092 2024-04-24 13:26:36.000000 vis4d-0.1/vis4d/common/util.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.543809 vis4d-0.1/vis4d/config/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      321 2024-04-24 13:26:25.000000 vis4d-0.1/vis4d/config/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    19095 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/config/config_dict.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8582 2024-04-24 13:26:36.000000 vis4d-0.1/vis4d/config/registry.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    11670 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/config/replicator.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    17951 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/config/show_connection.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1247 2024-04-24 13:26:36.000000 vis4d-0.1/vis4d/config/sweep.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6716 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/config/typing.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.599809 vis4d-0.1/vis4d/data/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      555 2023-07-03 10:21:11.000000 vis4d-0.1/vis4d/data/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4778 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/cbgs.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4818 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/const.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5210 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/data_pipe.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.667809 vis4d-0.1/vis4d/data/datasets/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      419 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3694 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2935 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/bdd100k.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10743 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/coco.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5656 2023-07-03 10:21:11.000000 vis4d-0.1/vis4d/data/datasets/imagenet.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    34589 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/datasets/nuscenes.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3510 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/nuscenes_detection.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8589 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/nuscenes_mono.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8796 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/nuscenes_trajectory.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8331 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/s3dis.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    27184 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/scalabel.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    21176 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/shift.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4312 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/datasets/torchvision.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12456 2024-04-30 12:05:33.000000 vis4d-0.1/vis4d/data/datasets/util.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.695809 vis4d-0.1/vis4d/data/io/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      231 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/io/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2403 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/io/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2255 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/io/file.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10602 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/io/hdf5.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      521 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/io/util.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7138 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/io/zip.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3819 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/iterable.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8037 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/loader.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7868 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/reference.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2611 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/resample.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3252 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/samplers.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.799809 vis4d-0.1/vis4d/data/transforms/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      120 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9528 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/affine.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6781 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/autoaugment.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8674 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    17604 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/crop.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    11967 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/flip.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2210 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/mask.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13546 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/mixup.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12423 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/mosaic.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1615 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/normalize.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5295 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/pad.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12307 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/photometric.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8694 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/point_sampling.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9324 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/points.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5447 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/post_process.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3493 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/transforms/random_erasing.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    18353 2024-05-02 21:04:55.000000 vis4d-0.1/vis4d/data/transforms/resize.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1687 2023-08-03 09:28:00.000000 vis4d-0.1/vis4d/data/transforms/select_sensor.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1517 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/data/transforms/to_tensor.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      615 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/data/typing.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.831809 vis4d-0.1/vis4d/engine/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       25 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/engine/__init__.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.895809 vis4d-0.1/vis4d/engine/callbacks/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      676 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6127 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3112 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/checkpoint.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1139 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/ema.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4410 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/engine/callbacks/evaluator.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4304 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/logging.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1607 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/trainer_state.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3585 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/visualizer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7348 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/callbacks/yolox_callbacks.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.935809 vis4d-0.1/vis4d/engine/connectors/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      725 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/connectors/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3752 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/connectors/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5124 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/connectors/multi_sensor.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4910 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/connectors/util.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7811 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/engine/experiment.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1093 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/flag.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7286 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/loss_module.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.963809 vis4d-0.1/vis4d/engine/optim/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      292 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/optim/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5863 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/optim/optimizer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9222 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/engine/optim/scheduler.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7243 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/engine/parser.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2361 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/run.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14371 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/trainer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7431 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/engine/util.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.975809 vis4d-0.1/vis4d/eval/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      114 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6203 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/base.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.995809 vis4d-0.1/vis4d/eval/bdd100k/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      249 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/bdd100k/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      995 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/bdd100k/detect.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3341 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/bdd100k/seg.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2803 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/bdd100k/track.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.003809 vis4d-0.1/vis4d/eval/coco/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      104 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/coco/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9593 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/coco/detect.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.027809 vis4d-0.1/vis4d/eval/common/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      350 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/common/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6427 2023-06-09 09:06:39.000000 vis4d-0.1/vis4d/eval/common/binary.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4445 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/common/cls.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7563 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/eval/common/depth.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4933 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/common/flow.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6603 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/common/seg.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.035809 vis4d-0.1/vis4d/eval/kitti/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       98 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/kitti/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2683 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/kitti/depth.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.047809 vis4d-0.1/vis4d/eval/metrics/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       20 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/metrics/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1049 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/metrics/cls.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4852 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/eval/metrics/depth.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1558 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/metrics/flow.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.063809 vis4d-0.1/vis4d/eval/nuscenes/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      184 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/nuscenes/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    11306 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/nuscenes/detect3d.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5327 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/nuscenes/track3d.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.111810 vis4d-0.1/vis4d/eval/scalabel/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      250 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/scalabel/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2215 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/scalabel/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4614 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/scalabel/detect.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5177 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/scalabel/track.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.143810 vis4d-0.1/vis4d/eval/shift/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      465 2023-06-09 09:06:38.000000 vis4d-0.1/vis4d/eval/shift/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1465 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/shift/depth.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      556 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/shift/detect.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      552 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/shift/flow.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10530 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/shift/multitask_writer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1831 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/shift/seg.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      629 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/shift/track.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      822 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/eval/utils.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.155809 vis4d-0.1/vis4d/model/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      232 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/model/__init__.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.167810 vis4d-0.1/vis4d/model/adapter/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      129 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/adapter/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3991 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/adapter/ema.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1399 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/model/adapter/flops.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.215810 vis4d-0.1/vis4d/model/cls/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      158 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/cls/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      257 2023-07-03 10:21:11.000000 vis4d-0.1/vis4d/model/cls/common.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4842 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/cls/vit.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.235810 vis4d-0.1/vis4d/model/detect/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       70 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/model/detect/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6511 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/detect/faster_rcnn.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7952 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/detect/mask_rcnn.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6381 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/detect/retinanet.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5310 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/detect/yolox.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.243810 vis4d-0.1/vis4d/model/detect3d/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       27 2023-08-25 09:31:21.000000 vis4d-0.1/vis4d/model/detect3d/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5221 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/detect3d/bevformer.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.259810 vis4d-0.1/vis4d/model/motion/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       21 2023-07-25 13:00:55.000000 vis4d-0.1/vis4d/model/motion/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9736 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/motion/velo_lstm.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.271810 vis4d-0.1/vis4d/model/seg/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       36 2023-04-14 18:49:01.000000 vis4d-0.1/vis4d/model/seg/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2301 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/seg/fcn_resnet.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4601 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/model/seg/semantic_fpn.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.279810 vis4d-0.1/vis4d/model/segment3d/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4288 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/segment3d/pointnet.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2838 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/model/segment3d/pointnetpp.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.291810 vis4d-0.1/vis4d/model/track/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       57 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/model/track/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    20090 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/track/qdtrack.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      668 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/track/util.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.299810 vis4d-0.1/vis4d/model/track3d/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       57 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/model/track3d/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    20943 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/model/track3d/cc_3dt.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.311810 vis4d-0.1/vis4d/op/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      416 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/op/__init__.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.359810 vis4d-0.1/vis4d/op/base/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      218 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1754 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9731 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/csp_darknet.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    15970 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/dla.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13764 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/pointnet.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    15986 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/pointnetpp.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    20419 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/base/resnet.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5751 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/unet.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3581 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/vgg.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9246 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/base/vit.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.383810 vis4d-0.1/vis4d/op/box/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       39 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/op/box/__init__.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.399810 vis4d-0.1/vis4d/op/box/anchor/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      227 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/anchor/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13297 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/anchor/anchor_generator.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8162 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/anchor/point_generator.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      732 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/anchor/util.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14436 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/box/box2d.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4530 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/box3d.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.471810 vis4d-0.1/vis4d/op/box/encoder/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      291 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/encoder/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3807 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/encoder/bevformer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7631 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/encoder/delta_xywh.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5272 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/encoder/qd_3dt.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      972 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/encoder/yolox.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.487810 vis4d-0.1/vis4d/op/box/matchers/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      206 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/matchers/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1004 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/matchers/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4532 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/matchers/max_iou.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9330 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/matchers/sim_ota.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.503810 vis4d-0.1/vis4d/op/box/poolers/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      186 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/poolers/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      602 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/poolers/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6783 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/poolers/roi_pooler.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2458 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/poolers/utils.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.519810 vis4d-0.1/vis4d/op/box/samplers/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      355 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/samplers/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2356 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/samplers/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7931 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/samplers/combined.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1126 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/samplers/pseudo.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1982 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/box/samplers/random.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.579810 vis4d-0.1/vis4d/op/detect/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       23 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/op/detect/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      451 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/common.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12497 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/dense_anchor.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7840 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/faster_rcnn.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14343 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/mask_rcnn.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    16244 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/detect/rcnn.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14467 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/retinanet.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    15586 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/rpn.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    25636 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect/yolox.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.599810 vis4d-0.1/vis4d/op/detect3d/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       26 2023-07-25 13:00:55.000000 vis4d-0.1/vis4d/op/detect3d/__init__.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.667810 vis4d-0.1/vis4d/op/detect3d/bevformer/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      132 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10575 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/bevformer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14626 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/decoder.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14090 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/encoder.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2267 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/grid_mask.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14179 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/spatial_cross_attention.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10074 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/temporal_self_attention.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9741 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/bevformer/transformer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      601 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/common.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    22844 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/detect3d/qd_3dt.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3865 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/detect3d/util.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.699810 vis4d-0.1/vis4d/op/fpp/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      371 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/fpp/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      848 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/fpp/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5434 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/fpp/dla_up.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4289 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/fpp/fpn.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5514 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/fpp/yolox_pafpn.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.711810 vis4d-0.1/vis4d/op/geometry/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       28 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/op/geometry/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4744 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/geometry/projection.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    17664 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/geometry/rotation.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3876 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/geometry/transform.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.823810 vis4d-0.1/vis4d/op/layer/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      602 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7960 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/layer/attention.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8467 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/conv2d.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4326 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/csp_layer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3123 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/deform_conv.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2090 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/drop.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3725 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/mlp.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12624 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/layer/ms_deform_attn.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2971 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/patch_embed.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9019 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/positional_encoding.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8464 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/layer/transformer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2272 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/layer/util.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3856 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/layer/weight_init.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.863810 vis4d-0.1/vis4d/op/loss/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      759 2023-07-27 00:26:02.000000 vis4d-0.1/vis4d/op/loss/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      758 2023-04-12 12:58:33.000000 vis4d-0.1/vis4d/op/loss/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3743 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/loss/common.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2422 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/loss/cross_entropy.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3616 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/loss/embedding_distance.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2657 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/loss/iou_loss.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2286 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/loss/multi_level_seg_loss.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1841 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/loss/multi_pos_cross_entropy.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1953 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/loss/orthogonal_transform_loss.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1700 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/loss/reducer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1426 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/loss/seg_cross_entropy_loss.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.879810 vis4d-0.1/vis4d/op/mask/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       43 2023-11-27 16:38:34.000000 vis4d-0.1/vis4d/op/mask/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9149 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/mask/util.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.891810 vis4d-0.1/vis4d/op/motion/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       25 2023-07-25 13:00:55.000000 vis4d-0.1/vis4d/op/motion/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2178 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/motion/kalman_filter.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1744 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/motion/velo_lstm.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.903810 vis4d-0.1/vis4d/op/seg/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       24 2023-04-14 18:49:01.000000 vis4d-0.1/vis4d/op/seg/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3791 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/seg/fcn.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4284 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/seg/semantic_fpn.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.931810 vis4d-0.1/vis4d/op/track/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       30 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/op/track/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1962 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/track/assignment.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      571 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/track/common.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1472 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/track/matching.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    25273 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/track/qdtrack.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.947811 vis4d-0.1/vis4d/op/track3d/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       33 2023-07-25 13:00:55.000000 vis4d-0.1/vis4d/op/track3d/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14273 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/op/track3d/cc_3dt.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      686 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/track3d/common.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      400 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/typing.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      878 2024-04-24 13:26:26.000000 vis4d-0.1/vis4d/op/util.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.967810 vis4d-0.1/vis4d/pl/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       57 2023-06-05 08:48:01.000000 vis4d-0.1/vis4d/pl/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       87 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/pl/__main__.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.979810 vis4d-0.1/vis4d/pl/callbacks/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      222 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/pl/callbacks/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7531 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/pl/callbacks/callback_wrapper.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      970 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/pl/callbacks/scheduler.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1341 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/pl/data_module.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4754 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/pl/run.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5022 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/pl/trainer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6957 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/pl/training_module.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.979810 vis4d-0.1/vis4d/state/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       52 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/state/__init__.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.987810 vis4d-0.1/vis4d/state/track/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       48 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/state/track/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10268 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/state/track/qdtrack.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:15.999811 vis4d-0.1/vis4d/state/track3d/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       51 2023-07-25 13:00:55.000000 vis4d-0.1/vis4d/state/track3d/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    18178 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/state/track3d/cc_3dt.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.015810 vis4d-0.1/vis4d/state/track3d/motion/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      205 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/state/track3d/motion/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1352 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/state/track3d/motion/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4296 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/state/track3d/motion/kf3d.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5066 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/state/track3d/motion/lstm_3d.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.027810 vis4d-0.1/vis4d/vis/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       64 2023-03-14 17:53:14.000000 vis4d-0.1/vis4d/vis/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1654 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/base.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.039811 vis4d-0.1/vis4d/vis/functional/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      482 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/functional/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    15103 2024-04-30 15:29:34.000000 vis4d-0.1/vis4d/vis/functional/image.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3137 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/functional/pointcloud.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.187811 vis4d-0.1/vis4d/vis/image/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      196 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    16159 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/bbox3d_visualizer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12655 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/bev_visualizer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7480 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/bounding_box_visualizer.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.199811 vis4d-0.1/vis4d/vis/image/canvas/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      168 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/canvas/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5476 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/canvas/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    21610 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/canvas/pillow_backend.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7634 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/seg_mask_visualizer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13824 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/vis/image/util.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.211811 vis4d-0.1/vis4d/vis/image/viewer/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      198 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/viewer/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      945 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/viewer/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1205 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/image/viewer/matplotlib_viewer.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.227811 vis4d-0.1/vis4d/vis/pointcloud/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      133 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/pointcloud/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7081 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/pointcloud/pointcloud_visualizer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9635 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/pointcloud/scene.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.243811 vis4d-0.1/vis4d/vis/pointcloud/viewer/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      226 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/pointcloud/viewer/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2773 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/pointcloud/viewer/base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5933 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/vis/pointcloud/viewer/open3d_viewer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      872 2024-04-10 22:23:17.000000 vis4d-0.1/vis4d/vis/util.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.251811 vis4d-0.1/vis4d/zoo/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1125 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/__init__.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.275811 vis4d-0.1/vis4d/zoo/base/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      571 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      565 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/callable.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.299811 vis4d-0.1/vis4d/zoo/base/data_connectors/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      490 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/data_connectors/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      413 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/data_connectors/cls.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      262 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/data_connectors/common.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      577 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/data_connectors/detection.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      680 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/data_connectors/seg.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      784 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/data_connectors/visualizers.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5379 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/dataloader.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.307811 vis4d-0.1/vis4d/zoo/base/datasets/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       31 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/__init__.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.323811 vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      506 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7383 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/detect.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6405 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/sem_seg.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6120 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/track.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.331811 vis4d-0.1/vis4d/zoo/base/datasets/coco/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      302 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/coco/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6759 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/coco/detection.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5451 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/coco/sem_seg.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5875 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/imagenet.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.343811 vis4d-0.1/vis4d/zoo/base/datasets/nuscenes/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      446 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/nuscenes/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3698 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/nuscenes/nuscenes.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1957 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/nuscenes/nuscenes_mono.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.355811 vis4d-0.1/vis4d/zoo/base/datasets/shift/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      705 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/shift/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13773 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/shift/common.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5261 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/datasets/shift/tasks.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.383811 vis4d-0.1/vis4d/zoo/base/models/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       29 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/models/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4828 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/models/faster_rcnn.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5067 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/models/mask_rcnn.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6488 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/models/qdtrack.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7288 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/models/yolox.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2733 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/optimizer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1161 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/pl_trainer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2674 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/base/runtime.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.387811 vis4d-0.1/vis4d/zoo/bdd100k/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1056 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/bdd100k/__init__.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.399811 vis4d-0.1/vis4d/zoo/bdd100k/faster_rcnn/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       32 2023-07-03 10:21:12.000000 vis4d-0.1/vis4d/zoo/bdd100k/faster_rcnn/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5598 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/faster_rcnn/faster_rcnn_r50_1x_bdd100k.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5625 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/faster_rcnn/faster_rcnn_r50_3x_bdd100k.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.415811 vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       30 2023-07-03 10:21:12.000000 vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5752 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_1x_bdd100k.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5873 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_3x_bdd100k.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5873 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_5x_bdd100k.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.423811 vis4d-0.1/vis4d/zoo/bdd100k/qdtrack/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       27 2023-12-01 09:54:18.000000 vis4d-0.1/vis4d/zoo/bdd100k/qdtrack/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4899 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/qdtrack/qdtrack_frcnn_r50_fpn_1x_bdd100k.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.451811 vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       32 2023-06-09 09:06:39.000000 vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6648 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r101_80k_bdd100k.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6404 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r50_40k_bdd100k.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6404 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r50_80k_bdd100k.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.483811 vis4d-0.1/vis4d/zoo/bevformer/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      224 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/bevformer/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5379 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bevformer/bevformer_base.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6687 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bevformer/bevformer_tiny.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2009 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bevformer/bevformer_vis.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5718 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/bevformer/data.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.535811 vis4d-0.1/vis4d/zoo/cc_3dt/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      536 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/cc_3dt/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4037 2024-04-12 10:27:07.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_bevformer_base_velo_lstm_nusc.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7309 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_kf3d_24e_nusc.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2885 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_pure_det_nusc.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1540 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_velo_lstm_24e_nusc.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7305 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r50_fpn_kf3d_12e_nusc.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3311 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_nusc_test.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2472 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_nusc_vis.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7583 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/data.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5445 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/model.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4905 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/velo_lstm_bevformer_base_100e_nusc.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4866 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/cc_3dt/velo_lstm_frcnn_r101_fpn_100e_nusc.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.539811 vis4d-0.1/vis4d/zoo/faster_rcnn/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      127 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/faster_rcnn/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6830 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/faster_rcnn/faster_rcnn_coco.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.547811 vis4d-0.1/vis4d/zoo/fcn_resnet/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      116 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/fcn_resnet/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5676 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/fcn_resnet/fcn_resnet_coco.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.559811 vis4d-0.1/vis4d/zoo/mask_rcnn/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      119 2023-12-01 09:54:19.000000 vis4d-0.1/vis4d/zoo/mask_rcnn/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6332 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/mask_rcnn/mask_rcnn_coco.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.575811 vis4d-0.1/vis4d/zoo/qdtrack/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      348 2024-04-24 13:26:43.000000 vis4d-0.1/vis4d/zoo/qdtrack/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8435 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/qdtrack/data_yolox.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5952 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/qdtrack/qdtrack_frcnn_r50_fpn_augs_1x_bdd100k.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5819 2024-04-24 13:26:43.000000 vis4d-0.1/vis4d/zoo/qdtrack/qdtrack_yolox_x_25e_bdd100k.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.583811 vis4d-0.1/vis4d/zoo/retinanet/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      119 2023-12-01 09:54:19.000000 vis4d-0.1/vis4d/zoo/retinanet/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6605 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/retinanet/retinanet_coco.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      719 2024-04-24 13:26:27.000000 vis4d-0.1/vis4d/zoo/run.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.587811 vis4d-0.1/vis4d/zoo/shift/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1283 2023-12-01 09:54:19.000000 vis4d-0.1/vis4d/zoo/shift/__init__.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.603811 vis4d-0.1/vis4d/zoo/shift/faster_rcnn/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       30 2023-07-11 09:39:24.000000 vis4d-0.1/vis4d/zoo/shift/faster_rcnn/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5898 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_12e_shift.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5899 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_36e_shift.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5851 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_6e_shift_all_domains.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.615811 vis4d-0.1/vis4d/zoo/shift/mask_rcnn/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       28 2023-07-11 09:39:24.000000 vis4d-0.1/vis4d/zoo/shift/mask_rcnn/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5970 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_12e_shift.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5971 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_36e_shift.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5923 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_6e_shift_all_domains.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.647811 vis4d-0.1/vis4d/zoo/shift/semantic_fpn/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       30 2023-07-11 09:39:24.000000 vis4d-0.1/vis4d/zoo/shift/semantic_fpn/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6573 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_160k_shift.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6543 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_160k_shift_all_domains.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6572 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_40k_shift.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6584 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_40k_shift_all_domains.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.659811 vis4d-0.1/vis4d/zoo/vit/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      211 2023-12-01 09:54:19.000000 vis4d-0.1/vis4d/zoo/vit/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5910 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/vit/vit_small_imagenet.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5895 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/vit/vit_tiny_imagenet.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.675811 vis4d-0.1/vis4d/zoo/yolox/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      196 2023-12-01 09:54:19.000000 vis4d-0.1/vis4d/zoo/yolox/__init__.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7780 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/yolox/data.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5523 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/yolox/yolox_s_300e_coco.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5644 2024-04-24 13:26:37.000000 vis4d-0.1/vis4d/zoo/yolox/yolox_tiny_300e_coco.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:14.407809 vis4d-0.1/vis4d-workspace/
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2129 2023-09-07 12:55:04.000000 vis4d-0.1/vis4d-workspace/convert.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4790 2024-04-11 16:51:37.000000 vis4d-0.1/vis4d-workspace/convert_bevformer.py
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2904 2023-07-13 08:24:28.000000 vis4d-0.1/vis4d-workspace/eval_nusc.py
-drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-14 22:03:16.679811 vis4d-0.1/vis4d.egg-info/
--rw-r--r--   0 yangyun  (577304) yangyun-group (478020)     4929 2024-05-14 22:02:22.000000 vis4d-0.1/vis4d.egg-info/PKG-INFO
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13499 2024-05-14 22:03:14.000000 vis4d-0.1/vis4d.egg-info/SOURCES.txt
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)        1 2024-05-14 22:02:22.000000 vis4d-0.1/vis4d.egg-info/dependency_links.txt
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      126 2024-05-14 22:02:22.000000 vis4d-0.1/vis4d.egg-info/entry_points.txt
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)      321 2024-05-14 22:02:22.000000 vis4d-0.1/vis4d.egg-info/requires.txt
--rw-rw----   0 yangyun  (577304) yangyun-group (478020)       22 2024-05-14 22:02:22.000000 vis4d-0.1/vis4d.egg-info/top_level.txt
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.450549 vis4d-0.1.1/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10804 2023-03-14 17:53:09.000000 vis4d-0.1.1/LICENSE
+-rw-r--r--   0 yangyun  (577304) yangyun-group (478020)     4937 2024-05-15 09:35:50.446549 vis4d-0.1.1/PKG-INFO
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3612 2024-05-14 22:05:05.000000 vis4d-0.1.1/README.md
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3385 2024-05-15 09:29:36.000000 vis4d-0.1.1/pyproject.toml
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.194546 vis4d-0.1.1/requirements/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      432 2024-05-15 08:59:24.000000 vis4d-0.1.1/requirements/install.txt
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       38 2024-05-15 09:35:50.454549 vis4d-0.1.1/setup.cfg
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.206546 vis4d-0.1.1/vis4d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      644 2024-05-15 09:28:17.000000 vis4d-0.1.1/vis4d/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       91 2024-04-24 13:26:25.000000 vis4d-0.1.1/vis4d/__main__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.374546 vis4d-0.1.1/vis4d/common/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      692 2024-04-24 13:26:25.000000 vis4d-0.1.1/vis4d/common/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5822 2024-04-24 13:26:25.000000 vis4d-0.1.1/vis4d/common/array.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14835 2024-04-24 13:26:25.000000 vis4d-0.1.1/vis4d/common/ckpt.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2886 2024-04-24 13:26:25.000000 vis4d-0.1.1/vis4d/common/dict.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13271 2024-04-09 12:01:41.000000 vis4d-0.1.1/vis4d/common/distributed.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1821 2024-04-24 13:26:36.000000 vis4d-0.1.1/vis4d/common/imports.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4308 2024-04-24 13:26:36.000000 vis4d-0.1.1/vis4d/common/logging.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1478 2024-04-24 13:26:25.000000 vis4d-0.1.1/vis4d/common/named_tuple.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2580 2024-04-24 13:26:25.000000 vis4d-0.1.1/vis4d/common/prettyprint.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1666 2024-04-24 13:26:25.000000 vis4d-0.1.1/vis4d/common/progress.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2039 2024-04-24 13:26:25.000000 vis4d-0.1.1/vis4d/common/slurm.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1733 2024-04-24 13:26:25.000000 vis4d-0.1.1/vis4d/common/time.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2207 2024-04-24 13:26:36.000000 vis4d-0.1.1/vis4d/common/typing.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3092 2024-04-24 13:26:36.000000 vis4d-0.1.1/vis4d/common/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.410546 vis4d-0.1.1/vis4d/config/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      321 2024-04-24 13:26:25.000000 vis4d-0.1.1/vis4d/config/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    19095 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/config/config_dict.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8582 2024-04-24 13:26:36.000000 vis4d-0.1.1/vis4d/config/registry.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    11670 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/config/replicator.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    17951 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/config/show_connection.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1247 2024-04-24 13:26:36.000000 vis4d-0.1.1/vis4d/config/sweep.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6716 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/config/typing.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.454546 vis4d-0.1.1/vis4d/data/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      555 2023-07-03 10:21:11.000000 vis4d-0.1.1/vis4d/data/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4778 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/cbgs.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4818 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/data/const.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5210 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/data_pipe.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.522547 vis4d-0.1.1/vis4d/data/datasets/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      419 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/datasets/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3694 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/datasets/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2935 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/datasets/bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10743 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/datasets/coco.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5656 2023-07-03 10:21:11.000000 vis4d-0.1.1/vis4d/data/datasets/imagenet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    34589 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/data/datasets/nuscenes.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3510 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/datasets/nuscenes_detection.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8589 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/datasets/nuscenes_mono.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8796 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/datasets/nuscenes_trajectory.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8331 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/datasets/s3dis.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    27184 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/datasets/scalabel.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    21176 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/datasets/shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4312 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/datasets/torchvision.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12456 2024-04-30 12:05:33.000000 vis4d-0.1.1/vis4d/data/datasets/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.554546 vis4d-0.1.1/vis4d/data/io/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      231 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/io/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2403 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/io/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2255 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/io/file.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10602 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/io/hdf5.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      521 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/io/util.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7138 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/io/zip.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3819 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/iterable.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8037 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/loader.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7868 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/reference.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2611 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/resample.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3252 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/samplers.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.662547 vis4d-0.1.1/vis4d/data/transforms/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      120 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/transforms/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9528 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/data/transforms/affine.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6781 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/transforms/autoaugment.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8674 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/transforms/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    17604 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/data/transforms/crop.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    11967 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/transforms/flip.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2210 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/data/transforms/mask.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13546 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/data/transforms/mixup.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12423 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/data/transforms/mosaic.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1615 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/transforms/normalize.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5295 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/transforms/pad.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12307 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/data/transforms/photometric.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8694 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/transforms/point_sampling.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9324 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/transforms/points.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5447 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/data/transforms/post_process.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3493 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/transforms/random_erasing.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    18353 2024-05-02 21:04:55.000000 vis4d-0.1.1/vis4d/data/transforms/resize.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1687 2023-08-03 09:28:00.000000 vis4d-0.1.1/vis4d/data/transforms/select_sensor.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1517 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/data/transforms/to_tensor.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      615 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/data/typing.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.702547 vis4d-0.1.1/vis4d/engine/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       25 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/engine/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.746547 vis4d-0.1.1/vis4d/engine/callbacks/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      676 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/callbacks/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6127 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/callbacks/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3112 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/callbacks/checkpoint.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1139 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/callbacks/ema.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4410 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/engine/callbacks/evaluator.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4304 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/callbacks/logging.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1607 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/callbacks/trainer_state.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3585 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/callbacks/visualizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7348 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/callbacks/yolox_callbacks.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.762547 vis4d-0.1.1/vis4d/engine/connectors/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      725 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/connectors/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3752 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/connectors/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5124 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/connectors/multi_sensor.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4910 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/connectors/util.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7811 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/engine/experiment.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1093 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/flag.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7286 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/loss_module.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.778547 vis4d-0.1.1/vis4d/engine/optim/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      292 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/optim/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5863 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/optim/optimizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9222 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/engine/optim/scheduler.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7243 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/engine/parser.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2361 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/run.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14371 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/trainer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7431 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/engine/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.790547 vis4d-0.1.1/vis4d/eval/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      114 2023-06-09 09:06:38.000000 vis4d-0.1.1/vis4d/eval/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6203 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/base.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.818547 vis4d-0.1.1/vis4d/eval/bdd100k/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      249 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/bdd100k/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      995 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/bdd100k/detect.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3341 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/bdd100k/seg.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2803 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/bdd100k/track.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.830547 vis4d-0.1.1/vis4d/eval/coco/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      104 2023-06-09 09:06:38.000000 vis4d-0.1.1/vis4d/eval/coco/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9593 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/coco/detect.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.858547 vis4d-0.1.1/vis4d/eval/common/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      350 2023-06-09 09:06:38.000000 vis4d-0.1.1/vis4d/eval/common/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6427 2023-06-09 09:06:39.000000 vis4d-0.1.1/vis4d/eval/common/binary.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4445 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/common/cls.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7563 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/eval/common/depth.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4933 2023-06-09 09:06:38.000000 vis4d-0.1.1/vis4d/eval/common/flow.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6603 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/common/seg.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.870547 vis4d-0.1.1/vis4d/eval/kitti/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       98 2023-06-09 09:06:38.000000 vis4d-0.1.1/vis4d/eval/kitti/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2683 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/kitti/depth.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.890547 vis4d-0.1.1/vis4d/eval/metrics/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       20 2023-06-09 09:06:38.000000 vis4d-0.1.1/vis4d/eval/metrics/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1049 2023-06-09 09:06:38.000000 vis4d-0.1.1/vis4d/eval/metrics/cls.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4852 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/eval/metrics/depth.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1558 2023-06-09 09:06:38.000000 vis4d-0.1.1/vis4d/eval/metrics/flow.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.902547 vis4d-0.1.1/vis4d/eval/nuscenes/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      184 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/nuscenes/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    11306 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/nuscenes/detect3d.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5327 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/nuscenes/track3d.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.926547 vis4d-0.1.1/vis4d/eval/scalabel/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      250 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/scalabel/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2215 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/scalabel/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4614 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/scalabel/detect.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5177 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/scalabel/track.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.962547 vis4d-0.1.1/vis4d/eval/shift/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      465 2023-06-09 09:06:38.000000 vis4d-0.1.1/vis4d/eval/shift/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1465 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/shift/depth.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      556 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/shift/detect.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      552 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/shift/flow.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10530 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/shift/multitask_writer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1831 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/shift/seg.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      629 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/shift/track.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      822 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/eval/utils.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.970547 vis4d-0.1.1/vis4d/model/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      232 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/model/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.990547 vis4d-0.1.1/vis4d/model/adapter/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      129 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/adapter/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3991 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/adapter/ema.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1399 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/model/adapter/flops.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.002547 vis4d-0.1.1/vis4d/model/cls/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      158 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/cls/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      257 2023-07-03 10:21:11.000000 vis4d-0.1.1/vis4d/model/cls/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4842 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/cls/vit.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.026547 vis4d-0.1.1/vis4d/model/detect/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       70 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/model/detect/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6511 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/detect/faster_rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7952 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/detect/mask_rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6381 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/detect/retinanet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5310 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/detect/yolox.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.034547 vis4d-0.1.1/vis4d/model/detect3d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       27 2023-08-25 09:31:21.000000 vis4d-0.1.1/vis4d/model/detect3d/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5221 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/detect3d/bevformer.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.046547 vis4d-0.1.1/vis4d/model/motion/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       21 2023-07-25 13:00:55.000000 vis4d-0.1.1/vis4d/model/motion/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9736 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/motion/velo_lstm.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.058547 vis4d-0.1.1/vis4d/model/seg/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       36 2023-04-14 18:49:01.000000 vis4d-0.1.1/vis4d/model/seg/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2301 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/seg/fcn_resnet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4601 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/model/seg/semantic_fpn.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.070547 vis4d-0.1.1/vis4d/model/segment3d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4288 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/segment3d/pointnet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2838 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/model/segment3d/pointnetpp.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.082547 vis4d-0.1.1/vis4d/model/track/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       57 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/model/track/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    20090 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/track/qdtrack.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      668 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/track/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.094547 vis4d-0.1.1/vis4d/model/track3d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       57 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/model/track3d/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    20943 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/model/track3d/cc_3dt.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.106547 vis4d-0.1.1/vis4d/op/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      416 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/op/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.154547 vis4d-0.1.1/vis4d/op/base/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      218 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/base/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1754 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/base/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9731 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/base/csp_darknet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    15970 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/base/dla.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13764 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/base/pointnet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    15986 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/base/pointnetpp.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    20419 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/base/resnet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5751 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/base/unet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3581 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/base/vgg.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9246 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/base/vit.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.170547 vis4d-0.1.1/vis4d/op/box/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       39 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/op/box/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.194548 vis4d-0.1.1/vis4d/op/box/anchor/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      227 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/anchor/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13297 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/anchor/anchor_generator.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8162 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/anchor/point_generator.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      732 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/anchor/util.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14436 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/box/box2d.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4530 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/box3d.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.218547 vis4d-0.1.1/vis4d/op/box/encoder/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      291 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/encoder/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3807 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/encoder/bevformer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7631 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/encoder/delta_xywh.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5272 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/encoder/qd_3dt.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      972 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/encoder/yolox.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.238547 vis4d-0.1.1/vis4d/op/box/matchers/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      206 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/matchers/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1004 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/matchers/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4532 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/matchers/max_iou.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9330 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/matchers/sim_ota.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.258548 vis4d-0.1.1/vis4d/op/box/poolers/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      186 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/poolers/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      602 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/poolers/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6783 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/poolers/roi_pooler.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2458 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/poolers/utils.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.282548 vis4d-0.1.1/vis4d/op/box/samplers/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      355 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/samplers/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2356 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/samplers/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7931 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/samplers/combined.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1126 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/samplers/pseudo.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1982 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/box/samplers/random.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.322548 vis4d-0.1.1/vis4d/op/detect/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       23 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/op/detect/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      451 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12497 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect/dense_anchor.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7840 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect/faster_rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14343 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect/mask_rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    16244 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/detect/rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14467 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect/retinanet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    15586 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect/rpn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    25636 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect/yolox.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.346548 vis4d-0.1.1/vis4d/op/detect3d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       26 2023-07-25 13:00:55.000000 vis4d-0.1.1/vis4d/op/detect3d/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.382548 vis4d-0.1.1/vis4d/op/detect3d/bevformer/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      132 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect3d/bevformer/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10575 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect3d/bevformer/bevformer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14626 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/detect3d/bevformer/decoder.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14090 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/detect3d/bevformer/encoder.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2267 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect3d/bevformer/grid_mask.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14179 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect3d/bevformer/spatial_cross_attention.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10074 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect3d/bevformer/temporal_self_attention.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9741 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect3d/bevformer/transformer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      601 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect3d/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    22844 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/detect3d/qd_3dt.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3865 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/detect3d/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.406548 vis4d-0.1.1/vis4d/op/fpp/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      371 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/fpp/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      848 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/fpp/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5434 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/fpp/dla_up.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4289 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/fpp/fpn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5514 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/fpp/yolox_pafpn.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.426548 vis4d-0.1.1/vis4d/op/geometry/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       28 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/op/geometry/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4744 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/geometry/projection.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    17664 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/geometry/rotation.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3876 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/geometry/transform.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.610548 vis4d-0.1.1/vis4d/op/layer/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      602 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/layer/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7960 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/layer/attention.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8467 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/layer/conv2d.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4326 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/layer/csp_layer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3123 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/layer/deform_conv.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2090 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/layer/drop.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3725 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/layer/mlp.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12624 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/layer/ms_deform_attn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2971 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/layer/patch_embed.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9019 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/layer/positional_encoding.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8464 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/layer/transformer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2272 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/layer/util.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3856 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/layer/weight_init.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.666548 vis4d-0.1.1/vis4d/op/loss/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      759 2023-07-27 00:26:02.000000 vis4d-0.1.1/vis4d/op/loss/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      758 2023-04-12 12:58:33.000000 vis4d-0.1.1/vis4d/op/loss/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3743 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/loss/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2422 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/loss/cross_entropy.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3616 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/loss/embedding_distance.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2657 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/loss/iou_loss.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2286 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/loss/multi_level_seg_loss.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1841 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/loss/multi_pos_cross_entropy.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1953 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/loss/orthogonal_transform_loss.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1700 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/loss/reducer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1426 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/loss/seg_cross_entropy_loss.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.674548 vis4d-0.1.1/vis4d/op/mask/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       43 2023-11-27 16:38:34.000000 vis4d-0.1.1/vis4d/op/mask/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9149 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/mask/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.686548 vis4d-0.1.1/vis4d/op/motion/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       25 2023-07-25 13:00:55.000000 vis4d-0.1.1/vis4d/op/motion/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2178 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/motion/kalman_filter.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1744 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/motion/velo_lstm.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.702548 vis4d-0.1.1/vis4d/op/seg/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       24 2023-04-14 18:49:01.000000 vis4d-0.1.1/vis4d/op/seg/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3791 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/seg/fcn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4284 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/seg/semantic_fpn.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.726548 vis4d-0.1.1/vis4d/op/track/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       30 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/op/track/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1962 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/track/assignment.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      571 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/track/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1472 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/track/matching.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    25273 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/track/qdtrack.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.738548 vis4d-0.1.1/vis4d/op/track3d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       33 2023-07-25 13:00:55.000000 vis4d-0.1.1/vis4d/op/track3d/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    14273 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/op/track3d/cc_3dt.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      686 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/track3d/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      400 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/typing.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      878 2024-04-24 13:26:26.000000 vis4d-0.1.1/vis4d/op/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.766548 vis4d-0.1.1/vis4d/pl/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       57 2023-06-05 08:48:01.000000 vis4d-0.1.1/vis4d/pl/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       87 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/pl/__main__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.778548 vis4d-0.1.1/vis4d/pl/callbacks/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      222 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/pl/callbacks/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7531 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/pl/callbacks/callback_wrapper.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      970 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/pl/callbacks/scheduler.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1341 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/pl/data_module.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4754 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/pl/run.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5022 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/pl/trainer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6957 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/pl/training_module.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.782548 vis4d-0.1.1/vis4d/state/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       52 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/state/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.794548 vis4d-0.1.1/vis4d/state/track/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       48 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/state/track/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    10268 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/state/track/qdtrack.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.806548 vis4d-0.1.1/vis4d/state/track3d/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       51 2023-07-25 13:00:55.000000 vis4d-0.1.1/vis4d/state/track3d/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    18178 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/state/track3d/cc_3dt.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.826548 vis4d-0.1.1/vis4d/state/track3d/motion/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      205 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/state/track3d/motion/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1352 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/state/track3d/motion/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4296 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/state/track3d/motion/kf3d.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5066 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/state/track3d/motion/lstm_3d.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.838548 vis4d-0.1.1/vis4d/vis/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       64 2023-03-14 17:53:14.000000 vis4d-0.1.1/vis4d/vis/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1654 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/base.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.850548 vis4d-0.1.1/vis4d/vis/functional/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      482 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/functional/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    15103 2024-04-30 15:29:34.000000 vis4d-0.1.1/vis4d/vis/functional/image.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3137 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/functional/pointcloud.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.890548 vis4d-0.1.1/vis4d/vis/image/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      196 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/image/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    16159 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/image/bbox3d_visualizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    12655 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/image/bev_visualizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7480 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/image/bounding_box_visualizer.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.906548 vis4d-0.1.1/vis4d/vis/image/canvas/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      168 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/image/canvas/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5476 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/image/canvas/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    21610 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/image/canvas/pillow_backend.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7634 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/image/seg_mask_visualizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13824 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/vis/image/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.922548 vis4d-0.1.1/vis4d/vis/image/viewer/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      198 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/image/viewer/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      945 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/image/viewer/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1205 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/image/viewer/matplotlib_viewer.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.934548 vis4d-0.1.1/vis4d/vis/pointcloud/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      133 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/pointcloud/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7081 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/pointcloud/pointcloud_visualizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     9635 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/pointcloud/scene.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.950549 vis4d-0.1.1/vis4d/vis/pointcloud/viewer/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      226 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/pointcloud/viewer/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2773 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/pointcloud/viewer/base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5933 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/vis/pointcloud/viewer/open3d_viewer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      872 2024-04-10 22:23:17.000000 vis4d-0.1.1/vis4d/vis/util.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:49.958548 vis4d-0.1.1/vis4d/zoo/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1125 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/zoo/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.002549 vis4d-0.1.1/vis4d/zoo/base/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      571 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      565 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/callable.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.030549 vis4d-0.1.1/vis4d/zoo/base/data_connectors/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      490 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/data_connectors/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      413 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/data_connectors/cls.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      262 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/data_connectors/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      577 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/data_connectors/detection.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      680 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/data_connectors/seg.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      784 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/data_connectors/visualizers.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5379 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/dataloader.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.042549 vis4d-0.1.1/vis4d/zoo/base/datasets/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       31 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.058549 vis4d-0.1.1/vis4d/zoo/base/datasets/bdd100k/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      506 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/bdd100k/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7383 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/bdd100k/detect.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6405 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/bdd100k/sem_seg.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6120 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/bdd100k/track.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.070549 vis4d-0.1.1/vis4d/zoo/base/datasets/coco/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      302 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/coco/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6759 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/coco/detection.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5451 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/coco/sem_seg.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5875 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/imagenet.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.090549 vis4d-0.1.1/vis4d/zoo/base/datasets/nuscenes/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      446 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/nuscenes/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3698 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/nuscenes/nuscenes.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1957 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/nuscenes/nuscenes_mono.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.106549 vis4d-0.1.1/vis4d/zoo/base/datasets/shift/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      705 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/shift/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13773 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/shift/common.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5261 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/datasets/shift/tasks.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.130549 vis4d-0.1.1/vis4d/zoo/base/models/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       29 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/models/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4828 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/models/faster_rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5067 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/models/mask_rcnn.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6488 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/models/qdtrack.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7288 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/models/yolox.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2733 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/optimizer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1161 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/pl_trainer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2674 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/base/runtime.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.134549 vis4d-0.1.1/vis4d/zoo/bdd100k/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1056 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.150549 vis4d-0.1.1/vis4d/zoo/bdd100k/faster_rcnn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       32 2023-07-03 10:21:12.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/faster_rcnn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5598 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/faster_rcnn/faster_rcnn_r50_1x_bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5625 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/faster_rcnn/faster_rcnn_r50_3x_bdd100k.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.166549 vis4d-0.1.1/vis4d/zoo/bdd100k/mask_rcnn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       30 2023-07-03 10:21:12.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/mask_rcnn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5752 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_1x_bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5873 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_3x_bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5873 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_5x_bdd100k.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.178549 vis4d-0.1.1/vis4d/zoo/bdd100k/qdtrack/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       27 2023-12-01 09:54:18.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/qdtrack/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4899 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/qdtrack/qdtrack_frcnn_r50_fpn_1x_bdd100k.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.194549 vis4d-0.1.1/vis4d/zoo/bdd100k/semantic_fpn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       32 2023-06-09 09:06:39.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/semantic_fpn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6648 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r101_80k_bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6404 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r50_40k_bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6404 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r50_80k_bdd100k.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.222549 vis4d-0.1.1/vis4d/zoo/bevformer/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      224 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/zoo/bevformer/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5379 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bevformer/bevformer_base.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6687 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bevformer/bevformer_tiny.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2009 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bevformer/bevformer_vis.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5718 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/bevformer/data.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.278549 vis4d-0.1.1/vis4d/zoo/cc_3dt/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      536 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/zoo/cc_3dt/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4037 2024-04-12 10:27:07.000000 vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_bevformer_base_velo_lstm_nusc.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7309 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_kf3d_24e_nusc.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2885 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_pure_det_nusc.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1540 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_velo_lstm_24e_nusc.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7305 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r50_fpn_kf3d_12e_nusc.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     3311 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_nusc_test.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2472 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_nusc_vis.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7583 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/cc_3dt/data.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5445 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/cc_3dt/model.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4905 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/cc_3dt/velo_lstm_bevformer_base_100e_nusc.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4866 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/cc_3dt/velo_lstm_frcnn_r101_fpn_100e_nusc.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.290549 vis4d-0.1.1/vis4d/zoo/faster_rcnn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      127 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/zoo/faster_rcnn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6830 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/faster_rcnn/faster_rcnn_coco.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.298549 vis4d-0.1.1/vis4d/zoo/fcn_resnet/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      116 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/zoo/fcn_resnet/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5676 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/fcn_resnet/fcn_resnet_coco.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.310549 vis4d-0.1.1/vis4d/zoo/mask_rcnn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      119 2023-12-01 09:54:19.000000 vis4d-0.1.1/vis4d/zoo/mask_rcnn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6332 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/mask_rcnn/mask_rcnn_coco.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.326549 vis4d-0.1.1/vis4d/zoo/qdtrack/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      348 2024-04-24 13:26:43.000000 vis4d-0.1.1/vis4d/zoo/qdtrack/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     8435 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/qdtrack/data_yolox.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5952 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/qdtrack/qdtrack_frcnn_r50_fpn_augs_1x_bdd100k.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5819 2024-04-24 13:26:43.000000 vis4d-0.1.1/vis4d/zoo/qdtrack/qdtrack_yolox_x_25e_bdd100k.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.334549 vis4d-0.1.1/vis4d/zoo/retinanet/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      119 2023-12-01 09:54:19.000000 vis4d-0.1.1/vis4d/zoo/retinanet/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6605 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/retinanet/retinanet_coco.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      719 2024-04-24 13:26:27.000000 vis4d-0.1.1/vis4d/zoo/run.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.342549 vis4d-0.1.1/vis4d/zoo/shift/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     1283 2023-12-01 09:54:19.000000 vis4d-0.1.1/vis4d/zoo/shift/__init__.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.358549 vis4d-0.1.1/vis4d/zoo/shift/faster_rcnn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       30 2023-07-11 09:39:24.000000 vis4d-0.1.1/vis4d/zoo/shift/faster_rcnn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5898 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_12e_shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5899 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_36e_shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5851 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_6e_shift_all_domains.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.378549 vis4d-0.1.1/vis4d/zoo/shift/mask_rcnn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       28 2023-07-11 09:39:24.000000 vis4d-0.1.1/vis4d/zoo/shift/mask_rcnn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5970 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_12e_shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5971 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_36e_shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5923 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_6e_shift_all_domains.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.398549 vis4d-0.1.1/vis4d/zoo/shift/semantic_fpn/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       30 2023-07-11 09:39:24.000000 vis4d-0.1.1/vis4d/zoo/shift/semantic_fpn/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6573 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_160k_shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6543 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_160k_shift_all_domains.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6572 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_40k_shift.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     6584 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_40k_shift_all_domains.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.414549 vis4d-0.1.1/vis4d/zoo/vit/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      211 2023-12-01 09:54:19.000000 vis4d-0.1.1/vis4d/zoo/vit/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5910 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/vit/vit_small_imagenet.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5895 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/vit/vit_tiny_imagenet.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.434549 vis4d-0.1.1/vis4d/zoo/yolox/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      196 2023-12-01 09:54:19.000000 vis4d-0.1.1/vis4d/zoo/yolox/__init__.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     7780 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/yolox/data.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5523 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/yolox/yolox_s_300e_coco.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     5644 2024-04-24 13:26:37.000000 vis4d-0.1.1/vis4d/zoo/yolox/yolox_tiny_300e_coco.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:48.266546 vis4d-0.1.1/vis4d-workspace/
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2129 2023-09-07 12:55:04.000000 vis4d-0.1.1/vis4d-workspace/convert.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     4790 2024-04-11 16:51:37.000000 vis4d-0.1.1/vis4d-workspace/convert_bevformer.py
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)     2904 2023-07-13 08:24:28.000000 vis4d-0.1.1/vis4d-workspace/eval_nusc.py
+drwxrwx---   0 yangyun  (577304) yangyun-group (478020)        0 2024-05-15 09:35:50.442549 vis4d-0.1.1/vis4d.egg-info/
+-rw-r--r--   0 yangyun  (577304) yangyun-group (478020)     4937 2024-05-15 09:35:08.000000 vis4d-0.1.1/vis4d.egg-info/PKG-INFO
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)    13499 2024-05-15 09:35:48.000000 vis4d-0.1.1/vis4d.egg-info/SOURCES.txt
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)        1 2024-05-15 09:35:08.000000 vis4d-0.1.1/vis4d.egg-info/dependency_links.txt
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      126 2024-05-15 09:35:08.000000 vis4d-0.1.1/vis4d.egg-info/entry_points.txt
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)      324 2024-05-15 09:35:08.000000 vis4d-0.1.1/vis4d.egg-info/requires.txt
+-rw-rw----   0 yangyun  (577304) yangyun-group (478020)       22 2024-05-15 09:35:08.000000 vis4d-0.1.1/vis4d.egg-info/top_level.txt
```

### Comparing `vis4d-0.1/LICENSE` & `vis4d-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/PKG-INFO` & `vis4d-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: vis4d
-Version: 0.1
+Version: 0.1.1
 Summary: Vis4D Python package for Visual 4D scene understanding
 Author-email: "VIS @ ETH" <i@yf.io>
 License: Apache 2.0
-Project-URL: Documentation, https://vis.xyz/4d/
+Project-URL: Documentation, https://docs.vis.xyz/4d
 Project-URL: Source, https://github.com/syscv/vis4d
 Project-URL: Tracker, https://github.com/syscv/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.0
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: appdirs
 Requires-Dist: cloudpickle
 Requires-Dist: cython
 Requires-Dist: devtools
@@ -30,16 +30,16 @@
 Requires-Dist: pycocotools
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: setuptools
 Requires-Dist: tensorboard
 Requires-Dist: termcolor
 Requires-Dist: terminaltables
 Requires-Dist: timm>=0.6.0
-Requires-Dist: torch>=1.10
-Requires-Dist: torchvision>=0.11
+Requires-Dist: torch>=2.0.0
+Requires-Dist: torchvision>=0.15.1
 Requires-Dist: tqdm
 Requires-Dist: utm
 Requires-Dist: wheel
 Requires-Dist: bdd100k
 Requires-Dist: scalabel
 Requires-Dist: nuscenes-devkit
 
@@ -150,15 +150,15 @@
 **Project Leads**
 - [Yung-Hsu Yang](https://royyang0714.github.io/)*
 - [Tobias Fischer](https://tobiasfshr.github.io/)*
  
 **Core Contributors**
 - [Thomas E. Huang](https://www.thomasehuang.com/)
 - [Tao Sun](https://www.suniique.com/)
-- [René Zurbrügg](https://github.com/renezurbruegg)
+- [René Zurbrügg](https://renezurbruegg.github.io/)
  
 **Advisors**
 - [Fisher Yu](https://www.yf.io/)
  
 `*` denotes equal contribution
 
 **We are open to contributions and suggestions, feel free to reach out to us.**
```

### Comparing `vis4d-0.1/README.md` & `vis4d-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 **Project Leads**
 - [Yung-Hsu Yang](https://royyang0714.github.io/)*
 - [Tobias Fischer](https://tobiasfshr.github.io/)*
  
 **Core Contributors**
 - [Thomas E. Huang](https://www.thomasehuang.com/)
 - [Tao Sun](https://www.suniique.com/)
-- [René Zurbrügg](https://github.com/renezurbruegg)
+- [René Zurbrügg](https://renezurbruegg.github.io/)
  
 **Advisors**
 - [Fisher Yu](https://www.yf.io/)
  
 `*` denotes equal contribution
 
 **We are open to contributions and suggestions, feel free to reach out to us.**
```

#### html2text {}

```diff
@@ -26,16 +26,16 @@
 his Ph.D. at ETH Zurich, [Thomas E. Huang](https://www.thomasehuang.com/
 ) helped contribute many models, [Tao Sun](https://www.suniique.com/
 ) implemented the ViT models and designed the evaluation pipeline, and[RenÃ©
 ZurbrÃ¼gg](https://github.com/renezurbruegg) designed the config system. ##
 Contributors **Project Leads** - [Yung-Hsu Yang](https://royyang0714.github.io/
 )* - [Tobias Fischer](https://tobiasfshr.github.io/)* **Core Contributors** -
 [Thomas E. Huang](https://www.thomasehuang.com/) - [Tao Sun](https://
-www.suniique.com/) - [RenÃ© ZurbrÃ¼gg](https://github.com/renezurbruegg)
-**Advisors** - [Fisher Yu](https://www.yf.io/) `*` denotes equal contribution
+www.suniique.com/) - [RenÃ© ZurbrÃ¼gg](https://renezurbruegg.github.io/
+) **Advisors** - [Fisher Yu](https://www.yf.io/) `*` denotes equal contribution
 **We are open to contributions and suggestions, feel free to reach out to us.**
 [Check out our contribution guidelines for this project](docs/source/dev_guide/
 contribute.rst) **Community Contributors** _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
 _i_m_a_g_e_?_r_e_p_o_=_S_y_s_C_V_/_v_i_s_4_d_]## Citation If you find Vis4D is useful for your
 research, please consider citing the following BibTeX entry. ```bibtex @misc
 {vis4d_2024, author = {{Yung-Hsu Yang and Tobias Fischer and Thomas E. Huang}
 and RenÃ© ZurbrÃ¼gg and Tao Sun and Fisher Yu}, title = {Vis4D}, howpublished =
```

### Comparing `vis4d-0.1/pyproject.toml` & `vis4d-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -108,20 +108,20 @@
     follow_imports = "normal"
     follow_imports_for_stubs = true
     ignore_missing_imports = true
 
 
 [project]
 name = "vis4d"
-version = "0.1"
+version = "0.1.1"
 authors = [{name = "VIS @ ETH", email = "i@yf.io"}]
 description = "Vis4D Python package for Visual 4D scene understanding"
 readme = "README.md"
 license = { text="Apache 2.0"}
-requires-python = ">=3.9.0"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
@@ -131,15 +131,15 @@
 [tool.setuptools.package-data]
 "*" = ["py.typed"]
 
 [tool.setuptools.packages.find]
 include = ["vis4d*"]
 
 [project.urls]
-"Documentation" = "https://vis.xyz/4d/"
+"Documentation" = "https://docs.vis.xyz/4d"
 "Source" = "https://github.com/syscv/vis4d"
 "Tracker" = "https://github.com/syscv/"
 
 [project.scripts]
 vis4d = "vis4d.engine.run:entrypoint"
 vis4d-pl = "vis4d.pl.run:entrypoint"
 vis4d-zoo = "vis4d.zoo.run:entrypoint"
```

### Comparing `vis4d-0.1/vis4d/__init__.py` & `vis4d-0.1.1/vis4d/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 It contains common operators and models, data pipelines and training recipes
 for a number of contemporary methods and provides a compositional framework
 for further research and development of 4D Vision algorithms.
 """
 
 import logging
 
+__version__ = "0.1.1"
+
 _root_logger = logging.getLogger()
 _logger = logging.getLogger(__name__)
 _logger.setLevel(logging.INFO)
 
 # if root logger has handlers, propagate messages up and let root logger
 # process them
 if not _root_logger.hasHandlers():  # pragma: no cover
```

### Comparing `vis4d-0.1/vis4d/common/__init__.py` & `vis4d-0.1.1/vis4d/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/array.py` & `vis4d-0.1.1/vis4d/common/array.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/ckpt.py` & `vis4d-0.1.1/vis4d/common/ckpt.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/dict.py` & `vis4d-0.1.1/vis4d/common/dict.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/distributed.py` & `vis4d-0.1.1/vis4d/common/distributed.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/imports.py` & `vis4d-0.1.1/vis4d/common/imports.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/logging.py` & `vis4d-0.1.1/vis4d/common/logging.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/named_tuple.py` & `vis4d-0.1.1/vis4d/common/named_tuple.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/prettyprint.py` & `vis4d-0.1.1/vis4d/common/prettyprint.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/progress.py` & `vis4d-0.1.1/vis4d/common/progress.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/slurm.py` & `vis4d-0.1.1/vis4d/common/slurm.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/time.py` & `vis4d-0.1.1/vis4d/common/time.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/typing.py` & `vis4d-0.1.1/vis4d/common/typing.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/common/util.py` & `vis4d-0.1.1/vis4d/common/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/config/config_dict.py` & `vis4d-0.1.1/vis4d/config/config_dict.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/config/registry.py` & `vis4d-0.1.1/vis4d/config/registry.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/config/replicator.py` & `vis4d-0.1.1/vis4d/config/replicator.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/config/show_connection.py` & `vis4d-0.1.1/vis4d/config/show_connection.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/config/sweep.py` & `vis4d-0.1.1/vis4d/config/sweep.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/config/typing.py` & `vis4d-0.1.1/vis4d/config/typing.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/__init__.py` & `vis4d-0.1.1/vis4d/data/__init__.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/cbgs.py` & `vis4d-0.1.1/vis4d/data/cbgs.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/const.py` & `vis4d-0.1.1/vis4d/data/const.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/data_pipe.py` & `vis4d-0.1.1/vis4d/data/data_pipe.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/base.py` & `vis4d-0.1.1/vis4d/data/datasets/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/bdd100k.py` & `vis4d-0.1.1/vis4d/data/datasets/bdd100k.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/coco.py` & `vis4d-0.1.1/vis4d/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/imagenet.py` & `vis4d-0.1.1/vis4d/data/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/nuscenes.py` & `vis4d-0.1.1/vis4d/data/datasets/nuscenes.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/nuscenes_detection.py` & `vis4d-0.1.1/vis4d/data/datasets/nuscenes_detection.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/nuscenes_mono.py` & `vis4d-0.1.1/vis4d/data/datasets/nuscenes_mono.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/nuscenes_trajectory.py` & `vis4d-0.1.1/vis4d/data/datasets/nuscenes_trajectory.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/s3dis.py` & `vis4d-0.1.1/vis4d/data/datasets/s3dis.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/scalabel.py` & `vis4d-0.1.1/vis4d/data/datasets/scalabel.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/shift.py` & `vis4d-0.1.1/vis4d/data/datasets/shift.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/torchvision.py` & `vis4d-0.1.1/vis4d/data/datasets/torchvision.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/datasets/util.py` & `vis4d-0.1.1/vis4d/data/datasets/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/io/base.py` & `vis4d-0.1.1/vis4d/data/io/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/io/file.py` & `vis4d-0.1.1/vis4d/data/io/file.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/io/hdf5.py` & `vis4d-0.1.1/vis4d/data/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/io/util.py` & `vis4d-0.1.1/vis4d/data/io/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/io/zip.py` & `vis4d-0.1.1/vis4d/data/io/zip.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/iterable.py` & `vis4d-0.1.1/vis4d/data/iterable.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/loader.py` & `vis4d-0.1.1/vis4d/data/loader.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/reference.py` & `vis4d-0.1.1/vis4d/data/reference.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/resample.py` & `vis4d-0.1.1/vis4d/data/resample.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/samplers.py` & `vis4d-0.1.1/vis4d/data/samplers.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/affine.py` & `vis4d-0.1.1/vis4d/data/transforms/affine.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/autoaugment.py` & `vis4d-0.1.1/vis4d/data/transforms/autoaugment.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/base.py` & `vis4d-0.1.1/vis4d/data/transforms/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/crop.py` & `vis4d-0.1.1/vis4d/data/transforms/crop.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/flip.py` & `vis4d-0.1.1/vis4d/data/transforms/flip.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/mask.py` & `vis4d-0.1.1/vis4d/data/transforms/mask.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/mixup.py` & `vis4d-0.1.1/vis4d/data/transforms/mixup.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/mosaic.py` & `vis4d-0.1.1/vis4d/data/transforms/mosaic.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/normalize.py` & `vis4d-0.1.1/vis4d/data/transforms/normalize.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/pad.py` & `vis4d-0.1.1/vis4d/data/transforms/pad.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/photometric.py` & `vis4d-0.1.1/vis4d/data/transforms/photometric.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/point_sampling.py` & `vis4d-0.1.1/vis4d/data/transforms/point_sampling.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/points.py` & `vis4d-0.1.1/vis4d/data/transforms/points.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/post_process.py` & `vis4d-0.1.1/vis4d/data/transforms/post_process.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/random_erasing.py` & `vis4d-0.1.1/vis4d/data/transforms/random_erasing.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/resize.py` & `vis4d-0.1.1/vis4d/data/transforms/resize.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/select_sensor.py` & `vis4d-0.1.1/vis4d/data/transforms/select_sensor.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/transforms/to_tensor.py` & `vis4d-0.1.1/vis4d/data/transforms/to_tensor.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/data/typing.py` & `vis4d-0.1.1/vis4d/data/typing.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/callbacks/__init__.py` & `vis4d-0.1.1/vis4d/engine/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/callbacks/base.py` & `vis4d-0.1.1/vis4d/engine/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/callbacks/checkpoint.py` & `vis4d-0.1.1/vis4d/engine/callbacks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/callbacks/ema.py` & `vis4d-0.1.1/vis4d/engine/callbacks/ema.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/callbacks/evaluator.py` & `vis4d-0.1.1/vis4d/engine/callbacks/evaluator.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/callbacks/logging.py` & `vis4d-0.1.1/vis4d/engine/callbacks/logging.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/callbacks/trainer_state.py` & `vis4d-0.1.1/vis4d/engine/callbacks/trainer_state.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/callbacks/visualizer.py` & `vis4d-0.1.1/vis4d/engine/callbacks/visualizer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/callbacks/yolox_callbacks.py` & `vis4d-0.1.1/vis4d/engine/callbacks/yolox_callbacks.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/connectors/__init__.py` & `vis4d-0.1.1/vis4d/engine/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/connectors/base.py` & `vis4d-0.1.1/vis4d/engine/connectors/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/connectors/multi_sensor.py` & `vis4d-0.1.1/vis4d/engine/connectors/multi_sensor.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/connectors/util.py` & `vis4d-0.1.1/vis4d/engine/connectors/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/experiment.py` & `vis4d-0.1.1/vis4d/engine/experiment.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/flag.py` & `vis4d-0.1.1/vis4d/engine/flag.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/loss_module.py` & `vis4d-0.1.1/vis4d/engine/loss_module.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/optim/optimizer.py` & `vis4d-0.1.1/vis4d/engine/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/optim/scheduler.py` & `vis4d-0.1.1/vis4d/engine/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/parser.py` & `vis4d-0.1.1/vis4d/engine/parser.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/run.py` & `vis4d-0.1.1/vis4d/engine/run.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/trainer.py` & `vis4d-0.1.1/vis4d/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/engine/util.py` & `vis4d-0.1.1/vis4d/engine/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/base.py` & `vis4d-0.1.1/vis4d/eval/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/bdd100k/detect.py` & `vis4d-0.1.1/vis4d/eval/bdd100k/detect.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/bdd100k/seg.py` & `vis4d-0.1.1/vis4d/eval/bdd100k/seg.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/bdd100k/track.py` & `vis4d-0.1.1/vis4d/eval/bdd100k/track.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/coco/detect.py` & `vis4d-0.1.1/vis4d/eval/coco/detect.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/common/binary.py` & `vis4d-0.1.1/vis4d/eval/common/binary.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/common/cls.py` & `vis4d-0.1.1/vis4d/eval/common/cls.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/common/depth.py` & `vis4d-0.1.1/vis4d/eval/common/depth.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/common/flow.py` & `vis4d-0.1.1/vis4d/eval/common/flow.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/common/seg.py` & `vis4d-0.1.1/vis4d/eval/common/seg.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/kitti/depth.py` & `vis4d-0.1.1/vis4d/eval/kitti/depth.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/metrics/cls.py` & `vis4d-0.1.1/vis4d/eval/metrics/cls.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/metrics/depth.py` & `vis4d-0.1.1/vis4d/eval/metrics/depth.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/metrics/flow.py` & `vis4d-0.1.1/vis4d/eval/metrics/flow.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/nuscenes/detect3d.py` & `vis4d-0.1.1/vis4d/eval/nuscenes/detect3d.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/nuscenes/track3d.py` & `vis4d-0.1.1/vis4d/eval/nuscenes/track3d.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/scalabel/base.py` & `vis4d-0.1.1/vis4d/eval/scalabel/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/scalabel/detect.py` & `vis4d-0.1.1/vis4d/eval/scalabel/detect.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/scalabel/track.py` & `vis4d-0.1.1/vis4d/eval/scalabel/track.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/shift/depth.py` & `vis4d-0.1.1/vis4d/eval/shift/depth.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/shift/detect.py` & `vis4d-0.1.1/vis4d/eval/shift/detect.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/shift/flow.py` & `vis4d-0.1.1/vis4d/eval/shift/flow.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/shift/multitask_writer.py` & `vis4d-0.1.1/vis4d/eval/shift/multitask_writer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/shift/seg.py` & `vis4d-0.1.1/vis4d/eval/shift/seg.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/shift/track.py` & `vis4d-0.1.1/vis4d/eval/shift/track.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/eval/utils.py` & `vis4d-0.1.1/vis4d/eval/utils.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/adapter/ema.py` & `vis4d-0.1.1/vis4d/model/adapter/ema.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/adapter/flops.py` & `vis4d-0.1.1/vis4d/model/adapter/flops.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/cls/vit.py` & `vis4d-0.1.1/vis4d/model/cls/vit.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/detect/faster_rcnn.py` & `vis4d-0.1.1/vis4d/model/detect/faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/detect/mask_rcnn.py` & `vis4d-0.1.1/vis4d/model/detect/mask_rcnn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/detect/retinanet.py` & `vis4d-0.1.1/vis4d/model/detect/retinanet.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/detect/yolox.py` & `vis4d-0.1.1/vis4d/model/detect/yolox.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/detect3d/bevformer.py` & `vis4d-0.1.1/vis4d/model/detect3d/bevformer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/motion/velo_lstm.py` & `vis4d-0.1.1/vis4d/model/motion/velo_lstm.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/seg/fcn_resnet.py` & `vis4d-0.1.1/vis4d/model/seg/fcn_resnet.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/seg/semantic_fpn.py` & `vis4d-0.1.1/vis4d/model/seg/semantic_fpn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/segment3d/pointnet.py` & `vis4d-0.1.1/vis4d/model/segment3d/pointnet.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/segment3d/pointnetpp.py` & `vis4d-0.1.1/vis4d/model/segment3d/pointnetpp.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/track/qdtrack.py` & `vis4d-0.1.1/vis4d/model/track/qdtrack.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/track/util.py` & `vis4d-0.1.1/vis4d/model/track/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/model/track3d/cc_3dt.py` & `vis4d-0.1.1/vis4d/model/track3d/cc_3dt.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/base/base.py` & `vis4d-0.1.1/vis4d/op/base/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/base/csp_darknet.py` & `vis4d-0.1.1/vis4d/op/base/csp_darknet.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/base/dla.py` & `vis4d-0.1.1/vis4d/op/base/dla.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/base/pointnet.py` & `vis4d-0.1.1/vis4d/op/base/pointnet.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/base/pointnetpp.py` & `vis4d-0.1.1/vis4d/op/base/pointnetpp.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/base/resnet.py` & `vis4d-0.1.1/vis4d/op/base/resnet.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/base/unet.py` & `vis4d-0.1.1/vis4d/op/base/unet.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/base/vgg.py` & `vis4d-0.1.1/vis4d/op/base/vgg.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/base/vit.py` & `vis4d-0.1.1/vis4d/op/base/vit.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/anchor/anchor_generator.py` & `vis4d-0.1.1/vis4d/op/box/anchor/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/anchor/point_generator.py` & `vis4d-0.1.1/vis4d/op/box/anchor/point_generator.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/anchor/util.py` & `vis4d-0.1.1/vis4d/op/box/anchor/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/box2d.py` & `vis4d-0.1.1/vis4d/op/box/box2d.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/box3d.py` & `vis4d-0.1.1/vis4d/op/box/box3d.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/encoder/bevformer.py` & `vis4d-0.1.1/vis4d/op/box/encoder/bevformer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/encoder/delta_xywh.py` & `vis4d-0.1.1/vis4d/op/box/encoder/delta_xywh.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/encoder/qd_3dt.py` & `vis4d-0.1.1/vis4d/op/box/encoder/qd_3dt.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/encoder/yolox.py` & `vis4d-0.1.1/vis4d/op/box/encoder/yolox.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/matchers/base.py` & `vis4d-0.1.1/vis4d/op/box/matchers/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/matchers/max_iou.py` & `vis4d-0.1.1/vis4d/op/box/matchers/max_iou.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/matchers/sim_ota.py` & `vis4d-0.1.1/vis4d/op/box/matchers/sim_ota.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/poolers/base.py` & `vis4d-0.1.1/vis4d/op/box/poolers/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/poolers/roi_pooler.py` & `vis4d-0.1.1/vis4d/op/box/poolers/roi_pooler.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/poolers/utils.py` & `vis4d-0.1.1/vis4d/op/box/poolers/utils.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/samplers/base.py` & `vis4d-0.1.1/vis4d/op/box/samplers/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/samplers/combined.py` & `vis4d-0.1.1/vis4d/op/box/samplers/combined.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/samplers/pseudo.py` & `vis4d-0.1.1/vis4d/op/box/samplers/pseudo.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/box/samplers/random.py` & `vis4d-0.1.1/vis4d/op/box/samplers/random.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect/dense_anchor.py` & `vis4d-0.1.1/vis4d/op/detect/dense_anchor.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect/faster_rcnn.py` & `vis4d-0.1.1/vis4d/op/detect/faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect/mask_rcnn.py` & `vis4d-0.1.1/vis4d/op/detect/mask_rcnn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect/rcnn.py` & `vis4d-0.1.1/vis4d/op/detect/rcnn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect/retinanet.py` & `vis4d-0.1.1/vis4d/op/detect/retinanet.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect/rpn.py` & `vis4d-0.1.1/vis4d/op/detect/rpn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect/yolox.py` & `vis4d-0.1.1/vis4d/op/detect/yolox.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect3d/bevformer/bevformer.py` & `vis4d-0.1.1/vis4d/op/detect3d/bevformer/bevformer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect3d/bevformer/decoder.py` & `vis4d-0.1.1/vis4d/op/detect3d/bevformer/decoder.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect3d/bevformer/encoder.py` & `vis4d-0.1.1/vis4d/op/detect3d/bevformer/encoder.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect3d/bevformer/grid_mask.py` & `vis4d-0.1.1/vis4d/op/detect3d/bevformer/grid_mask.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect3d/bevformer/spatial_cross_attention.py` & `vis4d-0.1.1/vis4d/op/detect3d/bevformer/spatial_cross_attention.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect3d/bevformer/temporal_self_attention.py` & `vis4d-0.1.1/vis4d/op/detect3d/bevformer/temporal_self_attention.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect3d/bevformer/transformer.py` & `vis4d-0.1.1/vis4d/op/detect3d/bevformer/transformer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect3d/common.py` & `vis4d-0.1.1/vis4d/op/detect3d/common.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect3d/qd_3dt.py` & `vis4d-0.1.1/vis4d/op/detect3d/qd_3dt.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/detect3d/util.py` & `vis4d-0.1.1/vis4d/op/detect3d/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/fpp/base.py` & `vis4d-0.1.1/vis4d/op/fpp/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/fpp/dla_up.py` & `vis4d-0.1.1/vis4d/op/fpp/dla_up.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/fpp/fpn.py` & `vis4d-0.1.1/vis4d/op/fpp/fpn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/fpp/yolox_pafpn.py` & `vis4d-0.1.1/vis4d/op/fpp/yolox_pafpn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/geometry/projection.py` & `vis4d-0.1.1/vis4d/op/geometry/projection.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/geometry/rotation.py` & `vis4d-0.1.1/vis4d/op/geometry/rotation.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/geometry/transform.py` & `vis4d-0.1.1/vis4d/op/geometry/transform.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/__init__.py` & `vis4d-0.1.1/vis4d/op/layer/__init__.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/attention.py` & `vis4d-0.1.1/vis4d/op/layer/attention.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/conv2d.py` & `vis4d-0.1.1/vis4d/op/layer/conv2d.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/csp_layer.py` & `vis4d-0.1.1/vis4d/op/layer/csp_layer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/deform_conv.py` & `vis4d-0.1.1/vis4d/op/layer/deform_conv.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/drop.py` & `vis4d-0.1.1/vis4d/op/layer/drop.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/mlp.py` & `vis4d-0.1.1/vis4d/op/layer/mlp.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/ms_deform_attn.py` & `vis4d-0.1.1/vis4d/op/layer/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/patch_embed.py` & `vis4d-0.1.1/vis4d/op/layer/patch_embed.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/positional_encoding.py` & `vis4d-0.1.1/vis4d/op/layer/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/transformer.py` & `vis4d-0.1.1/vis4d/op/layer/transformer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/util.py` & `vis4d-0.1.1/vis4d/op/layer/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/layer/weight_init.py` & `vis4d-0.1.1/vis4d/op/layer/weight_init.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/loss/__init__.py` & `vis4d-0.1.1/vis4d/op/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/loss/base.py` & `vis4d-0.1.1/vis4d/op/loss/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/loss/common.py` & `vis4d-0.1.1/vis4d/op/loss/common.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/loss/cross_entropy.py` & `vis4d-0.1.1/vis4d/op/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/loss/embedding_distance.py` & `vis4d-0.1.1/vis4d/op/loss/embedding_distance.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/loss/iou_loss.py` & `vis4d-0.1.1/vis4d/op/loss/iou_loss.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/loss/multi_level_seg_loss.py` & `vis4d-0.1.1/vis4d/op/loss/multi_level_seg_loss.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/loss/multi_pos_cross_entropy.py` & `vis4d-0.1.1/vis4d/op/loss/multi_pos_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/loss/orthogonal_transform_loss.py` & `vis4d-0.1.1/vis4d/op/loss/orthogonal_transform_loss.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/loss/reducer.py` & `vis4d-0.1.1/vis4d/op/loss/reducer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/loss/seg_cross_entropy_loss.py` & `vis4d-0.1.1/vis4d/op/loss/seg_cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/mask/util.py` & `vis4d-0.1.1/vis4d/op/mask/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/motion/kalman_filter.py` & `vis4d-0.1.1/vis4d/op/motion/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/motion/velo_lstm.py` & `vis4d-0.1.1/vis4d/op/motion/velo_lstm.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/seg/fcn.py` & `vis4d-0.1.1/vis4d/op/seg/fcn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/seg/semantic_fpn.py` & `vis4d-0.1.1/vis4d/op/seg/semantic_fpn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/track/assignment.py` & `vis4d-0.1.1/vis4d/op/track/assignment.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/track/common.py` & `vis4d-0.1.1/vis4d/op/track/common.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/track/matching.py` & `vis4d-0.1.1/vis4d/op/track/matching.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/track/qdtrack.py` & `vis4d-0.1.1/vis4d/op/track/qdtrack.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/track3d/cc_3dt.py` & `vis4d-0.1.1/vis4d/op/track3d/cc_3dt.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/track3d/common.py` & `vis4d-0.1.1/vis4d/op/track3d/common.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/op/util.py` & `vis4d-0.1.1/vis4d/op/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/pl/callbacks/callback_wrapper.py` & `vis4d-0.1.1/vis4d/pl/callbacks/callback_wrapper.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/pl/callbacks/scheduler.py` & `vis4d-0.1.1/vis4d/pl/callbacks/scheduler.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/pl/data_module.py` & `vis4d-0.1.1/vis4d/pl/data_module.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/pl/run.py` & `vis4d-0.1.1/vis4d/pl/run.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/pl/trainer.py` & `vis4d-0.1.1/vis4d/pl/trainer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/pl/training_module.py` & `vis4d-0.1.1/vis4d/pl/training_module.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/state/track/qdtrack.py` & `vis4d-0.1.1/vis4d/state/track/qdtrack.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/state/track3d/cc_3dt.py` & `vis4d-0.1.1/vis4d/state/track3d/cc_3dt.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/state/track3d/motion/base.py` & `vis4d-0.1.1/vis4d/state/track3d/motion/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/state/track3d/motion/kf3d.py` & `vis4d-0.1.1/vis4d/state/track3d/motion/kf3d.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/state/track3d/motion/lstm_3d.py` & `vis4d-0.1.1/vis4d/state/track3d/motion/lstm_3d.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/base.py` & `vis4d-0.1.1/vis4d/vis/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/functional/image.py` & `vis4d-0.1.1/vis4d/vis/functional/image.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/functional/pointcloud.py` & `vis4d-0.1.1/vis4d/vis/functional/pointcloud.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/image/bbox3d_visualizer.py` & `vis4d-0.1.1/vis4d/vis/image/bbox3d_visualizer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/image/bev_visualizer.py` & `vis4d-0.1.1/vis4d/vis/image/bev_visualizer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/image/bounding_box_visualizer.py` & `vis4d-0.1.1/vis4d/vis/image/bounding_box_visualizer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/image/canvas/base.py` & `vis4d-0.1.1/vis4d/vis/image/canvas/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/image/canvas/pillow_backend.py` & `vis4d-0.1.1/vis4d/vis/image/canvas/pillow_backend.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/image/seg_mask_visualizer.py` & `vis4d-0.1.1/vis4d/vis/image/seg_mask_visualizer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/image/util.py` & `vis4d-0.1.1/vis4d/vis/image/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/image/viewer/base.py` & `vis4d-0.1.1/vis4d/vis/image/viewer/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/image/viewer/matplotlib_viewer.py` & `vis4d-0.1.1/vis4d/vis/image/viewer/matplotlib_viewer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/pointcloud/pointcloud_visualizer.py` & `vis4d-0.1.1/vis4d/vis/pointcloud/pointcloud_visualizer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/pointcloud/scene.py` & `vis4d-0.1.1/vis4d/vis/pointcloud/scene.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/pointcloud/viewer/base.py` & `vis4d-0.1.1/vis4d/vis/pointcloud/viewer/base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/pointcloud/viewer/open3d_viewer.py` & `vis4d-0.1.1/vis4d/vis/pointcloud/viewer/open3d_viewer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/vis/util.py` & `vis4d-0.1.1/vis4d/vis/util.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/__init__.py` & `vis4d-0.1.1/vis4d/zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/__init__.py` & `vis4d-0.1.1/vis4d/zoo/base/__init__.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/callable.py` & `vis4d-0.1.1/vis4d/zoo/base/callable.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/data_connectors/detection.py` & `vis4d-0.1.1/vis4d/zoo/base/data_connectors/detection.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/data_connectors/seg.py` & `vis4d-0.1.1/vis4d/zoo/base/data_connectors/seg.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/data_connectors/visualizers.py` & `vis4d-0.1.1/vis4d/zoo/base/data_connectors/visualizers.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/dataloader.py` & `vis4d-0.1.1/vis4d/zoo/base/dataloader.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/detect.py` & `vis4d-0.1.1/vis4d/zoo/base/datasets/bdd100k/detect.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/sem_seg.py` & `vis4d-0.1.1/vis4d/zoo/base/datasets/bdd100k/sem_seg.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/datasets/bdd100k/track.py` & `vis4d-0.1.1/vis4d/zoo/base/datasets/bdd100k/track.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/datasets/coco/detection.py` & `vis4d-0.1.1/vis4d/zoo/base/datasets/coco/detection.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/datasets/coco/sem_seg.py` & `vis4d-0.1.1/vis4d/zoo/base/datasets/coco/sem_seg.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/datasets/imagenet.py` & `vis4d-0.1.1/vis4d/zoo/base/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/datasets/nuscenes/nuscenes.py` & `vis4d-0.1.1/vis4d/zoo/base/datasets/nuscenes/nuscenes.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/datasets/nuscenes/nuscenes_mono.py` & `vis4d-0.1.1/vis4d/zoo/base/datasets/nuscenes/nuscenes_mono.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/datasets/shift/__init__.py` & `vis4d-0.1.1/vis4d/zoo/base/datasets/shift/__init__.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/datasets/shift/common.py` & `vis4d-0.1.1/vis4d/zoo/base/datasets/shift/common.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/datasets/shift/tasks.py` & `vis4d-0.1.1/vis4d/zoo/base/datasets/shift/tasks.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/models/faster_rcnn.py` & `vis4d-0.1.1/vis4d/zoo/base/models/faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/models/mask_rcnn.py` & `vis4d-0.1.1/vis4d/zoo/base/models/mask_rcnn.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/models/qdtrack.py` & `vis4d-0.1.1/vis4d/zoo/base/models/qdtrack.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/models/yolox.py` & `vis4d-0.1.1/vis4d/zoo/base/models/yolox.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/optimizer.py` & `vis4d-0.1.1/vis4d/zoo/base/optimizer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/pl_trainer.py` & `vis4d-0.1.1/vis4d/zoo/base/pl_trainer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/base/runtime.py` & `vis4d-0.1.1/vis4d/zoo/base/runtime.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bdd100k/__init__.py` & `vis4d-0.1.1/vis4d/zoo/bdd100k/__init__.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bdd100k/faster_rcnn/faster_rcnn_r50_1x_bdd100k.py` & `vis4d-0.1.1/vis4d/zoo/bdd100k/faster_rcnn/faster_rcnn_r50_1x_bdd100k.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bdd100k/faster_rcnn/faster_rcnn_r50_3x_bdd100k.py` & `vis4d-0.1.1/vis4d/zoo/bdd100k/faster_rcnn/faster_rcnn_r50_3x_bdd100k.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_1x_bdd100k.py` & `vis4d-0.1.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_1x_bdd100k.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_3x_bdd100k.py` & `vis4d-0.1.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_3x_bdd100k.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_5x_bdd100k.py` & `vis4d-0.1.1/vis4d/zoo/bdd100k/mask_rcnn/mask_rcnn_r50_5x_bdd100k.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bdd100k/qdtrack/qdtrack_frcnn_r50_fpn_1x_bdd100k.py` & `vis4d-0.1.1/vis4d/zoo/bdd100k/qdtrack/qdtrack_frcnn_r50_fpn_1x_bdd100k.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r101_80k_bdd100k.py` & `vis4d-0.1.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r101_80k_bdd100k.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r50_40k_bdd100k.py` & `vis4d-0.1.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r50_40k_bdd100k.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r50_80k_bdd100k.py` & `vis4d-0.1.1/vis4d/zoo/bdd100k/semantic_fpn/semantic_fpn_r50_80k_bdd100k.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bevformer/bevformer_base.py` & `vis4d-0.1.1/vis4d/zoo/bevformer/bevformer_base.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bevformer/bevformer_tiny.py` & `vis4d-0.1.1/vis4d/zoo/bevformer/bevformer_tiny.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bevformer/bevformer_vis.py` & `vis4d-0.1.1/vis4d/zoo/bevformer/bevformer_vis.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/bevformer/data.py` & `vis4d-0.1.1/vis4d/zoo/bevformer/data.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/cc_3dt/__init__.py` & `vis4d-0.1.1/vis4d/zoo/cc_3dt/__init__.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_bevformer_base_velo_lstm_nusc.py` & `vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_bevformer_base_velo_lstm_nusc.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_kf3d_24e_nusc.py` & `vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_kf3d_24e_nusc.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_pure_det_nusc.py` & `vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_pure_det_nusc.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_velo_lstm_24e_nusc.py` & `vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r101_fpn_velo_lstm_24e_nusc.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r50_fpn_kf3d_12e_nusc.py` & `vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_frcnn_r50_fpn_kf3d_12e_nusc.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_nusc_test.py` & `vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_nusc_test.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/cc_3dt/cc_3dt_nusc_vis.py` & `vis4d-0.1.1/vis4d/zoo/cc_3dt/cc_3dt_nusc_vis.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/cc_3dt/data.py` & `vis4d-0.1.1/vis4d/zoo/cc_3dt/data.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/cc_3dt/model.py` & `vis4d-0.1.1/vis4d/zoo/cc_3dt/model.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/cc_3dt/velo_lstm_bevformer_base_100e_nusc.py` & `vis4d-0.1.1/vis4d/zoo/cc_3dt/velo_lstm_bevformer_base_100e_nusc.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/cc_3dt/velo_lstm_frcnn_r101_fpn_100e_nusc.py` & `vis4d-0.1.1/vis4d/zoo/cc_3dt/velo_lstm_frcnn_r101_fpn_100e_nusc.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/faster_rcnn/faster_rcnn_coco.py` & `vis4d-0.1.1/vis4d/zoo/faster_rcnn/faster_rcnn_coco.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/fcn_resnet/fcn_resnet_coco.py` & `vis4d-0.1.1/vis4d/zoo/fcn_resnet/fcn_resnet_coco.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/mask_rcnn/mask_rcnn_coco.py` & `vis4d-0.1.1/vis4d/zoo/mask_rcnn/mask_rcnn_coco.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/qdtrack/data_yolox.py` & `vis4d-0.1.1/vis4d/zoo/qdtrack/data_yolox.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/qdtrack/qdtrack_frcnn_r50_fpn_augs_1x_bdd100k.py` & `vis4d-0.1.1/vis4d/zoo/qdtrack/qdtrack_frcnn_r50_fpn_augs_1x_bdd100k.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/qdtrack/qdtrack_yolox_x_25e_bdd100k.py` & `vis4d-0.1.1/vis4d/zoo/qdtrack/qdtrack_yolox_x_25e_bdd100k.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/retinanet/retinanet_coco.py` & `vis4d-0.1.1/vis4d/zoo/retinanet/retinanet_coco.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/run.py` & `vis4d-0.1.1/vis4d/zoo/run.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/shift/__init__.py` & `vis4d-0.1.1/vis4d/zoo/shift/__init__.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_12e_shift.py` & `vis4d-0.1.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_12e_shift.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_36e_shift.py` & `vis4d-0.1.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_36e_shift.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_6e_shift_all_domains.py` & `vis4d-0.1.1/vis4d/zoo/shift/faster_rcnn/faster_rcnn_r50_6e_shift_all_domains.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_12e_shift.py` & `vis4d-0.1.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_12e_shift.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_36e_shift.py` & `vis4d-0.1.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_36e_shift.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_6e_shift_all_domains.py` & `vis4d-0.1.1/vis4d/zoo/shift/mask_rcnn/mask_rcnn_r50_6e_shift_all_domains.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_160k_shift.py` & `vis4d-0.1.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_160k_shift.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_160k_shift_all_domains.py` & `vis4d-0.1.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_160k_shift_all_domains.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_40k_shift.py` & `vis4d-0.1.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_40k_shift.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_40k_shift_all_domains.py` & `vis4d-0.1.1/vis4d/zoo/shift/semantic_fpn/semantic_fpn_r50_40k_shift_all_domains.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/vit/vit_small_imagenet.py` & `vis4d-0.1.1/vis4d/zoo/vit/vit_small_imagenet.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/vit/vit_tiny_imagenet.py` & `vis4d-0.1.1/vis4d/zoo/vit/vit_tiny_imagenet.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/yolox/data.py` & `vis4d-0.1.1/vis4d/zoo/yolox/data.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/yolox/yolox_s_300e_coco.py` & `vis4d-0.1.1/vis4d/zoo/yolox/yolox_s_300e_coco.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d/zoo/yolox/yolox_tiny_300e_coco.py` & `vis4d-0.1.1/vis4d/zoo/yolox/yolox_tiny_300e_coco.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d-workspace/convert.py` & `vis4d-0.1.1/vis4d-workspace/convert.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d-workspace/convert_bevformer.py` & `vis4d-0.1.1/vis4d-workspace/convert_bevformer.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d-workspace/eval_nusc.py` & `vis4d-0.1.1/vis4d-workspace/eval_nusc.py`

 * *Files identical despite different names*

### Comparing `vis4d-0.1/vis4d.egg-info/PKG-INFO` & `vis4d-0.1.1/vis4d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: vis4d
-Version: 0.1
+Version: 0.1.1
 Summary: Vis4D Python package for Visual 4D scene understanding
 Author-email: "VIS @ ETH" <i@yf.io>
 License: Apache 2.0
-Project-URL: Documentation, https://vis.xyz/4d/
+Project-URL: Documentation, https://docs.vis.xyz/4d
 Project-URL: Source, https://github.com/syscv/vis4d
 Project-URL: Tracker, https://github.com/syscv/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.0
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: appdirs
 Requires-Dist: cloudpickle
 Requires-Dist: cython
 Requires-Dist: devtools
@@ -30,16 +30,16 @@
 Requires-Dist: pycocotools
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: setuptools
 Requires-Dist: tensorboard
 Requires-Dist: termcolor
 Requires-Dist: terminaltables
 Requires-Dist: timm>=0.6.0
-Requires-Dist: torch>=1.10
-Requires-Dist: torchvision>=0.11
+Requires-Dist: torch>=2.0.0
+Requires-Dist: torchvision>=0.15.1
 Requires-Dist: tqdm
 Requires-Dist: utm
 Requires-Dist: wheel
 Requires-Dist: bdd100k
 Requires-Dist: scalabel
 Requires-Dist: nuscenes-devkit
 
@@ -150,15 +150,15 @@
 **Project Leads**
 - [Yung-Hsu Yang](https://royyang0714.github.io/)*
 - [Tobias Fischer](https://tobiasfshr.github.io/)*
  
 **Core Contributors**
 - [Thomas E. Huang](https://www.thomasehuang.com/)
 - [Tao Sun](https://www.suniique.com/)
-- [René Zurbrügg](https://github.com/renezurbruegg)
+- [René Zurbrügg](https://renezurbruegg.github.io/)
  
 **Advisors**
 - [Fisher Yu](https://www.yf.io/)
  
 `*` denotes equal contribution
 
 **We are open to contributions and suggestions, feel free to reach out to us.**
```

### Comparing `vis4d-0.1/vis4d.egg-info/SOURCES.txt` & `vis4d-0.1.1/vis4d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

