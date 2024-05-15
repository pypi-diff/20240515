# Comparing `tmp/torchmetrics-1.4.0.tar.gz` & `tmp/torchmetrics-1.4.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmetrics-1.4.0.tar", last modified: Mon May  6 09:20:31 2024, max compression
+gzip compressed data, was "torchmetrics-1.4.0.post0.tar", last modified: Wed May 15 11:25:04 2024, max compression
```

## Comparing `torchmetrics-1.4.0.tar` & `torchmetrics-1.4.0.post0.tar`

### file list

```diff
@@ -1,384 +1,385 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.205566 torchmetrics-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    76084 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19751 2024-05-06 09:20:31.205566 torchmetrics-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.145566 torchmetrics-1.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/_devel.txt
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/_doctest.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/_integrate.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/_tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/audio.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/audio_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/classification_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/detection.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/detection_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/image.txt
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/image_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/multimodal.txt
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/nominal_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/segmentation_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/text.txt
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/text_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/typing.txt
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements/visual.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:20:31.205566 torchmetrics-1.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)    10931 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.137566 torchmetrics-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.145566 torchmetrics-1.4.0/src/torchmetrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27285 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.145566 torchmetrics-1.4.0/src/torchmetrics/audio/
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/audio/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/audio/pesq.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/audio/pit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15368 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/audio/sdr.py
--rw-r--r--   0 runner    (1001) docker     (127)    12749 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/audio/snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/audio/srmr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/audio/stoi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.153566 torchmetrics-1.4.0/src/torchmetrics/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23385 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)    25578 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25440 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17268 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/calibration_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)    23851 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/dice.py
--rw-r--r--   0 runner    (1001) docker     (127)    18469 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/exact_match.py
--rw-r--r--   0 runner    (1001) docker     (127)    54203 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/f_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/group_fairness.py
--rw-r--r--   0 runner    (1001) docker     (127)    24058 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/hamming.py
--rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/hinge.py
--rw-r--r--   0 runner    (1001) docker     (127)    20528 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/jaccard.py
--rw-r--r--   0 runner    (1001) docker     (127)    17066 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/matthews_corrcoef.py
--rw-r--r--   0 runner    (1001) docker     (127)    25339 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/precision_fixed_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)    48233 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)    35008 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    16435 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)    25323 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/recall_fixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    30545 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/roc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18719 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/sensitivity_specificity.py
--rw-r--r--   0 runner    (1001) docker     (127)    23622 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/specificity.py
--rw-r--r--   0 runner    (1001) docker     (127)    18828 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/specificity_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    25896 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/classification/stat_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.153566 torchmetrics-1.4.0/src/torchmetrics/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/clustering/adjusted_mutual_info_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/clustering/adjusted_rand_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/clustering/calinski_harabasz_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/clustering/davies_bouldin_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/clustering/dunn_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/clustering/fowlkes_mallows_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/clustering/homogeneity_completeness_v_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/clustering/mutual_info_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/clustering/normalized_mutual_info_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/clustering/rand_score.py
--rw-r--r--   0 runner    (1001) docker     (127)    30559 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.157566 torchmetrics-1.4.0/src/torchmetrics/detection/
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/detection/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    43203 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/detection/_mean_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/detection/ciou.py
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/detection/diou.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/detection/giou.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/detection/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/detection/iou.py
--rw-r--r--   0 runner    (1001) docker     (127)    50902 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/detection/mean_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)    21979 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/detection/panoptic_qualities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.157566 torchmetrics-1.4.0/src/torchmetrics/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.157566 torchmetrics-1.4.0/src/torchmetrics/functional/audio/
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/audio/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/audio/pesq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/audio/pit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/audio/sdr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/audio/snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/audio/srmr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/audio/stoi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.161566 torchmetrics-1.4.0/src/torchmetrics/functional/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20015 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23719 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)    23230 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    16940 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/calibration_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)    27782 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/dice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/exact_match.py
--rw-r--r--   0 runner    (1001) docker     (127)    37932 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/f_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/group_fairness.py
--rw-r--r--   0 runner    (1001) docker     (127)    20724 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/hamming.py
--rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/hinge.py
--rw-r--r--   0 runner    (1001) docker     (127)    17187 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/jaccard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/matthews_corrcoef.py
--rw-r--r--   0 runner    (1001) docker     (127)    18072 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/precision_fixed_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)    36812 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)    47368 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/recall_fixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    28564 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/roc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22202 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/sensitivity_specificity.py
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/specificity.py
--rw-r--r--   0 runner    (1001) docker     (127)    23561 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/specificity_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    49987 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/classification/stat_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.161566 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/adjusted_mutual_info_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/adjusted_rand_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/calinski_harabasz_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/davies_bouldin_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/dunn_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/fowlkes_mallows_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/homogeneity_completeness_v_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/mutual_info_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/normalized_mutual_info_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/rand_score.py
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.161566 torchmetrics-1.4.0/src/torchmetrics/functional/detection/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/detection/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    20143 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/detection/_panoptic_quality_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/detection/ciou.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/detection/diou.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/detection/giou.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/detection/iou.py
--rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/detection/panoptic_qualities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.165566 torchmetrics-1.4.0/src/torchmetrics/functional/image/
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/d_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/d_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/ergas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/lpips.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.165566 torchmetrics-1.4.0/src/torchmetrics/functional/image/lpips_models/
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/lpips_models/alex.pth
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/lpips_models/squeeze.pth
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/lpips_models/vgg.pth
--rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/perceptual_path_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/psnrb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/qnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/rase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/rmse_sw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/scc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21773 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/tv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/uqi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/image/vif.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.165566 torchmetrics-1.4.0/src/torchmetrics/functional/multimodal/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/multimodal/clip_iqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/multimodal/clip_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.169566 torchmetrics-1.4.0/src/torchmetrics/functional/nominal/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/nominal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/nominal/cramers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/nominal/fleiss_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/nominal/pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/nominal/theils_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/nominal/tschuprows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/nominal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.169566 torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/cosine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/minkowski.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.173566 torchmetrics-1.4.0/src/torchmetrics/functional/regression/
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/concordance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/csi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/explained_variance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15232 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/kendall.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/log_cosh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/log_mse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/mae.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/mape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/minkowski.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/mse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/r2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/rse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/spearman.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/symmetric_mape.py
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/tweedie_deviance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/regression/wmape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.173566 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/fall_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/ndcg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/r_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/reciprocal_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.173566 torchmetrics-1.4.0/src/torchmetrics/functional/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/segmentation/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/segmentation/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (127)    45095 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/segmentation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.177566 torchmetrics-1.4.0/src/torchmetrics/functional/text/
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/cer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26128 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/chrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/eed.py
--rw-r--r--   0 runner    (1001) docker     (127)    16996 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11874 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/helper_embedding_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/infolm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/mer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)    21903 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/rouge.py
--rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/sacre_bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/squad.py
--rw-r--r--   0 runner    (1001) docker     (127)    23307 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/ter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/wer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/wil.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/functional/text/wip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.181566 torchmetrics-1.4.0/src/torchmetrics/image/
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/d_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/d_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/ergas.py
--rw-r--r--   0 runner    (1001) docker     (127)    21015 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/fid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/inception.py
--rw-r--r--   0 runner    (1001) docker     (127)    15638 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/kid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/lpip.py
--rw-r--r--   0 runner    (1001) docker     (127)    12652 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/mifid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/perceptual_path_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/psnrb.py
--rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/qnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/rase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/rmse_sw.py
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/scc.py
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/tv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/uqi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/image/vif.py
--rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.181566 torchmetrics-1.4.0/src/torchmetrics/multimodal/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/multimodal/clip_iqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/multimodal/clip_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.181566 torchmetrics-1.4.0/src/torchmetrics/nominal/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/nominal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/nominal/cramers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/nominal/fleiss_kappa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/nominal/pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/nominal/theils_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/nominal/tschuprows.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.185566 torchmetrics-1.4.0/src/torchmetrics/regression/
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/concordance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/csi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/explained_variance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/kendall.py
--rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/log_cosh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/log_mse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/mae.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/mape.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/minkowski.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/mse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/r2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/rse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/spearman.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/symmetric_mape.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/tweedie_deviance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/regression/wmape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.185566 torchmetrics-1.4.0/src/torchmetrics/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/fall_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/ndcg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    17854 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/r_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/retrieval/reciprocal_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.185566 torchmetrics-1.4.0/src/torchmetrics/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/segmentation/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/segmentation/mean_iou.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.189566 torchmetrics-1.4.0/src/torchmetrics/text/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/cer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/chrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/eed.py
--rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/infolm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/mer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/rouge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/sacre_bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/squad.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/ter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/wer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/wil.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/text/wip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.189566 torchmetrics-1.4.0/src/torchmetrics/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34595 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/utilities/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/utilities/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    13755 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/utilities/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/utilities/prints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.189566 torchmetrics-1.4.0/src/torchmetrics/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/wrappers/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/wrappers/bootstrapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/wrappers/classwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/wrappers/feature_share.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/wrappers/minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/wrappers/multioutput.py
--rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/wrappers/multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/wrappers/running.py
--rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-05-06 09:20:25.000000 torchmetrics-1.4.0/src/torchmetrics/wrappers/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:20:31.193566 torchmetrics-1.4.0/src/torchmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19751 2024-05-06 09:20:31.000000 torchmetrics-1.4.0/src/torchmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-06 09:20:31.000000 torchmetrics-1.4.0/src/torchmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:20:31.000000 torchmetrics-1.4.0/src/torchmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:20:31.000000 torchmetrics-1.4.0/src/torchmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-06 09:20:31.000000 torchmetrics-1.4.0/src/torchmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 09:20:31.000000 torchmetrics-1.4.0/src/torchmetrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.711582 torchmetrics-1.4.0.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)    76084 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-05-15 11:25:04.711582 torchmetrics-1.4.0.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.635582 torchmetrics-1.4.0.post0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/_devel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/_doctest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/_integrate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/audio.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/audio_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/classification_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/debug.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/detection.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/detection_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/image.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/image_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/multimodal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/nominal_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/segmentation_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/text.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/text_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/typing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements/visual.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:25:04.711582 torchmetrics-1.4.0.post0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10931 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.627582 torchmetrics-1.4.0.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.635582 torchmetrics-1.4.0.post0/src/torchmetrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27285 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.639582 torchmetrics-1.4.0.post0/src/torchmetrics/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/audio/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/audio/pesq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/audio/pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15368 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/audio/sdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12749 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/audio/snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/audio/srmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/audio/stoi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.643582 torchmetrics-1.4.0.post0/src/torchmetrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23385 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25578 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25440 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17268 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/calibration_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23851 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18469 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/exact_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54203 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/group_fairness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24058 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/hamming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/hinge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20528 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/jaccard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17066 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/matthews_corrcoef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25339 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/precision_fixed_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48233 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35008 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16435 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25323 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/recall_fixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30545 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18719 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/sensitivity_specificity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23622 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/specificity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18828 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/specificity_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25896 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/classification/stat_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.643582 torchmetrics-1.4.0.post0/src/torchmetrics/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/clustering/adjusted_mutual_info_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/clustering/adjusted_rand_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/clustering/calinski_harabasz_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/clustering/davies_bouldin_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/clustering/dunn_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/clustering/fowlkes_mallows_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/clustering/homogeneity_completeness_v_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/clustering/mutual_info_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/clustering/normalized_mutual_info_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/clustering/rand_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30559 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.647582 torchmetrics-1.4.0.post0/src/torchmetrics/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/detection/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43203 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/detection/_mean_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/detection/ciou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/detection/diou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/detection/giou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/detection/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/detection/iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50902 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/detection/mean_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21979 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/detection/panoptic_qualities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.647582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.647582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/pesq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/sdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/srmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/stoi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.651582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20015 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23719 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23230 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16940 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/calibration_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27782 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/exact_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37932 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16891 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/group_fairness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20724 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/hamming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/hinge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17187 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/jaccard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/matthews_corrcoef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18072 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/precision_fixed_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36812 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47368 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/recall_fixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28564 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/roc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22202 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/sensitivity_specificity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/specificity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23561 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/specificity_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49987 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/stat_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.655582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/adjusted_mutual_info_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/adjusted_rand_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/calinski_harabasz_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/davies_bouldin_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/dunn_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/fowlkes_mallows_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/homogeneity_completeness_v_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/mutual_info_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/normalized_mutual_info_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/rand_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.655582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20143 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/_panoptic_quality_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/ciou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/diou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/giou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/panoptic_qualities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.659582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/d_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/d_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/ergas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/lpips.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.659582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/lpips_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/lpips_models/alex.pth
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/lpips_models/squeeze.pth
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/lpips_models/vgg.pth
+-rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/perceptual_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/psnrb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/qnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/rase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/rmse_sw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21773 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/tv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/uqi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/vif.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.659582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/multimodal/clip_iqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/multimodal/clip_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.663582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/cramers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/fleiss_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/theils_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/tschuprows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.663582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/minkowski.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.667582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/concordance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/csi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/explained_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15232 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/kendall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/log_cosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/log_mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/mae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/mape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/minkowski.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/rse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/spearman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/symmetric_mape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/tweedie_deviance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/wmape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.667582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/fall_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/ndcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/r_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/reciprocal_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.667582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/segmentation/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/segmentation/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45095 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/segmentation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.671582 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/cer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26128 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/chrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/eed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16996 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11874 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/helper_embedding_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/infolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/mer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21903 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/sacre_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/squad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23307 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/ter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/wer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/wil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/wip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.675582 torchmetrics-1.4.0.post0/src/torchmetrics/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/d_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/d_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/ergas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21015 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/inception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15638 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/kid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/lpip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12652 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/mifid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/perceptual_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/psnrb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/qnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/rase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/rmse_sw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/tv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/uqi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/image/vif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.675582 torchmetrics-1.4.0.post0/src/torchmetrics/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/multimodal/clip_iqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/multimodal/clip_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.679582 torchmetrics-1.4.0.post0/src/torchmetrics/nominal/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/nominal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/nominal/cramers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/nominal/fleiss_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/nominal/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/nominal/theils_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/nominal/tschuprows.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.679582 torchmetrics-1.4.0.post0/src/torchmetrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/concordance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/csi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/explained_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/kendall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/log_cosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/log_mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/mae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/mape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/minkowski.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/rse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/spearman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/symmetric_mape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/tweedie_deviance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/regression/wmape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.683582 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/fall_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/ndcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17854 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/r_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/reciprocal_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.683582 torchmetrics-1.4.0.post0/src/torchmetrics/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/segmentation/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/segmentation/mean_iou.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.687582 torchmetrics-1.4.0.post0/src/torchmetrics/text/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/cer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/chrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/eed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/infolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/mer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/sacre_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/squad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/ter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/wer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/wil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/text/wip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.687582 torchmetrics-1.4.0.post0/src/torchmetrics/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34595 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/utilities/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/utilities/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13755 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/utilities/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/utilities/prints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.691582 torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/bootstrapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/classwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/feature_share.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/running.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-05-15 11:25:02.000000 torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:25:04.691582 torchmetrics-1.4.0.post0/src/torchmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-05-15 11:25:04.000000 torchmetrics-1.4.0.post0/src/torchmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-05-15 11:25:04.000000 torchmetrics-1.4.0.post0/src/torchmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:25:04.000000 torchmetrics-1.4.0.post0/src/torchmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:25:04.000000 torchmetrics-1.4.0.post0/src/torchmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-15 11:25:04.000000 torchmetrics-1.4.0.post0/src/torchmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 11:25:04.000000 torchmetrics-1.4.0.post0/src/torchmetrics.egg-info/top_level.txt
```

### Comparing `torchmetrics-1.4.0/CHANGELOG.md` & `torchmetrics-1.4.0.post0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/CITATION.cff` & `torchmetrics-1.4.0.post0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/LICENSE` & `torchmetrics-1.4.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/MANIFEST.in` & `torchmetrics-1.4.0.post0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/PKG-INFO` & `torchmetrics-1.4.0.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmetrics
-Version: 1.4.0
+Version: 1.4.0.post0
 Summary: PyTorch native Metrics
 Home-page: https://github.com/Lightning-AI/torchmetrics
 Download-URL: https://github.com/Lightning-AI/torchmetrics/archive/master.zip
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/torchmetrics/issues
@@ -29,134 +29,137 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>1.20.0
 Requires-Dist: packaging>17.1
 Requires-Dist: torch>=1.10.0
 Requires-Dist: typing-extensions; python_version < "3.9"
 Requires-Dist: lightning-utilities>=0.8.0
