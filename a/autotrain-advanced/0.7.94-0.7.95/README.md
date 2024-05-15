# Comparing `tmp/autotrain-advanced-0.7.94.tar.gz` & `tmp/autotrain-advanced-0.7.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.7.94.tar", last modified: Tue May 14 11:04:21 2024, max compression
+gzip compressed data, was "autotrain-advanced-0.7.95.tar", last modified: Wed May 15 14:36:37 2024, max compression
```

## Comparing `autotrain-advanced-0.7.94.tar` & `autotrain-advanced-0.7.95.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.871187 autotrain-advanced-0.7.94/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.94/LICENSE
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13452 2024-05-14 11:04:21.871187 autotrain-advanced-0.7.94/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2741 2024-05-04 09:15:32.000000 autotrain-advanced-0.7.94/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-14 11:04:21.871187 autotrain-advanced-0.7.94/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.94/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.847187 autotrain-advanced-0.7.94/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.851187 autotrain-advanced-0.7.94/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1450 2024-05-14 11:04:12.000000 autotrain-advanced-0.7.94/src/autotrain/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.851187 autotrain-advanced-0.7.94/src/autotrain/app/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.94/src/autotrain/app/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19905 2024-05-10 12:55:54.000000 autotrain-advanced-0.7.94/src/autotrain/app/api_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      885 2024-05-13 16:31:05.000000 autotrain-advanced-0.7.94/src/autotrain/app/app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.94/src/autotrain/app/db.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8352 2024-05-13 16:41:30.000000 autotrain-advanced-0.7.94/src/autotrain/app/models.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.94/src/autotrain/app/oauth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19092 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/app/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.851187 autotrain-advanced-0.7.94/src/autotrain/app/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.94/src/autotrain/app/static/logo.png
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.851187 autotrain-advanced-0.7.94/src/autotrain/app/templates/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.94/src/autotrain/app/templates/duplicate.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.94/src/autotrain/app/templates/error.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49758 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.94/src/autotrain/app/templates/index.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.94/src/autotrain/app/templates/login.html
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1594 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.94/src/autotrain/app/training_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17416 2024-05-13 16:38:01.000000 autotrain-advanced-0.7.94/src/autotrain/app/ui_routes.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3220 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.94/src/autotrain/app/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.851187 autotrain-advanced-0.7.94/src/autotrain/backends/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.94/src/autotrain/backends/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5071 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.94/src/autotrain/backends/base.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.94/src/autotrain/backends/endpoints.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.94/src/autotrain/backends/local.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.94/src/autotrain/backends/ngc.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.94/src/autotrain/backends/nvcf.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.94/src/autotrain/backends/spaces.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.851187 autotrain-advanced-0.7.94/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.94/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3012 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.94/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_api.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3668 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8313 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4098 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_object_detection.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10504 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_seq2seq.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_spacerunner.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8591 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8535 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_text_regression.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8512 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_token_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.94/src/autotrain/cli/run_tools.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16773 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.94/src/autotrain/cli/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11361 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.94/src/autotrain/commands.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.94/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19020 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.94/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.94/src/autotrain/help.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.94/src/autotrain/logging.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6407 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/parser.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.855187 autotrain-advanced-0.7.94/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.94/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.94/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.94/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.94/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12106 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.94/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2667 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.94/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      884 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.94/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.855187 autotrain-advanced-0.7.94/src/autotrain/tools/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.94/src/autotrain/tools/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.94/src/autotrain/tools/convert_to_kohya.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.94/src/autotrain/tools/merge_adapter.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.855187 autotrain-advanced-0.7.94/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/__init__.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.855187 autotrain-advanced-0.7.94/src/autotrain/trainers/clm/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/clm/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/clm/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/clm/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/clm/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/clm/train_clm_default.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/clm/train_clm_dpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/clm/train_clm_orpo.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/clm/train_clm_reward.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/clm/train_clm_sft.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    20504 2024-05-09 12:46:57.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/clm/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8195 2024-05-06 12:50:40.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/common.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.855187 autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/train.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/train_xl.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.855187 autotrain-advanced-0.7.94/src/autotrain/trainers/generic/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/generic/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/generic/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/generic/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/generic/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.855187 autotrain-advanced-0.7.94/src/autotrain/trainers/image_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/image_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7497 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/image_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/image_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1985 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/image_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/image_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.855187 autotrain-advanced-0.7.94/src/autotrain/trainers/object_detection/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/object_detection/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7185 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/object_detection/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1354 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/object_detection/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2143 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/object_detection/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7592 2024-05-14 11:01:54.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/object_detection/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.855187 autotrain-advanced-0.7.94/src/autotrain/trainers/seq2seq/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/seq2seq/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8908 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/seq2seq/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/seq2seq/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2585 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/seq2seq/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/seq2seq/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.855187 autotrain-advanced-0.7.94/src/autotrain/trainers/tabular/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/tabular/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12471 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/tabular/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/tabular/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/tabular/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.855187 autotrain-advanced-0.7.94/src/autotrain/trainers/text_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/text_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7738 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/text_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/text_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2037 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/text_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/text_classification/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.859187 autotrain-advanced-0.7.94/src/autotrain/trainers/text_regression/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/text_regression/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7019 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/text_regression/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/text_regression/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2036 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/text_regression/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2117 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/text_regression/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.859187 autotrain-advanced-0.7.94/src/autotrain/trainers/token_classification/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/token_classification/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7519 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/token_classification/__main__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/token_classification/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2038 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/token_classification/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1675 2024-04-25 05:15:09.000000 autotrain-advanced-0.7.94/src/autotrain/trainers/token_classification/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2082 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.94/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.859187 autotrain-advanced-0.7.94/src/autotrain_advanced.egg-info/
--rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13452 2024-05-14 11:04:21.000000 autotrain-advanced-0.7.94/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4885 2024-05-14 11:04:21.000000 autotrain-advanced-0.7.94/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-14 11:04:21.000000 autotrain-advanced-0.7.94/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-14 11:04:21.000000 autotrain-advanced-0.7.94/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3687 2024-05-14 11:04:21.000000 autotrain-advanced-0.7.94/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-14 11:04:21.000000 autotrain-advanced-0.7.94/src/autotrain_advanced.egg-info/top_level.txt
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-14 11:04:21.859187 autotrain-advanced-0.7.94/static/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.94/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.829802 autotrain-advanced-0.7.95/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.7.95/LICENSE
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-15 14:36:37.829802 autotrain-advanced-0.7.95/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3113 2024-05-15 14:23:32.000000 autotrain-advanced-0.7.95/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      445 2024-05-15 14:36:37.829802 autotrain-advanced-0.7.95/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2907 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.95/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.805803 autotrain-advanced-0.7.95/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.805803 autotrain-advanced-0.7.95/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1652 2024-05-15 14:36:15.000000 autotrain-advanced-0.7.95/src/autotrain/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.805803 autotrain-advanced-0.7.95/src/autotrain/app/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/app/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19905 2024-05-10 12:55:54.000000 autotrain-advanced-0.7.95/src/autotrain/app/api_routes.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      885 2024-05-13 16:31:05.000000 autotrain-advanced-0.7.95/src/autotrain/app/app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16255 2024-05-15 14:31:42.000000 autotrain-advanced-0.7.95/src/autotrain/app/colab.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      894 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/app/db.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8352 2024-05-13 16:41:30.000000 autotrain-advanced-0.7.95/src/autotrain/app/models.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5419 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/app/oauth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19137 2024-05-15 08:43:33.000000 autotrain-advanced-0.7.95/src/autotrain/app/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.805803 autotrain-advanced-0.7.95/src/autotrain/app/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/app/static/logo.png
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.805803 autotrain-advanced-0.7.95/src/autotrain/app/templates/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      860 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.95/src/autotrain/app/templates/duplicate.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      640 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.95/src/autotrain/app/templates/error.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    49758 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.95/src/autotrain/app/templates/index.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1892 2024-05-13 16:29:32.000000 autotrain-advanced-0.7.95/src/autotrain/app/templates/login.html
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1594 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/app/training_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17416 2024-05-13 16:38:01.000000 autotrain-advanced-0.7.95/src/autotrain/app/ui_routes.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3220 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/app/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.805803 autotrain-advanced-0.7.95/src/autotrain/backends/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.95/src/autotrain/backends/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5071 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/backends/base.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2256 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.95/src/autotrain/backends/endpoints.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      505 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.95/src/autotrain/backends/local.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3485 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.95/src/autotrain/backends/ngc.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7322 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/backends/nvcf.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3022 2024-05-07 16:28:18.000000 autotrain-advanced-0.7.95/src/autotrain/backends/spaces.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-08-16 09:09:21.000000 autotrain-advanced-0.7.95/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3012 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2024-05-10 12:03:00.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_api.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4099 2024-05-15 11:15:24.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12957 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8313 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    15649 2024-05-09 12:41:42.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4098 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_object_detection.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10504 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_seq2seq.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1810 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5236 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_spacerunner.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7221 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8591 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8535 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_text_regression.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8512 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_token_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3132 2024-04-25 11:56:15.000000 autotrain-advanced-0.7.95/src/autotrain/cli/run_tools.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16773 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/cli/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11361 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/commands.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       67 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.95/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    19020 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4146 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.95/src/autotrain/help.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      827 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.95/src/autotrain/logging.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7034 2024-05-15 11:35:44.000000 autotrain-advanced-0.7.95/src/autotrain/parser.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.7.95/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3426 2024-05-08 11:32:05.000000 autotrain-advanced-0.7.95/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9038 2023-12-20 14:25:52.000000 autotrain-advanced-0.7.95/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16934 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.95/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12106 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2667 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      884 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/tools/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-25 10:33:47.000000 autotrain-advanced-0.7.95/src/autotrain/tools/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      607 2024-04-25 12:20:04.000000 autotrain-advanced-0.7.95/src/autotrain/tools/convert_to_kohya.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1671 2024-04-25 11:42:45.000000 autotrain-advanced-0.7.95/src/autotrain/tools/merge_adapter.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/__init__.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-16 07:43:26.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1438 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2157 2023-12-14 12:02:22.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3359 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6444 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_default.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4142 2024-05-09 09:41:41.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_dpo.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3492 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_orpo.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4363 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_reward.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3421 2024-05-03 11:21:58.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_sft.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    20504 2024-05-09 12:46:57.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/clm/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8222 2024-05-15 11:27:08.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/common.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-31 11:25:29.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10320 2024-05-09 12:33:09.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9085 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4061 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    40543 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/train.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    58739 2024-04-09 12:48:20.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/train_xl.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21953 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2687 2024-04-22 14:51:07.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/trainers/generic/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 17:28:06.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/generic/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1108 2023-12-14 15:04:28.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/generic/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      596 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/generic/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3644 2024-04-05 11:56:59.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/generic/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.809803 autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7497 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      724 2023-12-14 22:46:05.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1985 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4457 2024-03-11 15:23:33.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7185 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1354 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2143 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7592 2024-05-14 11:01:54.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8908 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      767 2023-10-21 10:19:31.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2585 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1642 2023-10-24 15:04:44.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-30 10:26:10.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12471 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1410 2024-04-24 14:57:21.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    16790 2024-02-24 10:05:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-08-11 12:06:11.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7738 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1488 2023-08-15 09:44:56.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2037 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3309 2023-08-23 10:09:58.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7019 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1500 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2036 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2117 2024-04-29 12:27:43.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-11-03 11:47:09.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     7519 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/__main__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1265 2024-02-08 15:18:42.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2038 2024-05-14 10:44:24.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1675 2024-04-25 05:15:09.000000 autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2082 2024-05-13 16:25:30.000000 autotrain-advanced-0.7.95/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)    13824 2024-05-15 14:36:37.000000 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     4912 2024-05-15 14:36:37.000000 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-05-15 14:36:37.000000 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2024-05-15 14:36:37.000000 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3687 2024-05-15 14:36:37.000000 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2024-05-15 14:36:37.000000 autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-05-15 14:36:37.813803 autotrain-advanced-0.7.95/static/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    45750 2023-11-21 15:17:41.000000 autotrain-advanced-0.7.95/static/logo.png
```

### Comparing `autotrain-advanced-0.7.94/LICENSE` & `autotrain-advanced-0.7.95/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/PKG-INFO` & `autotrain-advanced-0.7.95/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.94
+Version: 0.7.95
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
@@ -239,18 +239,26 @@
 # 🤗 AutoTrain Advanced
 
 AutoTrain Advanced: faster and easier training and deployments of state-of-the-art machine learning models. AutoTrain Advanced is a no-code solution that allows you to train machine learning models in just a few clicks. Please note that you must upload data in correct format for project to be created. For help regarding proper data format and pricing, check out the documentation. 
 
 NOTE: AutoTrain is free! You only pay for the resources you use in case you decide to run AutoTrain on Hugging Face Spaces. When running locally, you only pay for the resources you use on your own infrastructure.
 
 
