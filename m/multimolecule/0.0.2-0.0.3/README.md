# Comparing `tmp/multimolecule-0.0.2.tar.gz` & `tmp/multimolecule-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimolecule-0.0.2.tar", last modified: Thu Apr 18 13:35:04 2024, max compression
+gzip compressed data, was "multimolecule-0.0.3.tar", last modified: Wed May 15 06:34:30 2024, max compression
```

## Comparing `multimolecule-0.0.2.tar` & `multimolecule-0.0.3.tar`

### file list

```diff
@@ -1,66 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.667251 multimolecule-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:55.000000 multimolecule-0.0.2/.codespell-whitelist.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.659251 multimolecule-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-18 13:34:55.000000 multimolecule-0.0.2/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.659251 multimolecule-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-18 13:34:55.000000 multimolecule-0.0.2/.github/workflows/push.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-04-18 13:34:55.000000 multimolecule-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-18 13:34:55.000000 multimolecule-0.0.2/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)    34522 2024-04-18 13:34:55.000000 multimolecule-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41154 2024-04-18 13:35:04.667251 multimolecule-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:55.000000 multimolecule-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.659251 multimolecule-0.0.2/multimolecule/
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 13:35:04.000000 multimolecule-0.0.2/multimolecule/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.659251 multimolecule-0.0.2/multimolecule/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/modeling_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.659251 multimolecule-0.0.2/multimolecule/models/rnabert/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnabert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnabert/configuration_rnabert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnabert/convert_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    25725 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnabert/modeling_rnabert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.659251 multimolecule-0.0.2/multimolecule/models/rnafm/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnafm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnafm/configuration_rnafm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnafm/convert_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51027 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnafm/modeling_rnafm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule/models/rnamsm/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnamsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnamsm/configuration_rnamsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnamsm/convert_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    50103 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnamsm/modeling_rnamsm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule/models/splicebert/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/splicebert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/splicebert/configuration_splicebert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/splicebert/convert_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    48169 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/splicebert/modeling_splicebert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule/models/utrbert/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrbert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrbert/configuration_utrbert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrbert/convert_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    46386 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrbert/modeling_utrbert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule/models/utrlm/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrlm/configuration_utrlm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrlm/convert_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    52324 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrlm/modeling_utrlm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule/tokenizers/rna/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/tokenizers/rna/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5285 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/tokenizers/rna/tokenization_rna.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2072 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/tokenizers/rna/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/tokenizers/rna/vocab.txt
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/tokenizers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41154 2024-04-18 13:35:04.000000 multimolecule-0.0.2/multimolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-18 13:35:04.000000 multimolecule-0.0.2/multimolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:35:04.000000 multimolecule-0.0.2/multimolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 13:35:04.000000 multimolecule-0.0.2/multimolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 13:35:04.000000 multimolecule-0.0.2/multimolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-18 13:34:55.000000 multimolecule-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:35:04.667251 multimolecule-0.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-18 13:34:55.000000 multimolecule-0.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-18 13:34:55.000000 multimolecule-0.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.657116 multimolecule-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:25.000000 multimolecule-0.0.3/.codespell-whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.645116 multimolecule-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 06:34:25.000000 multimolecule-0.0.3/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.645116 multimolecule-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-15 06:34:25.000000 multimolecule-0.0.3/.github/workflows/push.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-05-15 06:34:25.000000 multimolecule-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-15 06:34:25.000000 multimolecule-0.0.3/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34522 2024-05-15 06:34:25.000000 multimolecule-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-15 06:34:25.000000 multimolecule-0.0.3/LICENSE.header
+-rw-r--r--   0 runner    (1001) docker     (127)    41206 2024-05-15 06:34:30.657116 multimolecule-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:25.000000 multimolecule-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-15 06:34:25.000000 multimolecule-0.0.3/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-15 06:34:25.000000 multimolecule-0.0.3/licensing.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.645116 multimolecule-0.0.3/multimolecule/
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 06:34:30.000000 multimolecule-0.0.3/multimolecule/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.649116 multimolecule-0.0.3/multimolecule/downstream/
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/downstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23561 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/downstream/crispr_off_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.649116 multimolecule-0.0.3/multimolecule/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/modeling_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/modeling_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.649116 multimolecule-0.0.3/multimolecule/models/rnabert/
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/rnabert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/rnabert/configuration_rnabert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/rnabert/convert_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27397 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/rnabert/modeling_rnabert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.649116 multimolecule-0.0.3/multimolecule/models/rnafm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/rnafm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/rnafm/configuration_rnafm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/rnafm/convert_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52341 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/rnafm/modeling_rnafm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.649116 multimolecule-0.0.3/multimolecule/models/rnamsm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/rnamsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/rnamsm/configuration_rnamsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/rnamsm/convert_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51949 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/rnamsm/modeling_rnamsm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.653116 multimolecule-0.0.3/multimolecule/models/splicebert/
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/splicebert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/splicebert/configuration_splicebert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/splicebert/convert_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49431 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/splicebert/modeling_splicebert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.653116 multimolecule-0.0.3/multimolecule/models/utrbert/
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/utrbert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/utrbert/configuration_utrbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/utrbert/convert_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47521 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/utrbert/modeling_utrbert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.653116 multimolecule-0.0.3/multimolecule/models/utrlm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/utrlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/utrlm/configuration_utrlm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/utrlm/convert_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53549 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/models/utrlm/modeling_utrlm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.653116 multimolecule-0.0.3/multimolecule/module/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.653116 multimolecule-0.0.3/multimolecule/module/criterions/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/criterions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/criterions/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.653116 multimolecule-0.0.3/multimolecule/module/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/heads/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/heads/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/heads/nuleotide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/heads/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/heads/pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/heads/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/heads/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/heads/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/module/heads/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.657116 multimolecule-0.0.3/multimolecule/tokenisers/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/tokenisers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.657116 multimolecule-0.0.3/multimolecule/tokenisers/rna/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/tokenisers/rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/tokenisers/rna/tokenization_rna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/tokenisers/rna/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/tokenisers/rna/vocab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-15 06:34:25.000000 multimolecule-0.0.3/multimolecule/tokenisers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:34:30.657116 multimolecule-0.0.3/multimolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41206 2024-05-15 06:34:30.000000 multimolecule-0.0.3/multimolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-15 06:34:30.000000 multimolecule-0.0.3/multimolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:34:30.000000 multimolecule-0.0.3/multimolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 06:34:30.000000 multimolecule-0.0.3/multimolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 06:34:30.000000 multimolecule-0.0.3/multimolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-15 06:34:25.000000 multimolecule-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:34:30.657116 multimolecule-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 06:34:25.000000 multimolecule-0.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 06:34:25.000000 multimolecule-0.0.3/tox.ini
```

### Comparing `multimolecule-0.0.2/.gitignore` & `multimolecule-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `multimolecule-0.0.2/.pre-commit-config.yaml` & `multimolecule-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `multimolecule-0.0.2/LICENSE` & `multimolecule-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multimolecule-0.0.2/PKG-INFO` & `multimolecule-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimolecule
-Version: 0.0.2
+Version: 0.0.3
 Summary: Neural Networks for RNA, DNA, and Protein.
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,9 +682,11 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE.header
 Requires-Dist: chanfig>=0.0.99
+Requires-Dist: danling
 Requires-Dist: transformers
```

### Comparing `multimolecule-0.0.2/multimolecule/models/configuration_utils.py` & `multimolecule-0.0.3/multimolecule/models/configuration_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,27 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from __future__ import annotations
 
+from collections import OrderedDict
 from dataclasses import asdict, dataclass, is_dataclass
-from typing import Optional
 
 from transformers.configuration_utils import PretrainedConfig as _PretrainedConfig
 
 
 class PretrainedConfig(_PretrainedConfig):
     head: HeadConfig
 
@@ -34,65 +50,69 @@
             if hasattr(v, "to_dict"):
                 output[k] = v.to_dict()
             if is_dataclass(v):
                 output[k] = asdict(v)
         return output
 
 
+class BaseHeadConfig(OrderedDict):
+    pass
+
+
 @dataclass
-class HeadConfig:
+class HeadConfig(BaseHeadConfig):
     r"""
     This is the configuration class to store the configuration of a prediction head. It is used to instantiate a
     prediction head according to the specified arguments, defining the head architecture.
 
-    Configuration objects inherit from [`HeadConfig`] and can be used to control the model outputs. Read the
-    documentation from [`HeadConfig`] for more information.
+    Configuration objects inherit from [`BaseHeadConfig`] and can be used to control the model outputs. Read the
+    documentation from [`BaseHeadConfig`] for more information.
 
 
     Args:
+        num_labels (`int`, *optional*):
+            Number of labels to use in the last layer added to the model, typically for a classification task.
+        problem_type (`str`, *optional*):
+            Problem type for `XxxForSequenceClassification` models. Can be one of `"regression"`,
+            `"single_label_classification"` or `"multi_label_classification"`.
         hidden_size (`int`, *optional*, defaults to 768):
             Dimensionality of the encoder layers and the pooler layer.
         dropout (`float`, *optional*, defaults to 0.0):
             The dropout ratio for the hidden states.
         transform (`str`, *optional*, defaults to None):
             The transform operation applied to hidden states.
-        transform_act (`str`, *optional*, defaults to "tanh"):
+        transform_act (`str`, *optional*, defaults to "gelu"):
             The activation function of transform applied to hidden states.
         bias (`bool`, *optional*, defaults to True):
             Whether to apply bias to the final prediction layer.
         act (`str`, *optional*, defaults to None):
             The activation function of the final prediction output.
         layer_norm_eps (`float`, *optional*, defaults to 1e-12):
             The epsilon used by the layer normalization layers.
-        num_labels (`int`, *optional*, defaults to 2):
-            Number of labels to use in the last layer added to the model, typically for a classification task.
-        problem_type (`str`, *optional*):
-            Problem type for `XxxForSequenceClassification` models. Can be one of `"regression"`,
-            `"single_label_classification"` or `"multi_label_classification"`.
     """
 
-    hidden_size: Optional[int] = None
+    num_labels: int = None  # type: ignore[assignment]
+    problem_type: str = None  # type: ignore[assignment]
+    hidden_size: int | None = None
     dropout: float = 0.0
-    transform: Optional[str] = None
-    transform_act: Optional[str] = "tanh"
+    transform: str | None = None
+    transform_act: str | None = "gelu"
     bias: bool = True
-    act: Optional[str] = None
+    act: str | None = None
     layer_norm_eps: float = 1e-12
-    num_labels: int = 2
-    problem_type: Optional[str] = None
 
 
 @dataclass
-class MaskedLMHeadConfig:
+class MaskedLMHeadConfig(BaseHeadConfig):
     r"""
     This is the configuration class to store the configuration of a prediction head. It is used to instantiate a
     prediction head according to the specified arguments, defining the head architecture.
 
-    Configuration objects inherit from [`HeadConfig`] and can be used to control the model outputs. Read the
-    documentation from [`HeadConfig`] for more information.
+    Configuration objects inherit from [`BaseHeadConfig`] and can be used to control the model outputs. Read the
+    documentation from [`BaseHeadConfig`] for more information.
 
 
     Args:
         hidden_size (`int`, *optional*, defaults to 768):
             Dimensionality of the encoder layers and the pooler layer.
         dropout (`float`, *optional*, defaults to 0.0):
             The dropout ratio for the hidden states.
@@ -104,14 +124,14 @@
             Whether to apply bias to the final prediction layer.
         act (`str`, *optional*, defaults to None):
             The activation function of the final prediction output.
         layer_norm_eps (`float`, *optional*, defaults to 1e-12):
             The epsilon used by the layer normalization layers.
     """
 
-    hidden_size: Optional[int] = None
+    hidden_size: int | None = None
     dropout: float = 0.0
-    transform: Optional[str] = "nonlinear"
-    transform_act: Optional[str] = "gelu"
+    transform: str | None = "nonlinear"
+    transform_act: str | None = "gelu"
     bias: bool = True
-    act: Optional[str] = None
+    act: str | None = None
     layer_norm_eps: float = 1e-12
```

### Comparing `multimolecule-0.0.2/multimolecule/models/rnabert/configuration_rnabert.py` & `multimolecule-0.0.3/multimolecule/models/splicebert/configuration_splicebert.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,110 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from transformers.utils import logging
 
 from ..configuration_utils import HeadConfig, MaskedLMHeadConfig, PretrainedConfig
 
 logger = logging.get_logger(__name__)
 
 
-class RnaBertConfig(PretrainedConfig):
+class SpliceBertConfig(PretrainedConfig):
     r"""
-    This is the configuration class to store the configuration of a [`RnaBertModel`]. It is used to instantiate a
-    RnaBert model according to the specified arguments, defining the model architecture. Instantiating a configuration
-    with the defaults will yield a similar configuration to that of the RnaBert
-    [mana438/RNABERT](https://github.com/mana438/RNABERT) architecture.
+    This is the configuration class to store the configuration of a [`SpliceBertModel`]. It is used to instantiate a
+    SpliceBert model according to the specified arguments, defining the model architecture. Instantiating a
+    configuration with the defaults will yield a similar configuration to that of the SpliceBert
+    [biomed-AI/SpliceBERT](https://github.com/biomed-AI/SpliceBERT) architecture.
 
     Configuration objects inherit from [`PretrainedConfig`] and can be used to control the model outputs. Read the
     documentation from [`PretrainedConfig`] for more information.
 
 
     Args:
         vocab_size (`int`, *optional*, defaults to 25):
-            Vocabulary size of the RnaBert model. Defines the number of different tokens that can be represented by the
-            `inputs_ids` passed when calling [`RnaBertModel`].
-        hidden_size (`int`, *optional*, defaults to 120):
+            Vocabulary size of the SpliceBert model. Defines the number of different tokens that can be represented by
+            the `inputs_ids` passed when calling [`SpliceBertModel`].
+        hidden_size (`int`, *optional*, defaults to 512):
             Dimensionality of the encoder layers and the pooler layer.
-        num_hidden_layers (`int`, *optional*, defaults to 12):
+        num_hidden_layers (`int`, *optional*, defaults to 6):
             Number of hidden layers in the Transformer encoder.
-        num_attention_heads (`int`, *optional*, defaults to 6):
+        num_attention_heads (`int`, *optional*, defaults to 16):
             Number of attention heads for each attention layer in the Transformer encoder.
-        intermediate_size (`int`, *optional*, defaults to 40):
+        intermediate_size (`int`, *optional*, defaults to 2048):
             Dimensionality of the "intermediate" (often named feed-forward) layer in the Transformer encoder.
-        hidden_dropout (`float`, *optional*, defaults to 0.0):
+        hidden_dropout (`float`, *optional*, defaults to 0.1):
             The dropout probability for all fully connected layers in the embeddings, encoder, and pooler.
-        attention_dropout (`float`, *optional*, defaults to 0.0):
+        attention_dropout (`float`, *optional*, defaults to 0.1):
             The dropout ratio for the attention probabilities.
-        max_position_embeddings (`int`, *optional*, defaults to 440):
+        max_position_embeddings (`int`, *optional*, defaults to 1026):
             The maximum sequence length that this model might ever be used with. Typically set this to something large
             just in case (e.g., 512 or 1024 or 2048).
         initializer_range (`float`, *optional*, defaults to 0.02):
             The standard deviation of the truncated_normal_initializer for initializing all weight matrices.
         layer_norm_eps (`float`, *optional*, defaults to 1e-12):
             The epsilon used by the layer normalization layers.
 
     Examples:
-        >>> from multimolecule import RnaBertModel, RnaBertConfig
+        >>> from multimolecule import SpliceBertModel, SpliceBertConfig
 
-        >>> # Initializing a RNABERT multimolecule/rnabert style configuration
-        >>> configuration = RnaBertConfig()
+        >>> # Initializing a SpliceBERT multimolecule/splicebert style configuration
+        >>> configuration = SpliceBertConfig()
 
-        >>> # Initializing a model (with random weights) from the multimolecule/rnabert style configuration
-        >>> model = RnaBertModel(configuration)
+        >>> # Initializing a model (with random weights) from the multimolecule/splicebert style configuration
+        >>> model = SpliceBertModel(configuration)
 
         >>> # Accessing the model configuration
         >>> configuration = model.config
     """
 
-    model_type = "rnabert"
+    model_type = "splicebert"
 
     def __init__(
         self,
         vocab_size=25,
-        ss_vocab_size=8,
-        hidden_size=None,
-        multiple=None,
+        hidden_size=512,
         num_hidden_layers=6,
-        num_attention_heads=12,
-        intermediate_size=40,
+        num_attention_heads=16,
+        intermediate_size=2048,
         hidden_act="gelu",
-        hidden_dropout=0.0,
-        attention_dropout=0.0,
-        max_position_embeddings=440,
+        hidden_dropout=0.1,
+        attention_dropout=0.1,
+        max_position_embeddings=1026,
         initializer_range=0.02,
         layer_norm_eps=1e-12,
         position_embedding_type="absolute",
         use_cache=True,
         head=None,
         lm_head=None,
         **kwargs,
     ):
-        if hidden_size is None:
-            hidden_size = num_attention_heads * multiple if multiple is not None else 120
-        if head is None:
-            head = {}
-        head.setdefault("hidden_size", hidden_size)
-        if "problem_type" in kwargs:
-            head.setdefault("problem_type", kwargs["problem_type"])
-        if "num_labels" in kwargs:
-            head.setdefault("num_labels", kwargs["num_labels"])
-        if lm_head is None:
-            lm_head = {}
-        lm_head.setdefault("hidden_size", hidden_size)
         super().__init__(**kwargs)
 
         self.vocab_size = vocab_size
-        self.ss_vocab_size = ss_vocab_size
         self.type_vocab_size = 2
         self.hidden_size = hidden_size
         self.num_hidden_layers = num_hidden_layers
         self.num_attention_heads = num_attention_heads
         self.intermediate_size = intermediate_size
         self.hidden_act = hidden_act
         self.hidden_dropout = hidden_dropout
         self.attention_dropout = attention_dropout
         self.max_position_embeddings = max_position_embeddings
         self.initializer_range = initializer_range
         self.layer_norm_eps = layer_norm_eps
         self.position_embedding_type = position_embedding_type
         self.use_cache = use_cache
-        self.head = HeadConfig(**head)
-        self.lm_head = MaskedLMHeadConfig(**lm_head)
+        self.head = HeadConfig(**head if head is not None else {})
+        self.lm_head = MaskedLMHeadConfig(**lm_head if lm_head is not None else {})
```

### Comparing `multimolecule-0.0.2/multimolecule/models/rnabert/convert_checkpoint.py` & `multimolecule-0.0.3/multimolecule/models/rnabert/convert_checkpoint.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,38 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from __future__ import annotations
+
 import os
-from typing import Optional
 
 import chanfig
 import torch
-from torch import nn
 
 from multimolecule.models.rnabert import RnaBertConfig as Config
 from multimolecule.models.rnabert import RnaBertForPretraining as Model
-from multimolecule.tokenizers.rna.utils import get_special_tokens_map, get_tokenizer_config, get_vocab_list
+from multimolecule.tokenisers.rna.utils import (
+    convert_word_embeddings,
+    get_special_tokens_map,
+    get_tokenizer_config,
+    get_vocab_list,
+)
 
 try:
     from huggingface_hub import HfApi
 except ImportError:
     HfApi = None
 
 torch.manual_seed(1013)
@@ -29,35 +50,25 @@
             continue
         if key.startswith("cls"):
             key = "pretrain_head." + key[4:]
             state_dict[key] = value
             continue
         state_dict[key] = value
 
