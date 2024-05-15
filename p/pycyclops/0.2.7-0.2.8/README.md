# Comparing `tmp/pycyclops-0.2.7.tar.gz` & `tmp/pycyclops-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycyclops-0.2.7.tar", max compression
+gzip compressed data, was "pycyclops-0.2.8.tar", max compression
```

## Comparing `pycyclops-0.2.7.tar` & `pycyclops-0.2.8.tar`

### file list

```diff
@@ -1,170 +1,170 @@
--rw-r--r--   0        0        0    11347 2024-05-06 13:04:25.205522 pycyclops-0.2.7/LICENSE.md
--rw-r--r--   0        0        0     6440 2024-05-06 13:04:25.205522 pycyclops-0.2.7/README.md
--rw-r--r--   0        0        0       23 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/__init__.py
--rw-r--r--   0        0        0      192 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/__init__.py
--rw-r--r--   0        0        0    25741 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/aggregate.py
--rw-r--r--   0        0        0     4344 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/clean.py
--rw-r--r--   0        0        0     3469 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/constants.py
--rw-r--r--   0        0        0       39 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/df/__init__.py
--rw-r--r--   0        0        0    26086 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/df/feature.py
--rw-r--r--   0        0        0    26171 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/df/handle_types.py
--rw-r--r--   0        0        0    17267 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/df/normalize.py
--rw-r--r--   0        0        0    12116 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/df/split.py
--rw-r--r--   0        0        0    30240 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/df/vectorized.py
--rw-r--r--   0        0        0     3295 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/diagnoses.py
--rw-r--r--   0        0        0      118 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/features/__init__.py
--rw-r--r--   0        0        0     9640 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/features/medical_image.py
--rw-r--r--   0        0        0    17072 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/impute.py
--rw-r--r--   0        0        0     3228 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/loader.py
--rw-r--r--   0        0        0      638 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/packaged_loading_scripts/__init__.py
--rw-r--r--   0        0        0       36 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/packaged_loading_scripts/medical_imagefolder/__init__.py
--rw-r--r--   0        0        0     2110 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py
--rw-r--r--   0        0        0      881 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/preprocess.py
--rw-r--r--   0        0        0    32163 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/slicer.py
--rw-r--r--   0        0        0     6471 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/string_ops.py
--rw-r--r--   0        0        0     3027 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/transforms.py
--rw-r--r--   0        0        0    13157 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/data/utils.py
--rw-r--r--   0        0        0      139 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/__init__.py
--rw-r--r--   0        0        0    12362 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/evaluator.py
--rw-r--r--   0        0        0      159 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/fairness/__init__.py
--rw-r--r--   0        0        0     1104 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/fairness/config.py
--rw-r--r--   0        0        0    36125 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/fairness/evaluator.py
--rw-r--r--   0        0        0     1837 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0    13476 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/accuracy.py
--rw-r--r--   0        0        0    13702 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/auroc.py
--rw-r--r--   0        0        0     4899 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/average_precision.py
--rw-r--r--   0        0        0     2484 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/__init__.py
--rw-r--r--   0        0        0     7774 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/_stat_scores.py
--rw-r--r--   0        0        0     7217 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/accuracy.py
--rw-r--r--   0        0        0    11290 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/auroc.py
--rw-r--r--   0        0        0    11136 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/average_precision.py
--rw-r--r--   0        0        0    12934 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/confusion_matrix.py
--rw-r--r--   0        0        0     1349 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py
--rw-r--r--   0        0        0     2066 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/base.py
--rw-r--r--   0        0        0     3491 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py
--rw-r--r--   0        0        0     1062 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py
--rw-r--r--   0        0        0     3916 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py
--rw-r--r--   0        0        0    17182 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/f_score.py
--rw-r--r--   0        0        0     2614 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/__init__.py
--rw-r--r--   0        0        0    17136 2024-05-06 13:04:25.209522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py
--rw-r--r--   0        0        0    17396 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/accuracy.py
--rw-r--r--   0        0        0    25070 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/auroc.py
--rw-r--r--   0        0        0    26707 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/average_precision.py
--rw-r--r--   0        0        0    27926 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py
--rw-r--r--   0        0        0    34008 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/f_score.py
--rw-r--r--   0        0        0     2631 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/mae.py
--rw-r--r--   0        0        0     3551 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/mape.py
--rw-r--r--   0        0        0    12394 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py
--rw-r--r--   0        0        0     4101 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/mse.py
--rw-r--r--   0        0        0    16833 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py
--rw-r--r--   0        0        0    32246 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/precision_recall.py
--rw-r--r--   0        0        0    45990 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py
--rw-r--r--   0        0        0    25481 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/roc.py
--rw-r--r--   0        0        0     3612 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/smape.py
--rw-r--r--   0        0        0    16929 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/specificity.py
--rw-r--r--   0        0        0     3253 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/wmape.py
--rw-r--r--   0        0        0     1858 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/mae.py
--rw-r--r--   0        0        0     2498 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/mape.py
--rw-r--r--   0        0        0     6089 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py
--rw-r--r--   0        0        0    26623 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/metric.py
--rw-r--r--   0        0        0    22036 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/metric_dict.py
--rw-r--r--   0        0        0     3290 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/mse.py
--rw-r--r--   0        0        0     7802 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/negative_predictive_value.py
--rw-r--r--   0        0        0    33336 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/precision_recall.py
--rw-r--r--   0        0        0    19586 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/precision_recall_curve.py
--rw-r--r--   0        0        0     9557 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/roc.py
--rw-r--r--   0        0        0     2597 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/smape.py
--rw-r--r--   0        0        0    13798 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/specificity.py
--rw-r--r--   0        0        0      546 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/__init__.py
--rw-r--r--   0        0        0    36009 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/ops.py
--rw-r--r--   0        0        0     9057 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/types.py
--rw-r--r--   0        0        0     4589 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/validation.py
--rw-r--r--   0        0        0     2727 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/wmape.py
--rw-r--r--   0        0        0    26187 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/f_beta.py
--rw-r--r--   0        0        0     1815 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/factory.py
--rw-r--r--   0        0        0     1933 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/__init__.py
--rw-r--r--   0        0        0    16824 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/accuracy.py
--rw-r--r--   0        0        0    22142 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/auroc.py
--rw-r--r--   0        0        0     5544 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/average_precision.py
--rw-r--r--   0        0        0    26687 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/f_beta.py
--rw-r--r--   0        0        0    27455 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/precision_recall.py
--rw-r--r--   0        0        0    37364 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/precision_recall_curve.py
--rw-r--r--   0        0        0    21633 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/roc.py
--rw-r--r--   0        0        0    11342 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/sensitivity.py
--rw-r--r--   0        0        0    16029 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/specificity.py
--rw-r--r--   0        0        0    26592 2024-05-06 13:04:25.213522 pycyclops-0.2.7/cyclops/evaluate/metrics/functional/stat_scores.py
--rw-r--r--   0        0        0    32052 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/metric.py
--rw-r--r--   0        0        0    26995 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/precision_recall.py
--rw-r--r--   0        0        0    23073 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/precision_recall_curve.py
--rw-r--r--   0        0        0    13622 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/roc.py
--rw-r--r--   0        0        0    12350 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/sensitivity.py
--rw-r--r--   0        0        0    14376 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/specificity.py
--rw-r--r--   0        0        0    16991 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/stat_scores.py
--rw-r--r--   0        0        0    10157 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/metrics/utils.py
--rw-r--r--   0        0        0     2388 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/evaluate/utils.py
--rw-r--r--   0        0        0     1658 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/__init__.py
--rw-r--r--   0        0        0     7660 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/catalog.py
--rw-r--r--   0        0        0      727 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/densenet.yaml
--rw-r--r--   0        0        0      647 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/gru.yaml
--rw-r--r--   0        0        0       34 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/logistic_regression.yaml
--rw-r--r--   0        0        0      647 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/lstm.yaml
--rw-r--r--   0        0        0      117 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/mlp_classifier.yaml
--rw-r--r--   0        0        0      577 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/mlp_pt.yaml
--rw-r--r--   0        0        0      512 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/resnet.yaml
--rw-r--r--   0        0        0       53 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/rf_classifier.yaml
--rw-r--r--   0        0        0      590 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/rnn.yaml
--rw-r--r--   0        0        0       91 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/sgd_classifier.yaml
--rw-r--r--   0        0        0      180 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/configs/xgb_classifier.yaml
--rw-r--r--   0        0        0     1791 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/data.py
--rw-r--r--   0        0        0      266 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/neural_nets/__init__.py
--rw-r--r--   0        0        0     2226 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/neural_nets/gru.py
--rw-r--r--   0        0        0     2436 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/neural_nets/lstm.py
--rw-r--r--   0        0        0     3013 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/neural_nets/mlp.py
--rw-r--r--   0        0        0     2214 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/neural_nets/rnn.py
--rw-r--r--   0        0        0     2588 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/plotter.py
--rw-r--r--   0        0        0     7238 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/torch_utils.py
--rw-r--r--   0        0        0     4371 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/utils.py
--rw-r--r--   0        0        0      372 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/wrappers/__init__.py
--rw-r--r--   0        0        0    10026 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/wrappers/base.py
--rw-r--r--   0        0        0    49399 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/wrappers/pt_model.py
--rw-r--r--   0        0        0    39968 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/wrappers/sk_model.py
--rw-r--r--   0        0        0     9899 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/models/wrappers/utils.py
--rw-r--r--   0        0        0      468 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/__init__.py
--rw-r--r--   0        0        0    16172 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/clinical_applicator.py
--rw-r--r--   0        0        0    13248 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/detector.py
--rw-r--r--   0        0        0     2554 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/explainer.py
--rw-r--r--   0        0        0    13859 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/plotter.py
--rw-r--r--   0        0        0     9566 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/reductor.py
--rw-r--r--   0        0        0     9118 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/synthetic_applicator.py
--rw-r--r--   0        0        0    37496 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/tester.py
--rw-r--r--   0        0        0    18561 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/monitor/utils.py
--rw-r--r--   0        0        0       81 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/report/__init__.py
--rw-r--r--   0        0        0      100 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/report/model_card/__init__.py
--rw-r--r--   0        0        0     6005 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/report/model_card/base.py
--rw-r--r--   0        0        0    18872 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/report/model_card/fields.py
--rw-r--r--   0        0        0     3054 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/report/model_card/model_card.py
--rw-r--r--   0        0        0     6166 2024-05-06 13:04:25.217522 pycyclops-0.2.7/cyclops/report/model_card/sections.py
--rw-r--r--   0        0        0       37 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/plot/__init__.py
--rw-r--r--   0        0        0     3275 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/plot/base.py
--rw-r--r--   0        0        0    47331 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/plot/classification.py
--rw-r--r--   0        0        0     5463 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/plot/utils.py
--rw-r--r--   0        0        0    39651 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/report.py
--rw-r--r--   0        0        0     1828 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/templates/model_report/button.js
--rw-r--r--   0        0        0    15741 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/templates/model_report/macros.jinja
--rw-r--r--   0        0        0    14849 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/templates/model_report/model_report.jinja
--rw-r--r--   0        0        0    30509 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/templates/model_report/plot.js
--rw-r--r--   0        0        0    33209 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/report/utils.py
--rw-r--r--   0        0        0      143 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/tasks/__init__.py
--rw-r--r--   0        0        0     7447 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/tasks/base.py
--rw-r--r--   0        0        0    22027 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/tasks/classification.py
--rw-r--r--   0        0        0     4211 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/tasks/utils.py
--rw-r--r--   0        0        0       23 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/__init__.py
--rw-r--r--   0        0        0     4966 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/common.py
--rw-r--r--   0        0        0    10240 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/file.py
--rw-r--r--   0        0        0     2423 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/index.py
--rw-r--r--   0        0        0     3611 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/log.py
--rw-r--r--   0        0        0     2294 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/optional.py
--rw-r--r--   0        0        0     5571 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/plot.py
--rw-r--r--   0        0        0      874 2024-05-06 13:04:25.221522 pycyclops-0.2.7/cyclops/utils/profile.py
--rw-r--r--   0        0        0     6427 2024-05-06 13:04:25.229522 pycyclops-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     8871 1970-01-01 00:00:00.000000 pycyclops-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11347 2024-05-15 14:17:57.619942 pycyclops-0.2.8/LICENSE.md
+-rw-r--r--   0        0        0     6440 2024-05-15 14:17:57.619942 pycyclops-0.2.8/README.md
+-rw-r--r--   0        0        0       23 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/__init__.py
+-rw-r--r--   0        0        0    25741 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/aggregate.py
+-rw-r--r--   0        0        0     4344 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/clean.py
+-rw-r--r--   0        0        0     3469 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/constants.py
+-rw-r--r--   0        0        0       39 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/df/__init__.py
+-rw-r--r--   0        0        0    26086 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/df/feature.py
+-rw-r--r--   0        0        0    26171 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/df/handle_types.py
+-rw-r--r--   0        0        0    17267 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/df/normalize.py
+-rw-r--r--   0        0        0    12116 2024-05-15 14:17:57.619942 pycyclops-0.2.8/cyclops/data/df/split.py
+-rw-r--r--   0        0        0    30240 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/df/vectorized.py
+-rw-r--r--   0        0        0     3295 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/diagnoses.py
+-rw-r--r--   0        0        0      118 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/features/__init__.py
+-rw-r--r--   0        0        0     9640 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/features/medical_image.py
+-rw-r--r--   0        0        0    17072 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/impute.py
+-rw-r--r--   0        0        0     3228 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/loader.py
+-rw-r--r--   0        0        0      638 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/packaged_loading_scripts/__init__.py
+-rw-r--r--   0        0        0       36 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/packaged_loading_scripts/medical_imagefolder/__init__.py
+-rw-r--r--   0        0        0     2110 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py
+-rw-r--r--   0        0        0      881 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/preprocess.py
+-rw-r--r--   0        0        0    35159 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/slicer.py
+-rw-r--r--   0        0        0     6471 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/string_ops.py
+-rw-r--r--   0        0        0     3027 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/transforms.py
+-rw-r--r--   0        0        0    10934 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/data/utils.py
+-rw-r--r--   0        0        0      139 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/__init__.py
+-rw-r--r--   0        0        0    12764 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/evaluator.py
+-rw-r--r--   0        0        0      159 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/fairness/__init__.py
+-rw-r--r--   0        0        0     1104 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/fairness/config.py
+-rw-r--r--   0        0        0    37043 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/fairness/evaluator.py
+-rw-r--r--   0        0        0     1837 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0    13476 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/accuracy.py
+-rw-r--r--   0        0        0    13702 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/auroc.py
+-rw-r--r--   0        0        0     4899 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/average_precision.py
+-rw-r--r--   0        0        0     2484 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/__init__.py
+-rw-r--r--   0        0        0     7774 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/_stat_scores.py
+-rw-r--r--   0        0        0     7217 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/accuracy.py
+-rw-r--r--   0        0        0    11290 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/auroc.py
+-rw-r--r--   0        0        0    11136 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/average_precision.py
+-rw-r--r--   0        0        0    12934 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/confusion_matrix.py
+-rw-r--r--   0        0        0     1349 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py
+-rw-r--r--   0        0        0     2066 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/base.py
+-rw-r--r--   0        0        0     3491 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py
+-rw-r--r--   0        0        0     1062 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py
+-rw-r--r--   0        0        0     3916 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py
+-rw-r--r--   0        0        0    17182 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/f_score.py
+-rw-r--r--   0        0        0     2614 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/__init__.py
+-rw-r--r--   0        0        0    17136 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py
+-rw-r--r--   0        0        0    17396 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/accuracy.py
+-rw-r--r--   0        0        0    25070 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/auroc.py
+-rw-r--r--   0        0        0    26707 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/average_precision.py
+-rw-r--r--   0        0        0    27926 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py
+-rw-r--r--   0        0        0    34008 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/f_score.py
+-rw-r--r--   0        0        0     2631 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/mae.py
+-rw-r--r--   0        0        0     3551 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/mape.py
+-rw-r--r--   0        0        0    12394 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py
+-rw-r--r--   0        0        0     4101 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/mse.py
+-rw-r--r--   0        0        0    16833 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py
+-rw-r--r--   0        0        0    32246 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/precision_recall.py
+-rw-r--r--   0        0        0    45990 2024-05-15 14:17:57.623942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py
+-rw-r--r--   0        0        0    25481 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/roc.py
+-rw-r--r--   0        0        0     3612 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/smape.py
+-rw-r--r--   0        0        0    16929 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/specificity.py
+-rw-r--r--   0        0        0     3253 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/wmape.py
+-rw-r--r--   0        0        0     1858 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/mae.py
+-rw-r--r--   0        0        0     2498 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/mape.py
+-rw-r--r--   0        0        0     6089 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py
+-rw-r--r--   0        0        0    26623 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/metric.py
+-rw-r--r--   0        0        0    22036 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/metric_dict.py
+-rw-r--r--   0        0        0     3290 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/mse.py
+-rw-r--r--   0        0        0     7802 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/negative_predictive_value.py
+-rw-r--r--   0        0        0    33336 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/precision_recall.py
+-rw-r--r--   0        0        0    19586 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/precision_recall_curve.py
+-rw-r--r--   0        0        0     9557 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/roc.py
+-rw-r--r--   0        0        0     2597 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/smape.py
+-rw-r--r--   0        0        0    13798 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/specificity.py
+-rw-r--r--   0        0        0      546 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/__init__.py
+-rw-r--r--   0        0        0    36009 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/ops.py
+-rw-r--r--   0        0        0     9057 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/types.py
+-rw-r--r--   0        0        0     4589 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/validation.py
+-rw-r--r--   0        0        0     2727 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/wmape.py
+-rw-r--r--   0        0        0    26187 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/f_beta.py
+-rw-r--r--   0        0        0     1815 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/factory.py
+-rw-r--r--   0        0        0     1933 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/__init__.py
+-rw-r--r--   0        0        0    16824 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/accuracy.py
+-rw-r--r--   0        0        0    22142 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/auroc.py
+-rw-r--r--   0        0        0     5544 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/average_precision.py
+-rw-r--r--   0        0        0    26687 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/f_beta.py
+-rw-r--r--   0        0        0    27455 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/precision_recall.py
+-rw-r--r--   0        0        0    37364 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/precision_recall_curve.py
+-rw-r--r--   0        0        0    21633 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/roc.py
+-rw-r--r--   0        0        0    11342 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/sensitivity.py
+-rw-r--r--   0        0        0    16029 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/specificity.py
+-rw-r--r--   0        0        0    26592 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/functional/stat_scores.py
+-rw-r--r--   0        0        0    32052 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/metric.py
+-rw-r--r--   0        0        0    26995 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/precision_recall.py
+-rw-r--r--   0        0        0    23073 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/precision_recall_curve.py
+-rw-r--r--   0        0        0    13622 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/roc.py
+-rw-r--r--   0        0        0    12350 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/sensitivity.py
+-rw-r--r--   0        0        0    14376 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/specificity.py
+-rw-r--r--   0        0        0    16991 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/stat_scores.py
+-rw-r--r--   0        0        0    10157 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/metrics/utils.py
+-rw-r--r--   0        0        0     5784 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/evaluate/utils.py
+-rw-r--r--   0        0        0     1658 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/__init__.py
+-rw-r--r--   0        0        0     7660 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/catalog.py
+-rw-r--r--   0        0        0      727 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/densenet.yaml
+-rw-r--r--   0        0        0      647 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/gru.yaml
+-rw-r--r--   0        0        0       34 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/logistic_regression.yaml
+-rw-r--r--   0        0        0      647 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/lstm.yaml
+-rw-r--r--   0        0        0      117 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/mlp_classifier.yaml
+-rw-r--r--   0        0        0      577 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/mlp_pt.yaml
+-rw-r--r--   0        0        0      512 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/resnet.yaml
+-rw-r--r--   0        0        0       53 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/rf_classifier.yaml
+-rw-r--r--   0        0        0      590 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/rnn.yaml
+-rw-r--r--   0        0        0       91 2024-05-15 14:17:57.627942 pycyclops-0.2.8/cyclops/models/configs/sgd_classifier.yaml
+-rw-r--r--   0        0        0      180 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/configs/xgb_classifier.yaml
+-rw-r--r--   0        0        0     1791 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/data.py
+-rw-r--r--   0        0        0      266 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/neural_nets/__init__.py
+-rw-r--r--   0        0        0     2226 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/neural_nets/gru.py
+-rw-r--r--   0        0        0     2436 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/neural_nets/lstm.py
+-rw-r--r--   0        0        0     3013 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/neural_nets/mlp.py
+-rw-r--r--   0        0        0     2214 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/neural_nets/rnn.py
+-rw-r--r--   0        0        0     2588 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/plotter.py
+-rw-r--r--   0        0        0     7238 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/torch_utils.py
+-rw-r--r--   0        0        0     4371 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/utils.py
+-rw-r--r--   0        0        0      372 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/wrappers/__init__.py
+-rw-r--r--   0        0        0    10026 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/wrappers/base.py
+-rw-r--r--   0        0        0    49399 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/wrappers/pt_model.py
+-rw-r--r--   0        0        0    39985 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/wrappers/sk_model.py
+-rw-r--r--   0        0        0     9899 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/models/wrappers/utils.py
+-rw-r--r--   0        0        0      468 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/__init__.py
+-rw-r--r--   0        0        0    16172 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/clinical_applicator.py
+-rw-r--r--   0        0        0    13248 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/detector.py
+-rw-r--r--   0        0        0     2554 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/explainer.py
+-rw-r--r--   0        0        0    13859 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/plotter.py
+-rw-r--r--   0        0        0     9566 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/reductor.py
+-rw-r--r--   0        0        0     9118 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/synthetic_applicator.py
+-rw-r--r--   0        0        0    37496 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/tester.py
+-rw-r--r--   0        0        0    18561 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/monitor/utils.py
+-rw-r--r--   0        0        0       81 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/__init__.py
+-rw-r--r--   0        0        0      100 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/model_card/__init__.py
+-rw-r--r--   0        0        0     6005 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/model_card/base.py
+-rw-r--r--   0        0        0    18872 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/model_card/fields.py
+-rw-r--r--   0        0        0     3054 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/model_card/model_card.py
+-rw-r--r--   0        0        0     6166 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/model_card/sections.py
+-rw-r--r--   0        0        0       37 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/plot/__init__.py
+-rw-r--r--   0        0        0     3275 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/plot/base.py
+-rw-r--r--   0        0        0    47331 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/plot/classification.py
+-rw-r--r--   0        0        0     5463 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/plot/utils.py
+-rw-r--r--   0        0        0    39651 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/report.py
+-rw-r--r--   0        0        0     1828 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/templates/model_report/button.js
+-rw-r--r--   0        0        0    15741 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/templates/model_report/macros.jinja
+-rw-r--r--   0        0        0    14849 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/templates/model_report/model_report.jinja
+-rw-r--r--   0        0        0    30509 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/templates/model_report/plot.js
+-rw-r--r--   0        0        0    33209 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/report/utils.py
+-rw-r--r--   0        0        0      143 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/tasks/__init__.py
+-rw-r--r--   0        0        0     7447 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/tasks/base.py
+-rw-r--r--   0        0        0    22644 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/tasks/classification.py
+-rw-r--r--   0        0        0     4211 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/tasks/utils.py
+-rw-r--r--   0        0        0       23 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/__init__.py
+-rw-r--r--   0        0        0     4966 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/common.py
+-rw-r--r--   0        0        0    10240 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/file.py
+-rw-r--r--   0        0        0     2423 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/index.py
+-rw-r--r--   0        0        0     3611 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/log.py
+-rw-r--r--   0        0        0     2294 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/optional.py
+-rw-r--r--   0        0        0     5571 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/plot.py
+-rw-r--r--   0        0        0      874 2024-05-15 14:17:57.631942 pycyclops-0.2.8/cyclops/utils/profile.py
+-rw-r--r--   0        0        0     6427 2024-05-15 14:17:57.643941 pycyclops-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     8871 1970-01-01 00:00:00.000000 pycyclops-0.2.8/PKG-INFO
```

### Comparing `pycyclops-0.2.7/LICENSE.md` & `pycyclops-0.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/README.md` & `pycyclops-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/aggregate.py` & `pycyclops-0.2.8/cyclops/data/aggregate.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/clean.py` & `pycyclops-0.2.8/cyclops/data/clean.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/constants.py` & `pycyclops-0.2.8/cyclops/data/constants.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/df/feature.py` & `pycyclops-0.2.8/cyclops/data/df/feature.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/df/handle_types.py` & `pycyclops-0.2.8/cyclops/data/df/handle_types.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/df/normalize.py` & `pycyclops-0.2.8/cyclops/data/df/normalize.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/df/split.py` & `pycyclops-0.2.8/cyclops/data/df/split.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/df/vectorized.py` & `pycyclops-0.2.8/cyclops/data/df/vectorized.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/diagnoses.py` & `pycyclops-0.2.8/cyclops/data/diagnoses.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/features/medical_image.py` & `pycyclops-0.2.8/cyclops/data/features/medical_image.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/impute.py` & `pycyclops-0.2.8/cyclops/data/impute.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/loader.py` & `pycyclops-0.2.8/cyclops/data/loader.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/packaged_loading_scripts/__init__.py` & `pycyclops-0.2.8/cyclops/data/packaged_loading_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py` & `pycyclops-0.2.8/cyclops/data/packaged_loading_scripts/medical_imagefolder/medical_imagefolder.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/preprocess.py` & `pycyclops-0.2.8/cyclops/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/slicer.py` & `pycyclops-0.2.8/cyclops/data/slicer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Functions and classes for creating subsets of Hugging Face datasets."""
 
+import copy
 import datetime
+import itertools
 from dataclasses import dataclass, field
 from functools import partial
 from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
+import pyarrow as pa
+import pyarrow.compute as pc
+from datasets.formatting.formatting import LazyBatch
 from dateutil.parser import parse
-from pandas.api.types import is_datetime64_any_dtype, is_numeric_dtype
+from pyarrow import ArrowInvalid
 
 
 @dataclass
 class SliceSpec:
     """Specifications for creating a slices of a dataset.
 
     Parameters