-[![Deploy on Spaces](https://huggingface.co/datasets/huggingface/badges/resolve/main/deploy-on-spaces-md.svg)](https://huggingface.co/new-space?template=autotrain-projects/autotrain-advanced) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain.ipynb)
+## Run on Colab or Hugging Face Spaces
 
+- Run AutoTrain on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain.ipynb)
 
-## Installation
+
+- Deploy AutoTrain on Hugging Face Spaces: [![Deploy on Spaces](https://huggingface.co/datasets/huggingface/badges/resolve/main/deploy-on-spaces-md.svg)](https://huggingface.co/login?next=%2Fspaces%2Fautotrain-projects%2Fautotrain-advanced%3Fduplicate%3Dtrue)
+
+
+- Run AutoTrain UI on Colab via ngrok: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain_ngrok.ipynb)
+
+
+## Local Installation
 
 You can Install AutoTrain-Advanced python package via PIP. Please note you will need python >= 3.10 for AutoTrain Advanced to work properly.
 
     pip install autotrain-advanced
     
 Please make sure that you have git lfs installed. Check out the instructions here: https://github.com/git-lfs/git-lfs/wiki/Installation
```

### Comparing `autotrain-advanced-0.7.94/README.md` & `autotrain-advanced-0.7.95/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 # 🤗 AutoTrain Advanced
 
 AutoTrain Advanced: faster and easier training and deployments of state-of-the-art machine learning models. AutoTrain Advanced is a no-code solution that allows you to train machine learning models in just a few clicks. Please note that you must upload data in correct format for project to be created. For help regarding proper data format and pricing, check out the documentation. 
 
 NOTE: AutoTrain is free! You only pay for the resources you use in case you decide to run AutoTrain on Hugging Face Spaces. When running locally, you only pay for the resources you use on your own infrastructure.
 
 
-[![Deploy on Spaces](https://huggingface.co/datasets/huggingface/badges/resolve/main/deploy-on-spaces-md.svg)](https://huggingface.co/new-space?template=autotrain-projects/autotrain-advanced) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain.ipynb)
+## Run on Colab or Hugging Face Spaces
 
+- Run AutoTrain on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain.ipynb)
 
-## Installation
+
+- Deploy AutoTrain on Hugging Face Spaces: [![Deploy on Spaces](https://huggingface.co/datasets/huggingface/badges/resolve/main/deploy-on-spaces-md.svg)](https://huggingface.co/login?next=%2Fspaces%2Fautotrain-projects%2Fautotrain-advanced%3Fduplicate%3Dtrue)
+
+
+- Run AutoTrain UI on Colab via ngrok: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain_ngrok.ipynb)
+
+
+## Local Installation
 
 You can Install AutoTrain-Advanced python package via PIP. Please note you will need python >= 3.10 for AutoTrain Advanced to work properly.
 
     pip install autotrain-advanced
     
 Please make sure that you have git lfs installed. Check out the instructions here: https://github.com/git-lfs/git-lfs/wiki/Installation
```

### Comparing `autotrain-advanced-0.7.94/setup.py` & `autotrain-advanced-0.7.95/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/__init__.py` & `autotrain-advanced-0.7.95/src/autotrain/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,11 +34,20 @@
 
 warnings.filterwarnings("ignore", category=UserWarning, module="tensorflow")
 warnings.filterwarnings("ignore", category=UserWarning, module="transformers")
 warnings.filterwarnings("ignore", category=UserWarning, module="peft")
 warnings.filterwarnings("ignore", category=UserWarning, module="accelerate")
 warnings.filterwarnings("ignore", category=UserWarning, module="datasets")
 warnings.filterwarnings("ignore", category=FutureWarning, module="accelerate")
-
+warnings.filterwarnings("ignore", category=UserWarning, module="huggingface_hub")
 
 logger = Logger().get_logger()
-__version__ = "0.7.94"
+__version__ = "0.7.95"
+
+
+def is_colab():
+    try:
+        import google.colab
+
+        return True
+    except ImportError:
+        return False
```

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/api_routes.py` & `autotrain-advanced-0.7.95/src/autotrain/app/api_routes.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/app.py` & `autotrain-advanced-0.7.95/src/autotrain/app/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/db.py` & `autotrain-advanced-0.7.95/src/autotrain/app/db.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/models.py` & `autotrain-advanced-0.7.95/src/autotrain/app/models.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/oauth.py` & `autotrain-advanced-0.7.95/src/autotrain/app/oauth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/params.py` & `autotrain-advanced-0.7.95/src/autotrain/app/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,16 @@
         else:
             raise ValueError(f"Unknown task: {self.task}")
 
     def _munge_common_params(self):
         _params = json.loads(self.job_params_json)
         _params["token"] = self.token
         _params["project_name"] = f"{self.project_name}"
-        _params["push_to_hub"] = True
+        if "push_to_hub" not in _params:
+            _params["push_to_hub"] = True
         _params["data_path"] = self.data_path
         _params["username"] = self.username
         return _params
 
     def _munge_params_llm(self):
         _params = self._munge_common_params()
         _params["model"] = self.base_model
```

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/static/logo.png` & `autotrain-advanced-0.7.95/src/autotrain/app/static/logo.png`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/templates/duplicate.html` & `autotrain-advanced-0.7.95/src/autotrain/app/templates/duplicate.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/templates/error.html` & `autotrain-advanced-0.7.95/src/autotrain/app/templates/error.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/templates/index.html` & `autotrain-advanced-0.7.95/src/autotrain/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/templates/login.html` & `autotrain-advanced-0.7.95/src/autotrain/app/templates/login.html`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/training_api.py` & `autotrain-advanced-0.7.95/src/autotrain/app/training_api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/ui_routes.py` & `autotrain-advanced-0.7.95/src/autotrain/app/ui_routes.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/app/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/app/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/backends/base.py` & `autotrain-advanced-0.7.95/src/autotrain/backends/base.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/backends/endpoints.py` & `autotrain-advanced-0.7.95/src/autotrain/backends/endpoints.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/backends/ngc.py` & `autotrain-advanced-0.7.95/src/autotrain/backends/ngc.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/backends/nvcf.py` & `autotrain-advanced-0.7.95/src/autotrain/backends/nvcf.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/backends/spaces.py` & `autotrain-advanced-0.7.95/src/autotrain/backends/spaces.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_api.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_api.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_app.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         sys.stdout.write(line)
         sys.stdout.flush()
         log_file.write(line)
         log_file.flush()
 
 
 def run_app_command_factory(args):
-    return RunAutoTrainAppCommand(args.port, args.host, args.share, args.workers)
+    return RunAutoTrainAppCommand(args.port, args.host, args.share, args.workers, args.colab)
 
 
 class RunAutoTrainAppCommand(BaseAutoTrainCommand):
     @staticmethod
     def register_subcommand(parser: ArgumentParser):
         run_app_parser = parser.add_parser(
             "app",
@@ -55,26 +55,43 @@
         )
         run_app_parser.add_argument(
             "--share",
             action="store_true",
             help="Share the app on ngrok",
             required=False,
         )
+        run_app_parser.add_argument(
+            "--colab",
+            action="store_true",
+            help="Use app in colab",
+            required=False,
+        )
         run_app_parser.set_defaults(func=run_app_command_factory)
 
-    def __init__(self, port, host, share, workers):
+    def __init__(self, port, host, share, workers, colab):
         self.port = port
         self.host = host
         self.share = share
         self.workers = workers
+        self.colab = colab
 
     def run(self):
-        from pyngrok import ngrok
+
+        if self.colab:
+            from IPython.display import display
+
+            from autotrain.app.colab import colab_app
+
+            elements = colab_app()
+            display(elements)
+            return
 
         if self.share:
+            from pyngrok import ngrok
+
             os.system(f"fuser -n tcp -k {self.port}")
             authtoken = os.environ.get("NGROK_AUTH_TOKEN", "")
             if authtoken.strip() == "":
                 logger.info("NGROK_AUTH_TOKEN not set")
                 raise ValueError("NGROK_AUTH_TOKEN not set. Please set it!")
 
             ngrok.set_auth_token(authtoken)
```

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_image_classification.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_object_detection.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_object_detection.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_seq2seq.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_seq2seq.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_spacerunner.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_spacerunner.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_tabular.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_text_classification.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_text_regression.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_text_regression.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_token_classification.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_token_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/run_tools.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/run_tools.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/cli/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/cli/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/commands.py` & `autotrain-advanced-0.7.95/src/autotrain/commands.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/dataset.py` & `autotrain-advanced-0.7.95/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/help.py` & `autotrain-advanced-0.7.95/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/logging.py` & `autotrain-advanced-0.7.95/src/autotrain/logging.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/parser.py` & `autotrain-advanced-0.7.95/src/autotrain/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -70,24 +70,33 @@
         }
         self.task_aliases = {
             "llm": "lm_training",
             "llm_training": "lm_training",
             "llm_finetuning": "lm_training",
             "dreambooth": "dreambooth",
             "image_binary_classification": "image_multi_class_classification",
+            "image-binary-classification": "image_multi_class_classification",
             "image_classification": "image_multi_class_classification",
+            "image-classification": "image_multi_class_classification",
             "seq2seq": "seq2seq",
             "tabular": "tabular",
             "text_binary_classification": "text_multi_class_classification",
+            "text-binary-classification": "text_multi_class_classification",
             "text_classification": "text_multi_class_classification",
+            "text-classification": "text_multi_class_classification",
             "text_single_column_regression": "text_single_column_regression",
+            "text-single-column-regression": "text_single_column_regression",
             "text_regression": "text_single_column_regression",
+            "text-regression": "text_single_column_regression",
             "token_classification": "text_token_classification",
+            "token-classification": "text_token_classification",
             "image_object_detection": "image_object_detection",
+            "image-object-detection": "image_object_detection",
             "object_detection": "image_object_detection",
+            "object-detection": "image_object_detection",
         }
         task = self.config.get("task")
         self.task = self.task_aliases.get(task, task)
         if self.task is None:
             raise ValueError("Task is required in the configuration file")
         if self.task not in TASKS:
             raise ValueError(f"Task `{self.task}` is not supported")
```

### Comparing `autotrain-advanced-0.7.94/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.7.95/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.7.95/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.7.95/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.7.95/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/project.py` & `autotrain-advanced-0.7.95/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/tasks.py` & `autotrain-advanced-0.7.95/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/tools/convert_to_kohya.py` & `autotrain-advanced-0.7.95/src/autotrain/tools/convert_to_kohya.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/tools/merge_adapter.py` & `autotrain-advanced-0.7.95/src/autotrain/tools/merge_adapter.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/clm/__main__.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/clm/callbacks.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/clm/params.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/clm/train_clm_default.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_default.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/clm/train_clm_dpo.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_dpo.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/clm/train_clm_orpo.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_orpo.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/clm/train_clm_reward.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_reward.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/clm/train_clm_sft.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/train_clm_sft.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/clm/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/clm/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/common.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import requests
 from accelerate import PartialState
 from huggingface_hub import HfApi
 from pydantic import BaseModel
 from transformers import TrainerCallback, TrainerControl, TrainerState, TrainingArguments
 
-from autotrain import logger
+from autotrain import is_colab, logger
 
 
 ALLOW_REMOTE_CODE = os.environ.get("ALLOW_REMOTE_CODE", "true").lower() == "true"
 
 
 def get_file_sizes(directory):
     file_sizes = {}
@@ -166,15 +166,15 @@
         if len(self.project_name) > 50:
             raise ValueError("project_name cannot be more than 50 characters")
 
         # Parameters not supplied by the user
         defaults = set(self.model_fields.keys())
         supplied = set(data.keys())
         not_supplied = defaults - supplied
-        if not_supplied:
+        if not_supplied and not is_colab:
             logger.warning(f"Parameters not supplied by user and set to default: {', '.join(not_supplied)}")
 
         # Parameters that were supplied but not used
         # This is a naive implementation. It might catch some internal Pydantic params.
         unused = supplied - set(self.model_fields)
         if unused:
             logger.warning(f"Parameters supplied but not used: {', '.join(unused)}")
```

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/__main__.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/train.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/train.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/train_xl.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/train_xl.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/dreambooth/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/dreambooth/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/generic/__main__.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/generic/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/generic/params.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/generic/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/generic/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/generic/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/image_classification/__main__.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/image_classification/dataset.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/image_classification/params.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/image_classification/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/image_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/object_detection/__main__.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/object_detection/dataset.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/object_detection/params.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/object_detection/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/seq2seq/__main__.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/seq2seq/dataset.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/seq2seq/params.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/seq2seq/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/seq2seq/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/tabular/__main__.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/tabular/params.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/tabular/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/text_classification/__main__.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/text_classification/dataset.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/text_classification/params.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/text_classification/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/text_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/text_regression/__main__.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/text_regression/dataset.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/text_regression/params.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/text_regression/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/text_regression/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/token_classification/__main__.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/__main__.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/token_classification/dataset.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/token_classification/params.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/trainers/token_classification/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/trainers/token_classification/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain/utils.py` & `autotrain-advanced-0.7.95/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.7.94
+Version: 0.7.95
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
@@ -239,18 +239,26 @@
 # 🤗 AutoTrain Advanced
 
 AutoTrain Advanced: faster and easier training and deployments of state-of-the-art machine learning models. AutoTrain Advanced is a no-code solution that allows you to train machine learning models in just a few clicks. Please note that you must upload data in correct format for project to be created. For help regarding proper data format and pricing, check out the documentation. 
 
 NOTE: AutoTrain is free! You only pay for the resources you use in case you decide to run AutoTrain on Hugging Face Spaces. When running locally, you only pay for the resources you use on your own infrastructure.
 
 
-[![Deploy on Spaces](https://huggingface.co/datasets/huggingface/badges/resolve/main/deploy-on-spaces-md.svg)](https://huggingface.co/new-space?template=autotrain-projects/autotrain-advanced) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain.ipynb)
+## Run on Colab or Hugging Face Spaces
 
+- Run AutoTrain on Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain.ipynb)
 
-## Installation
+
+- Deploy AutoTrain on Hugging Face Spaces: [![Deploy on Spaces](https://huggingface.co/datasets/huggingface/badges/resolve/main/deploy-on-spaces-md.svg)](https://huggingface.co/login?next=%2Fspaces%2Fautotrain-projects%2Fautotrain-advanced%3Fduplicate%3Dtrue)
+
+
+- Run AutoTrain UI on Colab via ngrok: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/autotrain-advanced/blob/main/colabs/AutoTrain_ngrok.ipynb)
+
+
+## Local Installation
 
 You can Install AutoTrain-Advanced python package via PIP. Please note you will need python >= 3.10 for AutoTrain Advanced to work properly.
 
     pip install autotrain-advanced
     
 Please make sure that you have git lfs installed. Check out the instructions here: https://github.com/git-lfs/git-lfs/wiki/Installation
```

### Comparing `autotrain-advanced-0.7.94/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/autotrain/parser.py
 src/autotrain/project.py
 src/autotrain/tasks.py
 src/autotrain/utils.py
 src/autotrain/app/__init__.py
 src/autotrain/app/api_routes.py
 src/autotrain/app/app.py
+src/autotrain/app/colab.py
 src/autotrain/app/db.py
 src/autotrain/app/models.py
 src/autotrain/app/oauth.py
 src/autotrain/app/params.py
 src/autotrain/app/training_api.py
 src/autotrain/app/ui_routes.py
 src/autotrain/app/utils.py
```

### Comparing `autotrain-advanced-0.7.94/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.7.95/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.7.94/static/logo.png` & `autotrain-advanced-0.7.95/static/logo.png`

 * *Files identical despite different names*

