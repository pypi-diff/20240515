# Comparing `tmp/kan_gpt-1.0.1.tar.gz` & `tmp/kan_gpt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kan_gpt-1.0.1.tar", last modified: Thu May  9 07:46:24 2024, max compression
+gzip compressed data, was "kan_gpt-1.0.2.tar", last modified: Wed May 15 08:36:34 2024, max compression
```

## Comparing `kan_gpt-1.0.1.tar` & `kan_gpt-1.0.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:24.107515 kan_gpt-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-05-09 07:46:24.107515 kan_gpt-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:24.095515 kan_gpt-1.0.1/kan_gpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/download_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:24.099515 kan_gpt-1.0.1/kan_gpt/efficient_kan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/efficient_kan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/efficient_kan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:24.099515 kan_gpt-1.0.1/kan_gpt/kan/
--rw-r--r--   0 runner    (1001) docker     (127)    57987 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/KAN.py
--rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/LBFGS.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/Symbolic_KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:24.103515 kan_gpt-1.0.1/kan_gpt/kan/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_0_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_0_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_0_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_0_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_1_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_1_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_1_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_1_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_1_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_1_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_1_2_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_1_3_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/figures/sp_1_4_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/kan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:24.103515 kan_gpt-1.0.1/kan_gpt/mingpt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/mingpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/mingpt/bpe.py
--rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/mingpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/mingpt/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/mingpt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20656 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/kan_gpt/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:24.103515 kan_gpt-1.0.1/kan_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-05-09 07:46:24.000000 kan_gpt-1.0.1/kan_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-09 07:46:24.000000 kan_gpt-1.0.1/kan_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:46:24.000000 kan_gpt-1.0.1/kan_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 07:46:24.000000 kan_gpt-1.0.1/kan_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-09 07:46:24.000000 kan_gpt-1.0.1/kan_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 07:46:24.000000 kan_gpt-1.0.1/kan_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 07:46:24.107515 kan_gpt-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:24.103515 kan_gpt-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/tests/test_dataset_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/tests/test_efficient_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/tests/test_gpt_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/tests/test_gpt_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/tests/test_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-09 07:46:12.000000 kan_gpt-1.0.1/tests/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:34.909273 kan_gpt-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-15 08:36:34.909273 kan_gpt-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:34.897273 kan_gpt-1.0.2/kan_gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/download_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:34.901273 kan_gpt-1.0.2/kan_gpt/efficient_kan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/efficient_kan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/efficient_kan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:34.901273 kan_gpt-1.0.2/kan_gpt/kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    57987 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/KAN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/LBFGS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/Symbolic_KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:34.905273 kan_gpt-1.0.2/kan_gpt/kan/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_0_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_0_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_0_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_0_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_1_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_1_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_1_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_1_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_1_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_1_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_1_2_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_1_3_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/figures/sp_1_4_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/kan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:34.905273 kan_gpt-1.0.2/kan_gpt/mingpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/mingpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/mingpt/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/mingpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/mingpt/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/mingpt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20656 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/kan_gpt/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:34.905273 kan_gpt-1.0.2/kan_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-15 08:36:34.000000 kan_gpt-1.0.2/kan_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-15 08:36:34.000000 kan_gpt-1.0.2/kan_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:36:34.000000 kan_gpt-1.0.2/kan_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 08:36:34.000000 kan_gpt-1.0.2/kan_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-15 08:36:34.000000 kan_gpt-1.0.2/kan_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 08:36:34.000000 kan_gpt-1.0.2/kan_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:36:34.909273 kan_gpt-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:34.905273 kan_gpt-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/tests/test_dataset_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/tests/test_efficient_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/tests/test_gpt_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/tests/test_gpt_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/tests/test_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-15 08:36:27.000000 kan_gpt-1.0.2/tests/test_train.py
```

### Comparing `kan_gpt-1.0.1/HISTORY.md` & `kan_gpt-1.0.2/HISTORY.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Docs(README): absolute links. [Aditya NG]
+- Merge pull request #17 from KPCOFGS/main. [Aditya]
+
+  Update README.md
+- Update README.md. [Shixian Sheng]
+- Merge pull request #15 from eltociear/patch-1. [Aditya]
+
+  docs: Update README.md
+- Docs: Update README.md. [Ikko Eltociear Ashimine]
+
+  outine -> outline
+- Merge pull request #14 from TheMattBin/readme-update. [Aditya]
+- Update README.md. [Matthew Liu]
+
+
+1.0.1 (2024-05-09)
+------------------
+- Release: version 1.0.1 🚀 [Aditya NG]
 - Test(kan): coverage improved. [Aditya NG]
 - Docs(README,docs/): badges. [Aditya NG]
 - Docs(README.md): typo. [Aditya NG]
 
 
 1.0.0 (2024-05-09)
 ------------------