-Requires-Dist: pretty-errors==1.2.25
 Provides-Extra: audio
-Requires-Dist: torchaudio>=0.10.0; extra == "audio"
 Requires-Dist: pystoi>=0.3.0; extra == "audio"
+Requires-Dist: torchaudio>=0.10.0; extra == "audio"
+Provides-Extra: debug
+Requires-Dist: pretty-errors>=1.2.0; extra == "debug"
 Provides-Extra: detection
-Requires-Dist: pycocotools>2.0.0; extra == "detection"
 Requires-Dist: torchvision>=0.8; extra == "detection"
+Requires-Dist: pycocotools>2.0.0; extra == "detection"
 Provides-Extra: image
-Requires-Dist: torch-fidelity<=0.4.0; extra == "image"
 Requires-Dist: torchvision>=0.8; extra == "image"
 Requires-Dist: scipy>1.0.0; extra == "image"
+Requires-Dist: torch-fidelity<=0.4.0; extra == "image"
 Provides-Extra: multimodal
 Requires-Dist: transformers>=4.10.0; extra == "multimodal"
 Requires-Dist: piq<=0.8.0; extra == "multimodal"
 Provides-Extra: text
 Requires-Dist: transformers>4.4.0; extra == "text"
-Requires-Dist: sentencepiece>=0.2.0; extra == "text"
+Requires-Dist: ipadic>=1.0.0; extra == "text"
+Requires-Dist: regex>=2021.9.24; extra == "text"
 Requires-Dist: tqdm>=4.41.0; extra == "text"
 Requires-Dist: mecab-python3>=1.0.6; extra == "text"