@@ -56,18 +61,24 @@
           Defaults to None.
         - `negate`: A boolean flag indicating whether to negate the slice. If True, the
           slice selects rows where the feature value does not match the specification.
           Defaults to False.
         - `keep_nulls`: A boolean flag indicating whether to keep rows where the value
           is null. If used in conjunction with `negate`, the slice selects rows where
           the value is not null. Can be used on its own. Defaults to False.
-    validate : bool, default=True
-        Whether to validate the column names in the slice specifications.
+    intersections : List[Tuple[int]], int, optional, default=None
+        An indication of slices to intersect. If a list of tuples is provided, the
+        tuples should contain the indices of the slices to intersect. If an integer is
+        provided, it will be passed as the argument `r` in `itertools.combinations`,
+        and all combinations of `r` slices will be intersected. The intersections are
+        created _before_ the slices are registered.
     include_overall : bool, default=True
         Whether to include an `overall` slice that selects all examples.
+    validate : bool, default=True
+        Whether to validate the column names in the slice specifications.
     column_names : List[str], optional, default=None
         List of column names in the dataset. If provided and `validate` is True, it is
         used to validate the column names in the slice specifications.
 
 
     Attributes
     ----------
@@ -133,37 +144,57 @@
     feature_1:month=[6, 7, 8]
     feature_1:month=6, day=1
     feature_1:contains value_1
     feature_1:contains ['value_1', 'value_2']
     feature_1:value_1&feature_2:[2020-01-01 - inf]&feature_3:year=['2000', '2010', '2020']
     overall
 
