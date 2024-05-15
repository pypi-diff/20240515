# Comparing `tmp/lightwood-24.3.3.1.tar.gz` & `tmp/lightwood-24.5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightwood-24.3.3.1.tar", max compression
+gzip compressed data, was "lightwood-24.5.2.0.tar", max compression
```

## Comparing `lightwood-24.3.3.1.tar` & `lightwood-24.5.2.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0    35104 2024-03-19 10:24:34.166867 lightwood-24.3.3.1/LICENSE
--rw-r--r--   0        0        0    11131 2024-03-19 10:24:34.166867 lightwood-24.3.3.1/README.md
--rw-r--r--   0        0        0      398 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/__about__.py
--rw-r--r--   0        0        0      376 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/__init__.py
--rw-r--r--   0        0        0      883 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/__init__.py
--rw-r--r--   0        0        0     5255 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/analyze.py
--rw-r--r--   0        0        0     2456 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/base.py
--rw-r--r--   0        0        0     3463 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/explain.py
--rw-r--r--   0        0        0        0 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/helpers/__init__.py
--rw-r--r--   0        0        0     7250 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/helpers/acc_stats.py
--rw-r--r--   0        0        0     4305 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/helpers/conf_stats.py
--rw-r--r--   0        0        0     5163 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/helpers/feature_importance.py
--rw-r--r--   0        0        0     3949 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/helpers/pyod.py
--rw-r--r--   0        0        0     4156 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/helpers/shap.py
--rw-r--r--   0        0        0     1082 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/nc/LICENSE
--rw-r--r--   0        0        0        0 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/nc/__init__.py
--rw-r--r--   0        0        0     5255 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/nc/base.py
--rw-r--r--   0        0        0    29295 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/nc/calibrate.py
--rw-r--r--   0        0        0    16835 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/nc/icp.py
--rw-r--r--   0        0        0     5728 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/nc/metrics.py
--rw-r--r--   0        0        0    22328 2024-03-19 10:24:34.186867 lightwood-24.3.3.1/lightwood/analysis/nc/nc.py
--rw-r--r--   0        0        0     5722 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/analysis/nc/norm.py
--rw-r--r--   0        0        0    10049 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/analysis/nc/util.py
--rw-r--r--   0        0        0        0 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/analysis/nn_conf/__init__.py
--rw-r--r--   0        0        0     4369 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/analysis/nn_conf/temp_scale.py
--rw-r--r--   0        0        0     1068 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/analysis/nn_conf/temp_scale_license
--rw-r--r--   0        0        0      753 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/api/__init__.py
--rw-r--r--   0        0        0     6699 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/api/high_level.py
--rw-r--r--   0        0        0    30144 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/api/json_ai.py
--rw-r--r--   0        0        0     8904 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/api/predictor.py
--rw-r--r--   0        0        0    25315 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/api/types.py
--rw-r--r--   0        0        0      296 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/data/__init__.py
--rw-r--r--   0        0        0    10395 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/data/encoded_ds.py
--rw-r--r--   0        0        0     5142 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/data/timeseries_analyzer.py
--rw-r--r--   0        0        0    14743 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/data/timeseries_transform.py
--rw-r--r--   0        0        0     1770 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/__init__.py
--rw-r--r--   0        0        0       83 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/array/__init__.py
--rw-r--r--   0        0        0     5366 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/array/array.py
--rw-r--r--   0        0        0     4768 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/array/ts_cat_array.py
--rw-r--r--   0        0        0     4534 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/array/ts_num_array.py
--rw-r--r--   0        0        0      226 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/audio/__init__.py
--rw-r--r--   0        0        0     3575 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/audio/mfcc.py
--rw-r--r--   0        0        0     3960 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/base.py
--rw-r--r--   0        0        0      377 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/categorical/__init__.py
--rw-r--r--   0        0        0    10217 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/categorical/autoencoder.py
--rw-r--r--   0        0        0     8535 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/categorical/binary.py
--rw-r--r--   0        0        0     5348 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/categorical/gym.py
--rw-r--r--   0        0        0     1439 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/categorical/multihot.py
--rw-r--r--   0        0        0     7754 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/categorical/onehot.py
--rw-r--r--   0        0        0     2540 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/categorical/simple_label.py
--rw-r--r--   0        0        0      213 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/datetime/__init__.py
--rw-r--r--   0        0        0     3589 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/datetime/datetime.py
--rw-r--r--   0        0        0     4189 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/datetime/datetime_sin_normalizer.py
--rw-r--r--   0        0        0     2531 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/helpers.py
--rw-r--r--   0        0        0        0 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/identity/__init__.py
--rw-r--r--   0        0        0     1944 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/identity/identity.py
--rw-r--r--   0        0        0      144 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/image/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/image/helpers/__init__.py
--rw-r--r--   0        0        0     2170 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/image/helpers/img_to_vec.py
--rw-r--r--   0        0        0     4409 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/image/img_2_vec.py
--rw-r--r--   0        0        0      178 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/numeric/__init__.py
--rw-r--r--   0        0        0     7485 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/numeric/numeric.py
--rw-r--r--   0        0        0     4656 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/numeric/ts_numeric.py
--rw-r--r--   0        0        0      334 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/text/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/text/helpers/__init__.py
--rw-r--r--   0        0        0      652 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/text/helpers/pretrained_helpers.py
--rw-r--r--   0        0        0    15829 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/text/pretrained.py
--rw-r--r--   0        0        0     3987 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/text/short.py
--rw-r--r--   0        0        0      942 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/text/tfidf.py
--rw-r--r--   0        0        0     1432 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/text/vocab.py
--rw-r--r--   0        0        0       96 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/time_series/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/time_series/helpers/__init__.py
--rw-r--r--   0        0        0     1743 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/time_series/helpers/common.py
--rw-r--r--   0        0        0     3890 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/time_series/helpers/rnn_helpers.py
--rw-r--r--   0        0        0     5184 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/time_series/helpers/transformer_helpers.py
--rw-r--r--   0        0        0    23548 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/time_series/rnn.py
--rw-r--r--   0        0        0     2146 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/encoder/time_series/ts.py
--rw-r--r--   0        0        0      699 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/ensemble/__init__.py
--rw-r--r--   0        0        0     1625 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/ensemble/base.py
--rw-r--r--   0        0        0     3691 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/ensemble/best_of.py
--rw-r--r--   0        0        0      995 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/ensemble/embed.py
--rw-r--r--   0        0        0     1631 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/ensemble/identity.py
--rw-r--r--   0        0        0     1285 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/ensemble/mean_ensemble.py
--rw-r--r--   0        0        0     4042 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/ensemble/mode_ensemble.py
--rw-r--r--   0        0        0     3246 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/ensemble/stacked_ensemble.py
--rw-r--r--   0        0        0     2946 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/ensemble/ts_stacked_ensemble.py
--rw-r--r--   0        0        0     3212 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/ensemble/weighted_mean_ensemble.py
--rw-r--r--   0        0        0      945 2024-03-19 10:24:34.190867 lightwood-24.3.3.1/lightwood/helpers/__init__.py
--rw-r--r--   0        0        0    23048 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/codegen.py
--rw-r--r--   0        0        0     2047 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/constants.py
--rw-r--r--   0        0        0     3655 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/device.py
--rw-r--r--   0        0        0     1538 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/general.py
--rw-r--r--   0        0        0      580 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/io.py
--rw-r--r--   0        0        0     1403 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/log.py
--rw-r--r--   0        0        0      201 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/numeric.py
--rw-r--r--   0        0        0     2182 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/parallelism.py
--rw-r--r--   0        0        0      370 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/seed.py
--rw-r--r--   0        0        0     4321 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/templating.py
--rw-r--r--   0        0        0     1086 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/text.py
--rw-r--r--   0        0        0     4312 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/torch.py
--rw-r--r--   0        0        0     9733 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/helpers/ts.py
--rw-r--r--   0        0        0     1495 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/__init__.py
--rw-r--r--   0        0        0     5159 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/arima.py
--rw-r--r--   0        0        0     3952 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/base.py
--rw-r--r--   0        0        0     3147 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/ets.py
--rw-r--r--   0        0        0    11817 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/gluonts.py
--rw-r--r--   0        0        0        0 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/helpers/__init__.py
--rw-r--r--   0        0        0     2320 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/helpers/ar_net.py
--rw-r--r--   0        0        0     2902 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/helpers/default_net.py
--rw-r--r--   0        0        0     4278 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/helpers/qclassic_net.py
--rw-r--r--   0        0        0     5526 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/helpers/ranger.py
--rw-r--r--   0        0        0     2699 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/helpers/residual_net.py
--rw-r--r--   0        0        0      589 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/helpers/transform_corss_entropy_loss.py
--rw-r--r--   0        0        0     1955 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/helpers/ts.py
--rw-r--r--   0        0        0    16048 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/lightgbm.py
--rw-r--r--   0        0        0     3924 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/lightgbm_array.py
--rw-r--r--   0        0        0    15938 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/neural.py
--rw-r--r--   0        0        0     6935 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/neural_ts.py
--rw-r--r--   0        0        0    11999 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/nhits.py
--rw-r--r--   0        0        0     3450 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/prophet.py
--rw-r--r--   0        0        0      930 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/qclassic.py
--rw-r--r--   0        0        0     9092 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/random_forest.py
--rw-r--r--   0        0        0     4377 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/regression.py
--rw-r--r--   0        0        0    17465 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/sktime.py
--rw-r--r--   0        0        0     2859 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/tabtransformer.py
--rw-r--r--   0        0        0     2305 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/unit.py
--rw-r--r--   0        0        0    13389 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/xgboost.py
--rw-r--r--   0        0        0     3933 2024-03-19 10:24:34.194867 lightwood-24.3.3.1/lightwood/mixer/xgboost_array.py
--rw-r--r--   0        0        0     2021 2024-03-19 10:24:34.198867 lightwood-24.3.3.1/pyproject.toml
--rw-r--r--   0        0        0    13469 1970-01-01 00:00:00.000000 lightwood-24.3.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35104 2024-05-15 13:37:01.696938 lightwood-24.5.2.0/LICENSE
+-rw-r--r--   0        0        0    11131 2024-05-15 13:37:01.696938 lightwood-24.5.2.0/README.md
+-rw-r--r--   0        0        0      398 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/__about__.py
+-rw-r--r--   0        0        0      376 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/__init__.py
+-rw-r--r--   0        0        0      883 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/__init__.py
+-rw-r--r--   0        0        0     5255 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/analyze.py
+-rw-r--r--   0        0        0     2456 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/base.py
+-rw-r--r--   0        0        0     3463 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/explain.py
+-rw-r--r--   0        0        0        0 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/helpers/__init__.py
+-rw-r--r--   0        0        0     7250 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/helpers/acc_stats.py
+-rw-r--r--   0        0        0     4305 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/helpers/conf_stats.py
+-rw-r--r--   0        0        0     5163 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/helpers/feature_importance.py
+-rw-r--r--   0        0        0     3949 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/helpers/pyod.py
+-rw-r--r--   0        0        0     4156 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/helpers/shap.py
+-rw-r--r--   0        0        0     1082 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/nc/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/nc/__init__.py
+-rw-r--r--   0        0        0     5255 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/nc/base.py
+-rw-r--r--   0        0        0    29295 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/nc/calibrate.py
+-rw-r--r--   0        0        0    16835 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/nc/icp.py
+-rw-r--r--   0        0        0     5728 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/nc/metrics.py
+-rw-r--r--   0        0        0    22328 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/nc/nc.py
+-rw-r--r--   0        0        0     5722 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/nc/norm.py
+-rw-r--r--   0        0        0    10049 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/nc/util.py
+-rw-r--r--   0        0        0        0 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/nn_conf/__init__.py
+-rw-r--r--   0        0        0     4369 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/nn_conf/temp_scale.py
+-rw-r--r--   0        0        0     1068 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/analysis/nn_conf/temp_scale_license
+-rw-r--r--   0        0        0      753 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/api/__init__.py
+-rw-r--r--   0        0        0     6699 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/api/high_level.py
+-rw-r--r--   0        0        0    30144 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/api/json_ai.py
+-rw-r--r--   0        0        0     8904 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/api/predictor.py
+-rw-r--r--   0        0        0    25315 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/api/types.py
+-rw-r--r--   0        0        0      296 2024-05-15 13:37:01.716938 lightwood-24.5.2.0/lightwood/data/__init__.py
+-rw-r--r--   0        0        0    10395 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/data/encoded_ds.py
+-rw-r--r--   0        0        0     5142 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/data/timeseries_analyzer.py
+-rw-r--r--   0        0        0    14743 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/data/timeseries_transform.py
+-rw-r--r--   0        0        0     1770 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/__init__.py
+-rw-r--r--   0        0        0       83 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/array/__init__.py
+-rw-r--r--   0        0        0     5366 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/array/array.py
+-rw-r--r--   0        0        0     4768 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/array/ts_cat_array.py
+-rw-r--r--   0        0        0     4534 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/array/ts_num_array.py
+-rw-r--r--   0        0        0      226 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/audio/__init__.py
+-rw-r--r--   0        0        0     3575 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/audio/mfcc.py
+-rw-r--r--   0        0        0     3960 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/base.py
+-rw-r--r--   0        0        0      377 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/categorical/__init__.py
+-rw-r--r--   0        0        0    10217 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/categorical/autoencoder.py
+-rw-r--r--   0        0        0     8535 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/categorical/binary.py
+-rw-r--r--   0        0        0     5348 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/categorical/gym.py
+-rw-r--r--   0        0        0     1439 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/categorical/multihot.py
+-rw-r--r--   0        0        0     7754 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/categorical/onehot.py
+-rw-r--r--   0        0        0     2540 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/categorical/simple_label.py
+-rw-r--r--   0        0        0      213 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/datetime/__init__.py
+-rw-r--r--   0        0        0     3589 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/datetime/datetime.py
+-rw-r--r--   0        0        0     4189 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
+-rw-r--r--   0        0        0     2531 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/identity/__init__.py
+-rw-r--r--   0        0        0     1944 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/identity/identity.py
+-rw-r--r--   0        0        0      144 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/image/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/image/helpers/__init__.py
+-rw-r--r--   0        0        0     2170 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/image/helpers/img_to_vec.py
+-rw-r--r--   0        0        0     4409 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/image/img_2_vec.py
+-rw-r--r--   0        0        0      178 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/numeric/__init__.py
+-rw-r--r--   0        0        0     7485 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/numeric/numeric.py
+-rw-r--r--   0        0        0     4656 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/numeric/ts_numeric.py
+-rw-r--r--   0        0        0      334 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/text/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/text/helpers/__init__.py
+-rw-r--r--   0        0        0      652 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/text/helpers/pretrained_helpers.py
+-rw-r--r--   0        0        0    15829 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/text/pretrained.py
+-rw-r--r--   0        0        0     3987 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/text/short.py
+-rw-r--r--   0        0        0      942 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/text/tfidf.py
+-rw-r--r--   0        0        0     1432 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/text/vocab.py
+-rw-r--r--   0        0        0       96 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/time_series/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/time_series/helpers/__init__.py
+-rw-r--r--   0        0        0     1743 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/time_series/helpers/common.py
+-rw-r--r--   0        0        0     3890 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
+-rw-r--r--   0        0        0     5184 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
+-rw-r--r--   0        0        0    23548 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/time_series/rnn.py
+-rw-r--r--   0        0        0     2146 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/encoder/time_series/ts.py
+-rw-r--r--   0        0        0      699 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/ensemble/__init__.py
+-rw-r--r--   0        0        0     1625 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/ensemble/base.py
+-rw-r--r--   0        0        0     3691 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/ensemble/best_of.py
+-rw-r--r--   0        0        0      995 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/ensemble/embed.py
+-rw-r--r--   0        0        0     1631 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/ensemble/identity.py
+-rw-r--r--   0        0        0     1285 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/ensemble/mean_ensemble.py
+-rw-r--r--   0        0        0     4042 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/ensemble/mode_ensemble.py
+-rw-r--r--   0        0        0     3246 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/ensemble/stacked_ensemble.py
+-rw-r--r--   0        0        0     2946 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/ensemble/ts_stacked_ensemble.py
+-rw-r--r--   0        0        0     3212 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/ensemble/weighted_mean_ensemble.py
+-rw-r--r--   0        0        0      945 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/__init__.py
+-rw-r--r--   0        0        0    23048 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/codegen.py
+-rw-r--r--   0        0        0     2047 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/constants.py
+-rw-r--r--   0        0        0     3655 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/device.py
+-rw-r--r--   0        0        0     1538 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/general.py
+-rw-r--r--   0        0        0      580 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/io.py
+-rw-r--r--   0        0        0     1403 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/log.py
+-rw-r--r--   0        0        0      201 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/numeric.py
+-rw-r--r--   0        0        0     2182 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/parallelism.py
+-rw-r--r--   0        0        0      370 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/seed.py
+-rw-r--r--   0        0        0     4321 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/templating.py
+-rw-r--r--   0        0        0     1086 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/text.py
+-rw-r--r--   0        0        0     4312 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/torch.py
+-rw-r--r--   0        0        0     9733 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/helpers/ts.py
+-rw-r--r--   0        0        0     1495 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/mixer/__init__.py
+-rw-r--r--   0        0        0     5159 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/mixer/arima.py
+-rw-r--r--   0        0        0     3952 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/mixer/base.py
+-rw-r--r--   0        0        0     3147 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/mixer/ets.py
+-rw-r--r--   0        0        0    11817 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/mixer/gluonts.py
+-rw-r--r--   0        0        0        0 2024-05-15 13:37:01.720938 lightwood-24.5.2.0/lightwood/mixer/helpers/__init__.py
+-rw-r--r--   0        0        0     2320 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/helpers/ar_net.py
+-rw-r--r--   0        0        0     2902 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/helpers/default_net.py
+-rw-r--r--   0        0        0     4278 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/helpers/qclassic_net.py
+-rw-r--r--   0        0        0     5526 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/helpers/ranger.py
+-rw-r--r--   0        0        0     2699 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/helpers/residual_net.py
+-rw-r--r--   0        0        0      589 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
+-rw-r--r--   0        0        0     1955 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/helpers/ts.py
+-rw-r--r--   0        0        0    16048 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/lightgbm.py
+-rw-r--r--   0        0        0     3924 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/lightgbm_array.py
+-rw-r--r--   0        0        0    15938 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/neural.py
+-rw-r--r--   0        0        0     6935 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/neural_ts.py
+-rw-r--r--   0        0        0    11999 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/nhits.py
+-rw-r--r--   0        0        0     3450 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/prophet.py
+-rw-r--r--   0        0        0      930 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/qclassic.py
+-rw-r--r--   0        0        0     9092 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/random_forest.py
+-rw-r--r--   0        0        0     4377 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/regression.py
+-rw-r--r--   0        0        0    17465 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/sktime.py
+-rw-r--r--   0        0        0     2859 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/tabtransformer.py
+-rw-r--r--   0        0        0     2305 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/unit.py
+-rw-r--r--   0        0        0    13389 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/xgboost.py
+-rw-r--r--   0        0        0     3933 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/lightwood/mixer/xgboost_array.py
+-rw-r--r--   0        0        0     2035 2024-05-15 13:37:01.724938 lightwood-24.5.2.0/pyproject.toml
+-rw-r--r--   0        0        0    13483 1970-01-01 00:00:00.000000 lightwood-24.5.2.0/PKG-INFO
```

### Comparing `lightwood-24.3.3.1/LICENSE` & `lightwood-24.5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/README.md` & `lightwood-24.5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/__init__.py` & `lightwood-24.5.2.0/lightwood/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/analyze.py` & `lightwood-24.5.2.0/lightwood/analysis/analyze.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/base.py` & `lightwood-24.5.2.0/lightwood/analysis/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/explain.py` & `lightwood-24.5.2.0/lightwood/analysis/explain.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/helpers/acc_stats.py` & `lightwood-24.5.2.0/lightwood/analysis/helpers/acc_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/helpers/conf_stats.py` & `lightwood-24.5.2.0/lightwood/analysis/helpers/conf_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/helpers/feature_importance.py` & `lightwood-24.5.2.0/lightwood/analysis/helpers/feature_importance.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/helpers/pyod.py` & `lightwood-24.5.2.0/lightwood/analysis/helpers/pyod.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/helpers/shap.py` & `lightwood-24.5.2.0/lightwood/analysis/helpers/shap.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/nc/LICENSE` & `lightwood-24.5.2.0/lightwood/analysis/nc/LICENSE`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/nc/base.py` & `lightwood-24.5.2.0/lightwood/analysis/nc/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/nc/calibrate.py` & `lightwood-24.5.2.0/lightwood/analysis/nc/calibrate.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/nc/icp.py` & `lightwood-24.5.2.0/lightwood/analysis/nc/icp.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/nc/metrics.py` & `lightwood-24.5.2.0/lightwood/analysis/nc/metrics.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/nc/nc.py` & `lightwood-24.5.2.0/lightwood/analysis/nc/nc.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/nc/norm.py` & `lightwood-24.5.2.0/lightwood/analysis/nc/norm.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/nc/util.py` & `lightwood-24.5.2.0/lightwood/analysis/nc/util.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/nn_conf/temp_scale.py` & `lightwood-24.5.2.0/lightwood/analysis/nn_conf/temp_scale.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/analysis/nn_conf/temp_scale_license` & `lightwood-24.5.2.0/lightwood/analysis/nn_conf/temp_scale_license`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/api/__init__.py` & `lightwood-24.5.2.0/lightwood/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/api/high_level.py` & `lightwood-24.5.2.0/lightwood/api/high_level.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/api/json_ai.py` & `lightwood-24.5.2.0/lightwood/api/json_ai.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/api/predictor.py` & `lightwood-24.5.2.0/lightwood/api/predictor.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/api/types.py` & `lightwood-24.5.2.0/lightwood/api/types.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/data/encoded_ds.py` & `lightwood-24.5.2.0/lightwood/data/encoded_ds.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/data/timeseries_analyzer.py` & `lightwood-24.5.2.0/lightwood/data/timeseries_analyzer.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/data/timeseries_transform.py` & `lightwood-24.5.2.0/lightwood/data/timeseries_transform.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/__init__.py` & `lightwood-24.5.2.0/lightwood/encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/array/array.py` & `lightwood-24.5.2.0/lightwood/encoder/array/array.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/array/ts_cat_array.py` & `lightwood-24.5.2.0/lightwood/encoder/array/ts_cat_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/array/ts_num_array.py` & `lightwood-24.5.2.0/lightwood/encoder/array/ts_num_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/audio/mfcc.py` & `lightwood-24.5.2.0/lightwood/encoder/audio/mfcc.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/base.py` & `lightwood-24.5.2.0/lightwood/encoder/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/categorical/autoencoder.py` & `lightwood-24.5.2.0/lightwood/encoder/categorical/autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/categorical/binary.py` & `lightwood-24.5.2.0/lightwood/encoder/categorical/binary.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/categorical/gym.py` & `lightwood-24.5.2.0/lightwood/encoder/categorical/gym.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/categorical/multihot.py` & `lightwood-24.5.2.0/lightwood/encoder/categorical/multihot.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/categorical/onehot.py` & `lightwood-24.5.2.0/lightwood/encoder/categorical/onehot.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/categorical/simple_label.py` & `lightwood-24.5.2.0/lightwood/encoder/categorical/simple_label.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/datetime/datetime.py` & `lightwood-24.5.2.0/lightwood/encoder/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/datetime/datetime_sin_normalizer.py` & `lightwood-24.5.2.0/lightwood/encoder/datetime/datetime_sin_normalizer.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/helpers.py` & `lightwood-24.5.2.0/lightwood/encoder/helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/identity/identity.py` & `lightwood-24.5.2.0/lightwood/encoder/identity/identity.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/image/helpers/img_to_vec.py` & `lightwood-24.5.2.0/lightwood/encoder/image/helpers/img_to_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/image/img_2_vec.py` & `lightwood-24.5.2.0/lightwood/encoder/image/img_2_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/numeric/numeric.py` & `lightwood-24.5.2.0/lightwood/encoder/numeric/numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/numeric/ts_numeric.py` & `lightwood-24.5.2.0/lightwood/encoder/numeric/ts_numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/text/helpers/pretrained_helpers.py` & `lightwood-24.5.2.0/lightwood/encoder/text/helpers/pretrained_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/text/pretrained.py` & `lightwood-24.5.2.0/lightwood/encoder/text/pretrained.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/text/short.py` & `lightwood-24.5.2.0/lightwood/encoder/text/short.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/text/tfidf.py` & `lightwood-24.5.2.0/lightwood/encoder/text/tfidf.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/text/vocab.py` & `lightwood-24.5.2.0/lightwood/encoder/text/vocab.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/time_series/helpers/common.py` & `lightwood-24.5.2.0/lightwood/encoder/time_series/helpers/common.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/time_series/helpers/rnn_helpers.py` & `lightwood-24.5.2.0/lightwood/encoder/time_series/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/time_series/helpers/transformer_helpers.py` & `lightwood-24.5.2.0/lightwood/encoder/time_series/helpers/transformer_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/time_series/rnn.py` & `lightwood-24.5.2.0/lightwood/encoder/time_series/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/encoder/time_series/ts.py` & `lightwood-24.5.2.0/lightwood/encoder/time_series/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/ensemble/__init__.py` & `lightwood-24.5.2.0/lightwood/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/ensemble/base.py` & `lightwood-24.5.2.0/lightwood/ensemble/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/ensemble/best_of.py` & `lightwood-24.5.2.0/lightwood/ensemble/best_of.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/ensemble/embed.py` & `lightwood-24.5.2.0/lightwood/ensemble/embed.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/ensemble/identity.py` & `lightwood-24.5.2.0/lightwood/ensemble/identity.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/ensemble/mean_ensemble.py` & `lightwood-24.5.2.0/lightwood/ensemble/mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/ensemble/mode_ensemble.py` & `lightwood-24.5.2.0/lightwood/ensemble/mode_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/ensemble/stacked_ensemble.py` & `lightwood-24.5.2.0/lightwood/ensemble/stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/ensemble/ts_stacked_ensemble.py` & `lightwood-24.5.2.0/lightwood/ensemble/ts_stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/ensemble/weighted_mean_ensemble.py` & `lightwood-24.5.2.0/lightwood/ensemble/weighted_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/helpers/__init__.py` & `lightwood-24.5.2.0/lightwood/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/helpers/codegen.py` & `lightwood-24.5.2.0/lightwood/helpers/codegen.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/helpers/constants.py` & `lightwood-24.5.2.0/lightwood/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/helpers/device.py` & `lightwood-24.5.2.0/lightwood/helpers/device.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/helpers/general.py` & `lightwood-24.5.2.0/lightwood/helpers/general.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/helpers/io.py` & `lightwood-24.5.2.0/lightwood/helpers/io.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/helpers/log.py` & `lightwood-24.5.2.0/lightwood/helpers/log.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/helpers/parallelism.py` & `lightwood-24.5.2.0/lightwood/helpers/parallelism.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/helpers/templating.py` & `lightwood-24.5.2.0/lightwood/helpers/templating.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/helpers/text.py` & `lightwood-24.5.2.0/lightwood/helpers/text.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/helpers/torch.py` & `lightwood-24.5.2.0/lightwood/helpers/torch.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/helpers/ts.py` & `lightwood-24.5.2.0/lightwood/helpers/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/__init__.py` & `lightwood-24.5.2.0/lightwood/mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/arima.py` & `lightwood-24.5.2.0/lightwood/mixer/arima.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/base.py` & `lightwood-24.5.2.0/lightwood/mixer/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/ets.py` & `lightwood-24.5.2.0/lightwood/mixer/ets.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/gluonts.py` & `lightwood-24.5.2.0/lightwood/mixer/gluonts.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/helpers/ar_net.py` & `lightwood-24.5.2.0/lightwood/mixer/helpers/ar_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/helpers/default_net.py` & `lightwood-24.5.2.0/lightwood/mixer/helpers/default_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/helpers/qclassic_net.py` & `lightwood-24.5.2.0/lightwood/mixer/helpers/qclassic_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/helpers/ranger.py` & `lightwood-24.5.2.0/lightwood/mixer/helpers/ranger.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/helpers/residual_net.py` & `lightwood-24.5.2.0/lightwood/mixer/helpers/residual_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/helpers/transform_corss_entropy_loss.py` & `lightwood-24.5.2.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/helpers/ts.py` & `lightwood-24.5.2.0/lightwood/mixer/helpers/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/lightgbm.py` & `lightwood-24.5.2.0/lightwood/mixer/lightgbm.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/lightgbm_array.py` & `lightwood-24.5.2.0/lightwood/mixer/lightgbm_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/neural.py` & `lightwood-24.5.2.0/lightwood/mixer/neural.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/neural_ts.py` & `lightwood-24.5.2.0/lightwood/mixer/neural_ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/nhits.py` & `lightwood-24.5.2.0/lightwood/mixer/nhits.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/prophet.py` & `lightwood-24.5.2.0/lightwood/mixer/prophet.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/qclassic.py` & `lightwood-24.5.2.0/lightwood/mixer/qclassic.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/random_forest.py` & `lightwood-24.5.2.0/lightwood/mixer/random_forest.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/regression.py` & `lightwood-24.5.2.0/lightwood/mixer/regression.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/sktime.py` & `lightwood-24.5.2.0/lightwood/mixer/sktime.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/tabtransformer.py` & `lightwood-24.5.2.0/lightwood/mixer/tabtransformer.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/unit.py` & `lightwood-24.5.2.0/lightwood/mixer/unit.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/xgboost.py` & `lightwood-24.5.2.0/lightwood/mixer/xgboost.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/lightwood/mixer/xgboost_array.py` & `lightwood-24.5.2.0/lightwood/mixer/xgboost_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-24.3.3.1/pyproject.toml` & `lightwood-24.5.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "lightwood"
-version = "24.3.3.1"
+version = "24.5.2.0"
 description = "Lightwood is Legos for Machine Learning."
 authors = ["MindsDB Inc."]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 type_infer = ">=0.0.15"