+Requires-Dist: sentencepiece>=0.2.0; extra == "text"
 Requires-Dist: nltk>=3.6; extra == "text"
-Requires-Dist: ipadic>=1.0.0; extra == "text"
-Requires-Dist: regex>=2021.9.24; extra == "text"
 Provides-Extra: typing
 Requires-Dist: types-setuptools; extra == "typing"
+Requires-Dist: types-six; extra == "typing"
 Requires-Dist: types-tabulate; extra == "typing"
-Requires-Dist: types-protobuf; extra == "typing"
-Requires-Dist: mypy==1.9.0; extra == "typing"
-Requires-Dist: types-emoji; extra == "typing"
+Requires-Dist: types-PyYAML; extra == "typing"
 Requires-Dist: torch==2.3.0; extra == "typing"
 Requires-Dist: types-requests; extra == "typing"
-Requires-Dist: types-six; extra == "typing"
-Requires-Dist: types-PyYAML; extra == "typing"
+Requires-Dist: types-emoji; extra == "typing"
+Requires-Dist: mypy==1.9.0; extra == "typing"
+Requires-Dist: types-protobuf; extra == "typing"
 Provides-Extra: visual
 Requires-Dist: matplotlib>=3.3.0; extra == "visual"
 Requires-Dist: SciencePlots>=2.0.0; extra == "visual"
 Provides-Extra: all
-Requires-Dist: torchaudio>=0.10.0; extra == "all"
 Requires-Dist: pystoi>=0.3.0; extra == "all"
-Requires-Dist: pycocotools>2.0.0; extra == "all"
+Requires-Dist: torchaudio>=0.10.0; extra == "all"
+Requires-Dist: pretty-errors>=1.2.0; extra == "all"
 Requires-Dist: torchvision>=0.8; extra == "all"
-Requires-Dist: torch-fidelity<=0.4.0; extra == "all"
+Requires-Dist: pycocotools>2.0.0; extra == "all"
 Requires-Dist: torchvision>=0.8; extra == "all"
 Requires-Dist: scipy>1.0.0; extra == "all"
+Requires-Dist: torch-fidelity<=0.4.0; extra == "all"
 Requires-Dist: transformers>=4.10.0; extra == "all"
 Requires-Dist: piq<=0.8.0; extra == "all"
 Requires-Dist: transformers>4.4.0; extra == "all"
-Requires-Dist: sentencepiece>=0.2.0; extra == "all"
+Requires-Dist: ipadic>=1.0.0; extra == "all"
+Requires-Dist: regex>=2021.9.24; extra == "all"
 Requires-Dist: tqdm>=4.41.0; extra == "all"
 Requires-Dist: mecab-python3>=1.0.6; extra == "all"
+Requires-Dist: sentencepiece>=0.2.0; extra == "all"
 Requires-Dist: nltk>=3.6; extra == "all"
-Requires-Dist: ipadic>=1.0.0; extra == "all"
-Requires-Dist: regex>=2021.9.24; extra == "all"
 Requires-Dist: types-setuptools; extra == "all"
+Requires-Dist: types-six; extra == "all"
 Requires-Dist: types-tabulate; extra == "all"
-Requires-Dist: types-protobuf; extra == "all"
-Requires-Dist: mypy==1.9.0; extra == "all"
-Requires-Dist: types-emoji; extra == "all"
+Requires-Dist: types-PyYAML; extra == "all"
 Requires-Dist: torch==2.3.0; extra == "all"
 Requires-Dist: types-requests; extra == "all"
-Requires-Dist: types-six; extra == "all"
-Requires-Dist: types-PyYAML; extra == "all"
+Requires-Dist: types-emoji; extra == "all"
+Requires-Dist: mypy==1.9.0; extra == "all"
+Requires-Dist: types-protobuf; extra == "all"
 Requires-Dist: matplotlib>=3.3.0; extra == "all"
 Requires-Dist: SciencePlots>=2.0.0; extra == "all"
 Provides-Extra: dev
-Requires-Dist: torchaudio>=0.10.0; extra == "dev"
 Requires-Dist: pystoi>=0.3.0; extra == "dev"
-Requires-Dist: pycocotools>2.0.0; extra == "dev"
+Requires-Dist: torchaudio>=0.10.0; extra == "dev"
+Requires-Dist: pretty-errors>=1.2.0; extra == "dev"
 Requires-Dist: torchvision>=0.8; extra == "dev"
-Requires-Dist: torch-fidelity<=0.4.0; extra == "dev"
+Requires-Dist: pycocotools>2.0.0; extra == "dev"
 Requires-Dist: torchvision>=0.8; extra == "dev"
 Requires-Dist: scipy>1.0.0; extra == "dev"