+    >>> # a different way to create intersections/compound slices
+    >>> slice_spec = SliceSpec(
+    ...     spec_list=[
+    ...         {"feature_1": {"keep_nulls": False}},
+    ...         {"feature_2": {"keep_nulls": False}},
+    ...     ],
+    ...     include_overall=False,
+    ...     intersections=2,
+    ... )
+    >>> for slice_name, slice_func in slice_spec.slices():
+    ...     print(slice_name)
+    ...     # do something with slice_func here (e.g. dataset.filter(slice_func))
+    feature_1:non_null
+    feature_2:non_null
+    feature_1:non_null&feature_2:non_null
+
     """  # noqa: W505
 
     spec_list: List[Dict[str, Dict[str, Any]]] = field(
         default_factory=lambda: [{}],
         init=True,
         repr=True,
         hash=True,
         compare=True,
     )
+    intersections: Optional[Union[List[Tuple[int, ...]], int]] = None
     validate: bool = True
     include_overall: bool = True
     column_names: Optional[List[str]] = None
 
-    _registry: Dict[str, Callable[[Dict[str, Any]], Union[bool, List[bool]]]] = field(
+    _registry: Dict[str, Callable[[Dict[str, Any]], List[bool]]] = field(
         default_factory=dict,
         init=False,
         repr=False,
         hash=False,
         compare=False,
     )
 
     def __post_init__(self) -> None:
         """Create and register slice functions out of the slice specifications."""
+        self.spec_list = copy.deepcopy(self.spec_list)
+        if self.intersections is not None:
+            self._create_intersections()
         for slice_spec in self.spec_list:
             self._parse_and_register_slice_specs(slice_spec)
 
         if self.include_overall:
             self._registry["overall"] = overall
 
     def add_slice_spec(self, slice_spec: Dict[str, Dict[str, Any]]) -> None:
@@ -179,23 +210,48 @@
 
         """
         self._parse_and_register_slice_specs(slice_spec=slice_spec)
         self.spec_list.append(slice_spec)
 
     def get_slices(
         self,
-    ) -> Dict[str, Callable[[Dict[str, Any]], Union[bool, List[bool]]]]:
+    ) -> Dict[str, Callable[[Dict[str, Any]], List[bool]]]:
         """Return the slice function registry."""
         return self._registry
 
     def slices(self) -> Generator[Tuple[str, Callable[..., Any]], None, None]:
         """Return a generator of slice names and slice functions."""
         for registration_key, slice_function in self._registry.items():
             yield registration_key, slice_function
 
+    def _create_intersections(self) -> None:
+        """Create intersections of slices."""
+        intersect_list = []
+        if isinstance(self.intersections, list) and isinstance(
+            self.intersections[0], tuple
+        ):
+            for intersection in self.intersections:
+                intersect_dict = {}
+                for index in set(intersection):
+                    intersect_dict.update(self.spec_list[index])
+                intersect_list.append(intersect_dict)
+        elif isinstance(self.intersections, int):
+            combinations = itertools.combinations(self.spec_list, self.intersections)
+            for combination in combinations:
+                intersect_dict = {}
+                for slice_ in combination:
+                    intersect_dict.update(slice_)
+                intersect_list.append(intersect_dict)
+        else:
+            raise ValueError(
+                "Expected `intersections` to be a list of tuples or an integer. "
+                f"Got {self.intersections} instead.",
+            )
+        self.spec_list.extend(intersect_list)
+
     def _parse_and_register_slice_specs(
         self,
         slice_spec: Dict[str, Dict[str, Any]],
     ) -> None:
         """Construct and register a slice functions from slice specifications."""
         if not isinstance(slice_spec, dict):
             raise TypeError(
@@ -221,15 +277,15 @@
             slice_function = partial(compound_filter, slice_functions=slice_functions)
 
         self._registry[registration_key] = slice_function
 
     def _parse_single_spec_dict(
         self,
         slice_spec: Dict[str, Dict[str, Any]],
-    ) -> Tuple[str, Callable[..., Union[bool, List[bool]]]]:
+    ) -> Tuple[str, Callable[..., List[bool]]]:
         """Return the registration key and slice function for a single slice spec."""
         column_name, spec = next(iter(slice_spec.items()))
 
         # validate column name and spec
         self._check_column_names(column_names=column_name)
         if not isinstance(spec, dict):
             raise TypeError(
@@ -375,61 +431,65 @@
             raise TypeError(
                 "Expected `column_names` to be a string or list of strings."
                 f"Got {type(column_names)} instead.",
             )
 
 
 # filter functions
-def overall(examples: Dict[str, Any]) -> Union[bool, List[bool]]:
+def overall(examples: Union[pa.Table, LazyBatch]) -> List[bool]:
     """Return True for all examples.
 
     Parameters
     ----------
-    examples : Dict[str, Any]
-        A dictionary of features and values.
+    examples : pyarrow.Table, datasets.formatting.formatting.LazyBatch
+        A batch of examples.
 
     Returns
     -------
-    Union[bool, List[bool]]
-        A boolean or a list of booleans containing `True` for all examples.
+    List[bool]
+        A list of booleans containing `True` for all examples.
 
     """
-    result: List[bool] = np.ones_like(
-        next(iter(examples.values())),
-        dtype=bool,
-    ).tolist()
-    if len(result) == 1:
-        return result[0]
-    return result
+    _check_examples(examples)
+    return [True] * (
+        len(list(examples.values())[0])
+        if isinstance(examples, LazyBatch)
+        else len(examples)
+    )
 
 
 def filter_non_null(
-    examples: Dict[str, Any],
+    examples: Union[pa.Table, LazyBatch],
     column_names: Union[str, List[str]],
     negate: bool = False,
-) -> Union[bool, List[bool]]:
+) -> List[bool]:
     """Return True for all examples where the feature/column is not null.
 
     Parameters
     ----------
-    examples : Dict[str, Any]
-        A dictionary of features and values.
+    examples : pyarrow.Table, datasets.formatting.formatting.LazyBatch
+        A batch of examples to filter.
     column_names : Union[str, List[str]]
         The column name(s) on which to filter.
     negate : bool, optional, default=False
         If `True`, negate the filter, i.e. return `True` for all examples where
-        the value is null/nan.
+        the value is null.
 
     Returns
     -------
-    Union[bool, List[bool]]
-        A boolean or a list of booleans containing `True` for all examples where
-        the value is not null/nan.
+    List[bool]
+        A list of booleans containing `True` for all examples where the value is
+        not null.
+
+    Notes
+    -----
+    Floating-point NaN values will not be considered as null.
 
     """