-dataprep_ml = ">=0.0.18"
-mindsdb-evaluator = ">=0.0.12"
+dataprep_ml = ">=24.5.1.2,<24.6.1.0"
+mindsdb-evaluator = ">=0.0.13"
 numpy = ">1.23.0"
 nltk = ">=3.8, <3.9"
 pandas = ">=2.0.0, <2.1.0"
 torch = ">=2.0.0"
 requests = ">=2.0.0"
 transformers = ">=4.34.0"
 optuna = ">=3.1.0,<4.0.0"
@@ -26,32 +26,32 @@
 psutil = ">=5.7.0"
 scikit-learn = ">=1.0.0"
 dataclasses_json = ">=0.5.4"
 dill = "==0.3.6"
 sktime = ">=0.24.0,<0.25.0"
 statsforecast = "~=1.6.0"
 torch_optimizer = "==0.1.0"
-black = "==23.3.0"
+black = "==24.3.0"
 typing_extensions = ">= 4.8.0"
 colorlog = "==6.5.0"
 xgboost = ">=1.6.0, <=1.8.0"
 tab-transformer-pytorch = ">= 0.2.1"
 
 # dependencies for optional packages
 autopep8 = {version = ">=1.5.7", optional = true}
 flake8 = {version = ">=6.0.0", optional = true}
 librosa = {version = "==0.8.1", optional = true}