```

### Comparing `kan_gpt-1.0.1/LICENSE` & `kan_gpt-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/PKG-INFO` & `kan_gpt-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 1.0.1
+Version: 1.0.2
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -30,31 +30,31 @@
 Requires-Dist: lark; extra == "test"
 Requires-Dist: types-requests; extra == "test"
 Requires-Dist: requests-mock; extra == "test"
 
 # KAN-GPT
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/kan-gpt)
-![PyPI - Version](https://img.shields.io/pypi/v/kan-gpt)
+[![PyPI - Version](https://img.shields.io/pypi/v/kan-gpt)](https://pypi.org/project/kan-gpt/)
 [![codecov](https://codecov.io/gh/AdityaNG/kan-gpt/branch/main/graph/badge.svg?token=kan-gpt_token_here)](https://codecov.io/gh/AdityaNG/kan-gpt)
 [![CI](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml/badge.svg)](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml)
-![GitHub License](https://img.shields.io/github/license/AdityaNG/kan-gpt)
+[![GitHub License](https://img.shields.io/github/license/AdityaNG/kan-gpt)](https://github.com/AdityaNG/kan-gpt/blob/main/LICENSE)
 
 
 The PyTorch implementation of Generative Pre-trained Transformers (GPTs) using Kolmogorov-Arnold Networks (KANs) for language modeling
 
 ## Install it from PyPI
 
 ```bash
 pip install kan_gpt
 ```
 
 ## Usage
 
-Refer to the [KAN_GPT.ipynb](KAN_GPT.ipynb) and [kan_gpt/prompt.py](kan_gpt/prompt.py) for usage examples. The following is an outine of how to use the model:
+Refer to the [KAN_GPT.ipynb](https://github.com/AdityaNG/kan-gpt/blob/main/KAN_GPT.ipynb) and [kan_gpt/prompt.py](https://github.com/AdityaNG/kan-gpt/blob/main/kan_gpt/prompt.py) for usage examples. The following is an outline of how to use the model:
 
 ```py
 from kan_gpt.model import GPT
 from transformers import GPT2Tokenizer
 
 model_config = GPT.get_default_config()
 model_config.model_type = "gpt2"
@@ -157,15 +157,15 @@
   - [x] KAN: Forward-Backward test
   - [x] GPT: Forward-Backward test
   - [x] KAN_GPT: Forward-Backward test
   - [x] EFFICIENT_KAN: Forward-Backward test
 
 ## Development
 
-Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+Read the [CONTRIBUTING.md](https://github.com/AdityaNG/kan-gpt/blob/main/CONTRIBUTING.md) file.
 
 ## References
 
 - [minGPT](https://github.com/karpathy/minGPT)
 - [pykan](https://github.com/KindXiaoming/pykan)
 - [webtext](https://github.com/openai/gpt-2-output-dataset)
 - [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
```

### Comparing `kan_gpt-1.0.1/README.md` & `kan_gpt-1.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # KAN-GPT
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/kan-gpt)
-![PyPI - Version](https://img.shields.io/pypi/v/kan-gpt)
+[![PyPI - Version](https://img.shields.io/pypi/v/kan-gpt)](https://pypi.org/project/kan-gpt/)
 [![codecov](https://codecov.io/gh/AdityaNG/kan-gpt/branch/main/graph/badge.svg?token=kan-gpt_token_here)](https://codecov.io/gh/AdityaNG/kan-gpt)
 [![CI](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml/badge.svg)](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml)
-![GitHub License](https://img.shields.io/github/license/AdityaNG/kan-gpt)
+[![GitHub License](https://img.shields.io/github/license/AdityaNG/kan-gpt)](https://github.com/AdityaNG/kan-gpt/blob/main/LICENSE)
 
 
 The PyTorch implementation of Generative Pre-trained Transformers (GPTs) using Kolmogorov-Arnold Networks (KANs) for language modeling
 
 ## Install it from PyPI
 
 ```bash
 pip install kan_gpt
 ```
 
 ## Usage
 
-Refer to the [KAN_GPT.ipynb](KAN_GPT.ipynb) and [kan_gpt/prompt.py](kan_gpt/prompt.py) for usage examples. The following is an outine of how to use the model:
+Refer to the [KAN_GPT.ipynb](https://github.com/AdityaNG/kan-gpt/blob/main/KAN_GPT.ipynb) and [kan_gpt/prompt.py](https://github.com/AdityaNG/kan-gpt/blob/main/kan_gpt/prompt.py) for usage examples. The following is an outline of how to use the model:
 
 ```py
 from kan_gpt.model import GPT
 from transformers import GPT2Tokenizer
 
 model_config = GPT.get_default_config()
 model_config.model_type = "gpt2"
@@ -124,15 +124,15 @@
   - [x] KAN: Forward-Backward test
   - [x] GPT: Forward-Backward test
   - [x] KAN_GPT: Forward-Backward test
   - [x] EFFICIENT_KAN: Forward-Backward test
 
 ## Development
 
-Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+Read the [CONTRIBUTING.md](https://github.com/AdityaNG/kan-gpt/blob/main/CONTRIBUTING.md) file.
 
 ## References
 
 - [minGPT](https://github.com/karpathy/minGPT)
 - [pykan](https://github.com/KindXiaoming/pykan)
 - [webtext](https://github.com/openai/gpt-2-output-dataset)
 - [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
```

### Comparing `kan_gpt-1.0.1/kan_gpt/cli.py` & `kan_gpt-1.0.2/kan_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/dataset.py` & `kan_gpt-1.0.2/kan_gpt/dataset.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/download_dataset.py` & `kan_gpt-1.0.2/kan_gpt/download_dataset.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/efficient_kan/model.py` & `kan_gpt-1.0.2/kan_gpt/efficient_kan/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/KAN.py` & `kan_gpt-1.0.2/kan_gpt/kan/KAN.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/KANLayer.py` & `kan_gpt-1.0.2/kan_gpt/kan/KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/LBFGS.py` & `kan_gpt-1.0.2/kan_gpt/kan/LBFGS.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/Symbolic_KANLayer.py` & `kan_gpt-1.0.2/kan_gpt/kan/Symbolic_KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_0_0.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_0_1.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_0_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_0_2.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_0_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_0_3.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_0_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_0_4.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_0_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_1_0.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_1_1.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_1_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_1_2.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_1_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_1_3.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_1_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_0_1_4.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_0_1_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_1_0_0.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_1_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_1_1_0.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_1_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_1_2_0.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_1_2_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_1_3_0.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_1_3_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/figures/sp_1_4_0.png` & `kan_gpt-1.0.2/kan_gpt/kan/figures/sp_1_4_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/spline.py` & `kan_gpt-1.0.2/kan_gpt/kan/spline.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/kan/utils.py` & `kan_gpt-1.0.2/kan_gpt/kan/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/mingpt/bpe.py` & `kan_gpt-1.0.2/kan_gpt/mingpt/bpe.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/mingpt/model.py` & `kan_gpt-1.0.2/kan_gpt/mingpt/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/mingpt/trainer.py` & `kan_gpt-1.0.2/kan_gpt/mingpt/trainer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/mingpt/utils.py` & `kan_gpt-1.0.2/kan_gpt/mingpt/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/model.py` & `kan_gpt-1.0.2/kan_gpt/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/prompt.py` & `kan_gpt-1.0.2/kan_gpt/prompt.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/sweep.py` & `kan_gpt-1.0.2/kan_gpt/sweep.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt/train.py` & `kan_gpt-1.0.2/kan_gpt/train.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/kan_gpt.egg-info/PKG-INFO` & `kan_gpt-1.0.2/kan_gpt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 1.0.1
+Version: 1.0.2
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -30,31 +30,31 @@
 Requires-Dist: lark; extra == "test"
 Requires-Dist: types-requests; extra == "test"
 Requires-Dist: requests-mock; extra == "test"
 
 # KAN-GPT
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/kan-gpt)
-![PyPI - Version](https://img.shields.io/pypi/v/kan-gpt)
+[![PyPI - Version](https://img.shields.io/pypi/v/kan-gpt)](https://pypi.org/project/kan-gpt/)
 [![codecov](https://codecov.io/gh/AdityaNG/kan-gpt/branch/main/graph/badge.svg?token=kan-gpt_token_here)](https://codecov.io/gh/AdityaNG/kan-gpt)
 [![CI](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml/badge.svg)](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml)
-![GitHub License](https://img.shields.io/github/license/AdityaNG/kan-gpt)
+[![GitHub License](https://img.shields.io/github/license/AdityaNG/kan-gpt)](https://github.com/AdityaNG/kan-gpt/blob/main/LICENSE)
 
 
 The PyTorch implementation of Generative Pre-trained Transformers (GPTs) using Kolmogorov-Arnold Networks (KANs) for language modeling
 
 ## Install it from PyPI
 
 ```bash
 pip install kan_gpt
 ```
 
 ## Usage
 
-Refer to the [KAN_GPT.ipynb](KAN_GPT.ipynb) and [kan_gpt/prompt.py](kan_gpt/prompt.py) for usage examples. The following is an outine of how to use the model:
+Refer to the [KAN_GPT.ipynb](https://github.com/AdityaNG/kan-gpt/blob/main/KAN_GPT.ipynb) and [kan_gpt/prompt.py](https://github.com/AdityaNG/kan-gpt/blob/main/kan_gpt/prompt.py) for usage examples. The following is an outline of how to use the model:
 
 ```py
 from kan_gpt.model import GPT
 from transformers import GPT2Tokenizer
 
 model_config = GPT.get_default_config()
 model_config.model_type = "gpt2"
@@ -157,15 +157,15 @@
   - [x] KAN: Forward-Backward test
   - [x] GPT: Forward-Backward test
   - [x] KAN_GPT: Forward-Backward test
   - [x] EFFICIENT_KAN: Forward-Backward test
 
 ## Development
 
-Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+Read the [CONTRIBUTING.md](https://github.com/AdityaNG/kan-gpt/blob/main/CONTRIBUTING.md) file.
 
 ## References
 
 - [minGPT](https://github.com/karpathy/minGPT)
 - [pykan](https://github.com/KindXiaoming/pykan)
 - [webtext](https://github.com/openai/gpt-2-output-dataset)
 - [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
```

### Comparing `kan_gpt-1.0.1/kan_gpt.egg-info/SOURCES.txt` & `kan_gpt-1.0.2/kan_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/setup.py` & `kan_gpt-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/tests/test_dataset_download.py` & `kan_gpt-1.0.2/tests/test_dataset_download.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/tests/test_efficient_kan.py` & `kan_gpt-1.0.2/tests/test_efficient_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/tests/test_gpt_kan.py` & `kan_gpt-1.0.2/tests/test_gpt_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/tests/test_gpt_mlp.py` & `kan_gpt-1.0.2/tests/test_gpt_mlp.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/tests/test_kan.py` & `kan_gpt-1.0.2/tests/test_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.1/tests/test_train.py` & `kan_gpt-1.0.2/tests/test_train.py`

 * *Files identical despite different names*