+    _check_examples(examples)
     if not (
         isinstance(column_names, str)
         or (
             isinstance(column_names, list)
             and all(isinstance(key, str) for key in column_names)
         )
     ):
@@ -437,92 +497,97 @@
             "Expected `column_names` to be a string or list of strings. "
             f"Got {column_names} of type {type(column_names)}",
         )
 
     if isinstance(column_names, str):
         column_names = [column_names]
 
-    result = pd.notnull(examples[column_names[0]])
+    mask = pc.invert(pc.is_null(examples[column_names[0]]))
     for column_name in column_names[1:]:
-        result &= pd.notnull(examples[column_name])
+        mask = pc.and_not(mask, pc.is_null(examples[column_name]))
 
     if negate:
-        result = ~result
+        mask = pc.invert(mask)
 
-    return result.tolist()  # type: ignore
+    return mask.to_pylist()  # type: ignore
 
 
 def filter_value(
-    examples: Dict[str, Any],
+    examples: Union[pa.Table, LazyBatch],
     column_name: str,
     value: Union[Any, List[Any]],
     negate: bool = False,
     keep_nulls: bool = False,
-) -> Union[bool, List[bool]]:
+) -> List[bool]:
     """Return True for all examples where the feature/column has the given value.
 
     Parameters
     ----------
-    examples : Dict[str, Any]
-        A dictionary of features and values.
+    examples : pyarrow.Table, datasets.formatting.formatting.LazyBatch
+        A batch of examples to filter.
     column_name : str
         The column name on which to filter.
     value : Union[Any, List[Any]]
         The value or values to find. Exact match is performed.
     negate : bool, optional, default=False
         If `True`, return `True` for all examples where the column does not have
         the given value.
     keep_nulls : bool, optional, default=False
         If `True`, return `True` for all examples in the column where the value is null.
 
     Returns
     -------
-    Union[bool, List[bool]]
-        A boolean or a list of booleans containing `True` for all examples where
-        the feature has the given value or values.
+    List[bool]
+        A list of booleans containing `True` for all examples where the feature
+        has the given value or values.
 
     """
+    _check_examples(examples)
     value_is_datetime = is_datetime(value)  # only checks timestrings
 
-    value = pd.Series(
-        value,
-        dtype="datetime64[ns]" if value_is_datetime else None,
-    ).to_numpy()
-
-    example_values = pd.Series(
-        examples[column_name],
-        dtype="datetime64[ns]" if value_is_datetime else None,
-    ).to_numpy()
-
-    result = np.isin(example_values, value, invert=negate)
-
-    if keep_nulls:
-        result |= pd.isnull(example_values)
-    else:
-        result &= pd.notnull(example_values)
+    if not isinstance(value, list):
+        value = [value]
+    value_arr: pa.Array = pa.array(value)
+
+    if value_is_datetime:
+        value_arr = pc.cast(value_arr, pa.timestamp("ns"))
+
+    example_values = (
+        pc.cast(examples[column_name], pa.timestamp("ns"))
+        if value_is_datetime
+        else examples[column_name]
+    )
+
+    mask = pc.is_in(example_values, value_arr)
 
-    return result.tolist()  # type: ignore
+    if negate:
+        mask = pc.invert(mask)
+
+    nulls = pc.is_null(example_values)
+    mask = pc.or_(mask, nulls) if keep_nulls else pc.and_not(mask, nulls)
+
+    return mask.to_pylist()  # type: ignore
 
 
 def filter_range(
-    examples: Dict[str, Any],
+    examples: Union[pa.Table, LazyBatch],
     column_name: str,
     min_value: float = -np.inf,
     max_value: float = np.inf,
     min_inclusive: bool = True,
     max_inclusive: bool = True,
     negate: bool = False,
     keep_nulls: bool = False,
-) -> Union[bool, List[bool]]:
+) -> List[bool]:
     """Return True for all examples where the value is in the given range.
 
     Parameters
     ----------
-    examples : Dict[str, Any]
-        A dictionary of features and values.
+    examples : pyarrow.Table, datasets.formatting.formatting.LazyBatch
+        A batch of examples to filter.
     column_name : str
         The column name on which to filter.
     min_value : float, optional, default=-np.inf
         The minimum value of the range.
     max_value : float, optional, default=np.inf
         The maximum value of the range.
     min_inclusive : bool, optional, default=True
@@ -533,27 +598,28 @@
         If `True`, return `True` for all examples in the column where the value is
         not in the given range.
     keep_nulls : bool, optional, default=False
         If `True`, return `True` for all examples in the column where the value is null.
 
     Returns
     -------
-    Union[bool, List[bool]]
-        A boolean or a list of booleans containing `True` for all examples in the
-        column where the value is in the given range.
+    List[bool]
+        A list of booleans containing `True` for all examples in the column where
+        the value is in the given range.
 
     Raises
     ------
     ValueError
         If `max_value` is less than `min_value` or if `min_value` and `max_value`
         are equal and either `min_inclusive` or `max_inclusive` is False.
     TypeError
         If the column does not contain numeric or datetime values.
 
     """
+    _check_examples(examples)
     # handle datetime values
     min_value, max_value, value_is_datetime = _maybe_convert_to_datetime(
         min_value,
         max_value,
     )
 
     if min_value > max_value:
@@ -563,61 +629,68 @@
         )
     if min_value == max_value and not (min_inclusive and max_inclusive):
         raise ValueError(
             "`min_value` and `max_value` are equal and either `min_inclusive` or "
             "`max_inclusive` is False. This would result in an empty range.",
         )
 
-    example_values = pd.Series(
-        examples[column_name],
-        dtype="datetime64[ns]" if value_is_datetime else None,
-    )
+    example_values = pa.array(examples[column_name])
+    if value_is_datetime:
+        example_values = pc.cast(example_values, pa.timestamp("ns"))
+        min_value = np.repeat(min_value, len(example_values))  # type: ignore[assignment]
+        max_value = np.repeat(max_value, len(example_values))  # type: ignore[assignment]
 
     if not (  # column does not contain number or datetime values
-        is_numeric_dtype(example_values.dtype)
-        or is_datetime64_any_dtype(example_values.dtype)
+        pa.types.is_integer(example_values.type)
+        or pa.types.is_floating(example_values.type)
+        or pa.types.is_timestamp(example_values.type)
     ):
         raise TypeError(
             "Expected feature to be numeric or datetime, but got "
-            f"{example_values.dtype}.",
+            f"{example_values.type}.",
         )
 
-    result = (
-        ((example_values > min_value) & (example_values < max_value))
-        | ((example_values == min_value) & min_inclusive)
-        | ((example_values == max_value) & max_inclusive)
+    ge = (
+        pc.greater_equal(example_values, min_value)
+        if min_inclusive
+        else pc.greater(example_values, min_value)
+    )
+    le = (
+        pc.less_equal(example_values, max_value)
+        if max_inclusive
+        else pc.less(example_values, max_value)
     )
 
+    mask = pc.and_(ge, le).fill_null(False)
+
     if negate:
-        result = ~result
+        mask = pc.invert(mask)
 
-    if keep_nulls:
-        result |= pd.isnull(example_values)
-    else:
-        result &= pd.notnull(example_values)
+    nulls = pc.is_null(example_values)
+    mask = pc.or_(mask, nulls) if keep_nulls else pc.and_not(mask, nulls)
 
-    return result.tolist()  # type: ignore
+    return mask.to_pylist()  # type: ignore
 
 
 def filter_datetime(
-    examples: Dict[str, Any],
+    examples: Union[pa.Table, LazyBatch],
     column_name: str,
     year: Optional[Union[int, str, List[int], List[str]]] = None,
     month: Optional[Union[int, List[int]]] = None,
     day: Optional[Union[int, List[int]]] = None,
     hour: Optional[Union[int, List[int]]] = None,
     negate: bool = False,
     keep_nulls: bool = False,
-) -> Union[bool, List[bool]]:
+) -> List[bool]:
     """Return True for all examples where the datetime value matches the given datetime.
 
     Parameters
     ----------
-    examples : Dict[str, Any]
-        A dictionary of features and values.
+    examples : pyarrow.Table, datasets.formatting.formatting.LazyBatch
+        A batch of examples to filter.
     column_name : str
         The column name on which to filter.
     year : int, str, List[int], List[str], optional, default=None
         The year to match. If string, it must be a valid year string (e.g. "2020").
         If a list is provided, return `True` for all examples where the year matches
         any of the values in the list.
     month : int, List[int], optional, default=None
@@ -629,190 +702,186 @@
     hour : int, List[int], optional, default=None
         The hour to match. If a list is provided, return `True` for all examples
         where the hour matches any of the values in the list.
     negate : bool, optional, default=False
         If `True`, return `True` for all examples where the value does not match
         the given datetime components.
     keep_nulls : bool, optional, default=False
-        If `True`, return `True` for all examples that have a null/nan/NaT value.
+        If `True`, return `True` for all examples that have a null value.
 
     Returns
     -------
-    Union[bool, List[bool]]
-        A boolean or a list of booleans containing `True` for all examples where
-        the value of a column matches the given datetime components.
+    List[bool]
+        A list of booleans containing `True` for all examples where the value of
+        a column matches the given datetime components.
 
     Raises
     ------
     TypeError
         If the column does not contain datetime values.
 
     """
-    # make sure the column has datetime type
-    example_values = pd.Series(examples[column_name]).to_numpy()
+    _check_examples(examples)
+    example_values = pa.array(examples[column_name])
     try:
-        example_values = example_values.astype("datetime64")
-    except ValueError as exc:
+        example_values = pc.cast(example_values, pa.timestamp("ns"))
+    except ArrowInvalid as exc:
         raise TypeError(
             "Expected datetime feature, but got feature of type "
             f"{example_values.dtype.name}.",
         ) from exc
 