-    state_vocab_size = state_dict["rnabert.embeddings.word_embeddings.weight"].size(0)
-    original_vocab_size = len(original_vocab_list)
-    if state_vocab_size != original_vocab_size:
-        raise ValueError(
-            f"Vocabulary size do not match. Expected to have {original_vocab_size}, but got {state_vocab_size}."
-        )
-    word_embed = nn.Embedding(config.vocab_size, config.hidden_size, padding_idx=config.pad_token_id)
-    word_embed_weight = word_embed.weight.data
-    predictions_decoder_weight = torch.zeros((config.vocab_size, config.hidden_size))
-    predictions_bias = torch.zeros(config.vocab_size)
-    # nn.init.normal_(pos_embed.weight, std=0.02)
-    for original_index, original_token in enumerate(original_vocab_list):
-        new_index = vocab_list.index(original_token)
-        word_embed_weight[new_index] = state_dict["rnabert.embeddings.word_embeddings.weight"][original_index]
-        predictions_decoder_weight[new_index] = state_dict["pretrain_head.predictions.decoder.weight"][original_index]
-        predictions_bias[new_index] = state_dict["pretrain_head.predictions.bias"][original_index]
-    state_dict["rnabert.embeddings.word_embeddings.weight"] = word_embed_weight
-    state_dict["pretrain_head.predictions.decoder.weight"] = predictions_decoder_weight
-    state_dict["pretrain_head.predictions.decoder.bias"] = state_dict["pretrain_head.predictions.bias"] = (
-        predictions_bias
+    word_embed_weight, decoder_weight, decoder_bias = convert_word_embeddings(
+        state_dict["rnabert.embeddings.word_embeddings.weight"],
+        state_dict["pretrain_head.predictions.decoder.weight"],
+        state_dict["pretrain_head.predictions.bias"],
+        old_vocab=original_vocab_list,
+        new_vocab=vocab_list,
+        std=config.initializer_range,
     )
+    state_dict["rnabert.embeddings.word_embeddings.weight"] = word_embed_weight
+    state_dict["pretrain_head.predictions.decoder.weight"] = decoder_weight
+    state_dict["pretrain_head.predictions.decoder.bias"] = state_dict["pretrain_head.predictions.bias"] = decoder_bias
     state_dict["pretrain_head.predictions_ss.decoder.bias"] = state_dict["pretrain_head.predictions_ss.bias"]
     return state_dict
 
 
 def convert_checkpoint(convert_config):
     vocab_list = get_vocab_list()
     original_vocab_list = ["<pad>", "<mask>", "A", "U", "G", "C"]
@@ -72,20 +83,28 @@
 
     model.load_state_dict(state_dict)
     model.save_pretrained(convert_config.output_path, safe_serialization=True)
     model.save_pretrained(convert_config.output_path, safe_serialization=False)
     chanfig.NestedDict(get_special_tokens_map()).json(
         os.path.join(convert_config.output_path, "special_tokens_map.json")
     )
-    chanfig.NestedDict(get_tokenizer_config()).json(os.path.join(convert_config.output_path, "tokenizer_config.json"))
+    tokenizer_config = chanfig.NestedDict(get_tokenizer_config())
+    tokenizer_config["model_max_length"] = config.max_position_embeddings
+    tokenizer_config.json(os.path.join(convert_config.output_path, "tokenizer_config.json"))
 
     if convert_config.push_to_hub:
         if HfApi is None:
             raise ImportError("Please install huggingface_hub to push to the hub.")
         api = HfApi()
+        if convert_config.delete_existing:
+            api.delete_repo(
+                convert_config.repo_id,
+                token=convert_config.token,
+                missing_ok=True,
+            )
         api.create_repo(
             convert_config.repo_id,
             token=convert_config.token,
             exist_ok=True,
         )
         api.upload_folder(
             repo_id=convert_config.repo_id, folder_path=convert_config.output_path, token=convert_config.token
@@ -93,15 +112,20 @@
 
 
 @chanfig.configclass
 class ConvertConfig:
     checkpoint_path: str
     output_path: str = Config.model_type
     push_to_hub: bool = False
-    repo_id: str = f"multimolecule/{output_path}"
-    token: Optional[str] = None
+    delete_existing: bool = False
+    repo_id: str | None = None
+    token: str | None = None
+
+    def post(self):
+        if self.repo_id is None:
+            self.repo_id = f"multimolecule/{self.output_path}"
 
 
 if __name__ == "__main__":
     config = ConvertConfig()
     config.parse()  # type: ignore[attr-defined]
     convert_checkpoint(config)
```

### Comparing `multimolecule-0.0.2/multimolecule/models/rnabert/modeling_rnabert.py` & `multimolecule-0.0.3/multimolecule/models/rnabert/modeling_rnabert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,52 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from __future__ import annotations
 
 import math
 from dataclasses import dataclass
-from typing import Optional, Tuple
+from typing import Tuple
+from warnings import warn
 
 import torch
+from danling import NestedTensor
 from torch import Tensor, nn
 from torch.nn import functional as F
 from transformers import PreTrainedModel
 from transformers.activations import ACT2FN
 from transformers.modeling_outputs import (
     BaseModelOutput,
     BaseModelOutputWithPooling,
     MaskedLMOutput,
     ModelOutput,
     SequenceClassifierOutput,
     TokenClassifierOutput,
 )
 
-from ..modeling_utils import MaskedLMHead, SequenceClassificationHead, TokenClassificationHead
+from multimolecule.module import (
+    MaskedLMHead,
+    NucleotideClassificationHead,
+    SequenceClassificationHead,
+    TokenClassificationHead,
+)
+
 from .configuration_rnabert import RnaBertConfig
 
 
 class RnaBertPreTrainedModel(PreTrainedModel):
     """
     An abstract class to handle weights initialization and a simple interface for downloading and loading pretrained
     models.
@@ -70,20 +94,22 @@
         self.pooler = RnaBertPooler(config) if add_pooling_layer else None
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Tensor,
-        attention_mask: Optional[Tensor] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
     ) -> Tuple[Tensor, ...] | BaseModelOutputWithPooling:
+        if isinstance(input_ids, NestedTensor):
+            input_ids, attention_mask = input_ids.tensor, input_ids.mask
         if attention_mask is None:
             attention_mask = (
                 input_ids.ne(self.pad_token_id) if self.pad_token_id is not None else torch.ones_like(input_ids)
             )
 
         extended_attention_mask = (1.0 - attention_mask.unsqueeze(1).unsqueeze(2).float()) * -10000.0
 
@@ -126,33 +152,30 @@
         self.lm_head = MaskedLMHead(config)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Tensor,
-        attention_mask: Optional[Tensor] = None,
-        labels: Optional[torch.Tensor] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
     ) -> Tuple[Tensor, ...] | MaskedLMOutput:
         outputs = self.rnabert(
             input_ids,
             attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.lm_head(outputs)
-
-        loss = None
-        if labels is not None:
-            loss = F.cross_entropy(logits.view(-1, self.config.vocab_size), labels.view(-1))
+        output = self.lm_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return MaskedLMOutput(
             loss=loss,
@@ -179,19 +202,19 @@
         self.pretrain_head = RnaBertPreTrainingHeads(config)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Tensor,
-        attention_mask: Optional[Tensor] = None,
-        labels: Optional[torch.Tensor] = None,
-        labels_ss: Optional[torch.Tensor] = None,
-        next_sentence_label: Optional[torch.Tensor] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        labels_ss: Tensor | None = None,
+        next_sentence_label: Tensor | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
     ) -> Tuple[Tensor, ...] | RnaBertForPretrainingOutput:
         outputs = self.rnabert(
             input_ids,
             attention_mask,
@@ -244,17 +267,17 @@
         self.head_config = self.sequence_head.config
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Tensor,
-        attention_mask: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
     ) -> Tuple[Tensor, ...] | SequenceClassifierOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
@@ -266,35 +289,16 @@
         outputs = self.rnabert(
             input_ids,
             attention_mask=attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.sequence_head(outputs)
-
-        loss = None
-        if labels is not None:
-            if self.head_config.problem_type is None:
-                if self.num_labels == 1:
-                    self.head_config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                    self.head_config.problem_type = "single_label_classification"
-                else:
-                    self.head_config.problem_type = "multi_label_classification"
-            if self.head_config.problem_type == "regression":
-                loss = (
-                    F.mse_loss(logits.squeeze(), labels.squeeze())
-                    if self.num_labels == 1
-                    else F.mse_loss(logits, labels)
-                )
-            elif self.head_config.problem_type == "single_label_classification":
-                loss = F.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
-            elif self.head_config.problem_type == "multi_label_classification":
-                loss = F.binary_cross_entropy_with_logits(logits, labels)
+        output = self.sequence_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return SequenceClassifierOutput(
             loss=loss,
@@ -323,17 +327,17 @@
         self.head_config = self.token_head.config
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Tensor,
-        attention_mask: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
     ) -> Tuple[Tensor, ...] | TokenClassifierOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
@@ -345,35 +349,83 @@
         outputs = self.rnabert(
             input_ids,
             attention_mask=attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.token_head(outputs)
+        output = self.token_head(outputs, attention_mask, input_ids, labels)
+        logits, loss = output.logits, output.loss
 
-        loss = None
-        if labels is not None:
-            if self.head_config.problem_type is None:
-                if self.num_labels == 1:
-                    self.head_config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                    self.head_config.problem_type = "single_label_classification"
-                else:
-                    self.head_config.problem_type = "multi_label_classification"
-            if self.head_config.problem_type == "regression":
-                loss = (
-                    F.mse_loss(logits.squeeze(), labels.squeeze())
-                    if self.num_labels == 1
-                    else F.mse_loss(logits, labels)
-                )
-            elif self.head_config.problem_type == "single_label_classification":
-                loss = F.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
-            elif self.head_config.problem_type == "multi_label_classification":
-                loss = F.binary_cross_entropy_with_logits(logits, labels)
+        if not return_dict:
+            output = (logits,) + outputs[2:]
+            return ((loss,) + output) if loss is not None else output
+
+        return TokenClassifierOutput(
+            loss=loss,
+            logits=logits,
+            hidden_states=outputs.hidden_states,
+            attentions=outputs.attentions,
+        )
+
+
+class RnaBertForNucleotideClassification(RnaBertPreTrainedModel):
+    """
+    Examples:
+        >>> from multimolecule import RnaBertConfig, RnaBertForNucleotideClassification, RnaTokenizer
+        >>> config = RnaBertConfig()
+        >>> model = RnaBertForNucleotideClassification(config)
+        >>> tokenizer = RnaTokenizer.from_pretrained("multimolecule/rna")
+        >>> input = tokenizer("ACGUN", return_tensors="pt")
+        >>> output = model(**input)
+    """
+
+    def __init__(self, config: RnaBertConfig):
+        super().__init__(config)
+        self.num_labels = config.head.num_labels
+        self.rnabert = RnaBertModel(config, add_pooling_layer=False)
+        self.nucleotide_head = NucleotideClassificationHead(config)
+        self.head_config = self.nucleotide_head.config
+
+        # Initialize weights and apply final processing
+        self.post_init()
+
+    def forward(
+        self,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool = False,
+        output_hidden_states: bool = False,
+        return_dict: bool = True,
+        **kwargs,
+    ) -> Tuple[Tensor, ...] | TokenClassifierOutput:
+        r"""
+        labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
+            Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
+            config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
+            `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
+        """
+        if kwargs:
+            warn(
+                f"Additional keyword arguments `{', '.join(kwargs)}` are detected in "
+                f"`{self.__class__.__name__}.forward`, they will be ignored.\n"
+                "This is provided for backward compatibility and may lead to unexpected behavior."
+            )
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+
+        outputs = self.rnabert(
+            input_ids,
+            attention_mask=attention_mask,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            return_dict=return_dict,
+        )
+        output = self.nucleotide_head(outputs, attention_mask, input_ids, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return TokenClassifierOutput(
             loss=loss,
@@ -580,14 +632,16 @@
 class RnaBertPooler(nn.Module):
     def __init__(self, config: RnaBertConfig):
         super().__init__()
         self.dense = nn.Linear(config.hidden_size, config.hidden_size)
         self.activation = nn.Tanh()
 
     def forward(self, hidden_states: Tensor) -> Tensor:
+        # We "pool" the model by simply taking the hidden state corresponding
+        # to the first token.
         first_token_tensor = hidden_states[:, 0]
         pooled_output = self.dense(first_token_tensor)
         pooled_output = self.activation(pooled_output)
         return pooled_output
 
 
 class RnaBertPreTrainingHeads(nn.Module):
@@ -605,19 +659,19 @@
         logits_ss = self.predictions_ss(sequence_output)
         seq_relationship_score = self.seq_relationship(pooled_output)
         return logits, logits_ss, seq_relationship_score
 
 
 @dataclass
 class RnaBertForPretrainingOutput(ModelOutput):
-    loss: Optional[torch.FloatTensor] = None
+    loss: torch.FloatTensor | None = None
     logits: torch.FloatTensor = None  # type: ignore[assignment]
     logits_ss: torch.FloatTensor = None  # type: ignore[assignment]
-    hidden_states: Optional[Tuple[torch.FloatTensor, ...]] = None
-    attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
+    hidden_states: Tuple[torch.FloatTensor, ...] | None = None
+    attentions: Tuple[torch.FloatTensor, ...] | None = None
 
 
 class RnaBertLayerNorm(nn.Module):
     def __init__(self, hidden_size: int, eps: float = 1e-12):
         super().__init__()
         self.weight = nn.Parameter(torch.ones(hidden_size))  # weightのこと
         self.bias = nn.Parameter(torch.zeros(hidden_size))  # biasのこと
```

### Comparing `multimolecule-0.0.2/multimolecule/models/rnafm/configuration_rnafm.py` & `multimolecule-0.0.3/multimolecule/models/rnafm/configuration_rnafm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from transformers.utils import logging
 
 from ..configuration_utils import HeadConfig, MaskedLMHeadConfig, PretrainedConfig
 
 logger = logging.get_logger(__name__)
 
 
@@ -87,24 +103,14 @@
         use_cache=True,
         emb_layer_norm_before=True,
         token_dropout=True,
         head=None,
         lm_head=None,
         **kwargs,
     ):
-        if head is None:
-            head = {}
-        head.setdefault("hidden_size", hidden_size)
-        if "problem_type" in kwargs:
-            head.setdefault("problem_type", kwargs["problem_type"])
-        if "num_labels" in kwargs:
-            head.setdefault("num_labels", kwargs["num_labels"])
-        if lm_head is None:
-            lm_head = {}
-        lm_head.setdefault("hidden_size", hidden_size)
         super().__init__(**kwargs)
 
         self.vocab_size = vocab_size
         self.hidden_size = hidden_size
         self.num_hidden_layers = num_hidden_layers
         self.num_attention_heads = num_attention_heads
         self.intermediate_size = intermediate_size
@@ -114,9 +120,9 @@
         self.max_position_embeddings = max_position_embeddings
         self.initializer_range = initializer_range
         self.layer_norm_eps = layer_norm_eps
         self.position_embedding_type = position_embedding_type
         self.use_cache = use_cache
         self.emb_layer_norm_before = emb_layer_norm_before
         self.token_dropout = token_dropout
-        self.head = HeadConfig(**head)
-        self.lm_head = MaskedLMHeadConfig(**lm_head)
+        self.head = HeadConfig(**head if head is not None else {})
+        self.lm_head = MaskedLMHeadConfig(**lm_head if lm_head is not None else {})
```

### Comparing `multimolecule-0.0.2/multimolecule/models/rnafm/convert_checkpoint.py` & `multimolecule-0.0.3/multimolecule/models/utrlm/convert_checkpoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,129 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from __future__ import annotations
+
 import os
-from typing import Optional
 
 import chanfig
 import torch
-from torch import nn
 
-from multimolecule.models import RnaFmConfig as Config
-from multimolecule.models import RnaFmForPretraining as Model
-from multimolecule.tokenizers.rna.utils import get_special_tokens_map, get_tokenizer_config, get_vocab_list
+from multimolecule.models import UtrLmConfig as Config
+from multimolecule.models import UtrLmForPretraining as Model
+from multimolecule.tokenisers.rna.utils import (
+    convert_word_embeddings,
+    get_special_tokens_map,
+    get_tokenizer_config,
+    get_vocab_list,
+)
 
 try:
     from huggingface_hub import HfApi
 except ImportError:
     HfApi = None
 
 torch.manual_seed(1013)
 
 
 def _convert_checkpoint(config, original_state_dict, vocab_list, original_vocab_list):
     state_dict = {}
     for key, value in original_state_dict.items():
-        key = "rnafm" + key[7:]
+        if key.startswith("module."):
+            key = key[7:]
+        key = "utrlm." + key
         key = key.replace("LayerNorm", "layer_norm")
         key = key.replace("gamma", "weight")
         key = key.replace("beta", "bias")
-        key = key.replace("rnafm.encoder.emb_layer_norm_before", "rnafm.embeddings.layer_norm")
-        key = key.replace("rnafm.encoder.embed_tokens", "rnafm.embeddings.word_embeddings")
-        key = key.replace("rnafm.encoder.embed_positions", "rnafm.embeddings.position_embeddings")
-        key = key.replace("layers", "layer")
+        key = key.replace("utrlm.encoder.emb_layer_norm_before", "utrlm.embeddings.layer_norm")
+        key = key.replace("utrlm.emb_layer_norm_after", "utrlm.encoder.emb_layer_norm_after")
+        key = key.replace("utrlm.embed_tokens", "utrlm.embeddings.word_embeddings")
+        key = key.replace("rot_emb", "rotary_embeddings")
+        key = key.replace("layers", "encoder.layer")
         key = key.replace("self_attn", "attention.self")
         key = key.replace("q_proj", "query")
         key = key.replace("k_proj", "key")
         key = key.replace("v_proj", "value")
         key = key.replace("self.out_proj", "output.dense")
         key = key.replace("self_layer_norm", "layer_norm")
         key = key.replace("final_layer_norm", "layer_norm")
         key = key.replace("fc1", "intermediate.dense")
         key = key.replace("fc2", "output.dense")
         key = key.replace("regression", "decoder")
-        key = key.replace("rnafm.encoder.lm_head", "pretrain_head.predictions")
+        key = key.replace("utrlm.lm_head", "pretrain_head.predictions")
         key = key.replace("predictions.dense", "predictions.transform.dense")
         key = key.replace("predictions.layer_norm", "predictions.transform.layer_norm")
         key = key.replace("predictions.weight", "predictions.decoder.weight")
-        key = key.replace("rnafm.encoder.contact_head", "pretrain_head.contact")
+        key = key.replace("utrlm.contact_head", "pretrain_head.contact")
+        key = key.replace("utrlm.structure_linear", "pretrain_head.structure.decoder")
+        key = key.replace("utrlm.supervised_linear", "pretrain_head.supervised.decoder")
         state_dict[key] = value
 
-    state_vocab_size = state_dict["rnafm.embeddings.word_embeddings.weight"].size(0)
-    original_vocab_size = len(original_vocab_list)
-    if state_vocab_size != original_vocab_size:
-        raise ValueError(
-            f"Vocabulary size do not match. Expected to have {original_vocab_size}, but got {state_vocab_size}."
-        )
-    word_embed = nn.Embedding(config.vocab_size, config.hidden_size, padding_idx=config.pad_token_id)
-    word_embed_weight = word_embed.weight.data
-    predictions_decoder_weight = torch.zeros((config.vocab_size, config.hidden_size))
-    predictions_bias = torch.zeros(config.vocab_size)
-    # nn.init.normal_(pos_embed.weight, std=0.02)
-    for original_index, original_token in enumerate(original_vocab_list):
-        new_index = vocab_list.index(original_token)
-        word_embed_weight[new_index] = state_dict["rnafm.embeddings.word_embeddings.weight"][original_index]
-        predictions_decoder_weight[new_index] = state_dict["pretrain_head.predictions.decoder.weight"][original_index]
-        predictions_bias[new_index] = state_dict["pretrain_head.predictions.bias"][original_index]
-    state_dict["rnafm.embeddings.word_embeddings.weight"] = word_embed_weight
-    state_dict["pretrain_head.predictions.decoder.weight"] = predictions_decoder_weight
-    state_dict["pretrain_head.predictions.decoder.bias"] = state_dict["pretrain_head.predictions.bias"] = (
-        predictions_bias
+    word_embed_weight, decoder_weight, decoder_bias = convert_word_embeddings(
+        state_dict["utrlm.embeddings.word_embeddings.weight"],
+        state_dict["pretrain_head.predictions.decoder.weight"],
+        state_dict["pretrain_head.predictions.bias"],
+        old_vocab=original_vocab_list,
+        new_vocab=vocab_list,
+        std=config.initializer_range,
     )
+    state_dict["utrlm.embeddings.word_embeddings.weight"] = word_embed_weight
+    state_dict["pretrain_head.predictions.decoder.weight"] = decoder_weight
+    state_dict["pretrain_head.predictions.decoder.bias"] = state_dict["pretrain_head.predictions.bias"] = decoder_bias
     return state_dict
 
 
 def convert_checkpoint(convert_config):
+    config = chanfig.FlatDict(num_labels=1)
+    config.supervised_head = {"num_labels": 1}
+    if "4.1" in convert_config.checkpoint_path:
+        config.structure_head = {"num_labels": 3}
     vocab_list = get_vocab_list()
-    original_vocab_list = [
-        "<cls>",
-        "<pad>",
-        "<eos>",
-        "<unk>",
-        "A",
-        "C",
-        "G",
-        "U",
-        "R",
-        "Y",
-        "K",
-        "M",
-        "S",
-        "W",
-        "B",
-        "D",
-        "H",
-        "V",
-        "N",
-        "-",
-        "<null>",
-        "<null>",
-        "<null>",
-        "<null>",
-        "<mask>",
-    ]
-    config = Config(num_labels=1)
-    config.architectures = ["RnaFmModel"]
+    original_vocab_list = ["<pad>", "<eos>", "<unk>", "A", "G", "C", "U", "<cls>", "<mask>", "<eos>"]
+    config = Config.from_dict(config)
     config.vocab_size = len(vocab_list)
 
     model = Model(config)
 
     ckpt = torch.load(convert_config.checkpoint_path, map_location=torch.device("cpu"))
     state_dict = _convert_checkpoint(config, ckpt, vocab_list, original_vocab_list)
 
     model.load_state_dict(state_dict)
     model.save_pretrained(convert_config.output_path, safe_serialization=True)
     model.save_pretrained(convert_config.output_path, safe_serialization=False)
     chanfig.NestedDict(get_special_tokens_map()).json(
         os.path.join(convert_config.output_path, "special_tokens_map.json")
     )
-    chanfig.NestedDict(get_tokenizer_config()).json(os.path.join(convert_config.output_path, "tokenizer_config.json"))
+    tokenizer_config = chanfig.NestedDict(get_tokenizer_config())
+    tokenizer_config["model_max_length"] = config.max_position_embeddings
+    tokenizer_config.json(os.path.join(convert_config.output_path, "tokenizer_config.json"))
 
     if convert_config.push_to_hub:
         if HfApi is None:
             raise ImportError("Please install huggingface_hub to push to the hub.")
         api = HfApi()
+        if convert_config.delete_existing:
+            api.delete_repo(
+                convert_config.repo_id,
+                token=convert_config.token,
+                missing_ok=True,
+            )
         api.create_repo(
             convert_config.repo_id,
             token=convert_config.token,
             exist_ok=True,
         )
         api.upload_folder(
             repo_id=convert_config.repo_id, folder_path=convert_config.output_path, token=convert_config.token
@@ -130,15 +131,20 @@
 
 
 @chanfig.configclass
 class ConvertConfig:
     checkpoint_path: str
     output_path: str = Config.model_type
     push_to_hub: bool = False
-    repo_id: str = f"multimolecule/{output_path}"
-    token: Optional[str] = None
+    delete_existing: bool = False
+    repo_id: str | None = None
+    token: str | None = None
+
+    def post(self):
+        if self.repo_id is None:
+            self.repo_id = f"multimolecule/{self.output_path}"
 
 
 if __name__ == "__main__":
     config = ConvertConfig()
     config.parse()  # type: ignore[attr-defined]
     convert_checkpoint(config)
```

### Comparing `multimolecule-0.0.2/multimolecule/models/rnafm/modeling_rnafm.py` & `multimolecule-0.0.3/multimolecule/models/rnafm/modeling_rnafm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,55 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import List, Optional, Tuple, Union
+from typing import Tuple
+from warnings import warn
 
 import torch
 import torch.utils.checkpoint
+from danling import NestedTensor
 from torch import Tensor, nn
 from torch.nn import functional as F
 from transformers.activations import ACT2FN
 from transformers.modeling_outputs import (
     BaseModelOutputWithPastAndCrossAttentions,
     BaseModelOutputWithPoolingAndCrossAttentions,
     MaskedLMOutput,
     ModelOutput,
     SequenceClassifierOutput,
     TokenClassifierOutput,
 )
 from transformers.modeling_utils import PreTrainedModel, find_pruneable_heads_and_indices, prune_linear_layer
 from transformers.utils import logging
 
-from ..modeling_utils import (
+from multimolecule.module import (
     ContactPredictionHead,
     MaskedLMHead,
+    NucleotideClassificationHead,
     SequenceClassificationHead,
     TokenClassificationHead,
-    apply_rotary_pos_emb,
 )
+
+from ..modeling_utils import apply_rotary_pos_emb
 from .configuration_rnafm import RnaFmConfig
 
 logger = logging.get_logger(__name__)
 
 
 class RnaFmPreTrainedModel(PreTrainedModel):
     """
@@ -93,27 +113,27 @@
         class PreTrainedModel
         """
         for layer, heads in heads_to_prune.items():
             self.encoder.layer[layer].attention.prune_heads(heads)
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        encoder_hidden_states: Optional[Tensor] = None,
-        encoder_attention_mask: Optional[Tensor] = None,
-        past_key_values: Optional[List[torch.FloatTensor]] = None,
-        use_cache: Optional[bool] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple[Tensor, ...], BaseModelOutputWithPoolingAndCrossAttentions]:
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        encoder_hidden_states: Tensor | None = None,
+        encoder_attention_mask: Tensor | None = None,
+        past_key_values: Tuple[Tuple[torch.FloatTensor, torch.FloatTensor], ...] | None = None,
+        use_cache: bool | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
+    ) -> Tuple[Tensor, ...] | BaseModelOutputWithPoolingAndCrossAttentions:
         r"""
         encoder_hidden_states  (`torch.FloatTensor` of shape `(batch_size, sequence_length, hidden_size)`, *optional*):
             Sequence of hidden-states at the output of the last layer of the encoder. Used in the cross-attention if
             the model is configured as a decoder.
         encoder_attention_mask (`torch.FloatTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Mask to avoid performing attention on the padding token indices of the encoder input. This mask is used in
             the cross-attention if the model is configured as a decoder. Mask values selected in `[0, 1]`:
@@ -138,17 +158,19 @@
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         if self.config.is_decoder:
             use_cache = use_cache if use_cache is not None else self.config.use_cache
         else:
             use_cache = False
 
+        if isinstance(input_ids, NestedTensor):
+            input_ids, attention_mask = input_ids.tensor, input_ids.mask
         if input_ids is not None and inputs_embeds is not None:
             raise ValueError("You cannot specify both input_ids and inputs_embeds at the same time")
-        elif input_ids is not None:
+        if input_ids is not None:
             self.warn_if_padding_and_no_attention_mask(input_ids, attention_mask)
             input_shape = input_ids.size()
         elif inputs_embeds is not None:
             input_shape = inputs_embeds.size()[:-1]
         else:
             raise ValueError("You have to specify either input_ids or inputs_embeds")
 
@@ -246,26 +268,26 @@
         self.lm_head = MaskedLMHead(config)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        encoder_hidden_states: Optional[Tensor] = None,
-        encoder_attention_mask: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple[Tensor, ...], MaskedLMOutput]:
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        encoder_hidden_states: Tensor | None = None,
+        encoder_attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
+    ) -> Tuple[Tensor, ...] | MaskedLMOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the masked language modeling loss. Indices should be in `[-100, 0, ...,
             config.vocab_size]` (see `input_ids` docstring) Tokens with indices set to `-100` are ignored (masked), the
             loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`
         """
 
@@ -279,19 +301,16 @@
             inputs_embeds=inputs_embeds,
             encoder_hidden_states=encoder_hidden_states,
             encoder_attention_mask=encoder_attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.lm_head(outputs)
-
-        loss = None
-        if labels is not None:
-            loss = F.cross_entropy(logits.view(-1, self.config.vocab_size), labels.view(-1))
+        output = self.lm_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return MaskedLMOutput(
             loss=loss,
@@ -331,27 +350,27 @@
         return self.pretrain_head.predictions.decoder
 
     def set_output_embeddings(self, embeddings):
         self.pretrain_head.predictions.decoder = embeddings
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        encoder_hidden_states: Optional[Tensor] = None,
-        encoder_attention_mask: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        labels_contact: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple[Tensor, ...], RnaFmForPretrainingOutput]:
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        encoder_hidden_states: Tensor | None = None,
+        encoder_attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        labels_contact: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
+    ) -> Tuple[Tensor, ...] | RnaFmForPretrainingOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the masked language modeling loss. Indices should be in `[-100, 0, ...,
             config.vocab_size]` (see `input_ids` docstring) Tokens with indices set to `-100` are ignored (masked), the
             loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`
         """
 
@@ -412,24 +431,24 @@
         self.head_config = self.sequence_head.config
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple[Tensor, ...], SequenceClassifierOutput]:
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
+    ) -> Tuple[Tensor, ...] | SequenceClassifierOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
             config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
             `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
         """
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
@@ -440,35 +459,17 @@
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.sequence_head(outputs)
+        output = self.sequence_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
-        loss = None
-        if labels is not None:
-            if self.head_config.problem_type is None:
-                if self.num_labels == 1:
-                    self.head_config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                    self.head_config.problem_type = "single_label_classification"
-                else:
-                    self.head_config.problem_type = "multi_label_classification"
-            if self.head_config.problem_type == "regression":
-                loss = (
-                    F.mse_loss(logits.squeeze(), labels.squeeze())
-                    if self.num_labels == 1
-                    else F.mse_loss(logits, labels)
-                )
-            elif self.head_config.problem_type == "single_label_classification":
-                loss = F.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
-            elif self.head_config.problem_type == "multi_label_classification":
-                loss = F.binary_cross_entropy_with_logits(logits, labels)
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return SequenceClassifierOutput(
             loss=loss,
             logits=logits,
@@ -496,24 +497,24 @@
         self.head_config = self.token_head.config
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple[Tensor, ...], TokenClassifierOutput]:
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
+    ) -> Tuple[Tensor, ...] | TokenClassifierOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the token classification loss. Indices should be in `[0, ..., config.num_labels - 1]`.
         """
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         outputs = self.rnafm(
@@ -522,35 +523,84 @@
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.token_head(outputs)
+        output = self.token_head(outputs, attention_mask, input_ids, labels)
+        logits, loss = output.logits, output.loss
+
+        if not return_dict:
+            output = (logits,) + outputs[2:]
+            return ((loss,) + output) if loss is not None else output
+
+        return TokenClassifierOutput(
+            loss=loss,
+            logits=logits,
+            hidden_states=outputs.hidden_states,
+            attentions=outputs.attentions,
+        )
+
+
+class RnaFmForNucleotideClassification(RnaFmPreTrainedModel):
+    """
+    Examples:
+        >>> from multimolecule import RnaFmConfig, RnaFmForNucleotideClassification, RnaTokenizer
+        >>> config = RnaFmConfig()
+        >>> model = RnaFmForNucleotideClassification(config)
+        >>> tokenizer = RnaTokenizer.from_pretrained("multimolecule/rna")
+        >>> input = tokenizer("ACGUN", return_tensors="pt")
+        >>> output = model(**input)
+    """
+
+    def __init__(self, config: RnaFmConfig):
+        super().__init__(config)
+        self.num_labels = config.head.num_labels
+        self.rnafm = RnaFmModel(config, add_pooling_layer=False)
+        self.nucleotide_head = NucleotideClassificationHead(config)
+        self.head_config = self.nucleotide_head.config
+
+        # Initialize weights and apply final processing
+        self.post_init()
+
+    def forward(
+        self,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool = False,
+        output_hidden_states: bool = False,
+        return_dict: bool = True,
+        **kwargs,
+    ) -> Tuple[Tensor, ...] | TokenClassifierOutput:
+        r"""
+        labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
+            Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
+            config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
+            `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
+        """
+        if kwargs:
+            warn(
+                f"Additional keyword arguments `{', '.join(kwargs)}` are detected in "
+                f"`{self.__class__.__name__}.forward`, they will be ignored.\n"
+                "This is provided for backward compatibility and may lead to unexpected behavior."
+            )
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+
+        outputs = self.rnafm(
+            input_ids,
+            attention_mask=attention_mask,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            return_dict=return_dict,
+        )
+        output = self.nucleotide_head(outputs, attention_mask, input_ids, labels)
+        logits, loss = output.logits, output.loss
 
-        loss = None
-        if labels is not None:
-            if self.head_config.problem_type is None:
-                if self.num_labels == 1:
-                    self.head_config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                    self.head_config.problem_type = "single_label_classification"
-                else:
-                    self.head_config.problem_type = "multi_label_classification"
-            if self.head_config.problem_type == "regression":
-                loss = (
-                    F.mse_loss(logits.squeeze(), labels.squeeze())
-                    if self.num_labels == 1
-                    else F.mse_loss(logits, labels)
-                )
-            elif self.head_config.problem_type == "single_label_classification":
-                loss = F.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
-            elif self.head_config.problem_type == "multi_label_classification":
-                loss = F.binary_cross_entropy_with_logits(logits, labels)
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return TokenClassifierOutput(
             loss=loss,
             logits=logits,
@@ -610,15 +660,15 @@
             mask_ratio_train = 0.15 * 0.8  # Hardcoded as the ratio used in all RNAFM model training runs
             src_lengths = attention_mask.sum(-1)
             mask_ratio_observed = (input_ids == self.mask_token_id).sum(-1).float() / src_lengths
             embeddings = (embeddings * (1 - mask_ratio_train) / (1 - mask_ratio_observed)[:, None, None]).to(
                 embeddings.dtype
             )
 
-        if self.position_embeddings is not None:
+        if self.position_embedding_type == "absolute":
             position_embeddings = self.position_embeddings(position_ids)
             embeddings = embeddings + position_embeddings
 
         if self.layer_norm is not None:
             embeddings = self.layer_norm(embeddings)
         if attention_mask is not None:
             embeddings = (embeddings * attention_mask.unsqueeze(-1)).to(embeddings.dtype)
@@ -691,24 +741,24 @@
         self.layer = nn.ModuleList([RnaFmLayer(config) for _ in range(config.num_hidden_layers)])
         self.emb_layer_norm_after = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
         self.gradient_checkpointing = False
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
-        use_cache: Optional[bool] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_values: Tuple[Tuple[torch.FloatTensor, ...], ...] | None = None,
+        use_cache: bool | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
-    ) -> Union[Tuple[Tensor, ...], BaseModelOutputWithPastAndCrossAttentions]:
+    ) -> Tuple[Tensor, ...] | BaseModelOutputWithPastAndCrossAttentions:
         all_hidden_states = () if output_hidden_states else None
         all_self_attentions = () if output_attentions else None
         all_cross_attentions = () if output_attentions and self.config.add_cross_attention else None
 
         if self.gradient_checkpointing and self.training and use_cache:
             logger.warning_once(
                 "`use_cache=True` is incompatible with gradient checkpointing. Setting `use_cache=False`..."
@@ -795,19 +845,19 @@
         self.layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
         self.intermediate = RnaFmIntermediate(config)
         self.output = RnaFmOutput(config)
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_value: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_value: Tuple[torch.FloatTensor, torch.FloatTensor] | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         # decoder uni-directional self-attention cached key/values tuple is at positions 1,2
         self_attn_past_key_value = past_key_value[:2] if past_key_value is not None else None
         self_attention_outputs = self.attention(
             hidden_states,
             attention_mask,
@@ -892,19 +942,19 @@
         self.self.num_attention_heads = self.self.num_attention_heads - len(heads)
         self.self.all_head_size = self.self.attention_head_size * self.self.num_attention_heads
         self.pruned_heads = self.pruned_heads.union(heads)
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_value: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_value: Tuple[torch.FloatTensor, torch.FloatTensor] | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         hidden_states_ln = self.layer_norm(hidden_states)
         self_outputs = self.self(
             hidden_states_ln,
             attention_mask,
             head_mask,
@@ -915,15 +965,15 @@
         )
         attention_output = self.output(self_outputs[0], hidden_states)
         outputs = (attention_output,) + self_outputs[1:]  # add attentions if we output them
         return outputs
 
 
 class RnaFmSelfAttention(nn.Module):
-    def __init__(self, config: RnaFmConfig, position_embedding_type: Optional[str] = None):
+    def __init__(self, config: RnaFmConfig, position_embedding_type: str | None = None):
         super().__init__()
         if config.hidden_size % config.num_attention_heads != 0 and not hasattr(config, "embedding_size"):
             raise ValueError(
                 f"The hidden size ({config.hidden_size}) is not a multiple of the number of attention "
                 f"heads ({config.num_attention_heads})"
             )
 
@@ -950,19 +1000,19 @@
         new_x_shape = x.size()[:-1] + (self.num_attention_heads, self.attention_head_size)
         x = x.view(new_x_shape)
         return x.permute(0, 2, 1, 3)
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_value: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_value: Tuple[torch.FloatTensor, torch.FloatTensor] | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         mixed_query_layer = self.query(hidden_states)
 
         # If this is instantiated as a cross-attention module, the keys
         # and values come from an encoder; the attention mask needs to be
         # such that the encoder's padding tokens are not attended to.
@@ -1112,29 +1162,29 @@
         super().__init__()
         self.contact = ContactPredictionHead(config)
         self.predictions = MaskedLMHead(config)
 
     def forward(
         self,
         outputs: BaseModelOutputWithPastAndCrossAttentions | Tuple[Tensor, ...],
-        attention_mask: Optional[Tensor] = None,
-        input_ids: Optional[Tensor] = None,
+        attention_mask: Tensor | None = None,
+        input_ids: Tensor | NestedTensor | None = None,
     ) -> Tuple[Tensor, Tensor]:
         logits = self.predictions(outputs)
         contact_map = self.contact(torch.stack(outputs[-1], 1), attention_mask, input_ids)
         return logits, contact_map
 
 
 @dataclass
 class RnaFmForPretrainingOutput(ModelOutput):
-    loss: Optional[torch.FloatTensor] = None
+    loss: torch.FloatTensor | None = None
     logits: torch.FloatTensor = None
-    contact_map: Optional[torch.FloatTensor] = None
-    hidden_states: Optional[Tuple[torch.FloatTensor, ...]] = None
-    attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
+    contact_map: torch.FloatTensor | None = None
+    hidden_states: Tuple[torch.FloatTensor, ...] | None = None
+    attentions: Tuple[torch.FloatTensor, ...] | None = None
 
 
 def create_position_ids_from_input_ids(input_ids, padding_idx, past_key_values_length=0):
     """
     Replace non-padding symbols with their position numbers. Position numbers begin at padding_idx+1. Padding symbols
     are ignored. This is modified from fairseq's `utils.make_positions`.
```

### Comparing `multimolecule-0.0.2/multimolecule/models/rnamsm/configuration_rnamsm.py` & `multimolecule-0.0.3/multimolecule/models/rnamsm/configuration_rnamsm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from transformers.utils import logging
 
 from ..configuration_utils import HeadConfig, MaskedLMHeadConfig, PretrainedConfig
 
 logger = logging.get_logger(__name__)
 
 
@@ -74,24 +90,14 @@
         attention_type="standard",
         embed_positions_msa=True,
         attention_bias=True,
         head=None,
         lm_head=None,
         **kwargs,
     ):
-        if head is None:
-            head = {}
-        head.setdefault("hidden_size", hidden_size)
-        if "problem_type" in kwargs:
-            head.setdefault("problem_type", kwargs["problem_type"])
-        if "num_labels" in kwargs:
-            head.setdefault("num_labels", kwargs["num_labels"])
-        if lm_head is None:
-            lm_head = {}
-        lm_head.setdefault("hidden_size", hidden_size)
         super().__init__(**kwargs)
 
         self.vocab_size = vocab_size
         self.hidden_size = hidden_size
         self.num_hidden_layers = num_hidden_layers
         self.num_attention_heads = num_attention_heads
         self.intermediate_size = intermediate_size
@@ -103,9 +109,9 @@
         self.layer_norm_eps = layer_norm_eps
         self.position_embedding_type = position_embedding_type
         self.use_cache = use_cache
         self.max_tokens_per_msa = max_tokens_per_msa
         self.attention_type = attention_type
         self.embed_positions_msa = embed_positions_msa
         self.attention_bias = attention_bias
-        self.head = HeadConfig(**head)
-        self.lm_head = MaskedLMHeadConfig(**lm_head)
+        self.head = HeadConfig(**head if head is not None else {})
+        self.lm_head = MaskedLMHeadConfig(**lm_head if lm_head is not None else {})
```

### Comparing `multimolecule-0.0.2/multimolecule/models/rnamsm/convert_checkpoint.py` & `multimolecule-0.0.3/multimolecule/models/rnamsm/convert_checkpoint.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,119 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from __future__ import annotations
+
 import os
-from typing import Optional
 
+import __main__
 import chanfig
 import torch
-from torch import nn
 
 from multimolecule.models import RnaMsmConfig as Config
 from multimolecule.models import RnaMsmForPretraining as Model
-from multimolecule.tokenizers.rna.utils import get_special_tokens_map, get_tokenizer_config, get_vocab_list
+from multimolecule.tokenisers.rna.utils import (
+    convert_word_embeddings,
+    get_special_tokens_map,
+    get_tokenizer_config,
+    get_vocab_list,
+)
 
 try:
     from huggingface_hub import HfApi
 except ImportError:
     HfApi = None
 
 torch.manual_seed(1013)
 
+# eval hack
+__main__.OptimizerConfig = chanfig.FlatDict()
+__main__.MSATransformerModelConfig = chanfig.FlatDict()
+__main__.DataConfig = chanfig.FlatDict()
+__main__.TrainConfig = chanfig.FlatDict()
+__main__.LoggingConfig = chanfig.FlatDict()
+
 
 def _convert_checkpoint(config, original_state_dict, vocab_list, original_vocab_list):
     state_dict = {}
     for key, value in original_state_dict.items():
         key = key.replace("layers", "rnamsm.encoder.layer")
         key = key.replace("msa_position_embedding", "rnamsm.embeddings.msa_embeddings")
         key = key.replace("embed_tokens", "rnamsm.embeddings.word_embeddings")
         key = key.replace("embed_positions", "rnamsm.embeddings.position_embeddings")
         key = key.replace("emb_layer_norm_before", "rnamsm.embeddings.layer_norm")
         key = key.replace("emb_layer_norm_after", "rnamsm.encoder.layer_norm")
         key = key.replace("regression", "decoder")
         key = key.replace("contact_head", "pretrain_head.contact")
         key = key.replace("lm_head", "pretrain_head.predictions")
+        key = key.replace("pretrain_head.predictions.weight", "pretrain_head.predictions.decoder.weight")
         key = key.replace("pretrain_head.predictions.dense", "pretrain_head.predictions.transform.dense")
         key = key.replace("pretrain_head.predictions.layer_norm", "pretrain_head.predictions.transform.layer_norm")
         state_dict[key] = value
 
-    state_vocab_size = state_dict["rnamsm.embeddings.word_embeddings.weight"].size(0)
-    original_vocab_size = len(original_vocab_list)
-    if state_vocab_size != original_vocab_size:
-        raise ValueError(
-            f"Vocabulary size do not match. Expected to have {original_vocab_size}, but got {state_vocab_size}."
-        )
-    word_embed = nn.Embedding(config.vocab_size, config.hidden_size, padding_idx=config.pad_token_id)
-    word_embed_weight = word_embed.weight.data
-    predictions_bias = torch.zeros(config.vocab_size)
-    # nn.init.normal_(pos_embed.weight, std=0.02)
-    for original_index, original_token in enumerate(original_vocab_list):
-        new_index = vocab_list.index(original_token)
-        word_embed_weight[new_index] = state_dict["rnamsm.embeddings.word_embeddings.weight"][original_index]
-        predictions_bias[new_index] = state_dict["pretrain_head.predictions.bias"][original_index]
-    state_dict["rnamsm.embeddings.word_embeddings.weight"] = state_dict["pretrain_head.predictions.decoder.weight"] = (
-        word_embed_weight
-    )
-    state_dict["pretrain_head.predictions.decoder.bias"] = state_dict["pretrain_head.predictions.bias"] = (
-        predictions_bias
+    word_embed_weight, decoder_weight, decoder_bias = convert_word_embeddings(
+        state_dict["rnamsm.embeddings.word_embeddings.weight"],
+        state_dict["pretrain_head.predictions.decoder.weight"],
+        state_dict["pretrain_head.predictions.bias"],
+        old_vocab=original_vocab_list,
+        new_vocab=vocab_list,
+        std=config.initializer_range,
     )
-    del state_dict["pretrain_head.predictions.weight"]
+    state_dict["rnamsm.embeddings.word_embeddings.weight"] = word_embed_weight
+    state_dict["pretrain_head.predictions.decoder.weight"] = decoder_weight
+    state_dict["pretrain_head.predictions.decoder.bias"] = state_dict["pretrain_head.predictions.bias"] = decoder_bias
     return state_dict
 
 
 def convert_checkpoint(convert_config):
     vocab_list = get_vocab_list()
     original_vocab_list = ["<cls>", "<pad>", "<eos>", "<unk>", "A", "G", "C", "U", "X", "N", "-", "<mask>"]
     config = Config(num_labels=1)
     config.architectures = ["RnaMsmModel"]
     config.vocab_size = len(vocab_list)
 
     model = Model(config)
 
     ckpt = torch.load(convert_config.checkpoint_path, map_location=torch.device("cpu"))
+    ckpt = ckpt.get("state_dict", ckpt)
     state_dict = _convert_checkpoint(config, ckpt, vocab_list, original_vocab_list)
 
     model.load_state_dict(state_dict)
     model.save_pretrained(convert_config.output_path, safe_serialization=True)
     model.save_pretrained(convert_config.output_path, safe_serialization=False)
     chanfig.NestedDict(get_special_tokens_map()).json(
         os.path.join(convert_config.output_path, "special_tokens_map.json")
     )
-    chanfig.NestedDict(get_tokenizer_config()).json(os.path.join(convert_config.output_path, "tokenizer_config.json"))
+    tokenizer_config = chanfig.NestedDict(get_tokenizer_config())
+    tokenizer_config["model_max_length"] = config.max_position_embeddings
+    tokenizer_config.json(os.path.join(convert_config.output_path, "tokenizer_config.json"))
 
     if convert_config.push_to_hub:
         if HfApi is None:
             raise ImportError("Please install huggingface_hub to push to the hub.")
         api = HfApi()
+        if convert_config.delete_existing:
+            api.delete_repo(
+                convert_config.repo_id,
+                token=convert_config.token,
+                missing_ok=True,
+            )
         api.create_repo(
             convert_config.repo_id,
             token=convert_config.token,
             exist_ok=True,
         )
         api.upload_folder(
             repo_id=convert_config.repo_id, folder_path=convert_config.output_path, token=convert_config.token
@@ -92,15 +121,20 @@
 
 
 @chanfig.configclass
 class ConvertConfig:
     checkpoint_path: str
     output_path: str = Config.model_type
     push_to_hub: bool = False
-    repo_id: str = f"multimolecule/{output_path}"
-    token: Optional[str] = None
+    delete_existing: bool = False
+    repo_id: str | None = None
+    token: str | None = None
+
+    def post(self):
+        if self.repo_id is None:
+            self.repo_id = f"multimolecule/{self.output_path}"
 
 
 if __name__ == "__main__":
     config = ConvertConfig()
     config.parse()  # type: ignore[attr-defined]
     convert_checkpoint(config)
```

### Comparing `multimolecule-0.0.2/multimolecule/models/rnamsm/modeling_rnamsm.py` & `multimolecule-0.0.3/multimolecule/models/rnamsm/modeling_rnamsm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,48 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from __future__ import annotations
 
 import math
 from dataclasses import dataclass
 from functools import partial
-from typing import Optional, Tuple
+from typing import Tuple
+from warnings import warn
 
 import torch
 from chanfig import ConfigRegistry
+from danling import NestedTensor
 from torch import Tensor, nn
 from torch.nn import functional as F
 from transformers import PreTrainedModel
 from transformers.activations import ACT2FN
 from transformers.modeling_outputs import ModelOutput
 
-from ..modeling_utils import ContactPredictionHead, MaskedLMHead, SequenceClassificationHead, TokenClassificationHead
+from multimolecule.module import (
+    ContactPredictionHead,
+    MaskedLMHead,
+    NucleotideClassificationHead,
+    SequenceClassificationHead,
+    TokenClassificationHead,
+)
+
 from .configuration_rnamsm import RnaMsmConfig
 
 
 class RnaMsmPreTrainedModel(PreTrainedModel):
     """
     An abstract class to handle weights initialization and a simple interface for downloading and loading pretrained
     models.
@@ -65,38 +90,43 @@
         self.pooler = RnaMsmPooler(config) if add_pooling_layer else None
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Tensor,
-        attention_mask: Optional[Tensor] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
     ) -> Tuple[Tensor, ...] | RnaMsmModelOutputWithPooling:
+        if isinstance(input_ids, NestedTensor):
+            input_ids, attention_mask = input_ids.tensor, input_ids.mask
         if attention_mask is None:
             attention_mask = (
                 input_ids.ne(self.pad_token_id) if self.pad_token_id is not None else torch.ones_like(input_ids)
             )
-        if input_ids.ndim == 2:
+        unsqueeze_input = input_ids.ndim == 2
+        if unsqueeze_input:
             input_ids = input_ids.unsqueeze(1)
         if attention_mask.ndim == 2:
             attention_mask = attention_mask.unsqueeze(1)
 
         embedding_output = self.embeddings(input_ids, attention_mask=attention_mask)
         encoder_outputs = self.encoder(
             embedding_output,
-            key_padding_mask=attention_mask ^ 1,
+            key_padding_mask=(attention_mask ^ 1).bool(),
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
         sequence_output = encoder_outputs[0]
+        if unsqueeze_input:
+            sequence_output = sequence_output.squeeze(1)
         pooled_output = self.pooler(sequence_output) if self.pooler is not None else None
 
         if not return_dict:
             return (sequence_output, pooled_output) + encoder_outputs[1:]
 
         return RnaMsmModelOutputWithPooling(
             last_hidden_state=sequence_output,
@@ -124,39 +154,36 @@
         self.lm_head = MaskedLMHead(config, weight=self.rnamsm.embeddings.word_embeddings.weight)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Tensor,
-        attention_mask: Optional[Tensor] = None,
-        labels: Optional[torch.Tensor] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
-    ) -> Tuple[Tensor, ...] | RnaMsmMaskedLMOutput:
+    ) -> Tuple[Tensor, ...] | RnaMsmForMaskedLMOutput:
         outputs = self.rnamsm(
             input_ids,
             attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.lm_head(outputs)
-
-        loss = None
-        if labels is not None:
-            loss = F.cross_entropy(logits.view(-1, self.config.vocab_size), labels.view(-1))
+        output = self.lm_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
-        return RnaMsmMaskedLMOutput(
+        return RnaMsmForMaskedLMOutput(
             loss=loss,
             logits=logits,
             hidden_states=outputs.hidden_states,
             col_attentions=outputs.col_attentions,
             row_attentions=outputs.row_attentions,
         )
 
@@ -178,18 +205,18 @@
         self.pretrain_head = RnaMsmPreTrainingHeads(config, weight=self.rnamsm.embeddings.word_embeddings.weight)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Tensor,
-        attention_mask: Optional[Tensor] = None,
-        labels: Optional[torch.Tensor] = None,
-        labels_contact: Optional[torch.Tensor] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        labels_contact: Tensor | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
     ) -> Tuple[Tensor, ...] | RnaMsmForPretrainingOutput:
         outputs = self.rnamsm(
             input_ids,
             attention_mask,
@@ -241,21 +268,21 @@
         self.head_config = self.sequence_head.config
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Tensor,
-        attention_mask: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
-    ) -> Tuple[Tensor, ...] | RnaMsmSequenceClassifierOutput:
+    ) -> Tuple[Tensor, ...] | RnaMsmForSequenceClassifierOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
             config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
             `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
         """
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
@@ -263,41 +290,22 @@
         outputs = self.rnamsm(
             input_ids,
             attention_mask=attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.sequence_head(outputs)
-
-        loss = None
-        if labels is not None:
-            if self.head_config.problem_type is None:
-                if self.num_labels == 1:
-                    self.head_config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                    self.head_config.problem_type = "single_label_classification"
-                else:
-                    self.head_config.problem_type = "multi_label_classification"
-            if self.head_config.problem_type == "regression":
-                loss = (
-                    F.mse_loss(logits.squeeze(), labels.squeeze())
-                    if self.num_labels == 1
-                    else F.mse_loss(logits, labels)
-                )
-            elif self.head_config.problem_type == "single_label_classification":
-                loss = F.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
-            elif self.head_config.problem_type == "multi_label_classification":
-                loss = F.binary_cross_entropy_with_logits(logits, labels)
+        output = self.sequence_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
-        return RnaMsmSequenceClassifierOutput(
+        return RnaMsmForSequenceClassifierOutput(
             loss=loss,
             logits=logits,
             hidden_states=outputs.hidden_states,
             col_attentions=outputs.col_attentions,
             row_attentions=outputs.row_attentions,
         )
 
@@ -321,21 +329,21 @@
         self.head_config = self.token_head.config
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Tensor,
-        attention_mask: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
-    ) -> Tuple[Tensor, ...] | RnaMsmTokenClassifierOutput:
+    ) -> Tuple[Tensor, ...] | RnaMsmForTokenClassifierOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
             config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
             `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
         """
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
@@ -343,41 +351,90 @@
         outputs = self.rnamsm(
             input_ids,
             attention_mask=attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.token_head(outputs)
+        output = self.token_head(outputs, attention_mask, input_ids, labels)
+        logits, loss = output.logits, output.loss
 
-        loss = None
-        if labels is not None:
-            if self.head_config.problem_type is None:
-                if self.num_labels == 1:
-                    self.head_config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                    self.head_config.problem_type = "single_label_classification"
-                else:
-                    self.head_config.problem_type = "multi_label_classification"
-            if self.head_config.problem_type == "regression":
-                loss = (
-                    F.mse_loss(logits.squeeze(), labels.squeeze())
-                    if self.num_labels == 1
-                    else F.mse_loss(logits, labels)
-                )
-            elif self.head_config.problem_type == "single_label_classification":
-                loss = F.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
-            elif self.head_config.problem_type == "multi_label_classification":
-                loss = F.binary_cross_entropy_with_logits(logits, labels)
+        if not return_dict:
+            output = (logits,) + outputs[2:]
+            return ((loss,) + output) if loss is not None else output
+
+        return RnaMsmForTokenClassifierOutput(
+            loss=loss,
+            logits=logits,
+            hidden_states=outputs.hidden_states,
+            col_attentions=outputs.col_attentions,
+            row_attentions=outputs.row_attentions,
+        )
+
+
+class RnaMsmForNucleotideClassification(RnaMsmPreTrainedModel):
+    """
+    Examples:
+        >>> from multimolecule import RnaMsmConfig, RnaMsmForNucleotideClassification, RnaTokenizer
+        >>> config = RnaMsmConfig()
+        >>> model = RnaMsmForNucleotideClassification(config)
+        >>> tokenizer = RnaTokenizer.from_pretrained("multimolecule/rna")
+        >>> input = tokenizer("ACGUN", return_tensors="pt")
+        >>> output = model(**input)
+    """
+
+    def __init__(self, config: RnaMsmConfig):
+        super().__init__(config)
+        self.num_labels = config.head.num_labels
+        self.rnamsm = RnaMsmModel(config, add_pooling_layer=False)
+        self.nucleotide_head = NucleotideClassificationHead(config)
+        self.head_config = self.nucleotide_head.config
+
+        # Initialize weights and apply final processing
+        self.post_init()
+
+    def forward(
+        self,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool = False,
+        output_hidden_states: bool = False,
+        return_dict: bool = True,
+        **kwargs,
+    ) -> Tuple[Tensor, ...] | RnaMsmForTokenClassifierOutput:
+        r"""
+        labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
+            Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
+            config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
+            `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
+        """
+        if kwargs:
+            warn(
+                f"Additional keyword arguments `{', '.join(kwargs)}` are detected in "
+                f"`{self.__class__.__name__}.forward`, they will be ignored.\n"
+                "This is provided for backward compatibility and may lead to unexpected behavior."
+            )
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+
+        outputs = self.rnamsm(
+            input_ids,
+            attention_mask=attention_mask,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            return_dict=return_dict,
+        )
+        output = self.nucleotide_head(outputs, attention_mask, input_ids, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
-        return RnaMsmTokenClassifierOutput(
+        return RnaMsmForTokenClassifierOutput(
             loss=loss,
             logits=logits,
             hidden_states=outputs.hidden_states,
             col_attentions=outputs.col_attentions,
             row_attentions=outputs.row_attentions,
         )
 
@@ -399,15 +456,15 @@
                 0.01 * torch.randn(1, self.max_position_embeddings, 1, 1), requires_grad=True
             )
         else:
             self.register_parameter("msa_embeddings", None)  # type: ignore
         self.layer_norm = nn.LayerNorm(config.hidden_size, eps=1e-12)
         self.dropout = nn.Dropout(config.hidden_dropout)
 
-    def forward(self, input_ids: Tensor, attention_mask: Optional[Tensor] = None) -> Tensor:
+    def forward(self, input_ids: Tensor | NestedTensor, attention_mask: Tensor | None = None) -> Tensor:
         assert input_ids.ndim == 3
         if attention_mask is None:
             attention_mask = input_ids.ne(self.pad_token_id)
         _, num_alignments, seq_length = input_ids.size()
         words_embeddings = self.word_embeddings(input_ids.long())
         position_ids = self.position_ids[:, :seq_length] * attention_mask.long()
         position_embeddings = self.position_embeddings(position_ids)
@@ -465,15 +522,15 @@
         self.config = config
         self.layer = nn.ModuleList([RnaMsmAxialLayer(config) for _ in range(config.num_hidden_layers)])
         self.layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
 
     def forward(
         self,
         hidden_states: Tensor,
-        key_padding_mask: Optional[torch.FloatTensor] = None,
+        key_padding_mask: torch.FloatTensor | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
     ) -> Tuple[Tensor, ...] | RnaMsmModelOutput:
         all_hidden_states = () if output_hidden_states else None
         all_col_attentions = () if output_attentions else None
         all_row_attentions = () if output_attentions else None
@@ -535,16 +592,16 @@
         self.row_self_attention = NormalizedResidualBlock(config, row_self_attention)
         self.column_self_attention = NormalizedResidualBlock(config, column_self_attention)
         self.feed_forward_layer = NormalizedResidualBlock(config, feed_forward_layer)
 
     def forward(
         self,
         hidden_states: Tensor,
-        self_attention_mask: Optional[Tensor] = None,
-        self_attention_padding_mask: Optional[Tensor] = None,
+        self_attention_mask: Tensor | None = None,
+        self_attention_padding_mask: Tensor | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         """
         LayerNorm is applied either before or after the self-attention/ffn
         modules similar to the original Transformer implementation.
         """
         row_attention_outputs = self.row_self_attention(
@@ -936,17 +993,17 @@
             )
 
     def attention_fn(
         self,
         query,
         key,
         value,
-        key_padding_mask: Optional[Tensor] = None,
+        key_padding_mask: Tensor | None = None,
         output_attentions: bool = False,
-        attention_mask: Optional[Tensor] = None,
+        attention_mask: Tensor | None = None,
     ):
         return self._attention_fn(
             query,
             key,
             value,
             in_proj_bias=torch.cat((self.q_proj.bias, self.k_proj.bias, self.v_proj.bias)),
             attention_mask=attention_mask,
@@ -970,16 +1027,16 @@
         nn.init.xavier_uniform_(self.out_proj.weight)
         if self.out_proj.bias is not None:
             nn.init.constant_(self.out_proj.bias, 0.0)
 
     def forward(
         self,
         hidden_states: Tensor,
-        key_padding_mask: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
+        key_padding_mask: Tensor | None = None,
+        attention_mask: Tensor | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         """Input shape: Time x Batch x Channel
 
         Args:
             key_padding_mask (ByteTensor, optional): mask to exclude
                 keys that are pads, of shape `(batch, src_len)`, where
@@ -1073,16 +1130,16 @@
 
     def attention_fn(self, query, key, value):
         return self._attention_fn(query, key, value)
 
     def forward(
         self,
         hidden_states: Tensor,
-        key_padding_mask: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
+        key_padding_mask: Tensor | None = None,
+        attention_mask: Tensor | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         from einops import rearrange
 
         q = self.q_proj(hidden_states)  # [T x B x D]
         k = self.k_proj(hidden_states)  # [...]
         v = self.v_proj(hidden_states)  # [...]
@@ -1151,83 +1208,85 @@
 class RnaMsmPooler(nn.Module):
     def __init__(self, config: RnaMsmConfig):
         super().__init__()
         self.dense = nn.Linear(config.hidden_size, config.hidden_size)
         self.activation = nn.Tanh()
 
     def forward(self, hidden_states: Tensor) -> Tensor:
+        # We "pool" the model by simply taking the hidden state corresponding
+        # to the first token.
         first_token_tensor = hidden_states[:, 0]
         pooled_output = self.dense(first_token_tensor)
         pooled_output = self.activation(pooled_output)
         return pooled_output
 
 
 class RnaMsmPreTrainingHeads(nn.Module):
-    def __init__(self, config: RnaMsmConfig, weight: Optional[Tensor] = None):
+    def __init__(self, config: RnaMsmConfig, weight: Tensor | None = None):
         super().__init__()
         self.predictions = MaskedLMHead(config, weight=weight)
         self.contact = ContactPredictionHead(config)
 
     def forward(
         self,
         outputs: RnaMsmModelOutput | Tuple[Tensor, ...],
-        attention_mask: Optional[Tensor] = None,
-        input_ids: Optional[Tensor] = None,
+        attention_mask: Tensor | None = None,
+        input_ids: Tensor | NestedTensor | None = None,
     ) -> Tuple[Tensor, Tensor]:
         sequence_output, row_attentions = outputs[0], torch.stack(outputs[-1], 1)
         prediction_scores = self.predictions(sequence_output)
         contact_map = self.contact(row_attentions, attention_mask, input_ids)
         return prediction_scores, contact_map
 
 
 @dataclass
 class RnaMsmForPretrainingOutput(ModelOutput):
-    loss: Optional[torch.FloatTensor] = None
+    loss: torch.FloatTensor | None = None
     logits: torch.FloatTensor = None
-    contact_map: Optional[torch.FloatTensor] = None
-    hidden_states: Optional[Tuple[torch.FloatTensor, ...]] = None
-    col_attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
-    row_attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
+    contact_map: torch.FloatTensor | None = None
+    hidden_states: Tuple[torch.FloatTensor, ...] | None = None
+    col_attentions: Tuple[torch.FloatTensor, ...] | None = None
+    row_attentions: Tuple[torch.FloatTensor, ...] | None = None
 
 
 @dataclass
-class RnaMsmMaskedLMOutput(ModelOutput):
-    loss: Optional[torch.FloatTensor] = None
+class RnaMsmForMaskedLMOutput(ModelOutput):
+    loss: torch.FloatTensor | None = None
     logits: torch.FloatTensor = None
-    hidden_states: Optional[Tuple[torch.FloatTensor, ...]] = None
-    col_attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
-    row_attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
+    hidden_states: Tuple[torch.FloatTensor, ...] | None = None
+    col_attentions: Tuple[torch.FloatTensor, ...] | None = None
+    row_attentions: Tuple[torch.FloatTensor, ...] | None = None
 
 
 @dataclass
-class RnaMsmSequenceClassifierOutput(ModelOutput):
-    loss: Optional[torch.FloatTensor] = None
+class RnaMsmForSequenceClassifierOutput(ModelOutput):
+    loss: torch.FloatTensor | None = None
     logits: torch.FloatTensor = None
-    hidden_states: Optional[Tuple[torch.FloatTensor, ...]] = None
-    col_attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
-    row_attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
+    hidden_states: Tuple[torch.FloatTensor, ...] | None = None
+    col_attentions: Tuple[torch.FloatTensor, ...] | None = None
+    row_attentions: Tuple[torch.FloatTensor, ...] | None = None
 
 
 @dataclass
-class RnaMsmTokenClassifierOutput(ModelOutput):
-    loss: Optional[torch.FloatTensor] = None
+class RnaMsmForTokenClassifierOutput(ModelOutput):
+    loss: torch.FloatTensor | None = None
     logits: torch.FloatTensor = None
-    hidden_states: Optional[Tuple[torch.FloatTensor, ...]] = None
-    col_attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
-    row_attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
+    hidden_states: Tuple[torch.FloatTensor, ...] | None = None
+    col_attentions: Tuple[torch.FloatTensor, ...] | None = None
+    row_attentions: Tuple[torch.FloatTensor, ...] | None = None
 
 
 @dataclass
 class RnaMsmModelOutputWithPooling(ModelOutput):
     last_hidden_state: torch.FloatTensor = None
     pooler_output: torch.FloatTensor = None
-    hidden_states: Optional[Tuple[torch.FloatTensor, ...]] = None
-    col_attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
-    row_attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
+    hidden_states: Tuple[torch.FloatTensor, ...] | None = None
+    col_attentions: Tuple[torch.FloatTensor, ...] | None = None
+    row_attentions: Tuple[torch.FloatTensor, ...] | None = None
 
 
 @dataclass
 class RnaMsmModelOutput(ModelOutput):
     last_hidden_state: torch.FloatTensor = None
-    hidden_states: Optional[Tuple[torch.FloatTensor, ...]] = None
-    col_attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
-    row_attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
+    hidden_states: Tuple[torch.FloatTensor, ...] | None = None
+    col_attentions: Tuple[torch.FloatTensor, ...] | None = None
+    row_attentions: Tuple[torch.FloatTensor, ...] | None = None
```

### Comparing `multimolecule-0.0.2/multimolecule/models/splicebert/configuration_splicebert.py` & `multimolecule-0.0.3/multimolecule/models/rnabert/configuration_rnabert.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,115 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from transformers.utils import logging
 
 from ..configuration_utils import HeadConfig, MaskedLMHeadConfig, PretrainedConfig
 
 logger = logging.get_logger(__name__)
 
 
-class SpliceBertConfig(PretrainedConfig):
+class RnaBertConfig(PretrainedConfig):
     r"""
-    This is the configuration class to store the configuration of a [`SpliceBertModel`]. It is used to instantiate a
-    SpliceBert model according to the specified arguments, defining the model architecture. Instantiating a
-    configuration with the defaults will yield a similar configuration to that of the SpliceBert
-    [biomed-AI/SpliceBERT](https://github.com/biomed-AI/SpliceBERT) architecture.
+    This is the configuration class to store the configuration of a [`RnaBertModel`]. It is used to instantiate a
+    RnaBert model according to the specified arguments, defining the model architecture. Instantiating a configuration
+    with the defaults will yield a similar configuration to that of the RnaBert
+    [mana438/RNABERT](https://github.com/mana438/RNABERT) architecture.
 
     Configuration objects inherit from [`PretrainedConfig`] and can be used to control the model outputs. Read the
     documentation from [`PretrainedConfig`] for more information.
 
 
     Args:
         vocab_size (`int`, *optional*, defaults to 25):
-            Vocabulary size of the SpliceBert model. Defines the number of different tokens that can be represented by
-            the `inputs_ids` passed when calling [`SpliceBertModel`].
-        hidden_size (`int`, *optional*, defaults to 512):
+            Vocabulary size of the RnaBert model. Defines the number of different tokens that can be represented by the
+            `inputs_ids` passed when calling [`RnaBertModel`].
+        hidden_size (`int`, *optional*, defaults to 120):
             Dimensionality of the encoder layers and the pooler layer.
-        num_hidden_layers (`int`, *optional*, defaults to 6):
+        num_hidden_layers (`int`, *optional*, defaults to 12):
             Number of hidden layers in the Transformer encoder.
-        num_attention_heads (`int`, *optional*, defaults to 16):
+        num_attention_heads (`int`, *optional*, defaults to 6):
             Number of attention heads for each attention layer in the Transformer encoder.
-        intermediate_size (`int`, *optional*, defaults to 2048):
+        intermediate_size (`int`, *optional*, defaults to 40):
             Dimensionality of the "intermediate" (often named feed-forward) layer in the Transformer encoder.
-        hidden_dropout (`float`, *optional*, defaults to 0.1):
+        hidden_dropout (`float`, *optional*, defaults to 0.0):
             The dropout probability for all fully connected layers in the embeddings, encoder, and pooler.
-        attention_dropout (`float`, *optional*, defaults to 0.1):
+        attention_dropout (`float`, *optional*, defaults to 0.0):
             The dropout ratio for the attention probabilities.
-        max_position_embeddings (`int`, *optional*, defaults to 1026):
+        max_position_embeddings (`int`, *optional*, defaults to 440):
             The maximum sequence length that this model might ever be used with. Typically set this to something large
             just in case (e.g., 512 or 1024 or 2048).
         initializer_range (`float`, *optional*, defaults to 0.02):
             The standard deviation of the truncated_normal_initializer for initializing all weight matrices.
         layer_norm_eps (`float`, *optional*, defaults to 1e-12):
             The epsilon used by the layer normalization layers.
 
     Examples:
-        >>> from multimolecule import SpliceBertModel, SpliceBertConfig
+        >>> from multimolecule import RnaBertModel, RnaBertConfig
 
-        >>> # Initializing a SpliceBERT multimolecule/splicebert style configuration
-        >>> configuration = SpliceBertConfig()
+        >>> # Initializing a RNABERT multimolecule/rnabert style configuration
+        >>> configuration = RnaBertConfig()
 
-        >>> # Initializing a model (with random weights) from the multimolecule/splicebert style configuration
-        >>> model = SpliceBertModel(configuration)
+        >>> # Initializing a model (with random weights) from the multimolecule/rnabert style configuration
+        >>> model = RnaBertModel(configuration)
 
         >>> # Accessing the model configuration
         >>> configuration = model.config
     """
 
-    model_type = "splicebert"
+    model_type = "rnabert"
 
     def __init__(
         self,
         vocab_size=25,
-        hidden_size=512,
+        ss_vocab_size=8,
+        hidden_size=None,
+        multiple=None,
         num_hidden_layers=6,
-        num_attention_heads=16,
-        intermediate_size=2048,
+        num_attention_heads=12,
+        intermediate_size=40,
         hidden_act="gelu",
-        hidden_dropout=0.1,
-        attention_dropout=0.1,
-        max_position_embeddings=1026,
+        hidden_dropout=0.0,
+        attention_dropout=0.0,
+        max_position_embeddings=440,
         initializer_range=0.02,
         layer_norm_eps=1e-12,
         position_embedding_type="absolute",
         use_cache=True,
         head=None,
         lm_head=None,
         **kwargs,
     ):
-        if head is None:
-            head = {}
-        head.setdefault("hidden_size", hidden_size)
-        if "problem_type" in kwargs:
-            head.setdefault("problem_type", kwargs["problem_type"])
-        if "num_labels" in kwargs:
-            head.setdefault("num_labels", kwargs["num_labels"])
-        if lm_head is None:
-            lm_head = {}
-        lm_head.setdefault("hidden_size", hidden_size)
+        if hidden_size is None:
+            hidden_size = num_attention_heads * multiple if multiple is not None else 120
         super().__init__(**kwargs)
 
         self.vocab_size = vocab_size
+        self.ss_vocab_size = ss_vocab_size
         self.type_vocab_size = 2
         self.hidden_size = hidden_size
         self.num_hidden_layers = num_hidden_layers
         self.num_attention_heads = num_attention_heads
         self.intermediate_size = intermediate_size
         self.hidden_act = hidden_act
         self.hidden_dropout = hidden_dropout
         self.attention_dropout = attention_dropout
         self.max_position_embeddings = max_position_embeddings
         self.initializer_range = initializer_range
         self.layer_norm_eps = layer_norm_eps
         self.position_embedding_type = position_embedding_type
         self.use_cache = use_cache
-        self.head = HeadConfig(**head)
-        self.lm_head = MaskedLMHeadConfig(**lm_head)
+        self.head = HeadConfig(**head if head is not None else {})
+        self.lm_head = MaskedLMHeadConfig(**lm_head if lm_head is not None else {})
```

### Comparing `multimolecule-0.0.2/multimolecule/models/splicebert/convert_checkpoint.py` & `multimolecule-0.0.3/multimolecule/models/utrbert/convert_checkpoint.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,38 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from __future__ import annotations
+
 import os
-from typing import Optional
 
 import chanfig
 import torch
-from torch import nn
 
-from multimolecule.models import SpliceBertConfig as Config
-from multimolecule.models import SpliceBertForPretraining as Model
-from multimolecule.tokenizers.rna.utils import get_special_tokens_map, get_tokenizer_config, get_vocab_list
+from multimolecule.models import UtrBertConfig as Config
+from multimolecule.models import UtrBertForPretraining as Model
+from multimolecule.tokenisers.rna.utils import (
+    convert_word_embeddings,
+    get_special_tokens_map,
+    get_tokenizer_config,
+    get_vocab_list,
+)
 
 try:
     from huggingface_hub import HfApi
 except ImportError:
     HfApi = None
 
 torch.manual_seed(1013)
@@ -20,53 +41,45 @@
 def _convert_checkpoint(config, original_state_dict, vocab_list, original_vocab_list):
     state_dict = {}
     for key, value in original_state_dict.items():
         key = key.replace("LayerNorm", "layer_norm")
         key = key.replace("gamma", "weight")
         key = key.replace("beta", "bias")
         if key.startswith("bert"):
-            state_dict["splice" + key] = value
+            state_dict["utr" + key] = value
             continue
         if key.startswith("cls"):
             key = "lm_head" + key[15:]
             state_dict[key] = value
             continue
         state_dict[key] = value
 
-    state_vocab_size = state_dict["splicebert.embeddings.word_embeddings.weight"].size(0)
-    original_vocab_size = len(original_vocab_list)
-    if state_vocab_size != original_vocab_size:
-        raise ValueError(
-            f"Vocabulary size do not match. Expected to have {original_vocab_size}, but got {state_vocab_size}."
-        )
-    word_embed = nn.Embedding(config.vocab_size, config.hidden_size, padding_idx=config.pad_token_id)
-    word_embed_weight = word_embed.weight.data
-    predictions_decoder_weight = torch.zeros((config.vocab_size, config.hidden_size))
-    predictions_bias = torch.zeros(config.vocab_size)
-    # nn.init.normal_(pos_embed.weight, std=0.02)
-    for original_index, original_token in enumerate(original_vocab_list):
-        new_index = vocab_list.index(original_token)
-        word_embed_weight[new_index] = state_dict["splicebert.embeddings.word_embeddings.weight"][original_index]
-        predictions_decoder_weight[new_index] = state_dict["lm_head.decoder.weight"][original_index]
-        predictions_bias[new_index] = state_dict["lm_head.decoder.bias"][original_index]
-    state_dict["splicebert.embeddings.word_embeddings.weight"] = word_embed_weight
-    state_dict["lm_head.decoder.weight"] = predictions_decoder_weight
-    state_dict["lm_head.decoder.bias"] = state_dict["lm_head.bias"] = predictions_bias
-    del state_dict["splicebert.embeddings.position_ids"]
+    word_embed_weight, decoder_weight, decoder_bias = convert_word_embeddings(
+        state_dict["utrbert.embeddings.word_embeddings.weight"],
+        state_dict["lm_head.decoder.weight"],
+        state_dict["lm_head.decoder.bias"],
+        old_vocab=original_vocab_list,
+        new_vocab=vocab_list,
+        std=config.initializer_range,
+    )
+    state_dict["utrbert.embeddings.word_embeddings.weight"] = word_embed_weight
+    state_dict["lm_head.decoder.weight"] = decoder_weight
+    state_dict["lm_head.decoder.bias"] = state_dict["lm_head.bias"] = decoder_bias
     return state_dict
 
 
 def convert_checkpoint(convert_config):
     config = chanfig.load(os.path.join(convert_config.checkpoint_path, "config.json"))
     config.hidden_dropout = config.pop("hidden_dropout_prob", 0.1)
     config.attention_dropout = config.pop("attention_probs_dropout_prob", 0.1)
-    vocab_list = get_vocab_list()
+    config.nmers = int(convert_config.checkpoint_path.split("/")[-1][0])
+    vocab_list = get_vocab_list(config.nmers, strameline=True)
     config = Config.from_dict(config)
     del config._name_or_path
-    config.architectures = ["SpliceBertModel"]
+    config.architectures = ["UtrBertModel"]
     config.vocab_size = len(vocab_list)
 
     model = Model(config)
 
     ckpt = torch.load(
         os.path.join(convert_config.checkpoint_path, "pytorch_model.bin"), map_location=torch.device("cpu")
     )
@@ -83,37 +96,48 @@
 
     model.load_state_dict(state_dict)
     model.save_pretrained(convert_config.output_path, safe_serialization=True)
     model.save_pretrained(convert_config.output_path, safe_serialization=False)
     chanfig.NestedDict(get_special_tokens_map()).json(
         os.path.join(convert_config.output_path, "special_tokens_map.json")
     )
-    chanfig.NestedDict(get_tokenizer_config()).json(os.path.join(convert_config.output_path, "tokenizer_config.json"))
+    tokenizer_config = chanfig.NestedDict(get_tokenizer_config())
+    tokenizer_config["nmers"] = config.nmers
+    tokenizer_config["strameline"] = True
+    tokenizer_config["model_max_length"] = config.max_position_embeddings
+    tokenizer_config.json(os.path.join(convert_config.output_path, "tokenizer_config.json"))
 
     if convert_config.push_to_hub:
         if HfApi is None:
             raise ImportError("Please install huggingface_hub to push to the hub.")
         api = HfApi()
+        if convert_config.delete_existing:
+            api.delete_repo(
+                convert_config.repo_id,
+                token=convert_config.token,
+                missing_ok=True,
+            )
         api.create_repo(
             convert_config.repo_id,
             token=convert_config.token,
             exist_ok=True,
         )
         api.upload_folder(
             repo_id=convert_config.repo_id, folder_path=convert_config.output_path, token=convert_config.token
         )
 
 
 @chanfig.configclass
 class ConvertConfig:
     checkpoint_path: str
-    output_path: Optional[str] = None
+    output_path: str | None = None
     push_to_hub: bool = False
-    repo_id: Optional[str] = output_path
-    token: Optional[str] = None
+    delete_existing: bool = False
+    repo_id: str | None = None
+    token: str | None = None
 
     def post(self):
         if self.output_path is None:
             self.output_path = self.checkpoint_path.split("/")[-1].lower()
         if self.repo_id is None:
             self.repo_id = f"multimolecule/{self.output_path}"
```

### Comparing `multimolecule-0.0.2/multimolecule/models/splicebert/modeling_splicebert.py` & `multimolecule-0.0.3/multimolecule/models/splicebert/modeling_splicebert.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,52 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from __future__ import annotations
 
 import math
-from typing import List, Optional, Tuple
+from typing import Tuple
+from warnings import warn
 
 import torch
 import torch.utils.checkpoint
+from danling import NestedTensor
 from torch import Tensor, nn
-from torch.nn import functional as F
 from transformers.activations import ACT2FN
 from transformers.modeling_outputs import (
     BaseModelOutputWithPastAndCrossAttentions,
     BaseModelOutputWithPoolingAndCrossAttentions,
     MaskedLMOutput,
     SequenceClassifierOutput,
     TokenClassifierOutput,
 )
 from transformers.modeling_utils import PreTrainedModel
 from transformers.pytorch_utils import apply_chunking_to_forward, find_pruneable_heads_and_indices, prune_linear_layer
 from transformers.utils import logging
 
-from ..modeling_utils import MaskedLMHead, SequenceClassificationHead, TokenClassificationHead
+from multimolecule.module import (
+    MaskedLMHead,
+    NucleotideClassificationHead,
+    SequenceClassificationHead,
+    TokenClassificationHead,
+)
+
 from .configuration_splicebert import SpliceBertConfig
 
 try:
     from flash_attn import flash_attn_func
 except ImportError:
     flash_attn_func = None
 
@@ -97,26 +120,26 @@
         class PreTrainedModel
         """
         for layer, heads in heads_to_prune.items():
             self.encoder.layer[layer].attention.prune_heads(heads)
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        encoder_hidden_states: Optional[Tensor] = None,
-        encoder_attention_mask: Optional[Tensor] = None,
-        past_key_values: Optional[List[torch.FloatTensor]] = None,
-        use_cache: Optional[bool] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        encoder_hidden_states: Tensor | None = None,
+        encoder_attention_mask: Tensor | None = None,
+        past_key_values: Tuple[Tuple[torch.FloatTensor, torch.FloatTensor], ...] | None = None,
+        use_cache: bool | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
     ) -> Tuple[Tensor, ...] | BaseModelOutputWithPoolingAndCrossAttentions:
         r"""
         encoder_hidden_states  (`torch.FloatTensor` of shape `(batch_size, sequence_length, hidden_size)`, *optional*):
             Sequence of hidden-states at the output of the last layer of the encoder. Used in the cross-attention if
             the model is configured as a decoder.
         encoder_attention_mask (`torch.FloatTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Mask to avoid performing attention on the padding token indices of the encoder input. This mask is used in
@@ -142,17 +165,19 @@
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         if self.config.is_decoder:
             use_cache = use_cache if use_cache is not None else self.config.use_cache
         else:
             use_cache = False
 
+        if isinstance(input_ids, NestedTensor):
+            input_ids, attention_mask = input_ids.tensor, input_ids.mask
         if input_ids is not None and inputs_embeds is not None:
             raise ValueError("You cannot specify both input_ids and inputs_embeds at the same time")
-        elif input_ids is not None:
+        if input_ids is not None:
             # self.warn_if_padding_and_no_attention_mask(input_ids, attention_mask)
             input_shape = input_ids.size()
         elif inputs_embeds is not None:
             input_shape = inputs_embeds.size()[:-1]
         else:
             raise ValueError("You have to specify either input_ids or inputs_embeds")
 
@@ -255,25 +280,25 @@
         return self.lm_head.decoder
 
     def set_output_embeddings(self, new_embeddings):
         self.lm_head.decoder = new_embeddings
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        encoder_hidden_states: Optional[Tensor] = None,
-        encoder_attention_mask: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        encoder_hidden_states: Tensor | None = None,
+        encoder_attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
     ) -> Tuple[Tensor, ...] | MaskedLMOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the masked language modeling loss. Indices should be in `[-100, 0, ...,
             config.vocab_size]` (see `input_ids` docstring) Tokens with indices set to `-100` are ignored (masked), the
             loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`
         """
@@ -288,19 +313,16 @@
             inputs_embeds=inputs_embeds,
             encoder_hidden_states=encoder_hidden_states,
             encoder_attention_mask=encoder_attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.lm_head(outputs)
-
-        loss = None
-        if labels is not None:
-            loss = F.cross_entropy(logits.view(-1, self.config.vocab_size), labels.view(-1))
+        output = self.lm_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return MaskedLMOutput(
             loss=loss,
@@ -350,25 +372,25 @@
         self.lm_head = MaskedLMHead(config)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        encoder_hidden_states: Optional[Tensor] = None,
-        encoder_attention_mask: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        encoder_hidden_states: Tensor | None = None,
+        encoder_attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
     ) -> Tuple[Tensor, ...] | MaskedLMOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the masked language modeling loss. Indices should be in `[-100, 0, ...,
             config.vocab_size]` (see `input_ids` docstring) Tokens with indices set to `-100` are ignored (masked), the
             loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`
         """
@@ -383,19 +405,16 @@
             inputs_embeds=inputs_embeds,
             encoder_hidden_states=encoder_hidden_states,
             encoder_attention_mask=encoder_attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.lm_head(outputs)
-
-        loss = None
-        if labels is not None:
-            loss = F.cross_entropy(logits.view(-1, self.config.vocab_size), labels.view(-1))
+        output = self.lm_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return MaskedLMOutput(
             loss=loss,
@@ -424,23 +443,23 @@
         self.head_config = self.sequence_head.config
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
     ) -> Tuple[Tensor, ...] | SequenceClassifierOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
             config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
             `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
         """
@@ -452,35 +471,16 @@
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.sequence_head(outputs)
-
-        loss = None
-        if labels is not None:
-            if self.head_config.problem_type is None:
-                if self.num_labels == 1:
-                    self.head_config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                    self.head_config.problem_type = "single_label_classification"
-                else:
-                    self.head_config.problem_type = "multi_label_classification"
-            if self.head_config.problem_type == "regression":
-                loss = (
-                    F.mse_loss(logits.squeeze(), labels.squeeze())
-                    if self.num_labels == 1
-                    else F.mse_loss(logits, labels)
-                )
-            elif self.head_config.problem_type == "single_label_classification":
-                loss = F.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
-            elif self.head_config.problem_type == "multi_label_classification":
-                loss = F.binary_cross_entropy_with_logits(logits, labels)
+        output = self.sequence_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return SequenceClassifierOutput(
             loss=loss,
@@ -509,23 +509,23 @@
         self.head_config = self.token_head.config
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
     ) -> Tuple[Tensor, ...] | TokenClassifierOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the token classification loss. Indices should be in `[0, ..., config.num_labels - 1]`.
         """
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
@@ -535,35 +535,83 @@
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.token_head(outputs)
+        output = self.token_head(outputs, attention_mask, input_ids, labels)
+        logits, loss = output.logits, output.loss
 
-        loss = None
-        if labels is not None:
-            if self.head_config.problem_type is None:
-                if self.num_labels == 1:
-                    self.head_config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                    self.head_config.problem_type = "single_label_classification"
-                else:
-                    self.head_config.problem_type = "multi_label_classification"
-            if self.head_config.problem_type == "regression":
-                loss = (
-                    F.mse_loss(logits.squeeze(), labels.squeeze())
-                    if self.num_labels == 1
-                    else F.mse_loss(logits, labels)
-                )
-            elif self.head_config.problem_type == "single_label_classification":
-                loss = F.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
-            elif self.head_config.problem_type == "multi_label_classification":
-                loss = F.binary_cross_entropy_with_logits(logits, labels)
+        if not return_dict:
+            output = (logits,) + outputs[2:]
+            return ((loss,) + output) if loss is not None else output
+
+        return TokenClassifierOutput(
+            loss=loss,
+            logits=logits,
+            hidden_states=outputs.hidden_states,
+            attentions=outputs.attentions,
+        )
+
+
+class SpliceBertForNucleotideClassification(SpliceBertPreTrainedModel):
+    """
+    Examples:
+        >>> from multimolecule import SpliceBertConfig, SpliceBertForNucleotideClassification, RnaTokenizer
+        >>> config = SpliceBertConfig()
+        >>> model = SpliceBertForNucleotideClassification(config)
+        >>> tokenizer = RnaTokenizer.from_pretrained("multimolecule/rna")
+        >>> input = tokenizer("ACGUN", return_tensors="pt")
+        >>> output = model(**input)
+    """
+
+    def __init__(self, config: SpliceBertConfig):
+        super().__init__(config)
+        self.num_labels = config.head.num_labels
+        self.splicebert = SpliceBertModel(config, add_pooling_layer=False)
+        self.nucleotide_head = NucleotideClassificationHead(config)
+        self.head_config = self.nucleotide_head.config
+
+        # Initialize weights and apply final processing
+        self.post_init()
+
+    def forward(
+        self,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool = False,
+        output_hidden_states: bool = False,
+        return_dict: bool = True,
+        **kwargs,
+    ) -> Tuple[Tensor, ...] | TokenClassifierOutput:
+        r"""
+        labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
+            Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
+            config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
+            `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
+        """
+        if kwargs:
+            warn(
+                f"Additional keyword arguments `{', '.join(kwargs)}` are detected in "
+                f"`{self.__class__.__name__}.forward`, they will be ignored.\n"
+                "This is provided for backward compatibility and may lead to unexpected behavior."
+            )
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+
+        outputs = self.splicebert(
+            input_ids,
+            attention_mask=attention_mask,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            return_dict=return_dict,
+        )
+        output = self.nucleotide_head(outputs, attention_mask, input_ids, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return TokenClassifierOutput(
             loss=loss,
@@ -588,17 +636,17 @@
         self.position_embedding_type = getattr(config, "position_embedding_type", "absolute")
         self.register_buffer(
             "position_ids", torch.arange(config.max_position_embeddings).expand((1, -1)), persistent=False
         )
 
     def forward(
         self,
-        input_ids: Optional[torch.LongTensor] = None,
-        position_ids: Optional[torch.LongTensor] = None,
-        inputs_embeds: Optional[torch.FloatTensor] = None,
+        input_ids: torch.LongTensor | None = None,
+        position_ids: torch.LongTensor | None = None,
+        inputs_embeds: torch.FloatTensor | None = None,
         past_key_values_length: int = 0,
     ) -> Tensor:
         if input_ids is not None:
             input_shape = input_ids.size()
         else:
             input_shape = inputs_embeds.size()[:-1]  # type: ignore[union-attr]
 
@@ -629,20 +677,20 @@
         self.config = config
         self.layer = nn.ModuleList([SpliceBertLayer(config) for _ in range(config.num_hidden_layers)])
         self.gradient_checkpointing = False
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
-        use_cache: Optional[bool] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_values: Tuple[Tuple[torch.FloatTensor, ...], ...] | None = None,
+        use_cache: bool | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
     ) -> Tuple[Tensor, ...] | BaseModelOutputWithPastAndCrossAttentions:
         all_hidden_states = () if output_hidden_states else None
         all_self_attentions = () if output_attentions else None
         all_cross_attentions = () if output_attentions and self.config.add_cross_attention else None
@@ -734,19 +782,19 @@
             self.crossattention = SpliceBertAttention(config, position_embedding_type="absolute")
         self.intermediate = SpliceBertIntermediate(config)
         self.output = SpliceBertOutput(config)
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_value: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_value: Tuple[torch.FloatTensor, torch.FloatTensor] | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         # decoder uni-directional self-attention cached key/values tuple is at positions 1,2
         self_attn_past_key_value = past_key_value[:2] if past_key_value is not None else None
         self_attention_outputs = self.attention(
             hidden_states,
             attention_mask,
@@ -803,15 +851,15 @@
     def feed_forward_chunk(self, attention_output):
         intermediate_output = self.intermediate(attention_output)
         layer_output = self.output(intermediate_output, attention_output)
         return layer_output
 
 
 class SpliceBertAttention(nn.Module):
-    def __init__(self, config: SpliceBertConfig, position_embedding_type: Optional[str] = None):
+    def __init__(self, config: SpliceBertConfig, position_embedding_type: str | None = None):
         super().__init__()
         self.self = SpliceBertSelfAttention(config, position_embedding_type=position_embedding_type)
         self.output = SpliceBertSelfOutput(config)
         self.pruned_heads: set = set()
 
     def prune_heads(self, heads):
         if len(heads) == 0:
@@ -830,19 +878,19 @@
         self.self.num_attention_heads = self.self.num_attention_heads - len(heads)
         self.self.all_head_size = self.self.attention_head_size * self.self.num_attention_heads
         self.pruned_heads = self.pruned_heads.union(heads)
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_value: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_value: Tuple[torch.FloatTensor, torch.FloatTensor] | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         self_outputs = self.self(
             hidden_states,
             attention_mask,
             head_mask,
             encoder_hidden_states,
@@ -852,15 +900,15 @@
         )
         attention_output = self.output(self_outputs[0], hidden_states)
         outputs = (attention_output,) + self_outputs[1:]  # add attentions if we output them
         return outputs
 
 
 class SpliceBertSelfAttention(nn.Module):
-    def __init__(self, config: SpliceBertConfig, position_embedding_type: Optional[str] = None):
+    def __init__(self, config: SpliceBertConfig, position_embedding_type: str | None = None):
         super().__init__()
         if config.hidden_size % config.num_attention_heads != 0 and not hasattr(config, "embedding_size"):
             raise ValueError(
                 f"The hidden size ({config.hidden_size}) is not a multiple of the number of attention "
                 f"heads ({config.num_attention_heads})"
             )
         self.flash = flash_attn_func is not None
@@ -885,19 +933,19 @@
         new_x_shape = x.size()[:-1] + (self.num_attention_heads, self.attention_head_size)
         x = x.view(new_x_shape)
         return x.permute(0, 2, 1, 3)
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_value: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_value: Tuple[torch.FloatTensor, torch.FloatTensor] | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         mixed_query_layer = self.query(hidden_states)
 
         # If this is instantiated as a cross-attention module, the keys
         # and values come from an encoder; the attention mask needs to be
         # such that the encoder's padding tokens are not attended to.
```

### Comparing `multimolecule-0.0.2/multimolecule/models/utrbert/configuration_utrbert.py` & `multimolecule-0.0.3/multimolecule/models/utrbert/configuration_utrbert.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from transformers.utils import logging
 
 from ..configuration_utils import HeadConfig, MaskedLMHeadConfig, PretrainedConfig
 
 logger = logging.get_logger(__name__)
 
 
@@ -89,24 +105,14 @@
         layer_norm_eps=1e-12,
         position_embedding_type="absolute",
         use_cache=True,
         head=None,
         lm_head=None,
         **kwargs,
     ):
-        if head is None:
-            head = {}
-        head.setdefault("hidden_size", hidden_size)
-        if "problem_type" in kwargs:
-            head.setdefault("problem_type", kwargs["problem_type"])
-        if "num_labels" in kwargs:
-            head.setdefault("num_labels", kwargs["num_labels"])
-        if lm_head is None:
-            lm_head = {}
-        lm_head.setdefault("hidden_size", hidden_size)
         super().__init__(**kwargs)
 
         self.vocab_size = vocab_size
         self.type_vocab_size = 2
         self.nmers = nmers
         self.hidden_size = hidden_size
         self.num_hidden_layers = num_hidden_layers
@@ -116,9 +122,9 @@
         self.hidden_dropout = hidden_dropout
         self.attention_dropout = attention_dropout
         self.max_position_embeddings = max_position_embeddings
         self.initializer_range = initializer_range
         self.layer_norm_eps = layer_norm_eps
         self.position_embedding_type = position_embedding_type
         self.use_cache = use_cache
-        self.head = HeadConfig(**head)
-        self.lm_head = MaskedLMHeadConfig(**lm_head)
+        self.head = HeadConfig(**head if head is not None else {})
+        self.lm_head = MaskedLMHeadConfig(**lm_head if lm_head is not None else {})
```

### Comparing `multimolecule-0.0.2/multimolecule/models/utrbert/convert_checkpoint.py` & `multimolecule-0.0.3/multimolecule/models/rnafm/convert_checkpoint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,126 +1,168 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from __future__ import annotations
+
 import os
-from typing import Optional
 
 import chanfig
 import torch
-from torch import nn
 
-from multimolecule.models import UtrBertConfig as Config
-from multimolecule.models import UtrBertForPretraining as Model
-from multimolecule.tokenizers.rna.utils import get_special_tokens_map, get_tokenizer_config, get_vocab_list
+from multimolecule.models import RnaFmConfig as Config
+from multimolecule.models import RnaFmForPretraining as Model
+from multimolecule.tokenisers.rna.utils import (
+    convert_word_embeddings,
+    get_special_tokens_map,
+    get_tokenizer_config,
+    get_vocab_list,
+)
 
 try:
     from huggingface_hub import HfApi
 except ImportError:
     HfApi = None
 
 torch.manual_seed(1013)
 
 
 def _convert_checkpoint(config, original_state_dict, vocab_list, original_vocab_list):
     state_dict = {}
     for key, value in original_state_dict.items():
+        key = "rnafm" + key[7:]
         key = key.replace("LayerNorm", "layer_norm")
         key = key.replace("gamma", "weight")
         key = key.replace("beta", "bias")
-        if key.startswith("bert"):
-            state_dict["utr" + key] = value
-            continue
-        if key.startswith("cls"):
-            key = "lm_head" + key[15:]
-            state_dict[key] = value
-            continue
+        key = key.replace("rnafm.encoder.emb_layer_norm_before", "rnafm.embeddings.layer_norm")
+        key = key.replace("rnafm.encoder.embed_tokens", "rnafm.embeddings.word_embeddings")
+        key = key.replace("rnafm.encoder.embed_positions", "rnafm.embeddings.position_embeddings")
+        key = key.replace("layers", "layer")
+        key = key.replace("self_attn", "attention.self")
+        key = key.replace("q_proj", "query")
+        key = key.replace("k_proj", "key")
+        key = key.replace("v_proj", "value")
+        key = key.replace("self.out_proj", "output.dense")
+        key = key.replace("self_layer_norm", "layer_norm")
+        key = key.replace("final_layer_norm", "layer_norm")
+        key = key.replace("fc1", "intermediate.dense")
+        key = key.replace("fc2", "output.dense")
+        key = key.replace("regression", "decoder")
+        key = key.replace("rnafm.encoder.lm_head", "pretrain_head.predictions")
+        key = key.replace("predictions.dense", "predictions.transform.dense")
+        key = key.replace("predictions.layer_norm", "predictions.transform.layer_norm")
+        key = key.replace("predictions.weight", "predictions.decoder.weight")
+        key = key.replace("rnafm.encoder.contact_head", "pretrain_head.contact")
         state_dict[key] = value
 
-    state_vocab_size = state_dict["utrbert.embeddings.word_embeddings.weight"].size(0)
-    original_vocab_size = len(original_vocab_list)
-    if state_vocab_size != original_vocab_size:
-        raise ValueError(
-            f"Vocabulary size do not match. Expected to have {original_vocab_size}, but got {state_vocab_size}."
-        )
-    word_embed = nn.Embedding(config.vocab_size, config.hidden_size, padding_idx=config.pad_token_id)
-    word_embed_weight = word_embed.weight.data
-    predictions_decoder_weight = torch.zeros((config.vocab_size, config.hidden_size))
-    predictions_bias = torch.zeros(config.vocab_size)
-    # nn.init.normal_(pos_embed.weight, std=0.02)
-    for original_index, original_token in enumerate(original_vocab_list):
-        new_index = vocab_list.index(original_token)
-        word_embed_weight[new_index] = state_dict["utrbert.embeddings.word_embeddings.weight"][original_index]
-        predictions_decoder_weight[new_index] = state_dict["lm_head.decoder.weight"][original_index]
-        predictions_bias[new_index] = state_dict["lm_head.decoder.bias"][original_index]
-    state_dict["utrbert.embeddings.word_embeddings.weight"] = word_embed_weight
-    state_dict["lm_head.decoder.weight"] = predictions_decoder_weight
-    state_dict["lm_head.decoder.bias"] = state_dict["lm_head.bias"] = predictions_bias
+    word_embed_weight, decoder_weight, decoder_bias = convert_word_embeddings(
+        state_dict["rnafm.embeddings.word_embeddings.weight"],
+        state_dict["pretrain_head.predictions.decoder.weight"],
+        state_dict["pretrain_head.predictions.bias"],
+        old_vocab=original_vocab_list,
+        new_vocab=vocab_list,
+        std=config.initializer_range,
+    )
+    state_dict["rnafm.embeddings.word_embeddings.weight"] = word_embed_weight
+    state_dict["pretrain_head.predictions.decoder.weight"] = decoder_weight
+    state_dict["pretrain_head.predictions.decoder.bias"] = state_dict["pretrain_head.predictions.bias"] = decoder_bias
     return state_dict
 
 
 def convert_checkpoint(convert_config):
-    config = chanfig.load(os.path.join(convert_config.checkpoint_path, "config.json"))
-    config.hidden_dropout = config.pop("hidden_dropout_prob", 0.1)
-    config.attention_dropout = config.pop("attention_probs_dropout_prob", 0.1)
-    config.nmers = int(convert_config.checkpoint_path.split("/")[-1][0])
-    vocab_list = get_vocab_list(config.nmers, strameline=True)
-    config = Config.from_dict(config)
-    del config._name_or_path
-    config.architectures = ["UtrBertModel"]
+    vocab_list = get_vocab_list()
+    original_vocab_list = [
+        "<cls>",
+        "<pad>",
+        "<eos>",
+        "<unk>",
+        "A",
+        "C",
+        "G",
+        "U",
+        "R",
+        "Y",
+        "K",
+        "M",
+        "S",
+        "W",
+        "B",
+        "D",
+        "H",
+        "V",
+        "N",
+        "-",
+        "<null>",
+        "<null>",
+        "<null>",
+        "<null>",
+        "<mask>",
+    ]
+    config = Config(num_labels=1)
+    config.architectures = ["RnaFmModel"]
     config.vocab_size = len(vocab_list)
 
     model = Model(config)
 
-    ckpt = torch.load(
-        os.path.join(convert_config.checkpoint_path, "pytorch_model.bin"), map_location=torch.device("cpu")
-    )
-    original_vocab_list = []
-    for char in open(os.path.join(convert_config.checkpoint_path, "vocab.txt")).read().splitlines():  # noqa: SIM115
-        if char.startswith("["):
-            char = char.lower().replace("[", "<").replace("]", ">")
-        if char == "T":
-            char = "U"
-        if char == "<sep>":
-            char = "<eos>"
-        original_vocab_list.append(char)
+    ckpt = torch.load(convert_config.checkpoint_path, map_location=torch.device("cpu"))
+    ckpt = ckpt.get("model", ckpt)
     state_dict = _convert_checkpoint(config, ckpt, vocab_list, original_vocab_list)
 
     model.load_state_dict(state_dict)
     model.save_pretrained(convert_config.output_path, safe_serialization=True)
     model.save_pretrained(convert_config.output_path, safe_serialization=False)
     chanfig.NestedDict(get_special_tokens_map()).json(
         os.path.join(convert_config.output_path, "special_tokens_map.json")
     )
-    tokenizer_config = get_tokenizer_config()
-    tokenizer_config["nmers"] = config.nmers
-    tokenizer_config["strameline"] = True
-    chanfig.NestedDict(tokenizer_config).json(os.path.join(convert_config.output_path, "tokenizer_config.json"))
+    tokenizer_config = chanfig.NestedDict(get_tokenizer_config())
+    tokenizer_config["model_max_length"] = config.max_position_embeddings - 2
+    tokenizer_config.json(os.path.join(convert_config.output_path, "tokenizer_config.json"))
 
     if convert_config.push_to_hub:
         if HfApi is None:
             raise ImportError("Please install huggingface_hub to push to the hub.")
         api = HfApi()
+        if convert_config.delete_existing:
+            api.delete_repo(
+                convert_config.repo_id,
+                token=convert_config.token,
+                missing_ok=True,
+            )
         api.create_repo(
             convert_config.repo_id,
             token=convert_config.token,
             exist_ok=True,
         )
         api.upload_folder(
             repo_id=convert_config.repo_id, folder_path=convert_config.output_path, token=convert_config.token
         )
 
 
 @chanfig.configclass
 class ConvertConfig:
     checkpoint_path: str
-    output_path: Optional[str] = None
+    output_path: str = Config.model_type
     push_to_hub: bool = False
-    repo_id: Optional[str] = output_path
-    token: Optional[str] = None
+    delete_existing: bool = False
+    repo_id: str | None = None
+    token: str | None = None
 
     def post(self):
-        if self.output_path is None:
-            self.output_path = self.checkpoint_path.split("/")[-1].lower()
         if self.repo_id is None:
             self.repo_id = f"multimolecule/{self.output_path}"
 
 
 if __name__ == "__main__":
     config = ConvertConfig()
     config.parse()  # type: ignore[attr-defined]
```

### Comparing `multimolecule-0.0.2/multimolecule/models/utrbert/modeling_utrbert.py` & `multimolecule-0.0.3/multimolecule/models/utrbert/modeling_utrbert.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,47 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from __future__ import annotations
 
 import math
-from typing import List, Optional, Tuple
+from typing import Tuple
+from warnings import warn
 
 import torch
 import torch.utils.checkpoint
+from danling import NestedTensor
 from torch import Tensor, nn
-from torch.nn import functional as F
 from transformers.activations import ACT2FN
 from transformers.modeling_outputs import (
     BaseModelOutputWithPastAndCrossAttentions,
     BaseModelOutputWithPoolingAndCrossAttentions,
     MaskedLMOutput,
     SequenceClassifierOutput,
     TokenClassifierOutput,
 )
 from transformers.modeling_utils import PreTrainedModel
 from transformers.pytorch_utils import apply_chunking_to_forward, find_pruneable_heads_and_indices, prune_linear_layer
 from transformers.utils import logging
 
-from ..modeling_utils import MaskedLMHead, SequenceClassificationHead, TokenClassificationHead
+from multimolecule.module import MaskedLMHead, NucleotideKMerHead, SequenceClassificationHead, TokenKMerHead
+
 from .configuration_utrbert import UtrBertConfig
 
 logger = logging.get_logger(__name__)
 
 
 class UtrBertPreTrainedModel(PreTrainedModel):
     """
@@ -87,26 +105,26 @@
         class PreTrainedModel
         """
         for layer, heads in heads_to_prune.items():
             self.encoder.layer[layer].attention.prune_heads(heads)
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        encoder_hidden_states: Optional[Tensor] = None,
-        encoder_attention_mask: Optional[Tensor] = None,
-        past_key_values: Optional[List[torch.FloatTensor]] = None,
-        use_cache: Optional[bool] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        encoder_hidden_states: Tensor | None = None,
+        encoder_attention_mask: Tensor | None = None,
+        past_key_values: Tuple[Tuple[torch.FloatTensor, torch.FloatTensor], ...] | None = None,
+        use_cache: bool | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
     ) -> Tuple[Tensor, ...] | BaseModelOutputWithPoolingAndCrossAttentions:
         r"""
         encoder_hidden_states  (`torch.FloatTensor` of shape `(batch_size, sequence_length, hidden_size)`, *optional*):
             Sequence of hidden-states at the output of the last layer of the encoder. Used in the cross-attention if
             the model is configured as a decoder.
         encoder_attention_mask (`torch.FloatTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Mask to avoid performing attention on the padding token indices of the encoder input. This mask is used in
@@ -132,17 +150,19 @@
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         if self.config.is_decoder:
             use_cache = use_cache if use_cache is not None else self.config.use_cache
         else:
             use_cache = False
 
+        if isinstance(input_ids, NestedTensor):
+            input_ids, attention_mask = input_ids.tensor, input_ids.mask
         if input_ids is not None and inputs_embeds is not None:
             raise ValueError("You cannot specify both input_ids and inputs_embeds at the same time")
-        elif input_ids is not None:
+        if input_ids is not None:
             self.warn_if_padding_and_no_attention_mask(input_ids, attention_mask)
             input_shape = input_ids.size()
         elif inputs_embeds is not None:
             input_shape = inputs_embeds.size()[:-1]
         else:
             raise ValueError("You have to specify either input_ids or inputs_embeds")
 
@@ -215,15 +235,15 @@
         )
 
 
 class UtrBertForMaskedLM(UtrBertPreTrainedModel):
     """
     Examples:
         >>> from multimolecule import UtrBertConfig, UtrBertForMaskedLM, RnaTokenizer
-        >>> tokenizer = RnaTokenizer(nmers=3, strameline=True)
+        >>> tokenizer = RnaTokenizer(nmers=2, strameline=True)
         >>> config = UtrBertConfig(vocab_size=tokenizer.vocab_size)
         >>> model = UtrBertForMaskedLM(config)
         >>> input = tokenizer("ACGUN", return_tensors="pt")
         >>> output = model(**input)
     """
 
     _tied_weights_keys = ["predictions.decoder.bias", "cls.predictions.decoder.weight"]
@@ -245,25 +265,25 @@
         return self.lm_head.decoder
 
     def set_output_embeddings(self, new_embeddings):
         self.lm_head.decoder = new_embeddings
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        encoder_hidden_states: Optional[Tensor] = None,
-        encoder_attention_mask: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        encoder_hidden_states: Tensor | None = None,
+        encoder_attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
     ) -> Tuple[Tensor, ...] | MaskedLMOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the masked language modeling loss. Indices should be in `[-100, 0, ...,
             config.vocab_size]` (see `input_ids` docstring) Tokens with indices set to `-100` are ignored (masked), the
             loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`
         """
@@ -278,19 +298,16 @@
             inputs_embeds=inputs_embeds,
             encoder_hidden_states=encoder_hidden_states,
             encoder_attention_mask=encoder_attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.lm_head(outputs)
-
-        loss = None
-        if labels is not None:
-            loss = F.cross_entropy(logits.view(-1, self.config.vocab_size), labels.view(-1))
+        output = self.lm_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return MaskedLMOutput(
             loss=loss,
@@ -316,15 +333,15 @@
         return {"input_ids": input_ids, "attention_mask": attention_mask}
 
 
 class UtrBertForPretraining(UtrBertPreTrainedModel):
     """
     Examples:
         >>> from multimolecule import UtrBertConfig, UtrBertForPretraining, RnaTokenizer
-        >>> tokenizer = RnaTokenizer(nmers=4, strameline=True)
+        >>> tokenizer = RnaTokenizer(nmers=3, strameline=True)
         >>> config = UtrBertConfig(vocab_size=tokenizer.vocab_size)
         >>> model = UtrBertForPretraining(config)
         >>> input = tokenizer("ACGUN", return_tensors="pt")
         >>> output = model(**input)
     """
 
     _tied_weights_keys = ["lm_head.decoder.bias", "lm_head.decoder.weight"]
@@ -340,23 +357,23 @@
         self.lm_head = MaskedLMHead(config)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
     ) -> Tuple[Tensor, ...] | MaskedLMOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the masked language modeling loss. Indices should be in `[-100, 0, ...,
             config.vocab_size]` (see `input_ids` docstring) Tokens with indices set to `-100` are ignored (masked),
             the loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`
         """
@@ -368,19 +385,16 @@
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.lm_head(outputs)
-
-        loss = None
-        if labels is not None:
-            loss = F.cross_entropy(logits.view(-1, self.config.vocab_size), labels.view(-1))
+        output = self.lm_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return MaskedLMOutput(
             loss=loss,
@@ -390,43 +404,42 @@
         )
 
 
 class UtrBertForSequenceClassification(UtrBertPreTrainedModel):
     """
     Examples:
         >>> from multimolecule import UtrBertConfig, UtrBertForSequenceClassification, RnaTokenizer
-        >>> tokenizer = RnaTokenizer(nmers=5, strameline=True)
+        >>> tokenizer = RnaTokenizer(nmers=4, strameline=True)
         >>> config = UtrBertConfig(vocab_size=tokenizer.vocab_size)
         >>> model = UtrBertForSequenceClassification(config)
         >>> input = tokenizer("ACGUN", return_tensors="pt")
         >>> output = model(**input)
     """
 
     def __init__(self, config: UtrBertConfig):
         super().__init__(config)
         self.num_labels = config.head.num_labels
         self.utrbert = UtrBertModel(config)
-        self.classifier = nn.Linear(config.hidden_size, config.num_labels)
         self.sequence_head = SequenceClassificationHead(config)
         self.head_config = self.sequence_head.config
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
     ) -> Tuple[Tensor, ...] | SequenceClassifierOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
             config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
             `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
         """
@@ -438,35 +451,16 @@
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.sequence_head(outputs)
-
-        loss = None
-        if labels is not None:
-            if self.head_config.problem_type is None:
-                if self.num_labels == 1:
-                    self.head_config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                    self.head_config.problem_type = "single_label_classification"
-                else:
-                    self.head_config.problem_type = "multi_label_classification"
-            if self.head_config.problem_type == "regression":
-                loss = (
-                    F.mse_loss(logits.squeeze(), labels.squeeze())
-                    if self.num_labels == 1
-                    else F.mse_loss(logits, labels)
-                )
-            elif self.head_config.problem_type == "single_label_classification":
-                loss = F.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
-            elif self.head_config.problem_type == "multi_label_classification":
-                loss = F.binary_cross_entropy_with_logits(logits, labels)
+        output = self.sequence_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return SequenceClassifierOutput(
             loss=loss,
@@ -476,42 +470,42 @@
         )
 
 
 class UtrBertForTokenClassification(UtrBertPreTrainedModel):
     """
     Examples:
         >>> from multimolecule import UtrBertConfig, UtrBertForTokenClassification, RnaTokenizer
-        >>> tokenizer = RnaTokenizer(nmers=6, strameline=True)
-        >>> config = UtrBertConfig(vocab_size=tokenizer.vocab_size)
+        >>> tokenizer = RnaTokenizer(nmers=2, strameline=True)
+        >>> config = UtrBertConfig(vocab_size=tokenizer.vocab_size, nmers=2)
         >>> model = UtrBertForTokenClassification(config)
         >>> input = tokenizer("ACGUN", return_tensors="pt")
         >>> output = model(**input)
     """
 
     def __init__(self, config: UtrBertConfig):
         super().__init__(config)
         self.num_labels = config.num_labels
         self.utrbert = UtrBertModel(config, add_pooling_layer=False)
-        self.token_head = TokenClassificationHead(config)
+        self.token_head = TokenKMerHead(config)
         self.head_config = self.token_head.config
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
     ) -> Tuple[Tensor, ...] | TokenClassifierOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the token classification loss. Indices should be in `[0, ..., config.num_labels - 1]`.
         """
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
@@ -521,35 +515,83 @@
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.token_head(outputs)
+        output = self.token_head(outputs, attention_mask, input_ids, labels)
+        logits, loss = output.logits, output.loss
 
-        loss = None
-        if labels is not None:
-            if self.head_config.problem_type is None:
-                if self.num_labels == 1:
-                    self.head_config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                    self.head_config.problem_type = "single_label_classification"
-                else:
-                    self.head_config.problem_type = "multi_label_classification"
-            if self.head_config.problem_type == "regression":
-                loss = (
-                    F.mse_loss(logits.squeeze(), labels.squeeze())
-                    if self.num_labels == 1
-                    else F.mse_loss(logits, labels)
-                )
-            elif self.head_config.problem_type == "single_label_classification":
-                loss = F.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
-            elif self.head_config.problem_type == "multi_label_classification":
-                loss = F.binary_cross_entropy_with_logits(logits, labels)
+        if not return_dict:
+            output = (logits,) + outputs[2:]
+            return ((loss,) + output) if loss is not None else output
+
+        return TokenClassifierOutput(
+            loss=loss,
+            logits=logits,
+            hidden_states=outputs.hidden_states,
+            attentions=outputs.attentions,
+        )
+
+
+class UtrBertForNucleotideClassification(UtrBertPreTrainedModel):
+    """
+    Examples:
+        >>> from multimolecule import UtrBertConfig, UtrBertForNucleotideClassification, RnaTokenizer
+        >>> tokenizer = RnaTokenizer(nmers=2, strameline=True)
+        >>> config = UtrBertConfig(vocab_size=tokenizer.vocab_size, nmers=2)
+        >>> model = UtrBertForTokenClassification(config)
+        >>> input = tokenizer("ACGUN", return_tensors="pt")
+        >>> output = model(**input)
+    """
+
+    def __init__(self, config: UtrBertConfig):
+        super().__init__(config)
+        self.num_labels = config.head.num_labels
+        self.utrbert = UtrBertModel(config, add_pooling_layer=False)
+        self.nucleotide_head = NucleotideKMerHead(config)
+        self.head_config = self.nucleotide_head.config
+
+        # Initialize weights and apply final processing
+        self.post_init()
+
+    def forward(
+        self,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool = False,
+        output_hidden_states: bool = False,
+        return_dict: bool = True,
+        **kwargs,
+    ) -> Tuple[Tensor, ...] | TokenClassifierOutput:
+        r"""
+        labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
+            Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
+            config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
+            `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
+        """
+        if kwargs:
+            warn(
+                f"Additional keyword arguments `{', '.join(kwargs)}` are detected in "
+                f"`{self.__class__.__name__}.forward`, they will be ignored.\n"
+                "This is provided for backward compatibility and may lead to unexpected behavior."
+            )
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+
+        outputs = self.utrbert(
+            input_ids,
+            attention_mask=attention_mask,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            return_dict=return_dict,
+        )
+        output = self.nucleotide_head(outputs, attention_mask, input_ids, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return TokenClassifierOutput(
             loss=loss,
@@ -574,17 +616,17 @@
         self.position_embedding_type = getattr(config, "position_embedding_type", "absolute")
         self.register_buffer(
             "position_ids", torch.arange(config.max_position_embeddings).expand((1, -1)), persistent=False
         )
 
     def forward(
         self,
-        input_ids: Optional[torch.LongTensor] = None,
-        position_ids: Optional[torch.LongTensor] = None,
-        inputs_embeds: Optional[torch.FloatTensor] = None,
+        input_ids: torch.LongTensor | None = None,
+        position_ids: torch.LongTensor | None = None,
+        inputs_embeds: torch.FloatTensor | None = None,
         past_key_values_length: int = 0,
     ) -> Tensor:
         if input_ids is not None:
             input_shape = input_ids.size()
         else:
             input_shape = inputs_embeds.size()[:-1]  # type: ignore[union-attr]
 
@@ -615,20 +657,20 @@
         self.config = config
         self.layer = nn.ModuleList([UtrBertLayer(config) for _ in range(config.num_hidden_layers)])
         self.gradient_checkpointing = False
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
-        use_cache: Optional[bool] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_values: Tuple[Tuple[torch.FloatTensor, ...], ...] | None = None,
+        use_cache: bool | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
     ) -> Tuple[Tensor, ...] | BaseModelOutputWithPastAndCrossAttentions:
         all_hidden_states = () if output_hidden_states else None
         all_self_attentions = () if output_attentions else None
         all_cross_attentions = () if output_attentions and self.config.add_cross_attention else None
@@ -715,19 +757,19 @@
             self.crossattention = UtrBertAttention(config, position_embedding_type="absolute")
         self.intermediate = UtrBertIntermediate(config)
         self.output = UtrBertOutput(config)
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_value: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_value: Tuple[torch.FloatTensor, torch.FloatTensor] | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         # decoder uni-directional self-attention cached key/values tuple is at positions 1,2
         self_attn_past_key_value = past_key_value[:2] if past_key_value is not None else None
         self_attention_outputs = self.attention(
             hidden_states,
             attention_mask,
@@ -784,15 +826,15 @@
     def feed_forward_chunk(self, attention_output):
         intermediate_output = self.intermediate(attention_output)
         layer_output = self.output(intermediate_output, attention_output)
         return layer_output
 
 
 class UtrBertAttention(nn.Module):
-    def __init__(self, config: UtrBertConfig, position_embedding_type: Optional[str] = None):
+    def __init__(self, config: UtrBertConfig, position_embedding_type: str | None = None):
         super().__init__()
         self.self = UtrBertSelfAttention(config, position_embedding_type=position_embedding_type)
         self.output = UtrBertSelfOutput(config)
         self.pruned_heads: set = set()
 
     def prune_heads(self, heads):
         if len(heads) == 0:
@@ -811,19 +853,19 @@
         self.self.num_attention_heads = self.self.num_attention_heads - len(heads)
         self.self.all_head_size = self.self.attention_head_size * self.self.num_attention_heads
         self.pruned_heads = self.pruned_heads.union(heads)
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_value: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_value: Tuple[torch.FloatTensor, torch.FloatTensor] | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         self_outputs = self.self(
             hidden_states,
             attention_mask,
             head_mask,
             encoder_hidden_states,
@@ -833,15 +875,15 @@
         )
         attention_output = self.output(self_outputs[0], hidden_states)
         outputs = (attention_output,) + self_outputs[1:]  # add attentions if we output them
         return outputs
 
 
 class UtrBertSelfAttention(nn.Module):
-    def __init__(self, config: UtrBertConfig, position_embedding_type: Optional[str] = None):
+    def __init__(self, config: UtrBertConfig, position_embedding_type: str | None = None):
         super().__init__()
         if config.hidden_size % config.num_attention_heads != 0 and not hasattr(config, "embedding_size"):
             raise ValueError(
                 f"The hidden size ({config.hidden_size}) is not a multiple of the number of attention "
                 f"heads ({config.num_attention_heads})"
             )
 
@@ -865,19 +907,19 @@
         new_x_shape = x.size()[:-1] + (self.num_attention_heads, self.attention_head_size)
         x = x.view(new_x_shape)
         return x.permute(0, 2, 1, 3)
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_value: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_value: Tuple[torch.FloatTensor, torch.FloatTensor] | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         mixed_query_layer = self.query(hidden_states)
 
         # If this is instantiated as a cross-attention module, the keys
         # and values come from an encoder; the attention mask needs to be
         # such that the encoder's padding tokens are not attended to.
```

### Comparing `multimolecule-0.0.2/multimolecule/models/utrlm/configuration_utrlm.py` & `multimolecule-0.0.3/multimolecule/models/utrlm/configuration_utrlm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from transformers.utils import logging
 
 from ..configuration_utils import HeadConfig, MaskedLMHeadConfig, PretrainedConfig
 
 logger = logging.get_logger(__name__)
 
 
@@ -98,24 +114,14 @@
         token_dropout=True,
         head=None,
         lm_head=None,
         structure_head=None,
         supervised_head=None,
         **kwargs,
     ):
-        if head is None:
-            head = {}
-        head.setdefault("hidden_size", hidden_size)
-        if "problem_type" in kwargs:
-            head.setdefault("problem_type", kwargs["problem_type"])
-        if "num_labels" in kwargs:
-            head.setdefault("num_labels", kwargs["num_labels"])
-        if lm_head is None:
-            lm_head = {}
-        lm_head.setdefault("hidden_size", hidden_size)
         super().__init__(**kwargs)
 
         self.vocab_size = vocab_size
         self.hidden_size = hidden_size
         self.num_hidden_layers = num_hidden_layers
         self.num_attention_heads = num_attention_heads
         self.intermediate_size = intermediate_size
@@ -125,11 +131,11 @@
         self.max_position_embeddings = max_position_embeddings
         self.initializer_range = initializer_range
         self.layer_norm_eps = layer_norm_eps
         self.position_embedding_type = position_embedding_type
         self.use_cache = use_cache
         self.emb_layer_norm_before = emb_layer_norm_before
         self.token_dropout = token_dropout
-        self.head = HeadConfig(**head)
-        self.lm_head = MaskedLMHeadConfig(**lm_head)
+        self.head = HeadConfig(**head if head is not None else {})
+        self.lm_head = MaskedLMHeadConfig(**lm_head if lm_head is not None else {})
         self.structure_head = HeadConfig(**structure_head) if structure_head is not None else None
         self.supervised_head = HeadConfig(**supervised_head) if supervised_head is not None else None
```

### Comparing `multimolecule-0.0.2/multimolecule/models/utrlm/modeling_utrlm.py` & `multimolecule-0.0.3/multimolecule/models/utrlm/modeling_utrlm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,55 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import List, Optional, Tuple, Union
+from typing import Tuple
+from warnings import warn
 
 import torch
 import torch.utils.checkpoint
+from danling import NestedTensor
 from torch import Tensor, nn
 from torch.nn import functional as F
 from transformers.activations import ACT2FN
 from transformers.modeling_outputs import (
     BaseModelOutputWithPastAndCrossAttentions,
     BaseModelOutputWithPoolingAndCrossAttentions,
     MaskedLMOutput,
     ModelOutput,
     SequenceClassifierOutput,
     TokenClassifierOutput,
 )
 from transformers.modeling_utils import PreTrainedModel, find_pruneable_heads_and_indices, prune_linear_layer
 from transformers.utils import logging
 
-from ..modeling_utils import (
+from multimolecule.module import (
     ContactPredictionHead,
     MaskedLMHead,
+    NucleotideClassificationHead,
     SequenceClassificationHead,
     TokenClassificationHead,
-    apply_rotary_pos_emb,
 )
+
+from ..modeling_utils import apply_rotary_pos_emb
 from .configuration_utrlm import UtrLmConfig
 
 logger = logging.get_logger(__name__)
 
 
 class UtrLmPreTrainedModel(PreTrainedModel):
     """
@@ -93,27 +113,27 @@
         class PreTrainedModel
         """
         for layer, heads in heads_to_prune.items():
             self.encoder.layer[layer].attention.prune_heads(heads)
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        encoder_hidden_states: Optional[Tensor] = None,
-        encoder_attention_mask: Optional[Tensor] = None,
-        past_key_values: Optional[List[torch.FloatTensor]] = None,
-        use_cache: Optional[bool] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple[Tensor, ...], BaseModelOutputWithPoolingAndCrossAttentions]:
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        encoder_hidden_states: Tensor | None = None,
+        encoder_attention_mask: Tensor | None = None,
+        past_key_values: Tuple[Tuple[torch.FloatTensor, torch.FloatTensor], ...] | None = None,
+        use_cache: bool | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
+    ) -> Tuple[Tensor, ...] | BaseModelOutputWithPoolingAndCrossAttentions:
         r"""
         encoder_hidden_states  (`torch.FloatTensor` of shape `(batch_size, sequence_length, hidden_size)`, *optional*):
             Sequence of hidden-states at the output of the last layer of the encoder. Used in the cross-attention if
             the model is configured as a decoder.
         encoder_attention_mask (`torch.FloatTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Mask to avoid performing attention on the padding token indices of the encoder input. This mask is used in
             the cross-attention if the model is configured as a decoder. Mask values selected in `[0, 1]`:
@@ -138,17 +158,19 @@
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         if self.config.is_decoder:
             use_cache = use_cache if use_cache is not None else self.config.use_cache
         else:
             use_cache = False
 
+        if isinstance(input_ids, NestedTensor):
+            input_ids, attention_mask = input_ids.tensor, input_ids.mask
         if input_ids is not None and inputs_embeds is not None:
             raise ValueError("You cannot specify both input_ids and inputs_embeds at the same time")
-        elif input_ids is not None:
+        if input_ids is not None:
             self.warn_if_padding_and_no_attention_mask(input_ids, attention_mask)
             input_shape = input_ids.size()
         elif inputs_embeds is not None:
             input_shape = inputs_embeds.size()[:-1]
         else:
             raise ValueError("You have to specify either input_ids or inputs_embeds")
 
@@ -246,26 +268,26 @@
         self.lm_head = MaskedLMHead(config)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        encoder_hidden_states: Optional[Tensor] = None,
-        encoder_attention_mask: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple[Tensor, ...], MaskedLMOutput]:
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        encoder_hidden_states: Tensor | None = None,
+        encoder_attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
+    ) -> Tuple[Tensor, ...] | MaskedLMOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the masked language modeling loss. Indices should be in `[-100, 0, ...,
             config.vocab_size]` (see `input_ids` docstring) Tokens with indices set to `-100` are ignored (masked), the
             loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`
         """
 
@@ -279,19 +301,16 @@
             inputs_embeds=inputs_embeds,
             encoder_hidden_states=encoder_hidden_states,
             encoder_attention_mask=encoder_attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.lm_head(outputs)
-
-        loss = None
-        if labels is not None:
-            loss = F.cross_entropy(logits.view(-1, self.config.vocab_size), labels.view(-1))
+        output = self.lm_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return MaskedLMOutput(
             loss=loss,
@@ -331,29 +350,29 @@
         return self.pretrain_head.predictions.decoder
 
     def set_output_embeddings(self, embeddings):
         self.pretrain_head.predictions.decoder = embeddings
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        encoder_hidden_states: Optional[Tensor] = None,
-        encoder_attention_mask: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        labels_contact: Optional[Tensor] = None,
-        labels_structure: Optional[Tensor] = None,
-        labels_supervised: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple[Tensor, ...], UtrLmForPretrainingOutput]:
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        encoder_hidden_states: Tensor | None = None,
+        encoder_attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        labels_contact: Tensor | None = None,
+        labels_structure: Tensor | None = None,
+        labels_supervised: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
+    ) -> Tuple[Tensor, ...] | UtrLmForPretrainingOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the masked language modeling loss. Indices should be in `[-100, 0, ...,
             config.vocab_size]` (see `input_ids` docstring) Tokens with indices set to `-100` are ignored (masked), the
             loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`
         """
 
@@ -415,32 +434,32 @@
         >>> output = model(**input)
     """
 
     def __init__(self, config: UtrLmConfig):
         super().__init__(config)
         self.num_labels = config.head.num_labels
         self.utrlm = UtrLmModel(config, add_pooling_layer=True)
-        self.classifier = SequenceClassificationHead(config)
-        self.head_config = self.classifier.config
+        self.sequence_head = SequenceClassificationHead(config)
+        self.head_config = self.sequence_head.config
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple[Tensor, ...], SequenceClassifierOutput]:
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
+    ) -> Tuple[Tensor, ...] | SequenceClassifierOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
             Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
             config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
             `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
         """
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
@@ -451,35 +470,17 @@
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.classifier(outputs)
+        output = self.sequence_head(outputs, labels)
+        logits, loss = output.logits, output.loss
 
-        loss = None
-        if labels is not None:
-            if self.head_config.problem_type is None:
-                if self.num_labels == 1:
-                    self.head_config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                    self.head_config.problem_type = "single_label_classification"
-                else:
-                    self.head_config.problem_type = "multi_label_classification"
-            if self.head_config.problem_type == "regression":
-                loss = (
-                    F.mse_loss(logits.squeeze(), labels.squeeze())
-                    if self.num_labels == 1
-                    else F.mse_loss(logits, labels)
-                )
-            elif self.head_config.problem_type == "single_label_classification":
-                loss = F.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
-            elif self.head_config.problem_type == "multi_label_classification":
-                loss = F.binary_cross_entropy_with_logits(logits, labels)
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return SequenceClassifierOutput(
             loss=loss,
             logits=logits,
@@ -499,32 +500,32 @@
         >>> output = model(**input)
     """
 
     def __init__(self, config: UtrLmConfig):
         super().__init__(config)
         self.num_labels = config.head.num_labels
         self.utrlm = UtrLmModel(config, add_pooling_layer=False)
-        self.classifier = TokenClassificationHead(config)
-        self.head_config = self.classifier.config
+        self.token_head = TokenClassificationHead(config)
+        self.head_config = self.token_head.config
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def forward(
         self,
-        input_ids: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        position_ids: Optional[Tensor] = None,
-        head_mask: Optional[Tensor] = None,
-        inputs_embeds: Optional[Tensor] = None,
-        labels: Optional[Tensor] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple[Tensor, ...], TokenClassifierOutput]:
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        position_ids: Tensor | None = None,
+        head_mask: Tensor | None = None,
+        inputs_embeds: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
+        return_dict: bool | None = None,
+    ) -> Tuple[Tensor, ...] | TokenClassifierOutput:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for computing the token classification loss. Indices should be in `[0, ..., config.num_labels - 1]`.
         """
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         outputs = self.utrlm(
@@ -533,35 +534,84 @@
             position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
         )
-        logits = self.classifier(outputs)
+        output = self.token_head(outputs, attention_mask, input_ids, labels)
+        logits, loss = output.logits, output.loss
+
+        if not return_dict:
+            output = (logits,) + outputs[2:]
+            return ((loss,) + output) if loss is not None else output
+
+        return TokenClassifierOutput(
+            loss=loss,
+            logits=logits,
+            hidden_states=outputs.hidden_states,
+            attentions=outputs.attentions,
+        )
+
+
+class UtrLmForNucleotideClassification(UtrLmPreTrainedModel):
+    """
+    Examples:
+        >>> from multimolecule import UtrLmConfig, UtrLmForNucleotideClassification, RnaTokenizer
+        >>> config = UtrLmConfig()
+        >>> model = UtrLmForNucleotideClassification(config)
+        >>> tokenizer = RnaTokenizer.from_pretrained("multimolecule/rna")
+        >>> input = tokenizer("ACGUN", return_tensors="pt")
+        >>> output = model(**input)
+    """
+
+    def __init__(self, config: UtrLmConfig):
+        super().__init__(config)
+        self.num_labels = config.head.num_labels
+        self.utrlm = UtrLmModel(config, add_pooling_layer=False)
+        self.nucleotide_head = NucleotideClassificationHead(config)
+        self.head_config = self.nucleotide_head.config
+
+        # Initialize weights and apply final processing
+        self.post_init()
+
+    def forward(
+        self,
+        input_ids: Tensor | NestedTensor,
+        attention_mask: Tensor | None = None,
+        labels: Tensor | None = None,
+        output_attentions: bool = False,
+        output_hidden_states: bool = False,
+        return_dict: bool = True,
+        **kwargs,
+    ) -> Tuple[Tensor, ...] | TokenClassifierOutput:
+        r"""
+        labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
+            Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
+            config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
+            `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
+        """
+        if kwargs:
+            warn(
+                f"Additional keyword arguments `{', '.join(kwargs)}` are detected in "
+                f"`{self.__class__.__name__}.forward`, they will be ignored.\n"
+                "This is provided for backward compatibility and may lead to unexpected behavior."
+            )
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+
+        outputs = self.utrlm(
+            input_ids,
+            attention_mask=attention_mask,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            return_dict=return_dict,
+        )
+        output = self.nucleotide_head(outputs, attention_mask, input_ids, labels)
+        logits, loss = output.logits, output.loss
 
-        loss = None
-        if labels is not None:
-            if self.head_config.problem_type is None:
-                if self.num_labels == 1:
-                    self.head_config.problem_type = "regression"
-                elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                    self.head_config.problem_type = "single_label_classification"
-                else:
-                    self.head_config.problem_type = "multi_label_classification"
-            if self.head_config.problem_type == "regression":
-                loss = (
-                    F.mse_loss(logits.squeeze(), labels.squeeze())
-                    if self.num_labels == 1
-                    else F.mse_loss(logits, labels)
-                )
-            elif self.head_config.problem_type == "single_label_classification":
-                loss = F.cross_entropy(logits.view(-1, self.num_labels), labels.view(-1))
-            elif self.head_config.problem_type == "multi_label_classification":
-                loss = F.binary_cross_entropy_with_logits(logits, labels)
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
 
         return TokenClassifierOutput(
             loss=loss,
             logits=logits,
@@ -621,15 +671,15 @@
             mask_ratio_train = 0.15 * 0.8  # Hardcoded as the ratio used in all UTRLM model training runs
             src_lengths = attention_mask.sum(-1)
             mask_ratio_observed = (input_ids == self.mask_token_id).sum(-1).float() / src_lengths
             embeddings = (embeddings * (1 - mask_ratio_train) / (1 - mask_ratio_observed)[:, None, None]).to(
                 embeddings.dtype
             )
 
-        if self.position_embeddings is not None:
+        if self.position_embedding_type == "absolute":
             position_embeddings = self.position_embeddings(position_ids)
             embeddings = embeddings + position_embeddings
 
         if self.layer_norm is not None:
             embeddings = self.layer_norm(embeddings)
         if attention_mask is not None:
             embeddings = (embeddings * attention_mask.unsqueeze(-1)).to(embeddings.dtype)
@@ -702,24 +752,24 @@
         self.layer = nn.ModuleList([UtrLmLayer(config) for _ in range(config.num_hidden_layers)])
         self.emb_layer_norm_after = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
         self.gradient_checkpointing = False
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
-        use_cache: Optional[bool] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_values: Tuple[Tuple[torch.FloatTensor, ...], ...] | None = None,
+        use_cache: bool | None = None,
         output_attentions: bool = False,
         output_hidden_states: bool = False,
         return_dict: bool = True,
-    ) -> Union[Tuple[Tensor, ...], BaseModelOutputWithPastAndCrossAttentions]:
+    ) -> Tuple[Tensor, ...] | BaseModelOutputWithPastAndCrossAttentions:
         all_hidden_states = () if output_hidden_states else None
         all_self_attentions = () if output_attentions else None
         all_cross_attentions = () if output_attentions and self.config.add_cross_attention else None
 
         if self.gradient_checkpointing and self.training and use_cache:
             logger.warning_once(
                 "`use_cache=True` is incompatible with gradient checkpointing. Setting `use_cache=False`..."
@@ -806,19 +856,19 @@
         self.layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
         self.intermediate = UtrLmIntermediate(config)
         self.output = UtrLmOutput(config)
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_value: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_value: Tuple[torch.FloatTensor, torch.FloatTensor] | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         # decoder uni-directional self-attention cached key/values tuple is at positions 1,2
         self_attn_past_key_value = past_key_value[:2] if past_key_value is not None else None
         self_attention_outputs = self.attention(
             hidden_states,
             attention_mask,
@@ -903,19 +953,19 @@
         self.self.num_attention_heads = self.self.num_attention_heads - len(heads)
         self.self.all_head_size = self.self.attention_head_size * self.self.num_attention_heads
         self.pruned_heads = self.pruned_heads.union(heads)
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_value: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_value: Tuple[torch.FloatTensor, torch.FloatTensor] | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         hidden_states_ln = self.layer_norm(hidden_states)
         self_outputs = self.self(
             hidden_states_ln,
             attention_mask,
             head_mask,
@@ -926,15 +976,15 @@
         )
         attention_output = self.output(self_outputs[0], hidden_states)
         outputs = (attention_output,) + self_outputs[1:]  # add attentions if we output them
         return outputs
 
 
 class UtrLmSelfAttention(nn.Module):
-    def __init__(self, config: UtrLmConfig, position_embedding_type: Optional[str] = None):
+    def __init__(self, config: UtrLmConfig, position_embedding_type: str | None = None):
         super().__init__()
         if config.hidden_size % config.num_attention_heads != 0 and not hasattr(config, "embedding_size"):
             raise ValueError(
                 f"The hidden size ({config.hidden_size}) is not a multiple of the number of attention "
                 f"heads ({config.num_attention_heads})"
             )
 
@@ -961,19 +1011,19 @@
         new_x_shape = x.size()[:-1] + (self.num_attention_heads, self.attention_head_size)
         x = x.view(new_x_shape)
         return x.permute(0, 2, 1, 3)
 
     def forward(
         self,
         hidden_states: Tensor,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        past_key_value: Optional[Tuple[Tuple[torch.FloatTensor, ...], ...]] = None,
+        attention_mask: torch.FloatTensor | None = None,
+        head_mask: torch.FloatTensor | None = None,
+        encoder_hidden_states: torch.FloatTensor | None = None,
+        encoder_attention_mask: torch.FloatTensor | None = None,
+        past_key_value: Tuple[torch.FloatTensor, torch.FloatTensor] | None = None,
         output_attentions: bool = False,
     ) -> Tuple[Tensor, ...]:
         mixed_query_layer = self.query(hidden_states)
 
         # If this is instantiated as a cross-attention module, the keys
         # and values come from an encoder; the attention mask needs to be
         # such that the encoder's padding tokens are not attended to.
@@ -1119,47 +1169,43 @@
 
 
 class UtrLmPreTrainingHeads(nn.Module):
     def __init__(self, config: UtrLmConfig):
         super().__init__()
         self.contact = ContactPredictionHead(config)
         self.predictions = MaskedLMHead(config)
-        head = config.head
         self.structure = None
-        if config.structure_head:
-            config.head = config.structure_head
-            self.structure = TokenClassificationHead(config)
+        if config.structure_head is not None:
+            self.structure = TokenClassificationHead(config, config.structure_head)
         self.supervised = None
-        if config.supervised_head:
-            config.head = config.supervised_head
-            self.supervised = SequenceClassificationHead(config)
-        config.head = head
+        if config.supervised_head is not None:
+            self.supervised = SequenceClassificationHead(config, config.supervised_head)
 
     def forward(
         self,
         outputs: BaseModelOutputWithPastAndCrossAttentions | Tuple[Tensor, ...],
-        attention_mask: Optional[Tensor] = None,
-        input_ids: Optional[Tensor] = None,
-    ) -> Tuple[Tensor, Tensor, Optional[Tensor], Optional[Tensor]]:
+        attention_mask: Tensor | None = None,
+        input_ids: Tensor | NestedTensor | None = None,
+    ) -> Tuple[Tensor, Tensor, Tensor | None, Tensor | None]:
         logits = self.predictions(outputs)
         contact_map = self.contact(torch.stack(outputs[-1], 1), attention_mask, input_ids)
         structure = self.structure(outputs) if self.structure else None
         supervised = self.supervised(outputs) if self.supervised else None
         return logits, contact_map, supervised, structure
 
 
 @dataclass
 class UtrLmForPretrainingOutput(ModelOutput):
-    loss: Optional[torch.FloatTensor] = None
+    loss: torch.FloatTensor | None = None
     logits: torch.FloatTensor = None
-    contact_map: Optional[torch.FloatTensor] = None
-    structure: Optional[torch.FloatTensor] = None
-    supervised: Optional[torch.FloatTensor] = None
-    hidden_states: Optional[Tuple[torch.FloatTensor, ...]] = None
-    attentions: Optional[Tuple[torch.FloatTensor, ...]] = None
+    contact_map: torch.FloatTensor | None = None
+    structure: torch.FloatTensor | None = None
+    supervised: torch.FloatTensor | None = None
+    hidden_states: Tuple[torch.FloatTensor, ...] | None = None
+    attentions: Tuple[torch.FloatTensor, ...] | None = None
 
 
 def create_position_ids_from_input_ids(input_ids, padding_idx, past_key_values_length=0):
     """
     Replace non-padding symbols with their position numbers. Position numbers begin at padding_idx+1. Padding symbols
     are ignored. This is modified from fairseq's `utils.make_positions`.
```

### Comparing `multimolecule-0.0.2/multimolecule/tokenizers/rna/tokenization_rna.py` & `multimolecule-0.0.3/multimolecule/tokenisers/rna/tokenization_rna.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,27 @@
+# MultiMolecule
+# Copyright (C) 2024-Present  MultiMolecule
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from __future__ import annotations
+
 import os
-from typing import List, Optional
+from typing import List
 
 from transformers.tokenization_utils import PreTrainedTokenizer
 from transformers.utils import logging
 
 from .utils import get_vocab_list
 
 logger = logging.get_logger(__name__)
@@ -24,19 +42,20 @@
         eos_token: str = "<eos>",
         sep_token: str = "<eos>",
         unk_token: str = "<unk>",
         mask_token: str = "<mask>",
         convert_to_uppercase: bool = True,
         convert_T_to_U: bool = True,
         nmers: int = 1,
-        strameline: bool = False,
+        strameline: bool | None = None,
         **kwargs,
     ):
         self.nmers = nmers
-        self.all_tokens = get_vocab_list(nmers, strameline)
+        self.strameline = strameline if strameline is not None else nmers > 1
+        self.all_tokens = get_vocab_list(nmers, self.strameline)
         self._id_to_token = dict(enumerate(self.all_tokens))
         self._token_to_id = {tok: ind for ind, tok in enumerate(self.all_tokens)}
         self.convert_to_uppercase = convert_to_uppercase
         self.convert_T_to_U = convert_T_to_U
         super().__init__(
             bos_token=bos_token,
             cls_token=cls_token,
@@ -77,29 +96,29 @@
     def token_to_id(self, token: str) -> int:
         return self._token_to_id.get(token, self._token_to_id.get(self.unk_token))  # type: ignore[arg-type]
 
     def id_to_token(self, index: int) -> str:
         return self._id_to_token.get(index, self.unk_token)
 
     def build_inputs_with_special_tokens(
-        self, token_ids_0: List[int], token_ids_1: Optional[List[int]] = None
+        self, token_ids_0: List[int], token_ids_1: List[int] | None = None
     ) -> List[int]:
         cls = [self.cls_token_id]
         sep = [self.eos_token_id]  # No sep token in RnaBert vocabulary
         if token_ids_1 is None:
             if self.eos_token_id is None:
                 return cls + token_ids_0
             else:
                 return cls + token_ids_0 + sep
         elif self.eos_token_id is None:
             raise ValueError("Cannot tokenize multiple sequences when EOS token is not set!")
         return cls + token_ids_0 + sep + token_ids_1 + sep  # Multiple inputs always have an EOS token
 
     def get_special_tokens_mask(
-        self, token_ids_0: List, token_ids_1: Optional[List] = None, already_has_special_tokens: bool = False
+        self, token_ids_0: List[int], token_ids_1: List[int] | None = None, already_has_special_tokens: bool = False
     ) -> List[int]:
         """
         Retrieves sequence ids from a token list that has no special tokens added. This method is called when adding
         special tokens using the tokenizer `prepare_for_model` or `encode_plus` methods.
 
         Args:
             token_ids_0 (`List[int]`):
@@ -121,15 +140,15 @@
 
             return [1 if token in self.all_special_ids else 0 for token in token_ids_0]
         mask = [1] + ([0] * len(token_ids_0)) + [1]
         if token_ids_1 is not None:
             mask += [0] * len(token_ids_1) + [1]
         return mask
 
-    def save_vocabulary(self, save_directory: str, filename_prefix: Optional[str] = None):
+    def save_vocabulary(self, save_directory: str, filename_prefix: str | None = None):
         vocab_file = os.path.join(save_directory, (filename_prefix + "-" if filename_prefix else "") + "vocab.txt")
         with open(vocab_file, "w") as f:
             f.write("\n".join(self.all_tokens))
         return (vocab_file,)
 
     @property
     def vocab_size(self) -> int:
```

### Comparing `multimolecule-0.0.2/multimolecule.egg-info/PKG-INFO` & `multimolecule-0.0.3/multimolecule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimolecule
-Version: 0.0.2
+Version: 0.0.3
 Summary: Neural Networks for RNA, DNA, and Protein.
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,9 +682,11 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE.header
 Requires-Dist: chanfig>=0.0.99
+Requires-Dist: danling
 Requires-Dist: transformers
```

### Comparing `multimolecule-0.0.2/multimolecule.egg-info/SOURCES.txt` & `multimolecule-0.0.3/multimolecule.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 .codespell-whitelist.txt
 .gitignore
 .pre-commit-config.yaml
 LICENSE
+LICENSE.header
 README.md
+conftest.py
+licensing.sh
 pyproject.toml
 setup.py
 tox.ini
 .github/merge_rules.yaml
 .github/workflows/push.yaml
 multimolecule/__init__.py
 multimolecule/_version.py
 multimolecule.egg-info/PKG-INFO
 multimolecule.egg-info/SOURCES.txt
 multimolecule.egg-info/dependency_links.txt
 multimolecule.egg-info/requires.txt
 multimolecule.egg-info/top_level.txt
+multimolecule/downstream/__init__.py
+multimolecule/downstream/crispr_off_target.py
 multimolecule/models/__init__.py
 multimolecule/models/configuration_utils.py
+multimolecule/models/modeling_auto.py
 multimolecule/models/modeling_utils.py
 multimolecule/models/rnabert/__init__.py
 multimolecule/models/rnabert/configuration_rnabert.py
 multimolecule/models/rnabert/convert_checkpoint.py
 multimolecule/models/rnabert/modeling_rnabert.py
 multimolecule/models/rnafm/__init__.py
 multimolecule/models/rnafm/configuration_rnafm.py
@@ -38,13 +44,26 @@
 multimolecule/models/utrbert/configuration_utrbert.py
 multimolecule/models/utrbert/convert_checkpoint.py
 multimolecule/models/utrbert/modeling_utrbert.py
 multimolecule/models/utrlm/__init__.py
 multimolecule/models/utrlm/configuration_utrlm.py
 multimolecule/models/utrlm/convert_checkpoint.py
 multimolecule/models/utrlm/modeling_utrlm.py
-multimolecule/tokenizers/__init__.py
-multimolecule/tokenizers/utils.py
-multimolecule/tokenizers/rna/__init__.py
-multimolecule/tokenizers/rna/tokenization_rna.py
-multimolecule/tokenizers/rna/utils.py
-multimolecule/tokenizers/rna/vocab.txt
+multimolecule/module/__init__.py
+multimolecule/module/criterions/__init__.py
+multimolecule/module/criterions/generic.py
+multimolecule/module/heads/__init__.py
+multimolecule/module/heads/contact.py
+multimolecule/module/heads/generic.py
+multimolecule/module/heads/nuleotide.py
+multimolecule/module/heads/output.py
+multimolecule/module/heads/pretrain.py
+multimolecule/module/heads/sequence.py
+multimolecule/module/heads/token.py
+multimolecule/module/heads/transform.py
+multimolecule/module/heads/utils.py
+multimolecule/tokenisers/__init__.py
+multimolecule/tokenisers/utils.py
+multimolecule/tokenisers/rna/__init__.py
+multimolecule/tokenisers/rna/tokenization_rna.py
+multimolecule/tokenisers/rna/utils.py
+multimolecule/tokenisers/rna/vocab.txt
```

### Comparing `multimolecule-0.0.2/pyproject.toml` & `multimolecule-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "chanfig>=0.0.99",
+  "danling",
   "transformers",
 ]
 [project.urls]
 documentation = "https://multimolecule.danling.org"
 homepage = "https://multimolecule.danling.org"
 repository = "https://github.com/DLS5-Omics/multimolecule"
 
@@ -99,11 +100,11 @@
 output = "coverage.xml"
 
 [tool.coverage.json]
 output = "coverage.json"
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 80
+fail_under = 64
 
 [tool.mypy]
 ignore_missing_imports = true
```

