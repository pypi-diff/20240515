# Comparing `tmp/basetrainer-0.8.2.tar.gz` & `tmp/basetrainer-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basetrainer-0.8.2.tar", last modified: Mon Mar 25 00:35:42 2024, max compression
+gzip compressed data, was "basetrainer-0.8.3.tar", last modified: Wed May 15 09:01:24 2024, max compression
```

## Comparing `basetrainer-0.8.2.tar` & `basetrainer-0.8.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:37.000000 basetrainer-0.8.2/
--rwxrwx---   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 basetrainer-0.8.2/LICENCE
--rw-r-----   0 PKing     (1000) PKing     (1000)      226 2024-03-25 00:35:37.000000 basetrainer-0.8.2/PKG-INFO
--rw-r-----   0 PKing     (1000) PKing     (1000)    17572 2023-08-24 03:00:36.000000 basetrainer-0.8.2/README.rst
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:34.000000 basetrainer-0.8.2/basetrainer/
--rw-r-----   0 PKing     (1000) PKing     (1000)      141 2024-03-25 00:35:31.000000 basetrainer-0.8.2/basetrainer/__init__.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:34.000000 basetrainer-0.8.2/basetrainer/callbacks/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/callbacks/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     1166 2022-01-26 04:35:31.000000 basetrainer-0.8.2/basetrainer/callbacks/callbacks.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     3127 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/callbacks/log_history.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     1497 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/callbacks/losses_recorder.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     7368 2024-02-21 04:38:14.000000 basetrainer-0.8.2/basetrainer/callbacks/model_checkpoint.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     3208 2022-02-08 08:35:30.000000 basetrainer-0.8.2/basetrainer/callbacks/multi_losses_recorder.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:34.000000 basetrainer-0.8.2/basetrainer/criterion/
--rwxrwx---   0 PKing     (1000) PKing     (1000)        1 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/criterion/__init__.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     4592 2023-03-17 10:16:56.000000 basetrainer-0.8.2/basetrainer/criterion/criterion.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:34.000000 basetrainer-0.8.2/basetrainer/dataloader/
--rw-r-----   0 PKing     (1000) PKing     (1000)      114 2024-03-25 00:30:25.000000 basetrainer-0.8.2/basetrainer/dataloader/__init__.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     8310 2024-03-25 00:31:08.000000 basetrainer-0.8.2/basetrainer/dataloader/data_resample.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:35.000000 basetrainer-0.8.2/basetrainer/engine/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/engine/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     1510 2022-01-26 04:35:31.000000 basetrainer-0.8.2/basetrainer/engine/base.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     7863 2022-01-17 09:22:27.000000 basetrainer-0.8.2/basetrainer/engine/comm.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     5377 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/engine/engine.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     3920 2022-01-17 09:22:27.000000 basetrainer-0.8.2/basetrainer/engine/launch.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)     3082 2023-12-18 08:58:42.000000 basetrainer-0.8.2/basetrainer/engine/onnx_engine.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     5101 2023-12-18 08:58:42.000000 basetrainer-0.8.2/basetrainer/engine/trainer.py
--rw-r-----   0 PKing     (1000) PKing     (1000)    12287 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/engine/trt_engine.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:35.000000 basetrainer-0.8.2/basetrainer/metric/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/metric/__init__.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     4328 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/metric/accuracy_recorder.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:35.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/
--rwxrwx---   0 PKing     (1000) PKing     (1000)      168 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/__init__.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     3122 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/acc.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)     5457 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/classification_report.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     6586 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/eval_utils.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     1634 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/evaluate.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     2071 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/iou.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     4905 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/metrics.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     1424 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/pandas_tools.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     9529 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/pr.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     2469 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/psnr.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     7712 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/roc.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     7781 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/metric/eval_tools/verification.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:35.000000 basetrainer-0.8.2/basetrainer/metric/map_tools/
--rw-r-----   0 PKing     (1000) PKing     (1000)      114 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/metric/map_tools/__init__.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:35.000000 basetrainer-0.8.2/basetrainer/metric/map_tools/evaluator/
--rw-r-----   0 PKing     (1000) PKing     (1000)      119 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/metric/map_tools/evaluator/__init__.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)     7291 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/metric/map_tools/evaluator/bboxes_match.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)     2741 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/metric/map_tools/evaluator/iou.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)    10147 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/metric/map_tools/evaluator/map_eval.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)     6100 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/metric/map_tools/evaluator/map_eval_torch.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)     6477 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/metric/map_tools/map_metric.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:36.000000 basetrainer-0.8.2/basetrainer/models/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2022-01-17 09:46:24.000000 basetrainer-0.8.2/basetrainer/models/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     3339 2023-12-18 08:57:10.000000 basetrainer-0.8.2/basetrainer/models/build_models.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:36.000000 basetrainer-0.8.2/basetrainer/optimizer/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/optimizer/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     2588 2023-03-17 10:16:56.000000 basetrainer-0.8.2/basetrainer/optimizer/build_optimizer.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:36.000000 basetrainer-0.8.2/basetrainer/pruning/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.8.2/basetrainer/pruning/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)    11795 2024-02-20 01:18:45.000000 basetrainer-0.8.2/basetrainer/pruning/nni_pruning.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     2693 2022-01-17 09:22:27.000000 basetrainer-0.8.2/basetrainer/pruning/slim_pruning.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     6843 2021-12-28 07:55:24.000000 basetrainer-0.8.2/basetrainer/pruning/torch_pruning.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:36.000000 basetrainer-0.8.2/basetrainer/scheduler/
--rw-rw----   0 PKing     (1000) PKing     (1000)     2981 2023-12-20 01:45:34.000000 basetrainer-0.8.2/basetrainer/scheduler/CosineAnnealingLR.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     2141 2023-12-26 11:07:58.000000 basetrainer-0.8.2/basetrainer/scheduler/ExponentialLR.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     2633 2022-12-16 02:49:37.000000 basetrainer-0.8.2/basetrainer/scheduler/LambdaLR.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     3018 2021-12-28 07:55:23.000000 basetrainer-0.8.2/basetrainer/scheduler/MultiStepLR.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     4378 2021-12-28 07:55:24.000000 basetrainer-0.8.2/basetrainer/scheduler/MultiStepValue.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     1657 2021-12-28 07:55:24.000000 basetrainer-0.8.2/basetrainer/scheduler/WarmUpLR.py
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.8.2/basetrainer/scheduler/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     2150 2022-12-16 02:49:37.000000 basetrainer-0.8.2/basetrainer/scheduler/build_scheduler.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:37.000000 basetrainer-0.8.2/basetrainer/utils/
--rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.8.2/basetrainer/utils/__init__.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:37.000000 basetrainer-0.8.2/basetrainer/utils/converter/
--rw-rw----   0 PKing     (1000) PKing     (1000)      130 2023-01-05 11:21:37.000000 basetrainer-0.8.2/basetrainer/utils/converter/__init__.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     2764 2023-01-05 11:21:37.000000 basetrainer-0.8.2/basetrainer/utils/converter/onnx2trt.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     3147 2023-12-28 02:54:06.000000 basetrainer-0.8.2/basetrainer/utils/converter/pytorch2onnx.py
--rw-r-----   0 PKing     (1000) PKing     (1000)      151 2023-12-18 08:58:42.000000 basetrainer-0.8.2/basetrainer/utils/file_utils.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     5722 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/utils/heatmap_utils.py
--rw-r-----   0 PKing     (1000) PKing     (1000)      152 2023-12-18 08:58:42.000000 basetrainer-0.8.2/basetrainer/utils/image_utils.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     6849 2023-01-05 11:21:37.000000 basetrainer-0.8.2/basetrainer/utils/log.py
--rwxrwx---   0 PKing     (1000) PKing     (1000)     3781 2022-01-26 04:35:31.000000 basetrainer-0.8.2/basetrainer/utils/plot_utils.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     5037 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/utils/setup_config.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     1399 2021-12-28 07:55:24.000000 basetrainer-0.8.2/basetrainer/utils/summary.py
--rw-rw----   0 PKing     (1000) PKing     (1000)     4171 2023-01-05 11:21:37.000000 basetrainer-0.8.2/basetrainer/utils/torch_data.py
--rwxr-x---   0 PKing     (1000) PKing     (1000)    17131 2024-02-20 01:20:42.000000 basetrainer-0.8.2/basetrainer/utils/torch_tools.py
--rw-r-----   0 PKing     (1000) PKing     (1000)     6261 2023-08-24 03:00:36.000000 basetrainer-0.8.2/basetrainer/utils/torchcam_utils.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:34.000000 basetrainer-0.8.2/basetrainer.egg-info/
--rw-r-----   0 PKing     (1000) PKing     (1000)      226 2024-03-25 00:35:34.000000 basetrainer-0.8.2/basetrainer.egg-info/PKG-INFO
--rw-r-----   0 PKing     (1000) PKing     (1000)     2842 2024-03-25 00:35:34.000000 basetrainer-0.8.2/basetrainer.egg-info/SOURCES.txt
--rw-r-----   0 PKing     (1000) PKing     (1000)        1 2024-03-25 00:35:34.000000 basetrainer-0.8.2/basetrainer.egg-info/dependency_links.txt
--rw-r-----   0 PKing     (1000) PKing     (1000)        1 2023-08-23 09:06:15.000000 basetrainer-0.8.2/basetrainer.egg-info/not-zip-safe
--rw-r-----   0 PKing     (1000) PKing     (1000)       12 2024-03-25 00:35:34.000000 basetrainer-0.8.2/basetrainer.egg-info/top_level.txt
--rw-r-----   0 PKing     (1000) PKing     (1000)       38 2024-03-25 00:35:37.000000 basetrainer-0.8.2/setup.cfg
--rwxr-x---   0 PKing     (1000) PKing     (1000)     2115 2023-08-24 03:00:36.000000 basetrainer-0.8.2/setup.py
-drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-03-25 00:35:37.000000 basetrainer-0.8.2/test/
--rw-rw----   0 PKing     (1000) PKing     (1000)     3179 2023-12-26 11:08:42.000000 basetrainer-0.8.2/test/test_scheduler.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 basetrainer-0.8.3/LICENCE
+-rw-r-----   0 PKing     (1000) PKing     (1000)      254 2024-05-15 09:01:14.000000 basetrainer-0.8.3/PKG-INFO
+-rw-r-----   0 PKing     (1000) PKing     (1000)    17572 2023-08-24 03:00:36.000000 basetrainer-0.8.3/README.rst
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer/
+-rw-r-----   0 PKing     (1000) PKing     (1000)      141 2024-05-15 09:01:07.000000 basetrainer-0.8.3/basetrainer/__init__.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer/callbacks/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/callbacks/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     1166 2022-01-26 04:35:31.000000 basetrainer-0.8.3/basetrainer/callbacks/callbacks.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     3127 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/callbacks/log_history.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     1497 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/callbacks/losses_recorder.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     7368 2024-02-21 04:38:14.000000 basetrainer-0.8.3/basetrainer/callbacks/model_checkpoint.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     3208 2022-02-08 08:35:30.000000 basetrainer-0.8.3/basetrainer/callbacks/multi_losses_recorder.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer/criterion/
+-rwxrwx---   0 PKing     (1000) PKing     (1000)        1 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/criterion/__init__.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     4592 2023-03-17 10:16:56.000000 basetrainer-0.8.3/basetrainer/criterion/criterion.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer/dataloader/
+-rw-r-----   0 PKing     (1000) PKing     (1000)      114 2024-03-25 00:30:25.000000 basetrainer-0.8.3/basetrainer/dataloader/__init__.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     8310 2024-03-25 00:31:08.000000 basetrainer-0.8.3/basetrainer/dataloader/data_resample.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer/engine/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/engine/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     1510 2022-01-26 04:35:31.000000 basetrainer-0.8.3/basetrainer/engine/base.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     7863 2022-01-17 09:22:27.000000 basetrainer-0.8.3/basetrainer/engine/comm.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     5377 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/engine/engine.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     3920 2022-01-17 09:22:27.000000 basetrainer-0.8.3/basetrainer/engine/launch.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     3082 2023-12-18 08:58:42.000000 basetrainer-0.8.3/basetrainer/engine/onnx_engine.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     5101 2023-12-18 08:58:42.000000 basetrainer-0.8.3/basetrainer/engine/trainer.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)    12287 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/engine/trt_engine.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer/metric/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/__init__.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     4328 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/accuracy_recorder.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/
+-rwxrwx---   0 PKing     (1000) PKing     (1000)      168 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/__init__.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     3122 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/acc.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     5457 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/classification_report.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     6586 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/eval_utils.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     1634 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/evaluate.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     2071 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/iou.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     4905 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/metrics.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     1424 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/pandas_tools.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     9529 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/pr.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     2469 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/psnr.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     7712 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/roc.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     7781 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/metric/eval_tools/verification.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/
+-rw-r-----   0 PKing     (1000) PKing     (1000)      114 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/__init__.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/
+-rw-r-----   0 PKing     (1000) PKing     (1000)      119 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/__init__.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     7291 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/bboxes_match.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     2741 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/iou.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)    10147 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/map_eval.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     6100 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/map_eval_torch.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     6477 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/metric/map_tools/map_metric.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/models/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2022-01-17 09:46:24.000000 basetrainer-0.8.3/basetrainer/models/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     3339 2023-12-18 08:57:10.000000 basetrainer-0.8.3/basetrainer/models/build_models.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/optimizer/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/optimizer/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2588 2023-03-17 10:16:56.000000 basetrainer-0.8.3/basetrainer/optimizer/build_optimizer.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/pruning/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/pruning/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)    11795 2024-02-20 01:18:45.000000 basetrainer-0.8.3/basetrainer/pruning/nni_pruning.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2693 2022-01-17 09:22:27.000000 basetrainer-0.8.3/basetrainer/pruning/slim_pruning.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     6843 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/pruning/torch_pruning.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/scheduler/
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2981 2023-12-20 01:45:34.000000 basetrainer-0.8.3/basetrainer/scheduler/CosineAnnealingLR.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2141 2023-12-26 11:07:58.000000 basetrainer-0.8.3/basetrainer/scheduler/ExponentialLR.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2633 2022-12-16 02:49:37.000000 basetrainer-0.8.3/basetrainer/scheduler/LambdaLR.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     3018 2021-12-28 07:55:23.000000 basetrainer-0.8.3/basetrainer/scheduler/MultiStepLR.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     4378 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/scheduler/MultiStepValue.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     1657 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/scheduler/WarmUpLR.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/scheduler/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2150 2022-12-16 02:49:37.000000 basetrainer-0.8.3/basetrainer/scheduler/build_scheduler.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/utils/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/utils/__init__.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/basetrainer/utils/converter/
+-rw-rw----   0 PKing     (1000) PKing     (1000)      130 2023-01-05 11:21:37.000000 basetrainer-0.8.3/basetrainer/utils/converter/__init__.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     2764 2023-01-05 11:21:37.000000 basetrainer-0.8.3/basetrainer/utils/converter/onnx2trt.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     3147 2023-12-28 02:54:06.000000 basetrainer-0.8.3/basetrainer/utils/converter/pytorch2onnx.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)      151 2023-12-18 08:58:42.000000 basetrainer-0.8.3/basetrainer/utils/file_utils.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     5722 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/utils/heatmap_utils.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)      152 2023-12-18 08:58:42.000000 basetrainer-0.8.3/basetrainer/utils/image_utils.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     6849 2023-01-05 11:21:37.000000 basetrainer-0.8.3/basetrainer/utils/log.py
+-rwxrwx---   0 PKing     (1000) PKing     (1000)     3781 2022-01-26 04:35:31.000000 basetrainer-0.8.3/basetrainer/utils/plot_utils.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     5037 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/utils/setup_config.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     1399 2021-12-28 07:55:24.000000 basetrainer-0.8.3/basetrainer/utils/summary.py
+-rw-rw----   0 PKing     (1000) PKing     (1000)     4171 2023-01-05 11:21:37.000000 basetrainer-0.8.3/basetrainer/utils/torch_data.py
+-rwxr-x---   0 PKing     (1000) PKing     (1000)    17572 2024-05-15 09:01:07.000000 basetrainer-0.8.3/basetrainer/utils/torch_tools.py
+-rw-r-----   0 PKing     (1000) PKing     (1000)     6261 2023-08-24 03:00:36.000000 basetrainer-0.8.3/basetrainer/utils/torchcam_utils.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer.egg-info/
+-rw-r-----   0 PKing     (1000) PKing     (1000)      254 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer.egg-info/PKG-INFO
+-rw-r-----   0 PKing     (1000) PKing     (1000)     2842 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer.egg-info/SOURCES.txt
+-rw-r-----   0 PKing     (1000) PKing     (1000)        1 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer.egg-info/dependency_links.txt
+-rw-r-----   0 PKing     (1000) PKing     (1000)        1 2023-08-23 09:06:15.000000 basetrainer-0.8.3/basetrainer.egg-info/not-zip-safe
+-rw-r-----   0 PKing     (1000) PKing     (1000)       12 2024-05-15 09:01:13.000000 basetrainer-0.8.3/basetrainer.egg-info/top_level.txt
+-rw-r-----   0 PKing     (1000) PKing     (1000)       38 2024-05-15 09:01:14.000000 basetrainer-0.8.3/setup.cfg
+-rwxr-x---   0 PKing     (1000) PKing     (1000)     2115 2023-08-24 03:00:36.000000 basetrainer-0.8.3/setup.py
+drwxr-x---   0 PKing     (1000) PKing     (1000)        0 2024-05-15 09:01:14.000000 basetrainer-0.8.3/test/
+-rw-rw----   0 PKing     (1000) PKing     (1000)     3179 2023-12-26 11:08:42.000000 basetrainer-0.8.3/test/test_scheduler.py
```

### Comparing `basetrainer-0.8.2/LICENCE` & `basetrainer-0.8.3/LICENCE`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/README.rst` & `basetrainer-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/callbacks/callbacks.py` & `basetrainer-0.8.3/basetrainer/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/callbacks/log_history.py` & `basetrainer-0.8.3/basetrainer/callbacks/log_history.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/callbacks/losses_recorder.py` & `basetrainer-0.8.3/basetrainer/callbacks/losses_recorder.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/callbacks/model_checkpoint.py` & `basetrainer-0.8.3/basetrainer/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/callbacks/multi_losses_recorder.py` & `basetrainer-0.8.3/basetrainer/callbacks/multi_losses_recorder.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/criterion/criterion.py` & `basetrainer-0.8.3/basetrainer/criterion/criterion.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/dataloader/data_resample.py` & `basetrainer-0.8.3/basetrainer/dataloader/data_resample.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/engine/base.py` & `basetrainer-0.8.3/basetrainer/engine/base.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/engine/comm.py` & `basetrainer-0.8.3/basetrainer/engine/comm.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/engine/engine.py` & `basetrainer-0.8.3/basetrainer/engine/engine.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/engine/launch.py` & `basetrainer-0.8.3/basetrainer/engine/launch.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/engine/onnx_engine.py` & `basetrainer-0.8.3/basetrainer/engine/onnx_engine.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/engine/trainer.py` & `basetrainer-0.8.3/basetrainer/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/engine/trt_engine.py` & `basetrainer-0.8.3/basetrainer/engine/trt_engine.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/accuracy_recorder.py` & `basetrainer-0.8.3/basetrainer/metric/accuracy_recorder.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/eval_tools/acc.py` & `basetrainer-0.8.3/basetrainer/metric/eval_tools/acc.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/eval_tools/classification_report.py` & `basetrainer-0.8.3/basetrainer/metric/eval_tools/classification_report.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/eval_tools/eval_utils.py` & `basetrainer-0.8.3/basetrainer/metric/eval_tools/eval_utils.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/eval_tools/evaluate.py` & `basetrainer-0.8.3/basetrainer/metric/eval_tools/evaluate.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/eval_tools/iou.py` & `basetrainer-0.8.3/basetrainer/metric/eval_tools/iou.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/eval_tools/metrics.py` & `basetrainer-0.8.3/basetrainer/metric/eval_tools/metrics.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/eval_tools/pandas_tools.py` & `basetrainer-0.8.3/basetrainer/metric/eval_tools/pandas_tools.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/eval_tools/pr.py` & `basetrainer-0.8.3/basetrainer/metric/eval_tools/pr.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/eval_tools/psnr.py` & `basetrainer-0.8.3/basetrainer/metric/eval_tools/psnr.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/eval_tools/roc.py` & `basetrainer-0.8.3/basetrainer/metric/eval_tools/roc.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/eval_tools/verification.py` & `basetrainer-0.8.3/basetrainer/metric/eval_tools/verification.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/map_tools/evaluator/bboxes_match.py` & `basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/bboxes_match.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/map_tools/evaluator/iou.py` & `basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/iou.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/map_tools/evaluator/map_eval.py` & `basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/map_eval.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/map_tools/evaluator/map_eval_torch.py` & `basetrainer-0.8.3/basetrainer/metric/map_tools/evaluator/map_eval_torch.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/metric/map_tools/map_metric.py` & `basetrainer-0.8.3/basetrainer/metric/map_tools/map_metric.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/models/build_models.py` & `basetrainer-0.8.3/basetrainer/models/build_models.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/optimizer/build_optimizer.py` & `basetrainer-0.8.3/basetrainer/optimizer/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/pruning/nni_pruning.py` & `basetrainer-0.8.3/basetrainer/pruning/nni_pruning.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/pruning/slim_pruning.py` & `basetrainer-0.8.3/basetrainer/pruning/slim_pruning.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/pruning/torch_pruning.py` & `basetrainer-0.8.3/basetrainer/pruning/torch_pruning.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/scheduler/CosineAnnealingLR.py` & `basetrainer-0.8.3/basetrainer/scheduler/CosineAnnealingLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/scheduler/ExponentialLR.py` & `basetrainer-0.8.3/basetrainer/scheduler/ExponentialLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/scheduler/LambdaLR.py` & `basetrainer-0.8.3/basetrainer/scheduler/LambdaLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/scheduler/MultiStepLR.py` & `basetrainer-0.8.3/basetrainer/scheduler/MultiStepLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/scheduler/MultiStepValue.py` & `basetrainer-0.8.3/basetrainer/scheduler/MultiStepValue.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/scheduler/WarmUpLR.py` & `basetrainer-0.8.3/basetrainer/scheduler/WarmUpLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/scheduler/build_scheduler.py` & `basetrainer-0.8.3/basetrainer/scheduler/build_scheduler.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/utils/converter/onnx2trt.py` & `basetrainer-0.8.3/basetrainer/utils/converter/onnx2trt.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/utils/converter/pytorch2onnx.py` & `basetrainer-0.8.3/basetrainer/utils/converter/pytorch2onnx.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/utils/heatmap_utils.py` & `basetrainer-0.8.3/basetrainer/utils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/utils/log.py` & `basetrainer-0.8.3/basetrainer/utils/log.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/utils/plot_utils.py` & `basetrainer-0.8.3/basetrainer/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/utils/setup_config.py` & `basetrainer-0.8.3/basetrainer/utils/setup_config.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/utils/summary.py` & `basetrainer-0.8.3/basetrainer/utils/summary.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/utils/torch_data.py` & `basetrainer-0.8.3/basetrainer/utils/torch_data.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer/utils/torch_tools.py` & `basetrainer-0.8.3/basetrainer/utils/torch_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -470,7 +470,24 @@
     # print("Total Flops :{}".format(macs))
     # print("Total params:{}".format(params))
     print("===" * 10)
     print("inputs.shape:{}".format(inputs.shape))
     # print("output.shape:{}".format(output.shape))
     if plot:
         plot_model(model, output)
+
+
+def print_model_shape(inp, out):
+    """
+    打印模型输入输出维度
+    :param inp:
+    :param out:
+    :return:
+    """
+    if isinstance(inp, torch.Tensor): inp = [inp]
+    if isinstance(out, torch.Tensor): out = [out]
+    print("===" * 10)
+    for i in range(len(inp)):
+        print("input{}  {}".format(i, inp[i].shape))
+    for i in range(len(out)):
+        print("output{} {}".format(i, out[i].shape))
+    print("===" * 10)
```

### Comparing `basetrainer-0.8.2/basetrainer/utils/torchcam_utils.py` & `basetrainer-0.8.3/basetrainer/utils/torchcam_utils.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/basetrainer.egg-info/SOURCES.txt` & `basetrainer-0.8.3/basetrainer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/setup.py` & `basetrainer-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.8.2/test/test_scheduler.py` & `basetrainer-0.8.3/test/test_scheduler.py`

 * *Files identical despite different names*