+Requires-Dist: torch-fidelity<=0.4.0; extra == "dev"
 Requires-Dist: transformers>=4.10.0; extra == "dev"
 Requires-Dist: piq<=0.8.0; extra == "dev"
 Requires-Dist: transformers>4.4.0; extra == "dev"
-Requires-Dist: sentencepiece>=0.2.0; extra == "dev"
+Requires-Dist: ipadic>=1.0.0; extra == "dev"
+Requires-Dist: regex>=2021.9.24; extra == "dev"
 Requires-Dist: tqdm>=4.41.0; extra == "dev"
 Requires-Dist: mecab-python3>=1.0.6; extra == "dev"
+Requires-Dist: sentencepiece>=0.2.0; extra == "dev"
 Requires-Dist: nltk>=3.6; extra == "dev"
-Requires-Dist: ipadic>=1.0.0; extra == "dev"
-Requires-Dist: regex>=2021.9.24; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
+Requires-Dist: types-six; extra == "dev"
 Requires-Dist: types-tabulate; extra == "dev"
-Requires-Dist: types-protobuf; extra == "dev"
-Requires-Dist: mypy==1.9.0; extra == "dev"
-Requires-Dist: types-emoji; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: torch==2.3.0; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
-Requires-Dist: types-six; extra == "dev"
-Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: types-emoji; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: types-protobuf; extra == "dev"
 Requires-Dist: matplotlib>=3.3.0; extra == "dev"
 Requires-Dist: SciencePlots>=2.0.0; extra == "dev"
+Requires-Dist: scikit-image>=0.19.0; extra == "dev"
 Requires-Dist: mir-eval>=0.6; extra == "dev"
-Requires-Dist: pytorch-msssim==1.0.0; extra == "dev"
-Requires-Dist: sewar>=0.4.4; extra == "dev"
+Requires-Dist: faster-coco-eval>=1.3.3; extra == "dev"
+Requires-Dist: scipy>1.0.0; extra == "dev"
+Requires-Dist: numpy<1.27.0; extra == "dev"
+Requires-Dist: pandas>1.0.0; extra == "dev"
+Requires-Dist: fairlearn; extra == "dev"
 Requires-Dist: mecab-ko-dic>=1.0.0; extra == "dev"
-Requires-Dist: huggingface-hub<0.23; extra == "dev"
-Requires-Dist: statsmodels>0.13.5; extra == "dev"
+Requires-Dist: bert_score==0.3.13; extra == "dev"
+Requires-Dist: rouge-score>0.1.0; extra == "dev"
 Requires-Dist: dython<=0.7.5; extra == "dev"
-Requires-Dist: scipy>1.0.0; extra == "dev"
+Requires-Dist: netcal>1.0.0; extra == "dev"
+Requires-Dist: pytorch-msssim==1.0.0; extra == "dev"
 Requires-Dist: mecab-ko>=1.0.0; extra == "dev"
-Requires-Dist: pandas>1.0.0; extra == "dev"
-Requires-Dist: numpy<1.25.0; extra == "dev"
+Requires-Dist: huggingface-hub<0.23; extra == "dev"
+Requires-Dist: statsmodels>0.13.5; extra == "dev"
 Requires-Dist: torch_complex<=0.4.3; extra == "dev"
-Requires-Dist: scikit-image>=0.19.0; extra == "dev"
-Requires-Dist: pandas>=1.4.0; extra == "dev"
-Requires-Dist: netcal>1.0.0; extra == "dev"
-Requires-Dist: monai==1.3.0; extra == "dev"
+Requires-Dist: lpips<=0.1.4; extra == "dev"
 Requires-Dist: jiwer>=2.3.0; extra == "dev"
-Requires-Dist: fairlearn; extra == "dev"
-Requires-Dist: sacrebleu>=2.3.0; extra == "dev"
-Requires-Dist: fast-bss-eval>=0.1.0; extra == "dev"
 Requires-Dist: kornia>=0.6.7; extra == "dev"
-Requires-Dist: bert_score==0.3.13; extra == "dev"
-Requires-Dist: faster-coco-eval>=1.3.3; extra == "dev"
-Requires-Dist: lpips<=0.1.4; extra == "dev"
-Requires-Dist: rouge-score>0.1.0; extra == "dev"
+Requires-Dist: fast-bss-eval>=0.1.0; extra == "dev"
+Requires-Dist: pandas>=1.4.0; extra == "dev"
+Requires-Dist: sewar>=0.4.4; extra == "dev"
+Requires-Dist: sacrebleu>=2.3.0; extra == "dev"
+Requires-Dist: monai==1.3.0; extra == "dev"
 
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.4.0/docs/source/_static/images/logo.png" width="400px">
+<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.4.0.post0/docs/source/_static/images/logo.png" width="400px">
 
 **Machine learning metrics for distributed, scalable PyTorch applications.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="#what-is-torchmetrics">What is Torchmetrics</a> •