-    # convert the datetime values to year, month, day, hour
-    years, months, days = [
-        example_values.astype(f"M8[{unit}]") for unit in ["Y", "M", "D"]
-    ]
-
-    # get all the values that match the given datetime
-    # acknowledgement: https://stackoverflow.com/a/56260054
-    result = np.ones_like(example_values, dtype=bool)
-    if year is not None:
-        result &= np.isin(
-            element=years.astype(int) + 1970,
-            test_elements=np.asanyarray(year, dtype=int),
+    def _apply_mask(
+        values: pa.Int64Array,
+        value_set: Union[int, str, List[int], List[str]],
+        mask: pa.BooleanArray,
+    ) -> pa.BooleanArray:
+        if isinstance(value_set, (str, int)):
+            value_set = [value_set]  # type: ignore[assignment]
+
+        return pc.and_(
+            mask,
+            pc.is_in(
+                values,
+                pa.array(np.asanyarray(value_set, dtype=int), type=pa.int64()),
+            ),
         )
+
+    mask = pa.array([True] * len(example_values), type=pa.bool_())
+    if year is not None:
+        years = pc.year(example_values)
+        mask = _apply_mask(years, year, mask)
     if month is not None:
-        result &= np.isin(
-            element=((months - years) + 1).astype(int),
-            test_elements=np.asanyarray(month, dtype=int),
-        )
+        months = pc.month(example_values)
+        mask = _apply_mask(months, month, mask)
     if day is not None:
-        result &= np.isin(
-            element=((days - months) + 1).astype(int),
-            test_elements=np.asanyarray(day, dtype=int),
-        )
+        days = pc.year(example_values)
+        mask = _apply_mask(days, day, mask)
     if hour is not None:
-        result &= np.isin(
-            element=(example_values - days).astype("m8[h]").astype(int),
-            test_elements=np.asanyarray(hour, dtype=int),
-        )
+        hours = pc.hour(example_values)
+        mask = _apply_mask(hours, hour, mask)
 
     if negate:
-        result = ~result
+        mask = pc.invert(mask)
 
-    if keep_nulls:
-        result |= pd.isnull(example_values)
-    else:
-        result &= pd.notnull(example_values)
+    nulls = pc.is_null(example_values)
+    mask = pc.or_(mask, nulls) if keep_nulls else pc.and_not(mask, nulls)
 
-    return result.tolist()  # type: ignore
+    return mask.to_pylist()  # type: ignore
 
 
 def filter_string_contains(
-    examples: Dict[str, Any],
+    examples: Union[pa.Table, LazyBatch],
     column_name: str,
     contains: Union[str, List[str]],
     negate: bool = False,
     keep_nulls: bool = False,
-) -> Union[bool, List[bool]]:
+) -> List[bool]:
     """Return True for all examples where the value contains the given substring.
 
     Parameters
     ----------
-    examples : Dict[str, Any]
-        A dictionary of features and values.
+    examples : pyarrow.Table, datasets.formatting.formatting.LazyBatch
+        A batch of examples to filter.
     column_name : str
         The column name on which to filter.
     contains : str, List[str]
-        The substring to match. If a list is provided, return `True` for all
+        The substring(s) to match. If a list is provided, return `True` for all
         examples where the value contains any of the substrings in the list.
     negate : bool, optional, default=False
         If `True`, return `True` for all examples where the value does not contain
         the given substring.
     keep_nulls : bool, optional, default=False
         If `True`, return `True` for all examples that have a null value.
 
     Returns
     -------
-    Union[bool, List[bool]]
-        A boolean or a list of booleans containing `True` for all examples where
-        the value of a column contains the given substring.
+    List[bool]
+        A list of booleans containing `True` for all examples where the value of
+        a column contains the given substring.
 
     Raises
     ------
     TypeError
         If the column does not contain string values or if the values in
         `contains` are not strings.
 
     """
+    _check_examples(examples)
     # make sure the column has string type
-    example_values = pd.Series(examples[column_name])
-    if example_values.dtype.name != "object" and not isinstance(
-        example_values.dtype,
-        pd.StringDtype,
-    ):
+    example_values = pa.array(examples[column_name])
+    if not pa.types.is_string(example_values.type):
         raise ValueError(
             "Expected string feature, but got feature of type "
-            f"{example_values.dtype.name}.",
+            f"{example_values.type}.",
         )
-    if example_values.dtype.name == "object":  # object type could be string
-        try:
-            _ = example_values.str
-        except AttributeError as exc:
-            raise TypeError(
-                "Expected string feature, but got feature of type "
-                f"{example_values.dtype.name}.",
-            ) from exc
 
     # get all the values that contain the given substring
-    result = np.zeros_like(example_values, dtype=bool)
+    mask = pa.array([False] * len(example_values), type=pa.bool_())
     if isinstance(contains, str):
         contains = [contains]
 
     for substring in contains:
         if not isinstance(substring, str):
             raise TypeError(
                 f"Expected string value for `contains`, but got value of type "
                 f"{type(substring)}.",
             )
-        result |= example_values.str.contains(substring, case=False).to_numpy(
-            dtype=bool,
-        )
+        mask = pc.or_(mask, pc.match_substring(example_values, substring))
 
     if negate:
-        result = ~result
+        mask = pc.invert(mask)
 
-    if keep_nulls:
-        result |= pd.isnull(example_values)
-    else:
-        result &= pd.notnull(example_values)
+    nulls = pc.is_null(example_values)
+    mask = pc.or_(mask, nulls) if keep_nulls else pc.and_not(mask, nulls)
 
-    return result.tolist()  # type: ignore
+    return mask.to_pylist()  # type: ignore
 
 
 def compound_filter(
-    examples: Dict[str, Any],
-    slice_functions: List[Callable[..., Union[bool, List[bool]]]],
-) -> Union[bool, List[bool]]:
+    examples: Union[pa.Table, LazyBatch],
+    slice_functions: List[Callable[..., List[bool]]],
+) -> List[bool]:
     """Combine the result of multiple slices using bitwise AND.
 
     Parameters
     ----------
-    examples : Dict[str, Any]
+    examples : pyarrow.Table, datasets.formatting.formatting.LazyBatch
         A dictionary mapping column names to values.
-    slice_functions : List[Callable]
+    slice_functions : List[Callable[..., List[bool]]]
         A list of functions to apply to the examples. The signature of each
-        function should be: `slice_function(examples, **kwargs)`.
-        The result of each function should be a boolean or a list of booleans.
+        function should be: `slice_function(examples, **kwargs)`. The result of
+        each function should be a list of booleans.
 
     Returns
     -------
-    Union[bool, List[bool]]
-        A boolean or a list of booleans containing `True` for all examples where
-        each slice function returns `True`.
+    List[bool]
+        A list of booleans containing `True` for all examples where each slice
+        function returns `True`.
 
     """