-lightgbm = {version = ">=3.3.0,<=3.3.3", optional = true}
+lightgbm = {version = ">=4.3.0,<=4.4.0", optional = true}
 pystan = {version = "==2.19.1.1", optional = true}
 prophet = {version = "==1.1", optional = true}
 neuralforecast = {version = ">=1.6.4,<1.7.0", optional = true}
 mxnet = {version = ">=1.6.0,<2.0.0", optional = true}
 gluonts = {version = ">=0.13.2,<0.14.0", optional = true}
 torchvision = {version = ">=0.15.0", optional = true}
-pillow = {version = ">8.3.1", optional = true}
+pillow = {version = ">=10.3.0", optional = true}
 qiskit = {version = "==0.31.0", optional = true}
 shap = {version = ">=0.40.0", optional = true}
 pyod = {version = "==1.0.4", optional = true}
 suod = {version = ">=0.1.3", optional = true}
 
 [tool.poetry.extras]
 dev = [
```

### Comparing `lightwood-24.3.3.1/PKG-INFO` & `lightwood-24.5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 24.3.3.1
+Version: 24.5.2.0
 Summary: Lightwood is Legos for Machine Learning.
 License: GPL-3.0-only
 Author: MindsDB Inc.
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -14,31 +14,31 @@
 Provides-Extra: dev
 Provides-Extra: extra
 Provides-Extra: extra-ts
 Provides-Extra: image
 Provides-Extra: quantum
 Provides-Extra: xai
 Requires-Dist: autopep8 (>=1.5.7) ; extra == "dev"
-Requires-Dist: black (==23.3.0)
+Requires-Dist: black (==24.3.0)
 Requires-Dist: colorlog (==6.5.0)
 Requires-Dist: dataclasses_json (>=0.5.4)
-Requires-Dist: dataprep_ml (>=0.0.18)
+Requires-Dist: dataprep_ml (>=24.5.1.2,<24.6.1.0)
 Requires-Dist: dill (==0.3.6)
 Requires-Dist: flake8 (>=6.0.0) ; extra == "dev"
 Requires-Dist: gluonts (>=0.13.2,<0.14.0) ; extra == "extra-ts"
 Requires-Dist: librosa (==0.8.1) ; extra == "audio"
-Requires-Dist: lightgbm (>=3.3.0,<=3.3.3) ; extra == "extra"
-Requires-Dist: mindsdb-evaluator (>=0.0.12)
+Requires-Dist: lightgbm (>=4.3.0,<=4.4.0) ; extra == "extra"
+Requires-Dist: mindsdb-evaluator (>=0.0.13)
 Requires-Dist: mxnet (>=1.6.0,<2.0.0) ; extra == "extra-ts"
 Requires-Dist: neuralforecast (>=1.6.4,<1.7.0) ; extra == "extra-ts"
 Requires-Dist: nltk (>=3.8,<3.9)
 Requires-Dist: numpy (>1.23.0)
 Requires-Dist: optuna (>=3.1.0,<4.0.0)
 Requires-Dist: pandas (>=2.0.0,<2.1.0)
-Requires-Dist: pillow (>8.3.1) ; extra == "image"
+Requires-Dist: pillow (>=10.3.0) ; extra == "image"
 Requires-Dist: prophet (==1.1) ; extra == "extra-ts"
 Requires-Dist: psutil (>=5.7.0)
 Requires-Dist: pyod (==1.0.4) ; extra == "xai"
 Requires-Dist: pystan (==2.19.1.1) ; extra == "extra-ts"
 Requires-Dist: qiskit (==0.31.0) ; extra == "quantum"
 Requires-Dist: requests (>=2.0.0)
 Requires-Dist: scikit-learn (>=1.0.0)
```