@@ -173,16 +176,16 @@
 [![PyPI Status](https://badge.fury.io/py/torchmetrics.svg)](https://badge.fury.io/py/torchmetrics)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torchmetrics)
 ](https://pepy.tech/project/torchmetrics)
 [![Conda](https://img.shields.io/conda/v/conda-forge/torchmetrics?label=conda&color=success)](https://anaconda.org/conda-forge/torchmetrics)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/torchmetrics/blob/master/LICENSE)
 
 [![CI testing | CPU](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests.yml/badge.svg?event=push)](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests.yml)
-[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.4.0)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.4.0)
-[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.4.0/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
+[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.4.0.post0)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.4.0.post0)
+[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.4.0.post0/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Lightning-AI/torchmetrics/master.svg)](https://results.pre-commit.ci/latest/github/Lightning-AI/torchmetrics/master)
 
 [![Documentation Status](https://readthedocs.org/projects/torchmetrics/badge/?version=latest)](https://torchmetrics.readthedocs.io/en/latest/?badge=latest)
 [![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5844769.svg)](https://doi.org/10.5281/zenodo.5844769)
 [![JOSS status](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43/status.svg)](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43)
 
@@ -480,15 +483,15 @@
 values = []
 for i in range(10):
     values.append(acc(preds(i), target(i)))
 fig3, ax3 = acc.plot(values)
 ```
 
 <p align="center">
-  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.4.0/docs/source/_static/images/plot_example.png" width="1000">
+  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.4.0.post0/docs/source/_static/images/plot_example.png" width="1000">
 </p>
 
 For examples of plotting different metrics try running [this example file](examples/plotting.py).
 
 ## Contribute!
 
 The lightning + TorchMetrics team is hard at work adding even more metrics.
```

### Comparing `torchmetrics-1.4.0/README.md` & `torchmetrics-1.4.0.post0/README.md`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/requirements/_docs.txt` & `torchmetrics-1.4.0.post0/requirements/_docs.txt`

 * *Files 23% similar despite different names*

```diff
@@ -19,8 +19,7 @@
 -r _integrate.txt
 -r visual.txt
 -r audio.txt
 -r detection.txt
 -r image.txt
 -r multimodal.txt
 -r text.txt
--r text_test.txt
```

### Comparing `torchmetrics-1.4.0/requirements/_tests.txt` & `torchmetrics-1.4.0.post0/requirements/_tests.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # NOTE: the upper bound for the package version is only set for CI stability, and it is dropped while installing this package
 #  in case you want to preserve/enforce restrictions on the latest compatible version, add "strict" as an in-line comment
 
-coverage ==7.5.0
+coverage ==7.5.1
 pytest ==8.1.1
 pytest-cov ==5.0.0
 pytest-doctestplus ==1.2.1
 pytest-rerunfailures ==14.0
 pytest-timeout ==2.3.1
-pytest-xdist ==3.5.0
+pytest-xdist ==3.6.1
 phmdoctest ==1.4.0
 
 psutil <5.10.0
 pyGithub ==2.3.0
 fire <=0.6.0
 
 cloudpickle >1.3, <=3.0.0
```

### Comparing `torchmetrics-1.4.0/requirements/audio_test.txt` & `torchmetrics-1.4.0.post0/requirements/audio_test.txt`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/setup.py` & `torchmetrics-1.4.0.post0/setup.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/__about__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/__about__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.4.0"
+__version__ = "1.4.0.post0"
 __author__ = "Lightning-AI et al."
 __author_email__ = "name@pytorchlightning.ai"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2020-2023, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/torchmetrics"
 __docs__ = "PyTorch native Metrics"
 __docs_url__ = "https://lightning.ai/docs/torchmetrics/stable/"
```

### Comparing `torchmetrics-1.4.0/src/torchmetrics/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/aggregation.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/aggregation.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/audio/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/audio/_deprecated.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/audio/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/audio/pesq.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/audio/pesq.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/audio/pit.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/audio/pit.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/audio/sdr.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/audio/sdr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/audio/snr.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/audio/snr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/audio/srmr.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/audio/srmr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/audio/stoi.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/audio/stoi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/accuracy.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/auroc.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/average_precision.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/base.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/base.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/calibration_error.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/calibration_error.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/cohen_kappa.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/confusion_matrix.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/dice.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/dice.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/exact_match.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/exact_match.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/f_beta.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/f_beta.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/group_fairness.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/group_fairness.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/hamming.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/hamming.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/hinge.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/hinge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/jaccard.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/jaccard.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/matthews_corrcoef.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/matthews_corrcoef.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/precision_fixed_recall.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/precision_fixed_recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/precision_recall.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/precision_recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/precision_recall_curve.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/ranking.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/ranking.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/recall_fixed_precision.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/recall_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/roc.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/roc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/sensitivity_specificity.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/sensitivity_specificity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/specificity.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/specificity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/specificity_sensitivity.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/specificity_sensitivity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/classification/stat_scores.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/classification/stat_scores.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/clustering/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/clustering/adjusted_mutual_info_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/clustering/adjusted_mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/clustering/adjusted_rand_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/clustering/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/clustering/calinski_harabasz_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/clustering/calinski_harabasz_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/clustering/davies_bouldin_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/clustering/davies_bouldin_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/clustering/dunn_index.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/clustering/dunn_index.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/clustering/fowlkes_mallows_index.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/clustering/fowlkes_mallows_index.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/clustering/homogeneity_completeness_v_measure.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/clustering/homogeneity_completeness_v_measure.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/clustering/mutual_info_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/clustering/mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/clustering/normalized_mutual_info_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/clustering/normalized_mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/clustering/rand_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/clustering/rand_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/collections.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/collections.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/detection/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/detection/_deprecated.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/detection/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/detection/_mean_ap.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/detection/_mean_ap.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/detection/ciou.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/detection/ciou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/detection/diou.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/detection/diou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/detection/giou.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/detection/giou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/detection/helpers.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/detection/helpers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/detection/iou.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/detection/iou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/detection/mean_ap.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/detection/mean_ap.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/detection/panoptic_qualities.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/detection/panoptic_qualities.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/audio/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/audio/_deprecated.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/audio/pesq.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/pesq.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/audio/pit.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/pit.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/audio/sdr.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/sdr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/audio/snr.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/snr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/audio/srmr.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/srmr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/audio/stoi.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/audio/stoi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/accuracy.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/auroc.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/average_precision.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/calibration_error.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/calibration_error.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/cohen_kappa.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/confusion_matrix.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/dice.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/dice.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/exact_match.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/exact_match.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/f_beta.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/f_beta.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/group_fairness.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/group_fairness.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/hamming.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/hamming.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/hinge.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/hinge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/jaccard.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/jaccard.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/matthews_corrcoef.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/matthews_corrcoef.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/precision_fixed_recall.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/precision_fixed_recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/precision_recall.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/precision_recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/precision_recall_curve.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/ranking.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/ranking.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/recall_fixed_precision.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/recall_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/roc.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/roc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/sensitivity_specificity.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/sensitivity_specificity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/specificity.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/specificity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/specificity_sensitivity.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/specificity_sensitivity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/classification/stat_scores.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/classification/stat_scores.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/clustering/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/clustering/adjusted_mutual_info_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/adjusted_mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/clustering/adjusted_rand_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/clustering/calinski_harabasz_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/calinski_harabasz_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/clustering/davies_bouldin_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/davies_bouldin_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/clustering/dunn_index.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/dunn_index.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/clustering/fowlkes_mallows_index.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/fowlkes_mallows_index.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/clustering/homogeneity_completeness_v_measure.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/homogeneity_completeness_v_measure.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/clustering/mutual_info_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/clustering/normalized_mutual_info_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/normalized_mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/clustering/rand_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/rand_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/clustering/utils.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/detection/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/detection/_deprecated.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/detection/_panoptic_quality_common.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/_panoptic_quality_common.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/detection/ciou.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/ciou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/detection/diou.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/diou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/detection/giou.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/giou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/detection/iou.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/iou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/detection/panoptic_qualities.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/detection/panoptic_qualities.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/_deprecated.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/d_lambda.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/d_lambda.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/d_s.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/d_s.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/ergas.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/ergas.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/gradients.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/gradients.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/lpips.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/lpips.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/lpips_models/alex.pth` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/lpips_models/alex.pth`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/lpips_models/squeeze.pth` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/lpips_models/squeeze.pth`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/lpips_models/vgg.pth` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/lpips_models/vgg.pth`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/perceptual_path_length.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/perceptual_path_length.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/psnr.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/psnrb.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/psnrb.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/qnr.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/qnr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/rase.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/rase.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/rmse_sw.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/rmse_sw.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/sam.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/sam.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/scc.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/scc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/ssim.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/ssim.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/tv.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/tv.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/uqi.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/uqi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/utils.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/image/vif.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/image/vif.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/multimodal/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/multimodal/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/multimodal/clip_iqa.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/multimodal/clip_iqa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/multimodal/clip_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/multimodal/clip_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/nominal/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/nominal/cramers.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/cramers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/nominal/fleiss_kappa.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/fleiss_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/nominal/pearson.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/nominal/theils_u.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/theils_u.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/nominal/tschuprows.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/tschuprows.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/nominal/utils.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/nominal/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/cosine.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/cosine.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/euclidean.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/euclidean.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/helpers.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/helpers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/linear.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/linear.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/manhattan.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/manhattan.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/pairwise/minkowski.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/pairwise/minkowski.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/concordance.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/concordance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/cosine_similarity.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/csi.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/csi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/explained_variance.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/explained_variance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/kendall.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/kendall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/kl_divergence.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/log_cosh.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/log_cosh.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/log_mse.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/log_mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/mae.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/mae.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/mape.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/minkowski.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/minkowski.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/mse.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/pearson.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/r2.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/r2.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/rse.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/rse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/spearman.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/spearman.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/symmetric_mape.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/symmetric_mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/tweedie_deviance.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/tweedie_deviance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/utils.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/regression/wmape.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/regression/wmape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/_deprecated.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/auroc.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/auroc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/average_precision.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/fall_out.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/fall_out.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/hit_rate.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/ndcg.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/ndcg.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/precision.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/precision_recall_curve.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/r_precision.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/r_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/recall.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/retrieval/reciprocal_rank.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/retrieval/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/segmentation/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/segmentation/generalized_dice.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/segmentation/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/segmentation/mean_iou.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/segmentation/mean_iou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/segmentation/utils.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/_deprecated.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/bert.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/bert.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/bleu.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/cer.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/cer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/chrf.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/chrf.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/edit.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/edit.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/eed.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/eed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/helper.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/helper.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/helper_embedding_metric.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/helper_embedding_metric.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/infolm.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/infolm.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/mer.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/mer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/perplexity.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/rouge.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/rouge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/sacre_bleu.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/sacre_bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/squad.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/squad.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/ter.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/ter.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/wer.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/wer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/wil.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/wil.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/functional/text/wip.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/functional/text/wip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/_deprecated.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/d_lambda.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/d_lambda.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/d_s.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/d_s.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/ergas.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/ergas.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/fid.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/fid.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/inception.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/inception.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/kid.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/kid.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/lpip.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/lpip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/mifid.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/mifid.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/perceptual_path_length.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/perceptual_path_length.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/psnr.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/psnrb.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/psnrb.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/qnr.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/qnr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/rase.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/rase.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/rmse_sw.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/rmse_sw.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/sam.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/sam.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/scc.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/scc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/ssim.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/ssim.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/tv.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/tv.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/uqi.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/uqi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/image/vif.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/image/vif.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/metric.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/multimodal/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/multimodal/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/multimodal/clip_iqa.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/multimodal/clip_iqa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/multimodal/clip_score.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/multimodal/clip_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/nominal/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/nominal/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/nominal/cramers.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/nominal/cramers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/nominal/fleiss_kappa.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/nominal/fleiss_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/nominal/pearson.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/nominal/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/nominal/theils_u.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/nominal/theils_u.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/nominal/tschuprows.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/nominal/tschuprows.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/concordance.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/concordance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/cosine_similarity.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/csi.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/csi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/explained_variance.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/explained_variance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/kendall.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/kendall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/kl_divergence.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/log_cosh.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/log_cosh.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/log_mse.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/log_mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/mae.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/mae.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/mape.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/minkowski.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/minkowski.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/mse.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/pearson.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/r2.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/r2.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/rse.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/rse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/spearman.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/spearman.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/symmetric_mape.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/symmetric_mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/tweedie_deviance.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/tweedie_deviance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/regression/wmape.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/regression/wmape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/_deprecated.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/auroc.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/auroc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/average_precision.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/base.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/fall_out.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/fall_out.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/hit_rate.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/ndcg.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/ndcg.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/precision.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/precision_recall_curve.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/r_precision.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/r_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/recall.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/retrieval/reciprocal_rank.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/retrieval/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/segmentation/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/segmentation/generalized_dice.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/segmentation/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/segmentation/mean_iou.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/segmentation/mean_iou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/_deprecated.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/bert.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/bert.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/bleu.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/cer.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/cer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/chrf.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/chrf.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/edit.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/edit.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/eed.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/eed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/infolm.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/infolm.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/mer.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/mer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/perplexity.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/rouge.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/rouge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/sacre_bleu.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/sacre_bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/squad.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/squad.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/ter.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/ter.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/wer.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/wer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/wil.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/wil.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/text/wip.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/text/wip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/utilities/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/utilities/checks.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/utilities/checks.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/utilities/compute.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/utilities/compute.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/utilities/data.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/utilities/data.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/utilities/distributed.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/utilities/enums.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/utilities/exceptions.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/utilities/imports.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/utilities/plot.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/utilities/plot.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/utilities/prints.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/utilities/prints.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/wrappers/__init__.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/wrappers/abstract.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/abstract.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/wrappers/bootstrapping.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/bootstrapping.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/wrappers/classwise.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/classwise.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/wrappers/feature_share.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/feature_share.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/wrappers/minmax.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/minmax.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/wrappers/multioutput.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/multioutput.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/wrappers/multitask.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/multitask.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/wrappers/running.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/running.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics/wrappers/tracker.py` & `torchmetrics-1.4.0.post0/src/torchmetrics/wrappers/tracker.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.4.0/src/torchmetrics.egg-info/PKG-INFO` & `torchmetrics-1.4.0.post0/src/torchmetrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmetrics
-Version: 1.4.0
+Version: 1.4.0.post0
 Summary: PyTorch native Metrics
 Home-page: https://github.com/Lightning-AI/torchmetrics
 Download-URL: https://github.com/Lightning-AI/torchmetrics/archive/master.zip
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/torchmetrics/issues
@@ -29,134 +29,137 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>1.20.0
 Requires-Dist: packaging>17.1
 Requires-Dist: torch>=1.10.0
 Requires-Dist: typing-extensions; python_version < "3.9"
 Requires-Dist: lightning-utilities>=0.8.0
-Requires-Dist: pretty-errors==1.2.25
 Provides-Extra: audio
-Requires-Dist: torchaudio>=0.10.0; extra == "audio"
 Requires-Dist: pystoi>=0.3.0; extra == "audio"
+Requires-Dist: torchaudio>=0.10.0; extra == "audio"
+Provides-Extra: debug
+Requires-Dist: pretty-errors>=1.2.0; extra == "debug"
 Provides-Extra: detection
-Requires-Dist: pycocotools>2.0.0; extra == "detection"
 Requires-Dist: torchvision>=0.8; extra == "detection"
+Requires-Dist: pycocotools>2.0.0; extra == "detection"
 Provides-Extra: image
-Requires-Dist: torch-fidelity<=0.4.0; extra == "image"
 Requires-Dist: torchvision>=0.8; extra == "image"
 Requires-Dist: scipy>1.0.0; extra == "image"
+Requires-Dist: torch-fidelity<=0.4.0; extra == "image"
 Provides-Extra: multimodal
 Requires-Dist: transformers>=4.10.0; extra == "multimodal"
 Requires-Dist: piq<=0.8.0; extra == "multimodal"
 Provides-Extra: text
 Requires-Dist: transformers>4.4.0; extra == "text"
-Requires-Dist: sentencepiece>=0.2.0; extra == "text"
+Requires-Dist: ipadic>=1.0.0; extra == "text"
+Requires-Dist: regex>=2021.9.24; extra == "text"
 Requires-Dist: tqdm>=4.41.0; extra == "text"
 Requires-Dist: mecab-python3>=1.0.6; extra == "text"
+Requires-Dist: sentencepiece>=0.2.0; extra == "text"
 Requires-Dist: nltk>=3.6; extra == "text"
-Requires-Dist: ipadic>=1.0.0; extra == "text"
-Requires-Dist: regex>=2021.9.24; extra == "text"
 Provides-Extra: typing
 Requires-Dist: types-setuptools; extra == "typing"
+Requires-Dist: types-six; extra == "typing"
 Requires-Dist: types-tabulate; extra == "typing"
-Requires-Dist: types-protobuf; extra == "typing"
-Requires-Dist: mypy==1.9.0; extra == "typing"
-Requires-Dist: types-emoji; extra == "typing"
+Requires-Dist: types-PyYAML; extra == "typing"
 Requires-Dist: torch==2.3.0; extra == "typing"
 Requires-Dist: types-requests; extra == "typing"
-Requires-Dist: types-six; extra == "typing"
-Requires-Dist: types-PyYAML; extra == "typing"
+Requires-Dist: types-emoji; extra == "typing"
+Requires-Dist: mypy==1.9.0; extra == "typing"
+Requires-Dist: types-protobuf; extra == "typing"
 Provides-Extra: visual
 Requires-Dist: matplotlib>=3.3.0; extra == "visual"
 Requires-Dist: SciencePlots>=2.0.0; extra == "visual"
 Provides-Extra: all
-Requires-Dist: torchaudio>=0.10.0; extra == "all"
 Requires-Dist: pystoi>=0.3.0; extra == "all"
-Requires-Dist: pycocotools>2.0.0; extra == "all"
+Requires-Dist: torchaudio>=0.10.0; extra == "all"
+Requires-Dist: pretty-errors>=1.2.0; extra == "all"
 Requires-Dist: torchvision>=0.8; extra == "all"
-Requires-Dist: torch-fidelity<=0.4.0; extra == "all"
+Requires-Dist: pycocotools>2.0.0; extra == "all"
 Requires-Dist: torchvision>=0.8; extra == "all"
 Requires-Dist: scipy>1.0.0; extra == "all"
+Requires-Dist: torch-fidelity<=0.4.0; extra == "all"
 Requires-Dist: transformers>=4.10.0; extra == "all"
 Requires-Dist: piq<=0.8.0; extra == "all"
 Requires-Dist: transformers>4.4.0; extra == "all"
-Requires-Dist: sentencepiece>=0.2.0; extra == "all"
+Requires-Dist: ipadic>=1.0.0; extra == "all"
+Requires-Dist: regex>=2021.9.24; extra == "all"
 Requires-Dist: tqdm>=4.41.0; extra == "all"
 Requires-Dist: mecab-python3>=1.0.6; extra == "all"
+Requires-Dist: sentencepiece>=0.2.0; extra == "all"
 Requires-Dist: nltk>=3.6; extra == "all"
-Requires-Dist: ipadic>=1.0.0; extra == "all"
-Requires-Dist: regex>=2021.9.24; extra == "all"
 Requires-Dist: types-setuptools; extra == "all"
+Requires-Dist: types-six; extra == "all"
 Requires-Dist: types-tabulate; extra == "all"
-Requires-Dist: types-protobuf; extra == "all"
-Requires-Dist: mypy==1.9.0; extra == "all"
-Requires-Dist: types-emoji; extra == "all"
+Requires-Dist: types-PyYAML; extra == "all"
 Requires-Dist: torch==2.3.0; extra == "all"
 Requires-Dist: types-requests; extra == "all"
-Requires-Dist: types-six; extra == "all"
-Requires-Dist: types-PyYAML; extra == "all"
+Requires-Dist: types-emoji; extra == "all"
+Requires-Dist: mypy==1.9.0; extra == "all"
+Requires-Dist: types-protobuf; extra == "all"
 Requires-Dist: matplotlib>=3.3.0; extra == "all"
 Requires-Dist: SciencePlots>=2.0.0; extra == "all"
 Provides-Extra: dev
-Requires-Dist: torchaudio>=0.10.0; extra == "dev"
 Requires-Dist: pystoi>=0.3.0; extra == "dev"
-Requires-Dist: pycocotools>2.0.0; extra == "dev"
+Requires-Dist: torchaudio>=0.10.0; extra == "dev"
+Requires-Dist: pretty-errors>=1.2.0; extra == "dev"
 Requires-Dist: torchvision>=0.8; extra == "dev"
-Requires-Dist: torch-fidelity<=0.4.0; extra == "dev"
+Requires-Dist: pycocotools>2.0.0; extra == "dev"
 Requires-Dist: torchvision>=0.8; extra == "dev"
 Requires-Dist: scipy>1.0.0; extra == "dev"
+Requires-Dist: torch-fidelity<=0.4.0; extra == "dev"
 Requires-Dist: transformers>=4.10.0; extra == "dev"
 Requires-Dist: piq<=0.8.0; extra == "dev"
 Requires-Dist: transformers>4.4.0; extra == "dev"
-Requires-Dist: sentencepiece>=0.2.0; extra == "dev"
+Requires-Dist: ipadic>=1.0.0; extra == "dev"
+Requires-Dist: regex>=2021.9.24; extra == "dev"
 Requires-Dist: tqdm>=4.41.0; extra == "dev"
 Requires-Dist: mecab-python3>=1.0.6; extra == "dev"
+Requires-Dist: sentencepiece>=0.2.0; extra == "dev"
 Requires-Dist: nltk>=3.6; extra == "dev"
-Requires-Dist: ipadic>=1.0.0; extra == "dev"
-Requires-Dist: regex>=2021.9.24; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
+Requires-Dist: types-six; extra == "dev"
 Requires-Dist: types-tabulate; extra == "dev"
-Requires-Dist: types-protobuf; extra == "dev"
-Requires-Dist: mypy==1.9.0; extra == "dev"
-Requires-Dist: types-emoji; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: torch==2.3.0; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
-Requires-Dist: types-six; extra == "dev"
-Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: types-emoji; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: types-protobuf; extra == "dev"
 Requires-Dist: matplotlib>=3.3.0; extra == "dev"
 Requires-Dist: SciencePlots>=2.0.0; extra == "dev"
+Requires-Dist: scikit-image>=0.19.0; extra == "dev"
 Requires-Dist: mir-eval>=0.6; extra == "dev"
-Requires-Dist: pytorch-msssim==1.0.0; extra == "dev"
-Requires-Dist: sewar>=0.4.4; extra == "dev"
+Requires-Dist: faster-coco-eval>=1.3.3; extra == "dev"
+Requires-Dist: scipy>1.0.0; extra == "dev"
+Requires-Dist: numpy<1.27.0; extra == "dev"
+Requires-Dist: pandas>1.0.0; extra == "dev"
+Requires-Dist: fairlearn; extra == "dev"
 Requires-Dist: mecab-ko-dic>=1.0.0; extra == "dev"
-Requires-Dist: huggingface-hub<0.23; extra == "dev"
-Requires-Dist: statsmodels>0.13.5; extra == "dev"
+Requires-Dist: bert_score==0.3.13; extra == "dev"
+Requires-Dist: rouge-score>0.1.0; extra == "dev"
 Requires-Dist: dython<=0.7.5; extra == "dev"
-Requires-Dist: scipy>1.0.0; extra == "dev"
+Requires-Dist: netcal>1.0.0; extra == "dev"
+Requires-Dist: pytorch-msssim==1.0.0; extra == "dev"
 Requires-Dist: mecab-ko>=1.0.0; extra == "dev"
-Requires-Dist: pandas>1.0.0; extra == "dev"
-Requires-Dist: numpy<1.25.0; extra == "dev"
+Requires-Dist: huggingface-hub<0.23; extra == "dev"
+Requires-Dist: statsmodels>0.13.5; extra == "dev"
 Requires-Dist: torch_complex<=0.4.3; extra == "dev"
-Requires-Dist: scikit-image>=0.19.0; extra == "dev"
-Requires-Dist: pandas>=1.4.0; extra == "dev"
-Requires-Dist: netcal>1.0.0; extra == "dev"
-Requires-Dist: monai==1.3.0; extra == "dev"
+Requires-Dist: lpips<=0.1.4; extra == "dev"
 Requires-Dist: jiwer>=2.3.0; extra == "dev"
-Requires-Dist: fairlearn; extra == "dev"
-Requires-Dist: sacrebleu>=2.3.0; extra == "dev"
-Requires-Dist: fast-bss-eval>=0.1.0; extra == "dev"
 Requires-Dist: kornia>=0.6.7; extra == "dev"
-Requires-Dist: bert_score==0.3.13; extra == "dev"
-Requires-Dist: faster-coco-eval>=1.3.3; extra == "dev"
-Requires-Dist: lpips<=0.1.4; extra == "dev"
-Requires-Dist: rouge-score>0.1.0; extra == "dev"
+Requires-Dist: fast-bss-eval>=0.1.0; extra == "dev"
+Requires-Dist: pandas>=1.4.0; extra == "dev"
+Requires-Dist: sewar>=0.4.4; extra == "dev"
+Requires-Dist: sacrebleu>=2.3.0; extra == "dev"
+Requires-Dist: monai==1.3.0; extra == "dev"
 
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.4.0/docs/source/_static/images/logo.png" width="400px">
+<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.4.0.post0/docs/source/_static/images/logo.png" width="400px">
 
 **Machine learning metrics for distributed, scalable PyTorch applications.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="#what-is-torchmetrics">What is Torchmetrics</a> •
@@ -173,16 +176,16 @@
 [![PyPI Status](https://badge.fury.io/py/torchmetrics.svg)](https://badge.fury.io/py/torchmetrics)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torchmetrics)
 ](https://pepy.tech/project/torchmetrics)
 [![Conda](https://img.shields.io/conda/v/conda-forge/torchmetrics?label=conda&color=success)](https://anaconda.org/conda-forge/torchmetrics)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/torchmetrics/blob/master/LICENSE)
 
 [![CI testing | CPU](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests.yml/badge.svg?event=push)](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests.yml)
-[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.4.0)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.4.0)
-[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.4.0/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
+[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.4.0.post0)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.4.0.post0)
+[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.4.0.post0/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Lightning-AI/torchmetrics/master.svg)](https://results.pre-commit.ci/latest/github/Lightning-AI/torchmetrics/master)
 
 [![Documentation Status](https://readthedocs.org/projects/torchmetrics/badge/?version=latest)](https://torchmetrics.readthedocs.io/en/latest/?badge=latest)
 [![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5844769.svg)](https://doi.org/10.5281/zenodo.5844769)
 [![JOSS status](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43/status.svg)](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43)
 
@@ -480,15 +483,15 @@
 values = []
 for i in range(10):
     values.append(acc(preds(i), target(i)))
 fig3, ax3 = acc.plot(values)
 ```
 
 <p align="center">
-  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.4.0/docs/source/_static/images/plot_example.png" width="1000">
+  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.4.0.post0/docs/source/_static/images/plot_example.png" width="1000">
 </p>
 
 For examples of plotting different metrics try running [this example file](examples/plotting.py).
 
 ## Contribute!
 
 The lightning + TorchMetrics team is hard at work adding even more metrics.
```

### Comparing `torchmetrics-1.4.0/src/torchmetrics.egg-info/SOURCES.txt` & `torchmetrics-1.4.0.post0/src/torchmetrics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 requirements/_doctest.txt
 requirements/_integrate.txt
 requirements/_tests.txt
 requirements/audio.txt
 requirements/audio_test.txt
 requirements/base.txt
 requirements/classification_test.txt
+requirements/debug.txt
 requirements/detection.txt
 requirements/detection_test.txt
 requirements/image.txt
 requirements/image_test.txt
 requirements/multimodal.txt
 requirements/nominal_test.txt
 requirements/segmentation_test.txt
```

### Comparing `torchmetrics-1.4.0/src/torchmetrics.egg-info/requires.txt` & `torchmetrics-1.4.0.post0/src/torchmetrics.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,129 +1,133 @@
 numpy>1.20.0
 packaging>17.1
 torch>=1.10.0
 lightning-utilities>=0.8.0
-pretty-errors==1.2.25
 
 [:python_version < "3.9"]
 typing-extensions
 
 [all]
-torchaudio>=0.10.0
 pystoi>=0.3.0
-pycocotools>2.0.0
+torchaudio>=0.10.0
+pretty-errors>=1.2.0
 torchvision>=0.8
-torch-fidelity<=0.4.0
+pycocotools>2.0.0
 scipy>1.0.0
+torch-fidelity<=0.4.0
 transformers>=4.10.0
 piq<=0.8.0
 transformers>4.4.0
-sentencepiece>=0.2.0
+ipadic>=1.0.0
+regex>=2021.9.24
 tqdm>=4.41.0
 mecab-python3>=1.0.6
+sentencepiece>=0.2.0
 nltk>=3.6
-ipadic>=1.0.0
-regex>=2021.9.24
 types-setuptools
+types-six
 types-tabulate
-types-protobuf
-mypy==1.9.0
-types-emoji
+types-PyYAML
 torch==2.3.0
 types-requests
-types-six
-types-PyYAML
+types-emoji
+mypy==1.9.0
+types-protobuf
 matplotlib>=3.3.0
 SciencePlots>=2.0.0
 
 [audio]
-torchaudio>=0.10.0
 pystoi>=0.3.0
+torchaudio>=0.10.0
+
+[debug]
+pretty-errors>=1.2.0
 
 [detection]
-pycocotools>2.0.0
 torchvision>=0.8
+pycocotools>2.0.0
 
 [dev]
-torchaudio>=0.10.0
 pystoi>=0.3.0
-pycocotools>2.0.0
+torchaudio>=0.10.0
+pretty-errors>=1.2.0
 torchvision>=0.8
-torch-fidelity<=0.4.0
+pycocotools>2.0.0
 scipy>1.0.0
+torch-fidelity<=0.4.0
 transformers>=4.10.0
 piq<=0.8.0
 transformers>4.4.0
-sentencepiece>=0.2.0
+ipadic>=1.0.0
+regex>=2021.9.24
 tqdm>=4.41.0
 mecab-python3>=1.0.6
+sentencepiece>=0.2.0
 nltk>=3.6
-ipadic>=1.0.0
-regex>=2021.9.24
 types-setuptools
+types-six
 types-tabulate
-types-protobuf
-mypy==1.9.0
-types-emoji
+types-PyYAML
 torch==2.3.0
 types-requests
-types-six
-types-PyYAML
+types-emoji
+mypy==1.9.0
+types-protobuf
 matplotlib>=3.3.0
 SciencePlots>=2.0.0
+scikit-image>=0.19.0
 mir-eval>=0.6
-pytorch-msssim==1.0.0
-sewar>=0.4.4
+faster-coco-eval>=1.3.3
+numpy<1.27.0
+pandas>1.0.0
+fairlearn
 mecab-ko-dic>=1.0.0
-huggingface-hub<0.23
-statsmodels>0.13.5
+bert_score==0.3.13
+rouge-score>0.1.0
 dython<=0.7.5
+netcal>1.0.0
+pytorch-msssim==1.0.0
 mecab-ko>=1.0.0
-pandas>1.0.0
-numpy<1.25.0
+huggingface-hub<0.23
+statsmodels>0.13.5
 torch_complex<=0.4.3
-scikit-image>=0.19.0
-pandas>=1.4.0
-netcal>1.0.0
-monai==1.3.0
+lpips<=0.1.4
 jiwer>=2.3.0
-fairlearn
-sacrebleu>=2.3.0
-fast-bss-eval>=0.1.0
 kornia>=0.6.7
-bert_score==0.3.13
-faster-coco-eval>=1.3.3
-lpips<=0.1.4
-rouge-score>0.1.0
+fast-bss-eval>=0.1.0
+pandas>=1.4.0
+sewar>=0.4.4
+sacrebleu>=2.3.0
+monai==1.3.0
 
 [image]
-torch-fidelity<=0.4.0
 torchvision>=0.8
 scipy>1.0.0
+torch-fidelity<=0.4.0
 
 [multimodal]
 transformers>=4.10.0
 piq<=0.8.0
 
 [text]
 transformers>4.4.0
-sentencepiece>=0.2.0
+ipadic>=1.0.0
+regex>=2021.9.24
 tqdm>=4.41.0
 mecab-python3>=1.0.6
+sentencepiece>=0.2.0
 nltk>=3.6
-ipadic>=1.0.0
-regex>=2021.9.24
 
 [typing]
 types-setuptools
+types-six
 types-tabulate
-types-protobuf
-mypy==1.9.0
-types-emoji
+types-PyYAML
 torch==2.3.0
 types-requests
-types-six
-types-PyYAML
+types-emoji
+mypy==1.9.0
+types-protobuf
 
 [visual]
 matplotlib>=3.3.0
 SciencePlots>=2.0.0
```