-    result: Union[bool, List[bool]] = np.bitwise_and.reduce(
+    _check_examples(examples)
+    mask: List[bool] = np.bitwise_and.reduce(
         [slice_function(examples) for slice_function in slice_functions],
     )
 
-    return result
+    return mask
 
 
 # utility functions
+def _check_examples(examples: Union[pa.Table, LazyBatch]) -> None:
+    """Check the type of `examples."""
+    if not isinstance(examples, (pa.Table, LazyBatch)):
+        raise TypeError(
+            "Expected `examples` to be an instance of pyarrow.table or "
+            "datasets.formatting.formatting.LazyBatch but got "
+            f"{type(examples)}"
+        )
+
+
 def is_datetime(
     value: Union[
         str,
         datetime.datetime,
         np.datetime64,
         np.ndarray[Any, np.dtype[Any]],
         List[Any],
```

### Comparing `pycyclops-0.2.7/cyclops/data/string_ops.py` & `pycyclops-0.2.8/cyclops/data/string_ops.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/transforms.py` & `pycyclops-0.2.8/cyclops/data/transforms.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/data/utils.py` & `pycyclops-0.2.8/cyclops/data/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 """Utilities for datasets."""
 
 import logging
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union, get_args
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Union,
+    get_args,
+)
 
-import numpy as np
-import numpy.typing as npt
 import pandas as pd
 import PIL
 import psutil
 from datasets import Dataset, DatasetDict
 from datasets.features import (
     Array2D,
     Array3D,
     Array4D,
     Array5D,
     ClassLabel,
     Sequence,
     Value,
 )
-from numpy.typing import ArrayLike
 
 from cyclops.utils.common import to_list
 from cyclops.utils.log import setup_logging
 from cyclops.utils.optional import import_optional_module
 
 
 # Logging.
@@ -106,86 +112,14 @@
                     dataset[key].features[feature_name].decode = decode
     else:
         for feature_name, feature in dataset.features.items():
             if feature_name not in (exclude or []) and hasattr(feature, "decode"):
                 dataset.features[feature_name].decode = decode
 
 
-def get_columns_as_numpy_array(
-    dataset: Union[Dataset, Dict[str, ArrayLike]],
-    columns: Union[str, List[str]],
-) -> npt.NDArray[Any]:
-    """Get columns of dataset as numpy array.
-
-    Parameters
-    ----------
-    dataset : Dataset, Dict[str, ArrayLike]
-        A Hugging Face dataset object or a dictionary of arraylike objects.
-    columns : List[str], str
-        List of column names or single column name to get as numpy array.
-
-    Returns
-    -------
-    np.ndarray
-        Numpy array of columns.
-
-    """
-    if not isinstance(dataset, (Dataset, dict)):
-        raise TypeError(
-            "dataset must be a Hugging Face dataset or a dictionary of numpy arrays.",
-        )
-
-    if isinstance(columns, str):
-        columns = [columns]
-
-    if isinstance(dataset, Dataset) and dataset.format != "numpy":
-        with dataset.formatted_as("numpy", columns=columns, output_all_columns=True):
-            out_arr = np.stack([dataset[col] for col in columns], axis=-1).squeeze()
-    else:
-        out_arr = np.stack([dataset[col] for col in columns], axis=-1).squeeze()
-
-    if out_arr.ndim == 0:
-        out_arr = np.expand_dims(out_arr, axis=-1)
-
-    return out_arr  # type: ignore[no-any-return]
-
-
-def check_required_columns(
-    dataset_column_names: List[str],
-    *required_columns: Union[List[str], str, None],
-) -> None:
-    """Check if required columns are present in dataset.
-
-    Parameters
-    ----------
-    dataset_column_names : List[str]
-        List of column names in dataset.
-    required_columns : Union[List[str], str, None]
-        List of required column names or single required column name.
-
-    Raises
-    ------
-    ValueError
-        If a required column is not present in the dataset.
-
-    """
-    required_columns_ = [
-        column
-        for column in required_columns
-        if column is not None
-        for column in (column if isinstance(column, list) else [column])
-        if column is not None
-    ]
-    missing_columns = set(required_columns_) - set(dataset_column_names)
-    if missing_columns:
-        raise ValueError(
-            f"Dataset is missing the following required columns: {missing_columns}.",
-        )
-
-
 def feature_is_numeric(feature: FEATURE_TYPES) -> bool:
     """Check if Hugging Face dataset feature is numeric.
 
     Parameters
     ----------
     feature : Union[ClassLabel, Sequence, Value, Array2D, Array3D, Array4D, Array5D]
         Hugging Face dataset feature.
```

### Comparing `pycyclops-0.2.7/cyclops/evaluate/evaluator.py` & `pycyclops-0.2.8/cyclops/evaluate/evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Evaluate one or more models on a dataset."""
 
 import logging
 import warnings
 from dataclasses import asdict
-from typing import Any, Dict, List, Optional, Sequence, Union
+from typing import Any, Dict, List, Literal, Optional, Sequence, Union
 
 from datasets import Dataset, DatasetDict, config, load_dataset
 from datasets.splits import Split
 
 from cyclops.data.slicer import SliceSpec
-from cyclops.data.utils import (
-    check_required_columns,
-    get_columns_as_numpy_array,
-    set_decode,
-)
+from cyclops.data.utils import set_decode
 from cyclops.evaluate.fairness.config import FairnessConfig
 from cyclops.evaluate.fairness.evaluator import evaluate_fairness
 from cyclops.evaluate.metrics.experimental.metric import Metric
 from cyclops.evaluate.metrics.experimental.metric_dict import MetricDict
 from cyclops.evaluate.metrics.experimental.utils.types import Array
-from cyclops.evaluate.utils import _format_column_names, choose_split
+from cyclops.evaluate.utils import (
+    _format_column_names,
+    check_required_columns,
+    choose_split,
+    get_columns_as_array,
+)
 from cyclops.utils.log import setup_logging
 
 
 LOGGER = logging.getLogger(__name__)
 setup_logging(print_level="WARN", logger=LOGGER)
 
 
@@ -36,14 +37,15 @@
     slice_spec: Optional[SliceSpec] = None,
     split: Optional[Union[str, Split]] = None,
     batch_size: Optional[int] = config.DEFAULT_MAX_BATCH_SIZE,
     raise_on_empty_slice: bool = False,
     fairness_config: Optional[FairnessConfig] = None,
     override_fairness_metrics: bool = True,
     load_dataset_kwargs: Optional[Dict[str, Any]] = None,
+    array_lib: Literal["numpy", "torch", "cupy"] = "numpy",
 ) -> Dict[str, Any]:
     """Evaluate one or more models on a dataset using one or more metrics.
 
     Parameters
     ----------
     dataset : Union[str, Dataset, DatasetDict]
         The dataset to evaluate on. If a string, the dataset will be loaded
@@ -93,14 +95,17 @@
         to this function.
     override_fairness_metrics : bool, optional, default=True
         If True, the `metrics` argument in fairness_config will be overridden by
         the `metrics` argument provided to this function.
     load_dataset_kwargs : Dict[str, Any], optional
         Keyword arguments to pass to `datasets.load_dataset`. Only used if
         `dataset` is a string.
+    array_lib : {"numpy", "torch", "cupy"}, default="numpy"
+        The array library to use for the metric computation. The metric results
+        will be returned in the format of `array_lib`.
 
     Returns
     -------
     Dict[str, Any]
         A dictionary containing the results of the evaluation.
 
     Raises
@@ -127,14 +132,15 @@
         metrics=metrics,
         slice_spec=slice_spec,
         target_columns=target_columns,
         prediction_columns=prediction_columns,
         ignore_columns=ignore_columns,
         batch_size=batch_size,
         raise_on_empty_slice=raise_on_empty_slice,
+        array_lib=array_lib,
     )
 
     results = {}
     results.update(metric_results)
 
     if fairness_config is not None:
         if override_fairness_metrics:
@@ -228,27 +234,24 @@
     metrics: MetricDict,
     slice_spec: SliceSpec,
     target_columns: Union[str, List[str]],
     prediction_columns: Union[str, List[str]],
     ignore_columns: Optional[Union[str, List[str]]] = None,
     batch_size: Optional[int] = config.DEFAULT_MAX_BATCH_SIZE,
     raise_on_empty_slice: bool = False,
+    array_lib: Literal["numpy", "torch", "cupy"] = "numpy",
 ) -> Dict[str, Dict[str, Any]]:
     """Compute metrics for a dataset."""
     target_columns = _format_column_names(target_columns)
     prediction_columns = _format_column_names(prediction_columns)
 
     # temporarily stop decoding features to save memory
     set_decode(dataset, False, exclude=target_columns + prediction_columns)
 
-    with dataset.formatted_as(
-        "numpy",
-        columns=target_columns + prediction_columns,
-        output_all_columns=True,
-    ):
+    with dataset.formatted_as("arrow", columns=target_columns + prediction_columns):
         results: Dict[str, Dict[str, Any]] = {}
         for slice_name, slice_fn in slice_spec.slices():
             sliced_dataset = dataset.remove_columns(ignore_columns or []).filter(
                 slice_fn,
                 batched=True,
                 batch_size=batch_size,
                 desc=f"Filter -> {slice_name}",
@@ -271,32 +274,34 @@
                     metric_output: Dict[str, Array] = {
                         metric_name: float("NaN")  # type: ignore
                         for metric_name in metrics  # type: ignore
                     }
                 elif (
                     batch_size is None or batch_size < 0
                 ):  # dataset.iter does not support getting all batches at once
-                    targets = get_columns_as_numpy_array(
+                    targets = get_columns_as_array(
                         dataset=sliced_dataset,
                         columns=target_columns,
+                        array_lib=array_lib,
                     )
-                    predictions = get_columns_as_numpy_array(
+                    predictions = get_columns_as_array(
                         dataset=sliced_dataset,
                         columns=prediction_column,
+                        array_lib=array_lib,
                     )
                     metric_output = metrics(targets, predictions)
                 else:
                     for batch in sliced_dataset.iter(batch_size=batch_size):
-                        targets = get_columns_as_numpy_array(
-                            dataset=batch,
-                            columns=target_columns,
+                        targets = get_columns_as_array(
+                            dataset=batch, columns=target_columns, array_lib=array_lib
                         )
-                        predictions = get_columns_as_numpy_array(
+                        predictions = get_columns_as_array(
                             dataset=batch,
                             columns=prediction_column,
+                            array_lib=array_lib,
                         )
 
                         # update the metric state
                         metrics.update(targets, predictions)
 
                     metric_output = metrics.compute()
                     metrics.reset()
```

### Comparing `pycyclops-0.2.7/cyclops/evaluate/fairness/config.py` & `pycyclops-0.2.8/cyclops/evaluate/fairness/config.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/fairness/evaluator.py` & `pycyclops-0.2.8/cyclops/evaluate/fairness/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 """Fairness evaluator."""
 
 import inspect
 import itertools
 import logging
 import warnings
 from datetime import datetime
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Literal, Optional, Union
 
-import array_api_compat.numpy
 import numpy as np
 import pandas as pd
 from datasets import Dataset, config
 from datasets.features import Features
 
 from cyclops.data.slicer import SliceSpec, is_datetime
 from cyclops.data.utils import (
-    check_required_columns,
     feature_is_datetime,
     feature_is_numeric,
-    get_columns_as_numpy_array,
     set_decode,
 )
 from cyclops.evaluate.metrics.experimental.functional.precision_recall_curve import (
     _format_thresholds,
     _validate_thresholds,
 )
 from cyclops.evaluate.metrics.experimental.metric import Metric, OperatorMetric
 from cyclops.evaluate.metrics.experimental.metric_dict import MetricDict
 from cyclops.evaluate.metrics.experimental.utils.types import Array
 from cyclops.evaluate.metrics.factory import create_metric
-from cyclops.evaluate.utils import _format_column_names
+from cyclops.evaluate.utils import (
+    _SUPPORTED_ARRAY_LIBS,
+    _format_column_names,
+    check_required_columns,
+    get_columns_as_array,
+)
 from cyclops.utils.log import setup_logging
 
 
 LOGGER = logging.getLogger(__name__)
 setup_logging(print_level="WARN", logger=LOGGER)
 
 
-def evaluate_fairness(
+def evaluate_fairness(  # noqa: PLR0912
     metrics: Union[str, Callable[..., Any], Metric, MetricDict],
     dataset: Dataset,
     groups: Union[str, List[str]],
     target_columns: Union[str, List[str]],
     prediction_columns: Union[str, List[str]],
     group_values: Optional[Dict[str, Any]] = None,
     group_bins: Optional[Dict[str, Union[int, List[Any]]]] = None,
@@ -49,14 +51,15 @@
     thresholds: Optional[Union[int, List[float]]] = None,
     compute_optimal_threshold: bool = False,  # expensive operation
     remove_columns: Optional[Union[str, List[str]]] = None,
     batch_size: Optional[int] = config.DEFAULT_MAX_BATCH_SIZE,
     raise_on_empty_slice: bool = False,
     metric_name: Optional[str] = None,
     metric_kwargs: Optional[Dict[str, Any]] = None,
+    array_lib: Literal["torch", "numpy", "cupy"] = "numpy",
 ) -> Union[Dict[str, Dict[str, Any]], Dict[str, Dict[str, Dict[str, Any]]]]:
     """Compute fairness indicators.
 
     This function computes fairness indicators for a dataset that includes
     predictions and targets.
 
     Parameters
@@ -116,14 +119,17 @@
         Whether to raise an error if an empty slice is encountered when computing
         metrics. If False, the metric values for the slice will be set to `NaN`.
     metric_name : Optional[str], optional, default=None
         The name of the metric. If None, the name of the metric will be used.
     metric_kwargs : Optional[Dict[str, Any]], optional, default=None
         Keyword arguments to use when creating the metric. Only used if metrics is a
         string.
+    array_lib : {"numpy", "torch", "cupy"}, default="numpy"
+        The array library to use for the metric computation. The metric results
+        will be returned in the format of `array_lib`.
 
     Returns
     -------
     Union[Dict[str, Dict[str, Any]], Dict[str, Dict[str, Dict[str, Any]]]]
         A nested dictionary containing the metric values. The first level of the
         dictionary is keyed by the prediction columns. The second level of the
         dictionary is keyed by the metric names. The third level of the dictionary
@@ -142,22 +148,24 @@
 
     """
     # input validation and formatting
     if not isinstance(dataset, Dataset):
         raise TypeError(
             "Expected `dataset` to be of type `Dataset`, but got " f"{type(dataset)}.",
         )
+    if array_lib not in _SUPPORTED_ARRAY_LIBS:
+        raise NotImplementedError(f"The array library `{array_lib}` is not supported.")
     _validate_thresholds(thresholds)
 
     metrics_: Union[Callable[..., Any], MetricDict] = _format_metrics(
         metrics,
         metric_name,
         **(metric_kwargs or {}),
     )
-    fmt_thresholds = _format_thresholds(thresholds, xp=array_api_compat.numpy)
+    fmt_thresholds = _format_thresholds(thresholds, xp=_SUPPORTED_ARRAY_LIBS[array_lib])
     fmt_groups: List[str] = _format_column_names(groups)
     fmt_target_columns: List[str] = _format_column_names(target_columns)
     fmt_prediction_columns: List[str] = _format_column_names(prediction_columns)
 
     check_required_columns(
         dataset.column_names,
         fmt_groups,
@@ -171,17 +179,15 @@
     set_decode(
         dataset,
         decode=False,
         exclude=fmt_target_columns + fmt_prediction_columns,
     )  # don't decode columns that we don't need; pass dataset by reference
 
     with dataset.formatted_as(
-        "numpy",
-        columns=fmt_groups + fmt_target_columns + fmt_prediction_columns,
-        output_all_columns=True,
+        "arrow", columns=fmt_groups + fmt_target_columns + fmt_prediction_columns
     ):
         unique_values: Dict[str, List[Any]] = _get_unique_values(
             dataset=dataset,
             groups=fmt_groups,
             group_values=group_values,
         )
 
@@ -262,14 +268,15 @@
                     dataset=sliced_dataset,
                     target_columns=fmt_target_columns,
                     prediction_column=prediction_column,
                     slice_name=slice_name,
                     batch_size=batch_size,
                     metric_name=metric_name,
                     thresholds=fmt_thresholds,
+                    array_lib=array_lib,
                 )
                 # if metric_name does not exist, add it to the dictionary
                 # otherwise, update the dictionary for the metric_name
                 for key, slice_result in pred_result.items():
                     results[prediction_column].setdefault(key, {}).update(slice_result)
 
                 if compute_optimal_threshold:
@@ -283,21 +290,19 @@
 
     set_decode(dataset, decode=True)  # reset decode
 
     # compute parity metrics
     if group_base_values is not None:
         base_slice_name = _construct_base_slice_name(base_values=group_base_values)
         parity_results = _compute_parity_metrics(
-            results=results,
-            base_slice_name=base_slice_name,
+            results=results, base_slice_name=base_slice_name, array_lib=array_lib
         )
     else:
         parity_results = _compute_parity_metrics(
-            results=results,
-            base_slice_name="overall",
+            results=results, base_slice_name="overall", array_lib=array_lib
         )
 
     # add parity metrics to the results
     for pred_column, pred_results in parity_results.items():
         for slice_name, slice_results in pred_results.items():
             results[pred_column][slice_name].update(slice_results)
 
@@ -699,14 +704,15 @@
     metrics: Union[Callable[..., Any], MetricDict],
     dataset: Dataset,
     target_columns: List[str],
     prediction_column: str,
     threshold: Optional[float] = None,
     batch_size: Optional[int] = config.DEFAULT_MAX_BATCH_SIZE,
     metric_name: Optional[str] = None,
+    array_lib: Literal["torch", "numpy", "cupy"] = "numpy",
 ) -> Dict[str, Any]:
     """Compute the metrics for the dataset.
 
     Parameters
     ----------
     metrics : Union[Callable, MetricDict]
         The metrics to compute.
@@ -758,32 +764,28 @@
             results: Dict[str, Any] = {
                 metric_name: float("NaN")
                 for metric_name in metrics  # type: ignore[attr-defined]
             }
         elif (
             batch_size is None or batch_size <= 0
         ):  # dataset.iter does not support getting all rows
-            targets = get_columns_as_numpy_array(
-                dataset=dataset,
-                columns=target_columns,
-            )
-            predictions = get_columns_as_numpy_array(
-                dataset=dataset,
-                columns=prediction_column,
+            targets = get_columns_as_array(
+                dataset=dataset, columns=target_columns, array_lib=array_lib
+            )
+            predictions = get_columns_as_array(
+                dataset=dataset, columns=prediction_column, array_lib=array_lib
             )
             results = metrics(targets, predictions)
         else:
             for batch in dataset.iter(batch_size=batch_size):
-                targets = get_columns_as_numpy_array(
-                    dataset=batch,
-                    columns=target_columns,
+                targets = get_columns_as_array(
+                    dataset=batch, columns=target_columns, array_lib=array_lib
                 )
-                predictions = get_columns_as_numpy_array(
-                    dataset=batch,
-                    columns=prediction_column,
+                predictions = get_columns_as_array(
+                    dataset=batch, columns=prediction_column, array_lib=array_lib
                 )
 
                 metrics.update(targets, predictions)
 
             results = metrics.compute()
 
         metrics.reset()
@@ -793,18 +795,19 @@
         if metric_name is None:
             metric_name = getattr(metrics, "__name__", "Unnamed Metric")
 
         if len(dataset) == 0:
             warnings.warn(empty_dataset_msg, RuntimeWarning, stacklevel=1)
             return {metric_name.title(): float("NaN")}
 
-        targets = get_columns_as_numpy_array(dataset=dataset, columns=target_columns)
-        predictions = get_columns_as_numpy_array(
-            dataset=dataset,
-            columns=prediction_column,
+        targets = get_columns_as_array(
+            dataset=dataset, columns=target_columns, array_lib=array_lib
+        )
+        predictions = get_columns_as_array(
+            dataset=dataset, columns=prediction_column, array_lib=array_lib
         )
 
         # check if the callable can take thresholds as an argument
         if threshold is not None:
             if "threshold" in inspect.signature(metrics).parameters:
                 output = metrics(targets, predictions, threshold=threshold)
             else:
@@ -830,14 +833,15 @@
     dataset: Dataset,
     target_columns: List[str],
     prediction_column: str,
     slice_name: str,
     batch_size: Optional[int] = config.DEFAULT_MAX_BATCH_SIZE,
     metric_name: Optional[str] = None,
     thresholds: Optional[Array] = None,
+    array_lib: Literal["torch", "numpy", "cupy"] = "numpy",
 ) -> Dict[str, Dict[str, Any]]:
     """Compute metrics for a slice of a dataset.
 
     Parameters
     ----------
     metrics : Union[Callable, MetricDict]
         The metrics to compute.
@@ -851,14 +855,17 @@
         The name of the slice.
     batch_size : int
         The batch size to use for the computation.
     metric_name : Optional[str]
         The name of the metric to compute.
     thresholds : Optional[Array]
         The thresholds to use for the metrics.
+    array_lib : {"numpy", "torch", "cupy"}, default="numpy"
+        The array library to use for the metric computation. The metric results
+        will be returned in the format of `array_lib`.
 
     Returns
     -------
     Dict[str, Dict[str, Any]]
         The computed metrics.
 
     """
@@ -866,14 +873,15 @@
         metric_output = _compute_metrics(
             metrics=metrics,
             dataset=dataset,
             target_columns=target_columns,
             prediction_column=prediction_column,
             batch_size=batch_size,
             metric_name=metric_name,
+            array_lib=array_lib,
         )
 
         # result format -> {slice_name: {metric_name: metric_value}}
         return {slice_name: metric_output}
 
     results: Dict[str, Dict[str, Any]] = {}
     for threshold in thresholds:  # type: ignore[attr-defined]
@@ -881,14 +889,15 @@
             metrics=metrics,
             dataset=dataset,
             target_columns=target_columns,
             prediction_column=prediction_column,
             batch_size=batch_size,
             threshold=threshold,
             metric_name=metric_name,
+            array_lib=array_lib,
         )
 
         # result format -> {slice_name: {metric_name@threshold: metric_value}}
         for key, value in metric_output.items():
             results.setdefault(slice_name, {}).update({f"{key}@{threshold}": value})
     return results
 
@@ -923,30 +932,35 @@
             base_slice_name += f"{group}:{base_value}&"
     return base_slice_name[:-1]
 
 
 def _compute_parity_metrics(
     results: Dict[str, Dict[str, Dict[str, Any]]],
     base_slice_name: str,
+    array_lib: Literal["numpy", "torch", "cupy"],
 ) -> Dict[str, Dict[str, Dict[str, Any]]]:
     """Compute the parity metrics for each group and threshold if specified.
 
     Parameters
     ----------
     results : Dict[str, Dict[str, Dict[str, Any]]]
         A dictionary mapping the prediction column to the metrics dictionary.
     base_slice_name : str
         The name of the base slice.
+    array_lib : {"numpy", "torch", "cupy"}, default="numpy"
+        The array library to use for the metric computation. The metric results
+        will be returned in the format of `array_lib`.
 
     Returns
     -------
     Dict[str, Dict[str, Dict[str, Any]]]
         A dictionary mapping the prediction column to the metrics dictionary.
 
     """
+    xp = _SUPPORTED_ARRAY_LIBS[array_lib]
     parity_results: Dict[str, Dict[str, Dict[str, Any]]] = {}
 
     for key, prediction_result in results.items():
         parity_results[key] = {}
         for slice_name, slice_result in prediction_result.items():
             for metric_name, metric_value in slice_result.items():
                 if metric_name == "Group Size":
@@ -957,22 +971,17 @@
                 parity_metric_name = f"{metric_name_parts[0]} Parity"
                 if len(metric_name_parts) > 1:
                     parity_metric_name += f"@{metric_name_parts[1]}"
 
                 numerator = metric_value
                 denominator = prediction_result[base_slice_name][metric_name]
                 # value is NaN if either the numerator or denominator is NaN
-                if np.isnan(numerator).all() or np.isnan(denominator).all():
-                    parity_metric_value = np.nan
+                if xp.all(xp.isnan(numerator)) or xp.all(xp.isnan(denominator)):
+                    parity_metric_value = xp.nan
                 else:
-                    parity_metric_value = np.divide(  # type: ignore[assignment]
-                        numerator,
-                        denominator,
-                        out=np.zeros_like(numerator, dtype=np.float_),
-                        where=denominator != 0,
-                    )
+                    parity_metric_value = xp.divide(numerator, denominator)
 
                 parity_results[key].setdefault(slice_name, {}).update(
                     {parity_metric_name: parity_metric_value},
                 )
 
     return parity_results
```

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/__init__.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/accuracy.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/auroc.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/average_precision.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/__init__.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/_stat_scores.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/_stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/accuracy.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/auroc.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/average_precision.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/confusion_matrix.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/base.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/mpi4py.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/non_distributed.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/distributed_backends/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/f_score.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/f_score.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/__init__.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/_stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/accuracy.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/auroc.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/average_precision.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/f_score.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/f_score.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/mae.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/mae.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/mape.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/mape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/matthews_corr_coef.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/mse.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/mse.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/negative_predictive_value.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/precision_recall.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/roc.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/smape.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/smape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/specificity.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/functional/wmape.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/functional/wmape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/mae.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/mae.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/mape.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/mape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/matthews_corr_coef.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/metric.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/metric.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/metric_dict.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/metric_dict.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/mse.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/mse.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/negative_predictive_value.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/negative_predictive_value.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/precision_recall.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/precision_recall_curve.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/roc.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/smape.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/smape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/specificity.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/__init__.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/ops.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/ops.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/types.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/types.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/utils/validation.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/utils/validation.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/experimental/wmape.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/experimental/wmape.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/f_beta.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/f_beta.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/factory.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/factory.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/__init__.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/accuracy.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/accuracy.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/auroc.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/auroc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/average_precision.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/average_precision.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/f_beta.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/f_beta.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/precision_recall.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/precision_recall_curve.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/roc.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/sensitivity.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/sensitivity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/specificity.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/functional/stat_scores.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/functional/stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/metric.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/precision_recall.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/precision_recall.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/precision_recall_curve.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/roc.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/roc.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/sensitivity.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/sensitivity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/specificity.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/specificity.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/stat_scores.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/stat_scores.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/evaluate/metrics/utils.py` & `pycyclops-0.2.8/cyclops/evaluate/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/__init__.py` & `pycyclops-0.2.8/cyclops/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/catalog.py` & `pycyclops-0.2.8/cyclops/models/catalog.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/configs/densenet.yaml` & `pycyclops-0.2.8/cyclops/models/configs/densenet.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/configs/gru.yaml` & `pycyclops-0.2.8/cyclops/models/configs/gru.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/configs/lstm.yaml` & `pycyclops-0.2.8/cyclops/models/configs/lstm.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/configs/mlp_pt.yaml` & `pycyclops-0.2.8/cyclops/models/configs/mlp_pt.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/configs/resnet.yaml` & `pycyclops-0.2.8/cyclops/models/configs/resnet.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/configs/rnn.yaml` & `pycyclops-0.2.8/cyclops/models/configs/rnn.yaml`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/data.py` & `pycyclops-0.2.8/cyclops/models/data.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/neural_nets/gru.py` & `pycyclops-0.2.8/cyclops/models/neural_nets/gru.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/neural_nets/lstm.py` & `pycyclops-0.2.8/cyclops/models/neural_nets/lstm.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/neural_nets/mlp.py` & `pycyclops-0.2.8/cyclops/models/neural_nets/mlp.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/neural_nets/rnn.py` & `pycyclops-0.2.8/cyclops/models/neural_nets/rnn.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/plotter.py` & `pycyclops-0.2.8/cyclops/models/plotter.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/torch_utils.py` & `pycyclops-0.2.8/cyclops/models/torch_utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/utils.py` & `pycyclops-0.2.8/cyclops/models/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/wrappers/base.py` & `pycyclops-0.2.8/cyclops/models/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/wrappers/pt_model.py` & `pycyclops-0.2.8/cyclops/models/wrappers/pt_model.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/models/wrappers/sk_model.py` & `pycyclops-0.2.8/cyclops/models/wrappers/sk_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,15 @@
                     when using a numpy array or pandas dataframe as the input.",
                 )
 
             self.model_.partial_fit(X, y, classes=classes, **kwargs)
 
         return self
 
-    def fit(
+    def fit(  # noqa: PLR0912
         self,
         X: Union[ArrayLike, Dataset, DatasetDict],
         y: Optional[ArrayLike] = None,
         feature_columns: Optional[Union[str, List[str]]] = None,
         target_columns: Optional[Union[str, List[str]]] = None,
         transforms: Optional[Union[Pipeline, TransformerMixin, Callable]] = None,
         splits_mapping: dict = None,
```

### Comparing `pycyclops-0.2.7/cyclops/models/wrappers/utils.py` & `pycyclops-0.2.8/cyclops/models/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/monitor/clinical_applicator.py` & `pycyclops-0.2.8/cyclops/monitor/clinical_applicator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/monitor/detector.py` & `pycyclops-0.2.8/cyclops/monitor/detector.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/monitor/explainer.py` & `pycyclops-0.2.8/cyclops/monitor/explainer.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/monitor/plotter.py` & `pycyclops-0.2.8/cyclops/monitor/plotter.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/monitor/reductor.py` & `pycyclops-0.2.8/cyclops/monitor/reductor.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/monitor/synthetic_applicator.py` & `pycyclops-0.2.8/cyclops/monitor/synthetic_applicator.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/monitor/tester.py` & `pycyclops-0.2.8/cyclops/monitor/tester.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/monitor/utils.py` & `pycyclops-0.2.8/cyclops/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/model_card/base.py` & `pycyclops-0.2.8/cyclops/report/model_card/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/model_card/fields.py` & `pycyclops-0.2.8/cyclops/report/model_card/fields.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/model_card/model_card.py` & `pycyclops-0.2.8/cyclops/report/model_card/model_card.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/model_card/sections.py` & `pycyclops-0.2.8/cyclops/report/model_card/sections.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/plot/base.py` & `pycyclops-0.2.8/cyclops/report/plot/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/plot/classification.py` & `pycyclops-0.2.8/cyclops/report/plot/classification.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/plot/utils.py` & `pycyclops-0.2.8/cyclops/report/plot/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/report.py` & `pycyclops-0.2.8/cyclops/report/report.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/templates/model_report/button.js` & `pycyclops-0.2.8/cyclops/report/templates/model_report/button.js`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/templates/model_report/macros.jinja` & `pycyclops-0.2.8/cyclops/report/templates/model_report/macros.jinja`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/templates/model_report/model_report.jinja` & `pycyclops-0.2.8/cyclops/report/templates/model_report/model_report.jinja`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/templates/model_report/plot.js` & `pycyclops-0.2.8/cyclops/report/templates/model_report/plot.js`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/report/utils.py` & `pycyclops-0.2.8/cyclops/report/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/tasks/base.py` & `pycyclops-0.2.8/cyclops/tasks/base.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/tasks/classification.py` & `pycyclops-0.2.8/cyclops/tasks/classification.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Classification tasks."""
 
 import logging
 from functools import partial
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from datasets import Dataset, DatasetDict, config
 from sklearn.compose import ColumnTransformer
 from sklearn.exceptions import NotFittedError
 from sklearn.pipeline import Pipeline
@@ -267,14 +267,15 @@
         prediction_column_prefix: str = "predictions",
         splits_mapping: Optional[Dict[str, str]] = None,
         slice_spec: Optional[SliceSpec] = None,
         batch_size: int = config.DEFAULT_MAX_BATCH_SIZE,
         remove_columns: Optional[Union[str, List[str]]] = None,
         fairness_config: Optional[FairnessConfig] = None,
         override_fairness_metrics: bool = False,
+        array_lib: Literal["numpy", "torch", "cupy"] = "numpy",
     ) -> Tuple[Dict[str, Any], Dataset]:
         """Evaluate model(s) on a HuggingFace dataset.
 
         Parameters
         ----------
         dataset : Union[Dataset, DatasetDict]
             HuggingFace dataset.
@@ -301,14 +302,17 @@
             Unnecessary columns to be removed from the dataset, by default None
         fairness_config : Optional[FairnessConfig], optional
             The configuration for computing fairness metrics. If None, no fairness \
             metrics will be computed, by default None
         override_fairness_metrics : bool, optional
             If True, the `metrics` argument in fairness_config will be overridden by \
             the `metrics`, by default False
+        array_lib : {"numpy", "torch", "cupy"}, default="numpy"
+            The array library to use for the metric computation. The metric results
+            will be returned in the format of `array_lib`.
 
         Returns
         -------
         Dict[str, Any]
             Dictionary with evaluation results.
 
         """
@@ -370,14 +374,15 @@
                 f"{prediction_column_prefix}.{model_name}" for model_name in model_names
             ],
             ignore_columns=remove_columns,
             split=splits_mapping["test"],
             batch_size=batch_size,
             fairness_config=fairness_config,
             override_fairness_metrics=override_fairness_metrics,
+            array_lib=array_lib,
         )
         return results, dataset
 
 
 class MultilabelImageClassificationTask(BaseTask):
     """Binary tabular classification task."""
 
@@ -470,14 +475,15 @@
         prediction_column_prefix: str = "predictions",
         splits_mapping: Optional[Dict[str, str]] = None,
         slice_spec: Optional[SliceSpec] = None,
         batch_size: int = 64,
         remove_columns: Optional[Union[str, List[str]]] = None,
         fairness_config: Optional[FairnessConfig] = None,
         override_fairness_metrics: bool = False,
+        array_lib: Literal["numpy", "torch", "cupy"] = "numpy",
     ) -> Tuple[Dict[str, Any], Dataset]:
         """Evaluate model(s) on a HuggingFace dataset.
 
         Parameters
         ----------
         dataset : Union[Dataset, DatasetDict]
             HuggingFace dataset.
@@ -502,14 +508,17 @@
             Unnecessary columns to be removed from the dataset, by default None
         fairness_config : Optional[FairnessConfig], optional
             The configuration for computing fairness metrics. If None, no fairness \
             metrics will be computed, by default None
         override_fairness_metrics : bool, optional
             If True, the `metrics` argument in fairness_config will be overridden by \
             the `metrics`, by default False
+        array_lib : {"numpy", "torch", "cupy"}, default="numpy"
+            The array library to use for the metric computation. The metric results
+            will be returned in the format of `array_lib`.
 
         Returns
         -------
         Dict[str, Any]
             Dictionary with evaluation results.
 
         """
@@ -565,10 +574,11 @@
                 f"{prediction_column_prefix}.{model_name}" for model_name in model_names
             ],
             ignore_columns=remove_columns,
             split=splits_mapping["test"],
             batch_size=batch_size,
             fairness_config=fairness_config,
             override_fairness_metrics=override_fairness_metrics,
+            array_lib=array_lib,
         )
 
         return results, dataset
```

### Comparing `pycyclops-0.2.7/cyclops/tasks/utils.py` & `pycyclops-0.2.8/cyclops/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/utils/common.py` & `pycyclops-0.2.8/cyclops/utils/common.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/utils/file.py` & `pycyclops-0.2.8/cyclops/utils/file.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/utils/index.py` & `pycyclops-0.2.8/cyclops/utils/index.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/utils/log.py` & `pycyclops-0.2.8/cyclops/utils/log.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/utils/optional.py` & `pycyclops-0.2.8/cyclops/utils/optional.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/utils/plot.py` & `pycyclops-0.2.8/cyclops/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/cyclops/utils/profile.py` & `pycyclops-0.2.8/cyclops/utils/profile.py`

 * *Files identical despite different names*

### Comparing `pycyclops-0.2.7/pyproject.toml` & `pycyclops-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycyclops"
-version = "0.2.7"
+version = "0.2.8"
 description = "Framework for healthcare ML implementation"
 authors = ["Vector AI Engineering <cyclops@vectorinstitute.ai>"]
 license = "Apache-2.0"
 repository = "https://github.com/VectorInstitute/cyclops"
 documentation = "https://vectorinstitute.github.io/cyclops/"
 packages = [
     { include = "cyclops" },
@@ -142,15 +142,15 @@
 pyperf = "^2.6.3"
 
 [tool.poetry.group.deploy]
 optional = true
 
 [tool.poetry.group.deploy.dependencies]
 aiohttp = "^3.9.2"
-bentoml = { version = "1.2.0", extras = ["triton"] }
+bentoml = { version = "1.2.5", extras = ["triton"] }
 torchxrayvision = "^1.2.1"
 kaggle = "^1.5.13"
 onnx = "^1.15.0"
 skl2onnx = "^1.16.0"
 
 [tool.poetry.extras]
 torch = ["torch"]
```

### Comparing `pycyclops-0.2.7/PKG-INFO` & `pycyclops-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycyclops
-Version: 0.2.7
+Version: 0.2.8
 Summary: Framework for healthcare ML implementation
 Home-page: https://github.com/VectorInstitute/cyclops
 License: Apache-2.0
 Author: Vector AI Engineering
 Author-email: cyclops@vectorinstitute.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

